# Comparing `tmp/datana-0.3.1.2.tar.gz` & `tmp/datana-0.3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datana-0.3.1.2.tar", last modified: Wed May 10 13:01:17 2023, max compression
+gzip compressed data, was "datana-0.3.1.3.tar", last modified: Tue May 30 13:26:05 2023, max compression
```

## Comparing `datana-0.3.1.2.tar` & `datana-0.3.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:01:17.858216 datana-0.3.1.2/
--rw-rw-rw-   0        0        0      379 2023-05-10 13:01:17.857219 datana-0.3.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 13:01:17.825609 datana-0.3.1.2/datana/
--rw-rw-rw-   0        0        0       25 2022-09-09 06:43:52.000000 datana-0.3.1.2/datana/__init__.py
--rw-rw-rw-   0        0        0     1366 2023-02-24 08:51:40.000000 datana-0.3.1.2/datana/atom.py
--rw-rw-rw-   0        0        0     1137 2022-12-07 08:28:44.000000 datana-0.3.1.2/datana/dos.py
--rw-rw-rw-   0        0        0     6042 2023-05-09 06:10:24.000000 datana-0.3.1.2/datana/dynamic.py
--rw-rw-rw-   0        0        0     5411 2022-09-14 03:18:58.000000 datana-0.3.1.2/datana/figure.py
--rw-rw-rw-   0        0        0     1887 2023-02-24 08:53:44.000000 datana-0.3.1.2/datana/plotting.py
--rw-rw-rw-   0        0        0     4801 2022-09-14 06:41:22.000000 datana-0.3.1.2/datana/spectrum.py
--rw-rw-rw-   0        0        0    21857 2023-05-09 06:10:00.000000 datana-0.3.1.2/datana/structure.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:01:17.856250 datana-0.3.1.2/datana.egg-info/
--rw-rw-rw-   0        0        0      379 2023-05-10 13:01:15.000000 datana-0.3.1.2/datana.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-10 13:01:16.000000 datana-0.3.1.2/datana.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:01:15.000000 datana-0.3.1.2/datana.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-10 13:01:15.000000 datana-0.3.1.2/datana.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 13:01:17.858216 datana-0.3.1.2/setup.cfg
--rw-rw-rw-   0        0        0      542 2023-05-10 13:00:07.000000 datana-0.3.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:26:05.180585 datana-0.3.1.3/
+-rw-rw-rw-   0        0        0      379 2023-05-30 13:26:05.169201 datana-0.3.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 13:26:05.120711 datana-0.3.1.3/datana/
+-rw-rw-rw-   0        0        0       25 2022-09-09 06:43:52.000000 datana-0.3.1.3/datana/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-02-24 08:51:40.000000 datana-0.3.1.3/datana/atom.py
+-rw-rw-rw-   0        0        0     1137 2022-12-07 08:28:44.000000 datana-0.3.1.3/datana/dos.py
+-rw-rw-rw-   0        0        0     6042 2023-05-09 06:10:24.000000 datana-0.3.1.3/datana/dynamic.py
+-rw-rw-rw-   0        0        0     5411 2022-09-14 03:18:58.000000 datana-0.3.1.3/datana/figure.py
+-rw-rw-rw-   0        0        0     1887 2023-02-24 08:53:44.000000 datana-0.3.1.3/datana/plotting.py
+-rw-rw-rw-   0        0        0     4801 2022-09-14 06:41:22.000000 datana-0.3.1.3/datana/spectrum.py
+-rw-rw-rw-   0        0        0    23192 2023-05-30 07:05:14.000000 datana-0.3.1.3/datana/structure.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:26:05.166204 datana-0.3.1.3/datana.egg-info/
+-rw-rw-rw-   0        0        0      379 2023-05-30 13:26:05.000000 datana-0.3.1.3/datana.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-30 13:26:05.000000 datana-0.3.1.3/datana.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 13:26:05.000000 datana-0.3.1.3/datana.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-30 13:26:05.000000 datana-0.3.1.3/datana.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 13:26:05.180585 datana-0.3.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      542 2023-05-30 13:18:52.000000 datana-0.3.1.3/setup.py
```

### Comparing `datana-0.3.1.2/datana/atom.py` & `datana-0.3.1.3/datana/atom.py`

 * *Files identical despite different names*

### Comparing `datana-0.3.1.2/datana/dos.py` & `datana-0.3.1.3/datana/dos.py`

 * *Files identical despite different names*

### Comparing `datana-0.3.1.2/datana/dynamic.py` & `datana-0.3.1.3/datana/dynamic.py`

 * *Files identical despite different names*

### Comparing `datana-0.3.1.2/datana/figure.py` & `datana-0.3.1.3/datana/figure.py`

 * *Files identical despite different names*

### Comparing `datana-0.3.1.2/datana/plotting.py` & `datana-0.3.1.3/datana/plotting.py`

 * *Files identical despite different names*

### Comparing `datana-0.3.1.2/datana/spectrum.py` & `datana-0.3.1.3/datana/spectrum.py`

 * *Files identical despite different names*

### Comparing `datana-0.3.1.2/datana/structure.py` & `datana-0.3.1.3/datana/structure.py`

 * *Files 5% similar despite different names*

```diff
@@ -223,14 +223,40 @@
             else:
                 if(mode == 'Cartesian'):
                     for i in range(len(self._coords_cartesian)):
                         f.write(f'  {self._coords_cartesian[i][0]:.10f}  {self._coords_cartesian[i][1]:.10f}  {self._coords_cartesian[i][2]:.10f}\n')
                 else:
                     for i in range(len(self._coords_direct)):
                         f.write(f'  {self._coords_direct[i][0]:.10f}  {self._coords_direct[i][1]:.10f}  {self._coords_direct[i][2]:.10f}\n')
