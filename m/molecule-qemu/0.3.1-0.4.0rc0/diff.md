# Comparing `tmp/molecule-qemu-0.3.1.tar.gz` & `tmp/molecule-qemu-0.4.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-qemu-0.3.1.tar", last modified: Tue May 30 09:14:14 2023, max compression
+gzip compressed data, was "molecule-qemu-0.4.0rc0.tar", last modified: Tue May 30 09:14:41 2023, max compression
```

## Comparing `molecule-qemu-0.3.1.tar` & `molecule-qemu-0.4.0rc0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.851208 molecule-qemu-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.835208 molecule-qemu-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.843208 molecule-qemu-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/.github/workflows/ansible-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/.github/workflows/pycodestyle.yml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.843208 molecule-qemu-0.3.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-30 09:14:14.851208 molecule-qemu-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.843208 molecule-qemu-0.3.1/molecule_qemu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.847208 molecule-qemu-0.3.1/molecule_qemu/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.839208 molecule-qemu-0.3.1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.847208 molecule-qemu-0.3.1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.851208 molecule-qemu-0.3.1/molecule_qemu/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.851208 molecule-qemu-0.3.1/molecule_qemu/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/playbooks/templates/meta-data.j2
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/molecule_qemu/playbooks/templates/user-data.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:14.847208 molecule-qemu-0.3.1/molecule_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-30 09:14:14.000000 molecule-qemu-0.3.1/molecule_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-30 09:14:14.000000 molecule-qemu-0.3.1/molecule_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:14:14.000000 molecule-qemu-0.3.1/molecule_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 09:14:14.000000 molecule-qemu-0.3.1/molecule_qemu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 09:14:14.000000 molecule-qemu-0.3.1/molecule_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 09:14:14.000000 molecule-qemu-0.3.1/molecule_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 09:14:00.000000 molecule-qemu-0.3.1/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-30 09:14:14.851208 molecule-qemu-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.391757 molecule-qemu-0.4.0rc0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.383756 molecule-qemu-0.4.0rc0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.387757 molecule-qemu-0.4.0rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/.github/workflows/ansible-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/.github/workflows/pycodestyle.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.387757 molecule-qemu-0.4.0rc0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-30 09:14:41.391757 molecule-qemu-0.4.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.387757 molecule-qemu-0.4.0rc0/molecule_qemu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.391757 molecule-qemu-0.4.0rc0/molecule_qemu/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.383756 molecule-qemu-0.4.0rc0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.391757 molecule-qemu-0.4.0rc0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.391757 molecule-qemu-0.4.0rc0/molecule_qemu/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.391757 molecule-qemu-0.4.0rc0/molecule_qemu/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/playbooks/templates/meta-data.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/playbooks/templates/user-data.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.387757 molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-30 09:14:41.000000 molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-30 09:14:41.000000 molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:14:41.000000 molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 09:14:41.000000 molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 09:14:41.000000 molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 09:14:41.000000 molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-30 09:14:41.391757 molecule-qemu-0.4.0rc0/setup.cfg
```

### Comparing `molecule-qemu-0.3.1/.github/workflows/python-publish.yml` & `molecule-qemu-0.4.0rc0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.1/.github/workflows/release.yml` & `molecule-qemu-0.4.0rc0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.1/.gitignore` & `molecule-qemu-0.4.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.1/LICENSE` & `molecule-qemu-0.4.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.1/Makefile` & `molecule-qemu-0.4.0rc0/Makefile`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.1/PKG-INFO` & `molecule-qemu-0.4.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.3.1
+Version: 0.4.0rc0
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molecule-qemu-0.3.1/README.md` & `molecule-qemu-0.4.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.1/molecule_qemu/driver.py` & `molecule-qemu-0.4.0rc0/molecule_qemu/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.1/molecule_qemu/playbooks/create.yml` & `molecule-qemu-0.4.0rc0/molecule_qemu/playbooks/create.yml`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 - name: Create
   hosts: localhost
   gather_facts: false
   no_log: "{{ molecule_no_log }}"
 
   vars:
     molecule_ephemeral_directory: "{{ lookup('env', 'MOLECULE_EPHEMERAL_DIRECTORY') }}"
+    molecule_driver_directory: "{{ ( molecule_ephemeral_directory + '/../../.qemu/' ) | realpath }}"
     molecule_scenario_name: "{{ lookup('env', 'MOLECULE_SCENARIO_NAME') }}"
     molecule_project_name: "{{ lookup('env', 'MOLECULE_PROJECT_DIRECTORY') | basename }}"
     qemu_cap_hvf: false
     qemu_vm_image_arch: "x86_64"
     qemu_vm_image_format: "qcow2"
     qemu_vm_memory: "1024"
     qemu_vm_cpus: "2"
