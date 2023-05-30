# Comparing `tmp/molecule-qemu-0.3.0.tar.gz` & `tmp/molecule-qemu-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-qemu-0.3.0.tar", last modified: Fri May 26 06:03:26 2023, max compression
+gzip compressed data, was "molecule-qemu-0.3.1.tar", last modified: Tue May 30 09:14:14 2023, max compression
```

## Comparing `molecule-qemu-0.3.0.tar` & `molecule-qemu-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.987530 molecule-qemu-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.983530 molecule-qemu-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.983530 molecule-qemu-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/.github/workflows/ansible-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/.github/workflows/pycodestyle.yml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.983530 molecule-qemu-0.3.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-26 06:03:26.987530 molecule-qemu-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.983530 molecule-qemu-0.3.0/molecule_qemu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.987530 molecule-qemu-0.3.0/molecule_qemu/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.983530 molecule-qemu-0.3.0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.987530 molecule-qemu-0.3.0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.987530 molecule-qemu-0.3.0/molecule_qemu/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.987530 molecule-qemu-0.3.0/molecule_qemu/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/playbooks/templates/meta-data.j2
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/molecule_qemu/playbooks/templates/user-data.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:03:26.987530 molecule-qemu-0.3.0/molecule_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-26 06:03:26.000000 molecule-qemu-0.3.0/molecule_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-26 06:03:26.000000 molecule-qemu-0.3.0/molecule_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:03:26.000000 molecule-qemu-0.3.0/molecule_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 06:03:26.000000 molecule-qemu-0.3.0/molecule_qemu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 06:03:26.000000 molecule-qemu-0.3.0/molecule_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 06:03:26.000000 molecule-qemu-0.3.0/molecule_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 06:03:17.000000 molecule-qemu-0.3.0/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-26 06:03:26.987530 molecule-qemu-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.851208 molecule-qemu-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.835208 molecule-qemu-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.843208 molecule-qemu-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/.github/workflows/ansible-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/.github/workflows/pycodestyle.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.843208 molecule-qemu-0.3.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-30 09:14:14.851208 molecule-qemu-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.843208 molecule-qemu-0.3.1/molecule_qemu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.847208 molecule-qemu-0.3.1/molecule_qemu/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.839208 molecule-qemu-0.3.1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.847208 molecule-qemu-0.3.1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.851208 molecule-qemu-0.3.1/molecule_qemu/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.851208 molecule-qemu-0.3.1/molecule_qemu/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/playbooks/templates/meta-data.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/playbooks/templates/user-data.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.847208 molecule-qemu-0.3.1/molecule_qemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-30 09:14:14.000000 molecule-qemu-0.3.1/molecule_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-30 09:14:14.000000 molecule-qemu-0.3.1/molecule_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:14:14.000000 molecule-qemu-0.3.1/molecule_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 09:14:14.000000 molecule-qemu-0.3.1/molecule_qemu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 09:14:14.000000 molecule-qemu-0.3.1/molecule_qemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 09:14:14.000000 molecule-qemu-0.3.1/molecule_qemu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-30 09:14:14.851208 molecule-qemu-0.3.1/setup.cfg
```

### Comparing `molecule-qemu-0.3.0/.github/workflows/python-publish.yml` & `molecule-qemu-0.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.0/.github/workflows/release.yml` & `molecule-qemu-0.3.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.0/.gitignore` & `molecule-qemu-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.0/LICENSE` & `molecule-qemu-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.0/Makefile` & `molecule-qemu-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.0/PKG-INFO` & `molecule-qemu-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.3.0
+Version: 0.3.1
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -34,15 +34,15 @@
 
 Support of other platforms and guest OS is possible, but not tested.
 
 # Examples
 
 ## Example scenario
 ```bash
-molecule init scenario scenario_name -d molecule-qemu
+molecule init scenario default --driver-name molecule-qemu --verifier-name testinfra
 ```
 
 ## Example `molecule.yml`
 ```yaml
 ---
 dependency:
   name: galaxy
```

### Comparing `molecule-qemu-0.3.0/README.md` & `molecule-qemu-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 Support of other platforms and guest OS is possible, but not tested.
 
 # Examples
 
 ## Example scenario
 ```bash
-molecule init scenario scenario_name -d molecule-qemu
+molecule init scenario default --driver-name molecule-qemu --verifier-name testinfra
 ```
 
 ## Example `molecule.yml`
 ```yaml
 ---
 dependency:
   name: galaxy
```

### Comparing `molecule-qemu-0.3.0/molecule_qemu/driver.py` & `molecule-qemu-0.3.1/molecule_qemu/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.0/molecule_qemu/playbooks/create.yml` & `molecule-qemu-0.3.1/molecule_qemu/playbooks/create.yml`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         {{ item.path_disk }}
       args:
         creates: "{{ item.path_disk }}"
       loop: "{{ molecule_instances }}"
       loop_control:
         label: "{{ item.name }}"
 
-    - name: Launch VMs  # noqa: no-changed-when
+    - name: Launch VMs
       ansible.builtin.command: >
         qemu-system-{{ item.image_arch }}
         -name {{ item.name }}
         -boot d
         -cdrom {{ molecule_ephemeral_directory }}/run/cloud-init/{{ item.name }}.iso
         -hda {{ item.path_disk }}
         -m {{ item.vm_memory }}
@@ -200,14 +200,16 @@
         -bios {{ molecule_ephemeral_directory }}/run/QEMU_EFI.fd
         -cpu cortex-a72
         -machine virt,highmem=off
         {% if qemu_cap_hvf %}
         -accel hvf
         {% endif %}
         {% endif %}
+      args:
+        creates: "{{ item.path_pid }}"
       loop: "{{ molecule_instances }}"
       loop_control:
         label: "{{ item.name }}"
 
     ### ssh ###################################################################
     - name: Wait for SSH
       ansible.builtin.wait_for:
```

### Comparing `molecule-qemu-0.3.0/molecule_qemu/playbooks/destroy.yml` & `molecule-qemu-0.3.1/molecule_qemu/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.0/molecule_qemu.egg-info/PKG-INFO` & `molecule-qemu-0.3.1/molecule_qemu.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.3.0
+Version: 0.3.1
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -34,15 +34,15 @@
 
 Support of other platforms and guest OS is possible, but not tested.
 
 # Examples
 
 ## Example scenario
 ```bash
-molecule init scenario scenario_name -d molecule-qemu
+molecule init scenario default --driver-name molecule-qemu --verifier-name testinfra
 ```
 
 ## Example `molecule.yml`
 ```yaml
 ---
 dependency:
   name: galaxy
```

### Comparing `molecule-qemu-0.3.0/molecule_qemu.egg-info/SOURCES.txt` & `molecule-qemu-0.3.1/molecule_qemu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.0/pyproject.toml` & `molecule-qemu-0.3.1/pyproject.toml`

 * *Files identical despite different names*