+    
+    def to_cif(self, file_name = 'structure.cif'):
+        with open(file_name, 'w') as f:
+            f.write('data_created_by_datana\n')
+            f.write('loop_\n')
+            f.write('_symmetry_equiv_pos_as_xyz\n')
+            f.write('  x,y,z\n')
+            abc = self.get_abc()
+            f.write(f'_cell_length_a\t{abc[0]:.4f}\n')
+            f.write(f'_cell_length_b\t{abc[1]:.4f}\n')
+            f.write(f'_cell_length_c\t{abc[2]:.4f}\n')
+            angles = self.get_angles()
+            f.write(f'_cell_angle_alpha\t{angles[0]:.4f}\n')
+            f.write(f'_cell_angle_beta\t{angles[1]:.4f}\n')
+            f.write(f'_cell_angle_gamma\t{angles[2]:.4f}\n')
+            f.write('loop_\n')
+            f.write('_atom_site_label\n')
+            f.write('_atom_site_type_symbol\n')
+            f.write('_atom_site_fract_x\n')
+            f.write('_atom_site_fract_y\n')
+            f.write('_atom_site_fract_z\n')
+            f.write('_atom_site_U_iso_or_equiv\n')
+            f.write('_atom_site_adp_type\n')
+            f.write('_atom_site_occupancy\n')
+            for i in range(len(self._coords_cartesian)):
+                f.write(f'Atom{i}\t{self._species[i]}\t{self._coords_direct[i][0]:.5f}\t{self._coords_direct[i][1]:.5f}\t{self._coords_direct[i][2]:.5f}\t0.00000\tUiso\t1.00\n')
 
 class Structures:
     def __init__(self):
         self._structures = []
 
     def __str__(self):
         str_summary = 'Structures Summary\n'
```

### Comparing `datana-0.3.1.2/setup.py` & `datana-0.3.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
 	name = 'datana',
-	version = '0.3.1.2',
+	version = '0.3.1.3',
 	author = 'MasterLegend',
 	description = 'datana pakage',
 	long_description = 'Datana is a package for data processing in the field of chemistry. It can be used to process both computational and experimental data.',
 	long_description_content_type = 'text/markdown',
 	url = 'https://github.com/MasterLegend/datana',
 	py_modules = ['datana.spectrum', 'datana.figure', 'datana.atom', 'datana.structure', 'datana.dynamic', 'datana.dos', 'datana.plotting'],
 )
```