@@ -19,14 +20,15 @@
     - name: Register VMs data
       ansible.builtin.set_fact:
         instance: {
           "instance": "molecule-{{ molecule_project_name }}-{{ molecule_scenario_name }}-{{ item.name }}",
           "name": "{{ item.name }}",
 
           "image": "{{ item.image }}",
+          "image_checksum": "{{ item.image_checksum | default(omit) }}",
           "image_arch": "{{ item.image_arch | default(qemu_vm_image_arch) }}",
           "image_format": "{{ item.image_format | default(qemu_vm_image_format) }}",
 
           "ssh_host": "{{ item.ssh_host | default('127.0.0.1') }}",
           "ssh_port": "{{ item.ssh_port | default(10022) }}",
           "ssh_user": "{{ item.ssh_user }}",
 
@@ -75,14 +77,21 @@
 
     - name: Set hvf support
       ansible.builtin.set_fact:
         qemu_cap_hvf: "{{ hv_support.stdout | trim == 'kern.hv_support: 1' }}"
       when: hv_support is defined
 
     ### prerequisites #########################################################
+
+    - name: Create driver directory
+      ansible.builtin.file:
+        path: "{{ molecule_driver_directory }}"
+        state: directory
+        mode: "0755"
+
     - name: Create run directory
       ansible.builtin.file:
         path: "{{ molecule_ephemeral_directory }}/run/"
         state: directory
         mode: "0755"
 
     - name: Create OpenSSH key pair
@@ -90,38 +99,40 @@
         path: "{{ molecule_ephemeral_directory }}/run/id_ed25519"
         type: ed25519
       register: ssh_keypair
 
     - name: Fetch ARM VMs bios
       ansible.builtin.get_url:
         url: "https://releases.linaro.org/components/kernel/uefi-linaro/latest/release/qemu64/QEMU_EFI.fd"
-        dest: "{{ molecule_ephemeral_directory }}/run/QEMU_EFI.fd"
+        checksum: "sha256:42f915c44de6858f69ae6f1ffc9eaa3884d1b2ca97a7537d81312fb0dfd712cd"
+        dest: "{{ molecule_driver_directory }}/QEMU_EFI.fd"
         mode: "0644"
       when: "'aarch64' in molecule_instances | map(attribute='image_arch') | list | unique"
 
     ### images ###############################################################
     - name: Create images directory
       ansible.builtin.file:
-        path: "{{ molecule_ephemeral_directory }}/run/images/"
+        path: "{{ molecule_driver_directory }}/images/"
         state: directory
         mode: "0755"
 
     - name: Fetch images
       ansible.builtin.get_url:
-        url: "{{ item }}"
-        dest: "{{ molecule_ephemeral_directory }}/run/images/{{ item | basename }}"
+        url: "{{ item[0] }}"
+        checksum: "{{ item[1] }}"
+        dest: "{{ molecule_driver_directory }}/images/{{ item[0] | basename }}"
         mode: "0644"
-      loop: "{{ molecule_instances | map(attribute='image') | list | unique }}"
+      loop: "{{ molecule_instances | map(attribute='image') | zip(molecule_instances | map(attribute='image_checksum')) | list | unique }}"
       loop_control:
-        label: "{{ item | basename }}"
+        label: "{{ item[0] | basename }}"
       register: images
 
     - name: Get images
       ansible.builtin.set_fact:
-        images: "{{ images.results | map(attribute='item') | list | zip(images.results | map(attribute='dest') | list) }}"
+        images: "{{ 0 | extract(images.results | map(attribute='item')) | list | zip(images.results | map(attribute='dest') | list) }}"
         images_cache: {}
 
     - name: Set images cache
       ansible.builtin.set_fact:
         images_cache: "{{ images_cache | combine({item[0]: item[1]}) }}"
       loop: "{{ images }}"
       loop_control:
@@ -193,15 +204,15 @@
         -smp {{ item.vm_cpus }}
         -net nic
         -net user,hostfwd=tcp::{{ item.ssh_port }}-:22
         -display none
         -daemonize
         -pidfile {{ item.path_pid }}
         {% if item.image_arch == 'aarch64' %}
-        -bios {{ molecule_ephemeral_directory }}/run/QEMU_EFI.fd
+        -bios {{ molecule_driver_directory }}/QEMU_EFI.fd
         -cpu cortex-a72
         -machine virt,highmem=off
         {% if qemu_cap_hvf %}
         -accel hvf
         {% endif %}
         {% endif %}
       args:
```

### Comparing `molecule-qemu-0.3.1/molecule_qemu/playbooks/destroy.yml` & `molecule-qemu-0.4.0rc0/molecule_qemu/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.1/molecule_qemu.egg-info/PKG-INFO` & `molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.3.1
+Version: 0.4.0rc0
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molecule-qemu-0.3.1/molecule_qemu.egg-info/SOURCES.txt` & `molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.3.1/pyproject.toml` & `molecule-qemu-0.4.0rc0/pyproject.toml`

 * *Files identical despite different names*

