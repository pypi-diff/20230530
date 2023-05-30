# Comparing `tmp/shelxfile-8.tar.gz` & `tmp/shelxfile-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shelxfile-8.tar", last modified: Fri Jul  8 13:44:08 2022, max compression
+gzip compressed data, was "shelxfile-9.tar", last modified: Tue Jul 26 20:51:41 2022, max compression
```

## Comparing `shelxfile-8.tar` & `shelxfile-9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2022-07-08 13:44:08.435213 shelxfile-8/
--rw-rw-rw-   0        0        0     1091 2021-10-12 10:48:50.000000 shelxfile-8/LICENSE.md
--rw-rw-rw-   0        0        0     7635 2022-07-08 13:44:08.435213 shelxfile-8/PKG-INFO
--rw-rw-rw-   0        0        0     6972 2022-06-16 21:55:12.000000 shelxfile-8/README.md
--rw-rw-rw-   0        0        0      110 2021-10-12 10:48:50.000000 shelxfile-8/pyproject.toml
--rw-rw-rw-   0        0        0      814 2022-07-08 13:44:08.435213 shelxfile-8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-07-08 13:44:08.347368 shelxfile-8/shelxfile/
--rw-rw-rw-   0        0        0       45 2022-03-18 09:23:44.000000 shelxfile-8/shelxfile/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-08 13:44:08.378642 shelxfile-8/shelxfile/atoms/
--rw-rw-rw-   0        0        0        0 2021-10-12 10:48:50.000000 shelxfile-8/shelxfile/atoms/__init__.py
--rw-rw-rw-   0        0        0    12514 2022-07-08 09:37:24.000000 shelxfile-8/shelxfile/atoms/atom.py
--rw-rw-rw-   0        0        0     7498 2022-03-18 09:23:44.000000 shelxfile-8/shelxfile/atoms/atoms.py
-drwxrwxrwx   0        0        0        0 2022-07-08 13:44:08.378642 shelxfile-8/shelxfile/draw/
--rw-rw-rw-   0        0        0        0 2021-10-12 10:48:50.000000 shelxfile-8/shelxfile/draw/__init__.py
--rw-rw-rw-   0        0        0     6859 2022-03-18 09:23:44.000000 shelxfile-8/shelxfile/draw/draw_molecule.py
-drwxrwxrwx   0        0        0        0 2022-07-08 13:44:08.378642 shelxfile-8/shelxfile/fit/
--rw-rw-rw-   0        0        0        0 2021-10-12 10:48:50.000000 shelxfile-8/shelxfile/fit/__init__.py
--rw-rw-rw-   0        0        0    16642 2022-03-18 09:23:44.000000 shelxfile-8/shelxfile/fit/quatfit.py
-drwxrwxrwx   0        0        0        0 2022-07-08 13:44:08.403961 shelxfile-8/shelxfile/misc/
--rw-rw-rw-   0        0        0        0 2021-10-12 10:48:50.000000 shelxfile-8/shelxfile/misc/__init__.py
--rw-rw-rw-   0        0        0    28912 2022-03-18 09:23:44.000000 shelxfile-8/shelxfile/misc/dsrmath.py
--rw-rw-rw-   0        0        0    12185 2021-10-12 10:48:50.000000 shelxfile-8/shelxfile/misc/elements.py
--rw-rw-rw-   0        0        0    16472 2022-03-18 09:23:44.000000 shelxfile-8/shelxfile/misc/misc.py
-drwxrwxrwx   0        0        0        0 2022-07-08 13:44:08.403961 shelxfile-8/shelxfile/refine/
--rw-rw-rw-   0        0        0        0 2022-03-18 09:23:44.000000 shelxfile-8/shelxfile/refine/__init__.py
--rw-rw-rw-   0        0        0    12465 2022-03-18 09:23:44.000000 shelxfile-8/shelxfile/refine/refine.py
-drwxrwxrwx   0        0        0        0 2022-07-08 13:44:08.435213 shelxfile-8/shelxfile/shelx/
--rw-rw-rw-   0        0        0        0 2021-10-12 10:48:50.000000 shelxfile-8/shelxfile/shelx/__init__.py
--rw-rw-rw-   0        0        0    54092 2022-03-18 09:23:44.000000 shelxfile-8/shelxfile/shelx/cards.py
--rw-rw-rw-   0        0        0    16696 2021-11-02 16:29:38.000000 shelxfile-8/shelxfile/shelx/sdm.py
--rw-rw-rw-   0        0        0    13377 2021-11-02 16:29:38.000000 shelxfile-8/shelxfile/shelx/sdm_rust.py
--rw-rw-rw-   0        0        0    47616 2022-03-18 09:40:06.000000 shelxfile-8/shelxfile/shelx/shelx.py
-drwxrwxrwx   0        0        0        0 2022-07-08 13:44:08.363021 shelxfile-8/shelxfile.egg-info/
--rw-rw-rw-   0        0        0     7635 2022-07-08 13:44:08.000000 shelxfile-8/shelxfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      674 2022-07-08 13:44:08.000000 shelxfile-8/shelxfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-08 13:44:08.000000 shelxfile-8/shelxfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-07-08 13:44:08.000000 shelxfile-8/shelxfile.egg-info/top_level.txt
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2022-07-26 20:51:41.413246 shelxfile-9/
+-rw-r--r--   0 daniel     (501) staff       (20)     1071 2020-05-25 15:25:46.000000 shelxfile-9/LICENSE.md
+-rw-r--r--   0 daniel     (501) staff       (20)     7704 2022-07-26 20:51:41.413387 shelxfile-9/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)     7060 2022-07-26 20:37:23.000000 shelxfile-9/README.md
+-rw-r--r--   0 daniel     (501) staff       (20)      104 2021-05-23 18:43:32.000000 shelxfile-9/pyproject.toml
+-rw-r--r--   0 daniel     (501) staff       (20)      779 2022-07-26 20:51:41.414386 shelxfile-9/setup.cfg
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2022-07-26 20:51:41.404816 shelxfile-9/shelxfile/
+-rw-r--r--   0 daniel     (501) staff       (20)       44 2022-01-16 11:44:56.000000 shelxfile-9/shelxfile/__init__.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2022-07-26 20:51:41.407215 shelxfile-9/shelxfile/atoms/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2021-05-24 12:32:22.000000 shelxfile-9/shelxfile/atoms/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    12853 2022-07-25 14:31:25.000000 shelxfile-9/shelxfile/atoms/atom.py
+-rw-r--r--   0 daniel     (501) staff       (20)     8171 2022-07-25 14:31:25.000000 shelxfile-9/shelxfile/atoms/atoms.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2022-07-26 20:51:41.407707 shelxfile-9/shelxfile/draw/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2021-05-24 10:55:50.000000 shelxfile-9/shelxfile/draw/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     6658 2022-04-01 11:40:08.000000 shelxfile-9/shelxfile/draw/draw_molecule.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2022-07-26 20:51:41.408170 shelxfile-9/shelxfile/fit/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2021-05-24 10:55:50.000000 shelxfile-9/shelxfile/fit/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    16190 2022-07-25 14:31:25.000000 shelxfile-9/shelxfile/fit/quatfit.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2022-07-26 20:51:41.409495 shelxfile-9/shelxfile/misc/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2021-05-24 12:35:48.000000 shelxfile-9/shelxfile/misc/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    28059 2022-07-25 14:31:25.000000 shelxfile-9/shelxfile/misc/dsrmath.py
+-rw-r--r--   0 daniel     (501) staff       (20)    11577 2021-10-10 08:34:54.000000 shelxfile-9/shelxfile/misc/elements.py
+-rw-r--r--   0 daniel     (501) staff       (20)    15431 2022-07-26 20:28:39.000000 shelxfile-9/shelxfile/misc/misc.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2022-07-26 20:51:41.410047 shelxfile-9/shelxfile/refine/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2022-01-16 14:06:47.000000 shelxfile-9/shelxfile/refine/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    12159 2022-07-25 14:31:25.000000 shelxfile-9/shelxfile/refine/refine.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2022-07-26 20:51:41.412735 shelxfile-9/shelxfile/shelx/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2021-08-01 10:25:52.000000 shelxfile-9/shelxfile/shelx/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    53109 2022-07-25 14:31:25.000000 shelxfile-9/shelxfile/shelx/cards.py
+-rw-r--r--   0 daniel     (501) staff       (20)    16290 2021-10-31 19:31:46.000000 shelxfile-9/shelxfile/shelx/sdm.py
+-rw-r--r--   0 daniel     (501) staff       (20)    13061 2021-11-08 19:37:41.000000 shelxfile-9/shelxfile/shelx/sdm_rust.py
+-rw-r--r--   0 daniel     (501) staff       (20)    46655 2022-07-25 14:31:25.000000 shelxfile-9/shelxfile/shelx/shelx.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2022-07-26 20:51:41.406009 shelxfile-9/shelxfile.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)     7704 2022-07-26 20:51:41.000000 shelxfile-9/shelxfile.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      674 2022-07-26 20:51:41.000000 shelxfile-9/shelxfile.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2022-07-26 20:51:41.000000 shelxfile-9/shelxfile.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       10 2022-07-26 20:51:41.000000 shelxfile-9/shelxfile.egg-info/top_level.txt
```

### Comparing `shelxfile-8/LICENSE.md` & `shelxfile-9/LICENSE.md`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2018 Daniel Kratzert
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2018 Daniel Kratzert
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `shelxfile-8/PKG-INFO` & `shelxfile-9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,232 +1,245 @@
-Metadata-Version: 2.1
-Name: shelxfile
-Version: 8
-Summary: A parser for SHELXL results files.
-Home-page: https://github.com/dkratzert/ShelXFile
-Author: Daniel Kratzert
-Author-email: dkratzert@gmx.de
-License: Beerware License
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: Environment :: Console
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# Shelxfile
-<a href="https://repology.org/project/python:shelxfile/versions">
-    <img src="https://repology.org/badge/vertical-allrepos/python:shelxfile.svg" alt="Packaging status" align="right">
-</a>
-
-[![Unit tests](https://github.com/dkratzert/ShelXFile/actions/workflows/python-package.yml/badge.svg)](https://github.com/dkratzert/ShelXFile/actions/workflows/python-package.yml)
-![Contributions](https://img.shields.io/badge/contributions-welcome-blue)
-
-This is a full implementation of the SHELXL[[1](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)] file syntax. Additionally it is able to edit SHELX properties using Python.
-The implementation is Python3-only and supports SHELXL after 2017 (You should not use old versions anyway).
-Shelxfile may eventually become a new heart of DSR[[2](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)] and is already used as file parser in StructureFinder[[3](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)].
-
-Shelxfile always keeps the file order intact. Every SHELX instruction like DFIX or an atom is stored as an class object in the list Shelxfile.\_reslist. When writing the Shelxfile content to disk, it wites the \_reslist content to disk.
-
-Shelxfile tries to detect all possible syntax errors that SHELXL would not like either. If Shelxfile.DEBUG is True, more output about syntax and other errors are printed out. Otherwise, the parser is quiet except for really severe errors like a missing unit cell.
-
-Not every part of Shelxfile is complete, for example it will not recognize if you add restraints with atom names that are not in the SHELX file. Please help me improving it!
-
-Examples:
-
-
-```python
-pip install shelxfile
-
->>> from shelxfile import Shelxfile
->>> shx = Shelxfile()
->>> shx.read_file('src/tests/resources/p21c.res')  # or .read_string() 
->>> shx.cell
-CELL 0.71073 10.5086 20.9035 20.5072 90 94.13 90
-
->>> list(shx.cell)
-[10.5086, 20.9035, 20.5072, 90.0, 94.13, 90.0]
-
->>> shx.cell.volume
-4493.047384590458
-
->>> shx.cell.a
-10.5086
-
-# You can overwrite any parameter in a shelx file:
->>> shx.plan
-20
-
->>> shx.plan = 30
->>> shx.plan
-30
-
->>> shx.atoms
-O1     3    0.074835    0.238436    0.402457   -31.00000    0.01579    0.03095      0.01852   -0.00468   -0.00210    0.01153
-C1     1    0.028576    0.234542    0.337234   -31.00000    0.02311    0.03617      0.01096   -0.01000    0.00201    0.00356
-C2     1    0.121540    0.194460    0.298291   -31.00000    0.02960    0.04586      0.01555   -0.00485   -0.00023    0.01102
-F
-...
-
->>> a = shx.atoms.get_atom_by_name('F1_2')  # Atom F1 in residue 2
->>> a
-Atom ID: 258  # <- The Atom ID is the index number in the Shelxfile._reslist list
-
->>> str(a)
-'F1    4    0.245205    0.192674    0.649231   -21.00000    0.05143    0.03826    0.03193   -0.00579   -0.01865   -0.00485'
-
->>> a.to_isotropic()
->>> str(a)
-'F1    4    0.245205    0.192674   0.649231  -21.00000    0.04000'
-
->>> a.position  # position in the SHELX .res file
-273
-
->>> str(shx._reslist[273])  # In regular code, do not access shx._reslist directly!
-'F1    4    0.245205    0.192674   0.649231  -21.00000    0.04000'
-
->>> a.name
-'F1'
-
->>> a.element
-'F'
-
->>> a.resinum
-2
-
->>> a.part
-2
-
->>> shx.sfac2elem(4)
-'F'
-
->>> shx.elem2sfac('F')
-4
-
->>> a.find_atoms_around(dist=2.0, only_part=1)
-[Atom ID: 254, Atom ID: 256, Atom ID: 260]  # Found some atoms 
-
->>> [str(x) for x in a.find_atoms_around(dist=2.2, only_part=2)]
-['C2     1    0.192984    0.140449    0.621265   -21.00000    0.04315    0.02747      0.02385    0.00686   -0.00757    0.00126', 
-'F2     4    0.264027    0.090306    0.642441   -21.00000    0.06073    0.04450      0.03972    0.01630   -0.01260    0.01460', 
-'F3     4    0.078582    0.131920    0.643529   -21.00000    0.05691    0.04955      0.03374    0.01040    0.01881    0.00375']
-
->>> a.cart_coords
-[1.617897551082389, 4.027560959000001, 13.279336538026433]
-
->>> a.frac_coords
-[0.245205, 0.192674, 0.649231]
-
->>> a.occupancy
-1.0
-
->>> a.sfac_num
-4
-
->>>[x for x in a.find_atoms_around(dist=2.5, only_part=2)]
-[Atom ID: 254, Atom ID: 256, Atom ID: 260, Atom ID: 262]
-
->>> for x in a.find_atoms_around(dist=2.5, only_part=2):
-...    x.delete()
-
->>> [x for x in a.find_atoms_around(dist=2.5, only_part=2)]
-[]  # Atoms are now deleted from shx._reslist.
-
->>> shx.restraints
-SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4
-SADI_CCF3 0.02 F1 C2 F2 C2 F3 C2 F4 C3 F5 C3 F6 C3 F7 C4 F8 C4 F9 C4
-SADI_CCF3 0.04 C2 C3 C3 C4 C2 C4
-SADI_CCF3 0.04 O1 C2 O1 C3 O1 C4
-SADI_CCF3 0.04 F1 F2 F2 F3 F3 F1 F4 F5 F5 F6 F6 F4 F7 F8 F8 F9 F9 F7
-...
-
->>> shx.restraints[1]
-SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4
-
-str(shx.restraints[1])
-'SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4'
-
-shx.restraints[1].residue_class
-'CCF3'
-
-shx.restraints[1].s
-0.02
-
-```
-
-Writes current shx object to test.ins
-All lines in Shelxfile._reslist get wrapped after 79 characters with " =\n " as
-specified by SHELXL during the file writing.
-
-```python
->>> shx.write_shelx_file('test.ins')
-```
-No matter if you loaded a .res or .ins file with refine(), SHELXL refines the structure of the Shelxfile() object:
-
-```python
->>> shx.insert_anis()
->>> shx.refine(2)
-
- Running SHELXL with "/usr/local/bin/shelxl -b3000 /Users/daniel/GitHub/Shelxfile/tests/p21c" and "L.S. 2"
- wR2 =  0.1143 before cycle   1 for   10786 data and    945 /    945 parameters
- wR2 =  0.1025 before cycle   2 for   10786 data and    945 /    945 parameters
- wR2 =  0.1006 before cycle   3 for   10786 data and      0 /    945 parameters
- SHELXL Version 2018/3
-```
-```python
-# Symmcards that are implied by lattice symmetry are generated on-the-fly:
->>> shx.symmcards
-| 1  0  0|   | 0.0|
-| 0  1  0| + | 0.0|
-| 0  0  1|   | 0.0|
-
-|-1  0  0|   | 0.0|
-| 0 -1  0| + | 0.0|
-| 0  0 -1|   | 0.0|
-
-|-1  0  0|   | 0.0|
-| 0  1  0| + | 0.5|
-| 0  0 -1|   | 0.5|
-
-| 1  0  0|   | 0.0|
-| 0 -1  0| + |-0.5|
-| 0  0  1|   |-0.5|
-
-# Complete or "grow" structures with higher symmetry: 
->>> shx = Shelxfile('./tests/p-31c.res')
-len(shx.atoms)
-88
-p = shx.grow()
-len(p)
-208
-
-# The (bond) angle between three atoms:
->>> at1 = shx.atoms.get_atom_by_name('O1_4')
->>> at2 = shx.atoms.get_atom_by_name('C1_4')
->>> at3 = shx.atoms.get_atom_by_name('C2_4')
->>> shx.atoms.angle(at1, at2, at3)
-109.688123
-
-# The torsion angle between four atoms:
->>> at1 = shx.atoms.get_atom_by_name('O1')
->>> at2 = shx.atoms.get_atom_by_name('C1')
->>> at3 = shx.atoms.get_atom_by_name('C2')
->>> at4 = shx.atoms.get_atom_by_name('F1')
->>> shx.atoms.torsion_angle(at1, at2, at3, at4)
-74.095731
-
-```
-
-and many more...
-
-## References
-[1] http://shelx.uni-goettingen.de/, G. M. Sheldrick, Acta Cryst. (2015). C71, 3-8.
-https://doi.org/10.1107/S2053229614024218
-
-[2] https://github.com/dkratzert/DSR
-
-[3] https://github.com/dkratzert/StructureFinder
-
+Metadata-Version: 2.1
+Name: shelxfile
+Version: 9
+Summary: A parser for SHELXL results files.
+Home-page: https://github.com/dkratzert/ShelXFile
+Author: Daniel Kratzert
+Author-email: dkratzert@gmx.de
+License: Beerware License
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Classifier: Environment :: Console
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# Shelxfile
+<a href="https://repology.org/project/python:shelxfile/versions">
+    <img src="https://repology.org/badge/vertical-allrepos/python:shelxfile.svg" alt="Packaging status" align="right">
+</a>
+
+[![Unit tests](https://github.com/dkratzert/ShelXFile/actions/workflows/python-package.yml/badge.svg)](https://github.com/dkratzert/ShelXFile/actions/workflows/python-package.yml)
+![Contributions](https://img.shields.io/badge/contributions-welcome-blue)
+
+This is a full implementation of the SHELXL[[1](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)] file syntax. Additionally it is able to edit SHELX properties using Python.
+The implementation is Python3-only and supports SHELXL after 2017 (You should not use old versions anyway).
+Shelxfile may eventually become a new heart of DSR[[2](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)] and is already used as file parser in StructureFinder[[3](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)].
+
+Shelxfile always keeps the file order intact. Every SHELX instruction like DFIX or an atom is stored as an class object in the list Shelxfile.\_reslist. When writing the Shelxfile content to disk, it wites the \_reslist content to disk.
+
+Shelxfile tries to detect all possible syntax errors that SHELXL would not like either. If Shelxfile.DEBUG is True, more output about syntax and other errors are printed out. Otherwise, the parser is quiet except for really severe errors like a missing unit cell.
+
+Not every part of Shelxfile is complete, for example it will not recognize if you add restraints with atom names that are not in the SHELX file. Please help me improving it!
+
+Examples:
+
+
+```python
+pip install shelxfile
+
+>>> from shelxfile import Shelxfile
+>>> shx = Shelxfile()
+>>> shx.read_file('src/tests/resources/p21c.res')  # or .read_string() 
+>>> shx.cell
+CELL 0.71073 10.5086 20.9035 20.5072 90 94.13 90
+
+>>> list(shx.cell)
+[10.5086, 20.9035, 20.5072, 90.0, 94.13, 90.0]
+
+>>> shx.cell.volume
+4493.047384590458
+
+>>> shx.cell.a
+10.5086
+
+# You can overwrite any parameter in a shelx file:
+>>> shx.plan
+PLAN 20
+
+>>> shx.plan.npeaks
+20
+
+>>> shx.plan.set('PLAN 30')
+>>> shx.plan
+PLAN 30
+
+>>> shx.atoms
+O1     3    0.074835    0.238436    0.402457   -31.00000    0.01579    0.03095      0.01852   -0.00468   -0.00210    0.01153
+C1     1    0.028576    0.234542    0.337234   -31.00000    0.02311    0.03617      0.01096   -0.01000    0.00201    0.00356
+C2     1    0.121540    0.194460    0.298291   -31.00000    0.02960    0.04586      0.01555   -0.00485   -0.00023    0.01102
+F
+...
+
+>>> shx.atoms.hydrogen_atoms
+[Atom ID: 81, Atom ID: 88, Atom ID: 95, ... ]
+
+>>> shx.atoms.n_hydrogen_atoms
+24
+
+# Atoms with a riding model e.g. hydrogen atom riding on a carbon atom:
+>>> shx.atoms.riding_atoms
+[Atom ID: 81, Atom ID: 88, Atom ID: 95, ... ]
+
+>>> a = shx.atoms.get_atom_by_name('F1_2')  # Atom F1 in residue 2
+>>> a
+Atom ID: 258  # <- The Atom ID is the index number in the Shelxfile._reslist list
+
+>>> str(a)
+'F1    4    0.245205    0.192674    0.649231   -21.00000    0.05143    0.03826    0.03193   -0.00579   -0.01865   -0.00485'
+
+>>> a.to_isotropic()
+>>> str(a)
+'F1    4    0.245205    0.192674   0.649231  -21.00000    0.04000'
+
+>>> a.position  # position in the SHELX .res file
+273
+
+>>> str(shx._reslist[273])  # In regular code, do not access shx._reslist directly!
+'F1    4    0.245205    0.192674   0.649231  -21.00000    0.04000'
+
+>>> a.name
+'F1'
+
+>>> a.element
+'F'
+
+>>> a.resinum
+2
+
+>>> a.part
+2
+
+>>> shx.sfac2elem(4)
+'F'
+
+>>> shx.elem2sfac('F')
+4
+
+>>> a.find_atoms_around(dist=2.0, only_part=1)
+[Atom ID: 254, Atom ID: 256, Atom ID: 260]  # Found some atoms 
+
+>>> [str(x) for x in a.find_atoms_around(dist=2.2, only_part=2)]
+['C2     1    0.192984    0.140449    0.621265   -21.00000    0.04315    0.02747      0.02385    0.00686   -0.00757    0.00126', 
+'F2     4    0.264027    0.090306    0.642441   -21.00000    0.06073    0.04450      0.03972    0.01630   -0.01260    0.01460', 
+'F3     4    0.078582    0.131920    0.643529   -21.00000    0.05691    0.04955      0.03374    0.01040    0.01881    0.00375']
+
+>>> a.cart_coords
+[1.617897551082389, 4.027560959000001, 13.279336538026433]
+
+>>> a.frac_coords
+[0.245205, 0.192674, 0.649231]
+
+>>> a.occupancy
+1.0
+
+>>> a.sfac_num
+4
+
+>>>[x for x in a.find_atoms_around(dist=2.5, only_part=2)]
+[Atom ID: 254, Atom ID: 256, Atom ID: 260, Atom ID: 262]
+
+>>> for x in a.find_atoms_around(dist=2.5, only_part=2):
+...    x.delete()
+
+>>> [x for x in a.find_atoms_around(dist=2.5, only_part=2)]
+[]  # Atoms are now deleted from shx._reslist.
+
+>>> shx.restraints
+SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4
+SADI_CCF3 0.02 F1 C2 F2 C2 F3 C2 F4 C3 F5 C3 F6 C3 F7 C4 F8 C4 F9 C4
+SADI_CCF3 0.04 C2 C3 C3 C4 C2 C4
+SADI_CCF3 0.04 O1 C2 O1 C3 O1 C4
+SADI_CCF3 0.04 F1 F2 F2 F3 F3 F1 F4 F5 F5 F6 F6 F4 F7 F8 F8 F9 F9 F7
+...
+
+>>> shx.restraints[1]
+SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4
+
+str(shx.restraints[1])
+'SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4'
+
+shx.restraints[1].residue_class
+'CCF3'
+
+shx.restraints[1].s
+0.02
+
+```
+
+Writes current shx object to test.ins
+All lines in Shelxfile._reslist get wrapped after 79 characters with " =\n " as
+specified by SHELXL during the file writing.
+
+```python
+>>> shx.write_shelx_file('test.ins')
+```
+No matter if you loaded a .res or .ins file with refine(), SHELXL refines the structure of the Shelxfile() object:
+
+```python
+>>> shx.insert_anis()
+>>> shx.refine(2)
+
+ Running SHELXL with "/usr/local/bin/shelxl -b3000 /Users/daniel/GitHub/Shelxfile/tests/p21c" and "L.S. 2"
+ wR2 =  0.1143 before cycle   1 for   10786 data and    945 /    945 parameters
+ wR2 =  0.1025 before cycle   2 for   10786 data and    945 /    945 parameters
+ wR2 =  0.1006 before cycle   3 for   10786 data and      0 /    945 parameters
+ SHELXL Version 2018/3
+```
+```python
+# Symmcards that are implied by lattice symmetry are generated on-the-fly:
+>>> shx.symmcards
+| 1  0  0|   | 0.0|
+| 0  1  0| + | 0.0|
+| 0  0  1|   | 0.0|
+
+|-1  0  0|   | 0.0|
+| 0 -1  0| + | 0.0|
+| 0  0 -1|   | 0.0|
+
+|-1  0  0|   | 0.0|
+| 0  1  0| + | 0.5|
+| 0  0 -1|   | 0.5|
+
+| 1  0  0|   | 0.0|
+| 0 -1  0| + |-0.5|
+| 0  0  1|   |-0.5|
+
+# Complete or "grow" structures with higher symmetry: 
+>>> shx = Shelxfile('./tests/p-31c.res')
+len(shx.atoms)
+88
+p = shx.grow()
+len(p)
+208
+
+# The (bond) angle between three atoms:
+>>> at1 = shx.atoms.get_atom_by_name('O1_4')
+>>> at2 = shx.atoms.get_atom_by_name('C1_4')
+>>> at3 = shx.atoms.get_atom_by_name('C2_4')
+>>> shx.atoms.angle(at1, at2, at3)
+109.688123
+
+# The torsion angle between four atoms:
+>>> at1 = shx.atoms.get_atom_by_name('O1')
+>>> at2 = shx.atoms.get_atom_by_name('C1')
+>>> at3 = shx.atoms.get_atom_by_name('C2')
+>>> at4 = shx.atoms.get_atom_by_name('F1')
+>>> shx.atoms.torsion_angle(at1, at2, at3, at4)
+74.095731
+
+```
+
+and many more...
+
+## References
+[1] http://shelx.uni-goettingen.de/, G. M. Sheldrick, Acta Cryst. (2015). C71, 3-8.
+https://doi.org/10.1107/S2053229614024218
+
+[2] https://github.com/dkratzert/DSR
+
+[3] https://github.com/dkratzert/StructureFinder
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shelxfile Version: 8 Summary: A parser for SHELXL
+Metadata-Version: 2.1 Name: shelxfile Version: 9 Summary: A parser for SHELXL
 results files. Home-page: https://github.com/dkratzert/ShelXFile Author: Daniel
 Kratzert Author-email: dkratzert@gmx.de License: Beerware License Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
 Engineering :: Chemistry Classifier: Environment :: Console Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
@@ -28,25 +28,29 @@
 not recognize if you add restraints with atom names that are not in the SHELX
 file. Please help me improving it! Examples: ```python pip install shelxfile
 >>> from shelxfile import Shelxfile >>> shx = Shelxfile() >>> shx.read_file
 ('src/tests/resources/p21c.res') # or .read_string() >>> shx.cell CELL 0.71073
 10.5086 20.9035 20.5072 90 94.13 90 >>> list(shx.cell) [10.5086, 20.9035,
 20.5072, 90.0, 94.13, 90.0] >>> shx.cell.volume 4493.047384590458 >>>
 shx.cell.a 10.5086 # You can overwrite any parameter in a shelx file: >>>
-shx.plan 20 >>> shx.plan = 30 >>> shx.plan 30 >>> shx.atoms O1 3 0.074835
-0.238436 0.402457 -31.00000 0.01579 0.03095 0.01852 -0.00468 -0.00210 0.01153
-C1 1 0.028576 0.234542 0.337234 -31.00000 0.02311 0.03617 0.01096 -0.01000
-0.00201 0.00356 C2 1 0.121540 0.194460 0.298291 -31.00000 0.02960 0.04586
-0.01555 -0.00485 -0.00023 0.01102 F ... >>> a = shx.atoms.get_atom_by_name
-('F1_2') # Atom F1 in residue 2 >>> a Atom ID: 258 # <- The Atom ID is the
-index number in the Shelxfile._reslist list >>> str(a) 'F1 4 0.245205 0.192674
-0.649231 -21.00000 0.05143 0.03826 0.03193 -0.00579 -0.01865 -0.00485' >>>
-a.to_isotropic() >>> str(a) 'F1 4 0.245205 0.192674 0.649231 -21.00000 0.04000'
->>> a.position # position in the SHELX .res file 273 >>> str(shx._reslist[273])
-# In regular code, do not access shx._reslist directly! 'F1 4 0.245205 0.192674
+shx.plan PLAN 20 >>> shx.plan.npeaks 20 >>> shx.plan.set('PLAN 30') >>>
+shx.plan PLAN 30 >>> shx.atoms O1 3 0.074835 0.238436 0.402457 -31.00000
+0.01579 0.03095 0.01852 -0.00468 -0.00210 0.01153 C1 1 0.028576 0.234542
+0.337234 -31.00000 0.02311 0.03617 0.01096 -0.01000 0.00201 0.00356 C2 1
+0.121540 0.194460 0.298291 -31.00000 0.02960 0.04586 0.01555 -0.00485 -0.00023
+0.01102 F ... >>> shx.atoms.hydrogen_atoms [Atom ID: 81, Atom ID: 88, Atom ID:
+95, ... ] >>> shx.atoms.n_hydrogen_atoms 24 # Atoms with a riding model e.g.
+hydrogen atom riding on a carbon atom: >>> shx.atoms.riding_atoms [Atom ID: 81,
+Atom ID: 88, Atom ID: 95, ... ] >>> a = shx.atoms.get_atom_by_name('F1_2') #
+Atom F1 in residue 2 >>> a Atom ID: 258 # <- The Atom ID is the index number in
+the Shelxfile._reslist list >>> str(a) 'F1 4 0.245205 0.192674 0.649231 -
+21.00000 0.05143 0.03826 0.03193 -0.00579 -0.01865 -0.00485' >>> a.to_isotropic
+() >>> str(a) 'F1 4 0.245205 0.192674 0.649231 -21.00000 0.04000' >>>
+a.position # position in the SHELX .res file 273 >>> str(shx._reslist[273]) #
+In regular code, do not access shx._reslist directly! 'F1 4 0.245205 0.192674
 0.649231 -21.00000 0.04000' >>> a.name 'F1' >>> a.element 'F' >>> a.resinum 2
 >>> a.part 2 >>> shx.sfac2elem(4) 'F' >>> shx.elem2sfac('F') 4 >>>
 a.find_atoms_around(dist=2.0, only_part=1) [Atom ID: 254, Atom ID: 256, Atom
 ID: 260] # Found some atoms >>> [str(x) for x in a.find_atoms_around(dist=2.2,
 only_part=2)] ['C2 1 0.192984 0.140449 0.621265 -21.00000 0.04315 0.02747
 0.02385 0.00686 -0.00757 0.00126', 'F2 4 0.264027 0.090306 0.642441 -21.00000
 0.06073 0.04450 0.03972 0.01630 -0.01260 0.01460', 'F3 4 0.078582 0.131920
```

### Comparing `shelxfile-8/README.md` & `shelxfile-9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,213 +1,226 @@
-# Shelxfile
-<a href="https://repology.org/project/python:shelxfile/versions">
-    <img src="https://repology.org/badge/vertical-allrepos/python:shelxfile.svg" alt="Packaging status" align="right">
-</a>
-
-[![Unit tests](https://github.com/dkratzert/ShelXFile/actions/workflows/python-package.yml/badge.svg)](https://github.com/dkratzert/ShelXFile/actions/workflows/python-package.yml)
-![Contributions](https://img.shields.io/badge/contributions-welcome-blue)
-
-This is a full implementation of the SHELXL[[1](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)] file syntax. Additionally it is able to edit SHELX properties using Python.
-The implementation is Python3-only and supports SHELXL after 2017 (You should not use old versions anyway).
-Shelxfile may eventually become a new heart of DSR[[2](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)] and is already used as file parser in StructureFinder[[3](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)].
-
-Shelxfile always keeps the file order intact. Every SHELX instruction like DFIX or an atom is stored as an class object in the list Shelxfile.\_reslist. When writing the Shelxfile content to disk, it wites the \_reslist content to disk.
-
-Shelxfile tries to detect all possible syntax errors that SHELXL would not like either. If Shelxfile.DEBUG is True, more output about syntax and other errors are printed out. Otherwise, the parser is quiet except for really severe errors like a missing unit cell.
-
-Not every part of Shelxfile is complete, for example it will not recognize if you add restraints with atom names that are not in the SHELX file. Please help me improving it!
-
-Examples:
-
-
-```python
-pip install shelxfile
-
->>> from shelxfile import Shelxfile
->>> shx = Shelxfile()
->>> shx.read_file('src/tests/resources/p21c.res')  # or .read_string() 
->>> shx.cell
-CELL 0.71073 10.5086 20.9035 20.5072 90 94.13 90
-
->>> list(shx.cell)
-[10.5086, 20.9035, 20.5072, 90.0, 94.13, 90.0]
-
->>> shx.cell.volume
-4493.047384590458
-
->>> shx.cell.a
-10.5086
-
-# You can overwrite any parameter in a shelx file:
->>> shx.plan
-20
-
->>> shx.plan = 30
->>> shx.plan
-30
-
->>> shx.atoms
-O1     3    0.074835    0.238436    0.402457   -31.00000    0.01579    0.03095      0.01852   -0.00468   -0.00210    0.01153
-C1     1    0.028576    0.234542    0.337234   -31.00000    0.02311    0.03617      0.01096   -0.01000    0.00201    0.00356
-C2     1    0.121540    0.194460    0.298291   -31.00000    0.02960    0.04586      0.01555   -0.00485   -0.00023    0.01102
-F
-...
-
->>> a = shx.atoms.get_atom_by_name('F1_2')  # Atom F1 in residue 2
->>> a
-Atom ID: 258  # <- The Atom ID is the index number in the Shelxfile._reslist list
-
->>> str(a)
-'F1    4    0.245205    0.192674    0.649231   -21.00000    0.05143    0.03826    0.03193   -0.00579   -0.01865   -0.00485'
-
->>> a.to_isotropic()
->>> str(a)
-'F1    4    0.245205    0.192674   0.649231  -21.00000    0.04000'
-
->>> a.position  # position in the SHELX .res file
-273
-
->>> str(shx._reslist[273])  # In regular code, do not access shx._reslist directly!
-'F1    4    0.245205    0.192674   0.649231  -21.00000    0.04000'
-
->>> a.name
-'F1'
-
->>> a.element
-'F'
-
->>> a.resinum
-2
-
->>> a.part
-2
-
->>> shx.sfac2elem(4)
-'F'
-
->>> shx.elem2sfac('F')
-4
-
->>> a.find_atoms_around(dist=2.0, only_part=1)
-[Atom ID: 254, Atom ID: 256, Atom ID: 260]  # Found some atoms 
-
->>> [str(x) for x in a.find_atoms_around(dist=2.2, only_part=2)]
-['C2     1    0.192984    0.140449    0.621265   -21.00000    0.04315    0.02747      0.02385    0.00686   -0.00757    0.00126', 
-'F2     4    0.264027    0.090306    0.642441   -21.00000    0.06073    0.04450      0.03972    0.01630   -0.01260    0.01460', 
-'F3     4    0.078582    0.131920    0.643529   -21.00000    0.05691    0.04955      0.03374    0.01040    0.01881    0.00375']
-
->>> a.cart_coords
-[1.617897551082389, 4.027560959000001, 13.279336538026433]
-
->>> a.frac_coords
-[0.245205, 0.192674, 0.649231]
-
->>> a.occupancy
-1.0
-
->>> a.sfac_num
-4
-
->>>[x for x in a.find_atoms_around(dist=2.5, only_part=2)]
-[Atom ID: 254, Atom ID: 256, Atom ID: 260, Atom ID: 262]
-
->>> for x in a.find_atoms_around(dist=2.5, only_part=2):
-...    x.delete()
-
->>> [x for x in a.find_atoms_around(dist=2.5, only_part=2)]
-[]  # Atoms are now deleted from shx._reslist.
-
->>> shx.restraints
-SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4
-SADI_CCF3 0.02 F1 C2 F2 C2 F3 C2 F4 C3 F5 C3 F6 C3 F7 C4 F8 C4 F9 C4
-SADI_CCF3 0.04 C2 C3 C3 C4 C2 C4
-SADI_CCF3 0.04 O1 C2 O1 C3 O1 C4
-SADI_CCF3 0.04 F1 F2 F2 F3 F3 F1 F4 F5 F5 F6 F6 F4 F7 F8 F8 F9 F9 F7
-...
-
->>> shx.restraints[1]
-SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4
-
-str(shx.restraints[1])
-'SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4'
-
-shx.restraints[1].residue_class
-'CCF3'
-
-shx.restraints[1].s
-0.02
-
-```
-
-Writes current shx object to test.ins
-All lines in Shelxfile._reslist get wrapped after 79 characters with " =\n " as
-specified by SHELXL during the file writing.
-
-```python
->>> shx.write_shelx_file('test.ins')
-```
-No matter if you loaded a .res or .ins file with refine(), SHELXL refines the structure of the Shelxfile() object:
-
-```python
->>> shx.insert_anis()
->>> shx.refine(2)
-
- Running SHELXL with "/usr/local/bin/shelxl -b3000 /Users/daniel/GitHub/Shelxfile/tests/p21c" and "L.S. 2"
- wR2 =  0.1143 before cycle   1 for   10786 data and    945 /    945 parameters
- wR2 =  0.1025 before cycle   2 for   10786 data and    945 /    945 parameters
- wR2 =  0.1006 before cycle   3 for   10786 data and      0 /    945 parameters
- SHELXL Version 2018/3
-```
-```python
-# Symmcards that are implied by lattice symmetry are generated on-the-fly:
->>> shx.symmcards
-| 1  0  0|   | 0.0|
-| 0  1  0| + | 0.0|
-| 0  0  1|   | 0.0|
-
-|-1  0  0|   | 0.0|
-| 0 -1  0| + | 0.0|
-| 0  0 -1|   | 0.0|
-
-|-1  0  0|   | 0.0|
-| 0  1  0| + | 0.5|
-| 0  0 -1|   | 0.5|
-
-| 1  0  0|   | 0.0|
-| 0 -1  0| + |-0.5|
-| 0  0  1|   |-0.5|
-
-# Complete or "grow" structures with higher symmetry: 
->>> shx = Shelxfile('./tests/p-31c.res')
-len(shx.atoms)
-88
-p = shx.grow()
-len(p)
-208
-
-# The (bond) angle between three atoms:
->>> at1 = shx.atoms.get_atom_by_name('O1_4')
->>> at2 = shx.atoms.get_atom_by_name('C1_4')
->>> at3 = shx.atoms.get_atom_by_name('C2_4')
->>> shx.atoms.angle(at1, at2, at3)
-109.688123
-
-# The torsion angle between four atoms:
->>> at1 = shx.atoms.get_atom_by_name('O1')
->>> at2 = shx.atoms.get_atom_by_name('C1')
->>> at3 = shx.atoms.get_atom_by_name('C2')
->>> at4 = shx.atoms.get_atom_by_name('F1')
->>> shx.atoms.torsion_angle(at1, at2, at3, at4)
-74.095731
-
-```
-
-and many more...
-
-## References
-[1] http://shelx.uni-goettingen.de/, G. M. Sheldrick, Acta Cryst. (2015). C71, 3-8.
-https://doi.org/10.1107/S2053229614024218
-
-[2] https://github.com/dkratzert/DSR
-
-[3] https://github.com/dkratzert/StructureFinder
-
+# Shelxfile
+<a href="https://repology.org/project/python:shelxfile/versions">
+    <img src="https://repology.org/badge/vertical-allrepos/python:shelxfile.svg" alt="Packaging status" align="right">
+</a>
+
+[![Unit tests](https://github.com/dkratzert/ShelXFile/actions/workflows/python-package.yml/badge.svg)](https://github.com/dkratzert/ShelXFile/actions/workflows/python-package.yml)
+![Contributions](https://img.shields.io/badge/contributions-welcome-blue)
+
+This is a full implementation of the SHELXL[[1](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)] file syntax. Additionally it is able to edit SHELX properties using Python.
+The implementation is Python3-only and supports SHELXL after 2017 (You should not use old versions anyway).
+Shelxfile may eventually become a new heart of DSR[[2](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)] and is already used as file parser in StructureFinder[[3](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)].
+
+Shelxfile always keeps the file order intact. Every SHELX instruction like DFIX or an atom is stored as an class object in the list Shelxfile.\_reslist. When writing the Shelxfile content to disk, it wites the \_reslist content to disk.
+
+Shelxfile tries to detect all possible syntax errors that SHELXL would not like either. If Shelxfile.DEBUG is True, more output about syntax and other errors are printed out. Otherwise, the parser is quiet except for really severe errors like a missing unit cell.
+
+Not every part of Shelxfile is complete, for example it will not recognize if you add restraints with atom names that are not in the SHELX file. Please help me improving it!
+
+Examples:
+
+
+```python
+pip install shelxfile
+
+>>> from shelxfile import Shelxfile
+>>> shx = Shelxfile()
+>>> shx.read_file('src/tests/resources/p21c.res')  # or .read_string() 
+>>> shx.cell
+CELL 0.71073 10.5086 20.9035 20.5072 90 94.13 90
+
+>>> list(shx.cell)
+[10.5086, 20.9035, 20.5072, 90.0, 94.13, 90.0]
+
+>>> shx.cell.volume
+4493.047384590458
+
+>>> shx.cell.a
+10.5086
+
+# You can overwrite any parameter in a shelx file:
+>>> shx.plan
+PLAN 20
+
+>>> shx.plan.npeaks
+20
+
+>>> shx.plan.set('PLAN 30')
+>>> shx.plan
+PLAN 30
+
+>>> shx.atoms
+O1     3    0.074835    0.238436    0.402457   -31.00000    0.01579    0.03095      0.01852   -0.00468   -0.00210    0.01153
+C1     1    0.028576    0.234542    0.337234   -31.00000    0.02311    0.03617      0.01096   -0.01000    0.00201    0.00356
+C2     1    0.121540    0.194460    0.298291   -31.00000    0.02960    0.04586      0.01555   -0.00485   -0.00023    0.01102
+F
+...
+
+>>> shx.atoms.hydrogen_atoms
+[Atom ID: 81, Atom ID: 88, Atom ID: 95, ... ]
+
+>>> shx.atoms.n_hydrogen_atoms
+24
+
+# Atoms with a riding model e.g. hydrogen atom riding on a carbon atom:
+>>> shx.atoms.riding_atoms
+[Atom ID: 81, Atom ID: 88, Atom ID: 95, ... ]
+
+>>> a = shx.atoms.get_atom_by_name('F1_2')  # Atom F1 in residue 2
+>>> a
+Atom ID: 258  # <- The Atom ID is the index number in the Shelxfile._reslist list
+
+>>> str(a)
+'F1    4    0.245205    0.192674    0.649231   -21.00000    0.05143    0.03826    0.03193   -0.00579   -0.01865   -0.00485'
+
+>>> a.to_isotropic()
+>>> str(a)
+'F1    4    0.245205    0.192674   0.649231  -21.00000    0.04000'
+
+>>> a.position  # position in the SHELX .res file
+273
+
+>>> str(shx._reslist[273])  # In regular code, do not access shx._reslist directly!
+'F1    4    0.245205    0.192674   0.649231  -21.00000    0.04000'
+
+>>> a.name
+'F1'
+
+>>> a.element
+'F'
+
+>>> a.resinum
+2
+
+>>> a.part
+2
+
+>>> shx.sfac2elem(4)
+'F'
+
+>>> shx.elem2sfac('F')
+4
+
+>>> a.find_atoms_around(dist=2.0, only_part=1)
+[Atom ID: 254, Atom ID: 256, Atom ID: 260]  # Found some atoms 
+
+>>> [str(x) for x in a.find_atoms_around(dist=2.2, only_part=2)]
+['C2     1    0.192984    0.140449    0.621265   -21.00000    0.04315    0.02747      0.02385    0.00686   -0.00757    0.00126', 
+'F2     4    0.264027    0.090306    0.642441   -21.00000    0.06073    0.04450      0.03972    0.01630   -0.01260    0.01460', 
+'F3     4    0.078582    0.131920    0.643529   -21.00000    0.05691    0.04955      0.03374    0.01040    0.01881    0.00375']
+
+>>> a.cart_coords
+[1.617897551082389, 4.027560959000001, 13.279336538026433]
+
+>>> a.frac_coords
+[0.245205, 0.192674, 0.649231]
+
+>>> a.occupancy
+1.0
+
+>>> a.sfac_num
+4
+
+>>>[x for x in a.find_atoms_around(dist=2.5, only_part=2)]
+[Atom ID: 254, Atom ID: 256, Atom ID: 260, Atom ID: 262]
+
+>>> for x in a.find_atoms_around(dist=2.5, only_part=2):
+...    x.delete()
+
+>>> [x for x in a.find_atoms_around(dist=2.5, only_part=2)]
+[]  # Atoms are now deleted from shx._reslist.
+
+>>> shx.restraints
+SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4
+SADI_CCF3 0.02 F1 C2 F2 C2 F3 C2 F4 C3 F5 C3 F6 C3 F7 C4 F8 C4 F9 C4
+SADI_CCF3 0.04 C2 C3 C3 C4 C2 C4
+SADI_CCF3 0.04 O1 C2 O1 C3 O1 C4
+SADI_CCF3 0.04 F1 F2 F2 F3 F3 F1 F4 F5 F5 F6 F6 F4 F7 F8 F8 F9 F9 F7
+...
+
+>>> shx.restraints[1]
+SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4
+
+str(shx.restraints[1])
+'SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4'
+
+shx.restraints[1].residue_class
+'CCF3'
+
+shx.restraints[1].s
+0.02
+
+```
+
+Writes current shx object to test.ins
+All lines in Shelxfile._reslist get wrapped after 79 characters with " =\n " as
+specified by SHELXL during the file writing.
+
+```python
+>>> shx.write_shelx_file('test.ins')
+```
+No matter if you loaded a .res or .ins file with refine(), SHELXL refines the structure of the Shelxfile() object:
+
+```python
+>>> shx.insert_anis()
+>>> shx.refine(2)
+
+ Running SHELXL with "/usr/local/bin/shelxl -b3000 /Users/daniel/GitHub/Shelxfile/tests/p21c" and "L.S. 2"
+ wR2 =  0.1143 before cycle   1 for   10786 data and    945 /    945 parameters
+ wR2 =  0.1025 before cycle   2 for   10786 data and    945 /    945 parameters
+ wR2 =  0.1006 before cycle   3 for   10786 data and      0 /    945 parameters
+ SHELXL Version 2018/3
+```
+```python
+# Symmcards that are implied by lattice symmetry are generated on-the-fly:
+>>> shx.symmcards
+| 1  0  0|   | 0.0|
+| 0  1  0| + | 0.0|
+| 0  0  1|   | 0.0|
+
+|-1  0  0|   | 0.0|
+| 0 -1  0| + | 0.0|
+| 0  0 -1|   | 0.0|
+
+|-1  0  0|   | 0.0|
+| 0  1  0| + | 0.5|
+| 0  0 -1|   | 0.5|
+
+| 1  0  0|   | 0.0|
+| 0 -1  0| + |-0.5|
+| 0  0  1|   |-0.5|
+
+# Complete or "grow" structures with higher symmetry: 
+>>> shx = Shelxfile('./tests/p-31c.res')
+len(shx.atoms)
+88
+p = shx.grow()
+len(p)
+208
+
+# The (bond) angle between three atoms:
+>>> at1 = shx.atoms.get_atom_by_name('O1_4')
+>>> at2 = shx.atoms.get_atom_by_name('C1_4')
+>>> at3 = shx.atoms.get_atom_by_name('C2_4')
+>>> shx.atoms.angle(at1, at2, at3)
+109.688123
+
+# The torsion angle between four atoms:
+>>> at1 = shx.atoms.get_atom_by_name('O1')
+>>> at2 = shx.atoms.get_atom_by_name('C1')
+>>> at3 = shx.atoms.get_atom_by_name('C2')
+>>> at4 = shx.atoms.get_atom_by_name('F1')
+>>> shx.atoms.torsion_angle(at1, at2, at3, at4)
+74.095731
+
+```
+
+and many more...
+
+## References
+[1] http://shelx.uni-goettingen.de/, G. M. Sheldrick, Acta Cryst. (2015). C71, 3-8.
+https://doi.org/10.1107/S2053229614024218
+
+[2] https://github.com/dkratzert/DSR
+
+[3] https://github.com/dkratzert/StructureFinder
+
```

#### html2text {}

```diff
@@ -19,23 +19,27 @@
 Shelxfile is complete, for example it will not recognize if you add restraints
 with atom names that are not in the SHELX file. Please help me improving it!
 Examples: ```python pip install shelxfile >>> from shelxfile import Shelxfile
 >>> shx = Shelxfile() >>> shx.read_file('src/tests/resources/p21c.res') # or
 .read_string() >>> shx.cell CELL 0.71073 10.5086 20.9035 20.5072 90 94.13 90
 >>> list(shx.cell) [10.5086, 20.9035, 20.5072, 90.0, 94.13, 90.0] >>>
 shx.cell.volume 4493.047384590458 >>> shx.cell.a 10.5086 # You can overwrite
-any parameter in a shelx file: >>> shx.plan 20 >>> shx.plan = 30 >>> shx.plan
-30 >>> shx.atoms O1 3 0.074835 0.238436 0.402457 -31.00000 0.01579 0.03095
-0.01852 -0.00468 -0.00210 0.01153 C1 1 0.028576 0.234542 0.337234 -31.00000
-0.02311 0.03617 0.01096 -0.01000 0.00201 0.00356 C2 1 0.121540 0.194460
-0.298291 -31.00000 0.02960 0.04586 0.01555 -0.00485 -0.00023 0.01102 F ... >>>
-a = shx.atoms.get_atom_by_name('F1_2') # Atom F1 in residue 2 >>> a Atom ID:
-258 # <- The Atom ID is the index number in the Shelxfile._reslist list >>> str
-(a) 'F1 4 0.245205 0.192674 0.649231 -21.00000 0.05143 0.03826 0.03193 -0.00579
--0.01865 -0.00485' >>> a.to_isotropic() >>> str(a) 'F1 4 0.245205 0.192674
+any parameter in a shelx file: >>> shx.plan PLAN 20 >>> shx.plan.npeaks 20 >>>
+shx.plan.set('PLAN 30') >>> shx.plan PLAN 30 >>> shx.atoms O1 3 0.074835
+0.238436 0.402457 -31.00000 0.01579 0.03095 0.01852 -0.00468 -0.00210 0.01153
+C1 1 0.028576 0.234542 0.337234 -31.00000 0.02311 0.03617 0.01096 -0.01000
+0.00201 0.00356 C2 1 0.121540 0.194460 0.298291 -31.00000 0.02960 0.04586
+0.01555 -0.00485 -0.00023 0.01102 F ... >>> shx.atoms.hydrogen_atoms [Atom ID:
+81, Atom ID: 88, Atom ID: 95, ... ] >>> shx.atoms.n_hydrogen_atoms 24 # Atoms
+with a riding model e.g. hydrogen atom riding on a carbon atom: >>>
+shx.atoms.riding_atoms [Atom ID: 81, Atom ID: 88, Atom ID: 95, ... ] >>> a =
+shx.atoms.get_atom_by_name('F1_2') # Atom F1 in residue 2 >>> a Atom ID: 258 #
+<- The Atom ID is the index number in the Shelxfile._reslist list >>> str(a)
+'F1 4 0.245205 0.192674 0.649231 -21.00000 0.05143 0.03826 0.03193 -0.00579 -
+0.01865 -0.00485' >>> a.to_isotropic() >>> str(a) 'F1 4 0.245205 0.192674
 0.649231 -21.00000 0.04000' >>> a.position # position in the SHELX .res file
 273 >>> str(shx._reslist[273]) # In regular code, do not access shx._reslist
 directly! 'F1 4 0.245205 0.192674 0.649231 -21.00000 0.04000' >>> a.name 'F1'
 >>> a.element 'F' >>> a.resinum 2 >>> a.part 2 >>> shx.sfac2elem(4) 'F' >>>
 shx.elem2sfac('F') 4 >>> a.find_atoms_around(dist=2.0, only_part=1) [Atom ID:
 254, Atom ID: 256, Atom ID: 260] # Found some atoms >>> [str(x) for x in
 a.find_atoms_around(dist=2.2, only_part=2)] ['C2 1 0.192984 0.140449 0.621265 -
```

### Comparing `shelxfile-8/setup.cfg` & `shelxfile-9/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,49 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2073 6865 6c78 6669 6c65 0d0a 7665   = shelxfile..ve
-00000020: 7273 696f 6e20 3d20 380d 0a61 7574 686f  rsion = 8..autho
-00000030: 7220 3d20 4461 6e69 656c 204b 7261 747a  r = Daniel Kratz
-00000040: 6572 740d 0a61 7574 686f 725f 656d 6169  ert..author_emai
-00000050: 6c20 3d20 646b 7261 747a 6572 7440 676d  l = dkratzert@gm
-00000060: 782e 6465 0d0a 6c69 6365 6e73 6520 3d20  x.de..license = 
-00000070: 4265 6572 7761 7265 204c 6963 656e 7365  Beerware License
-00000080: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
-00000090: 4120 7061 7273 6572 2066 6f72 2053 4845  A parser for SHE
-000000a0: 4c58 4c20 7265 7375 6c74 7320 6669 6c65  LXL results file
-000000b0: 732e 0d0a 7572 6c20 3d20 6874 7470 733a  s...url = https:
-000000c0: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6b72  //github.com/dkr
-000000d0: 6174 7a65 7274 2f53 6865 6c58 4669 6c65  atzert/ShelXFile
-000000e0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-000000f0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
-00000100: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
-00000110: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
-00000120: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
-00000130: 6f77 6e0d 0a63 6c61 7373 6966 6965 7273  own..classifiers
-00000140: 203d 200d 0a09 496e 7465 6e64 6564 2041   = ...Intended A
-00000150: 7564 6965 6e63 6520 3a3a 2053 6369 656e  udience :: Scien
-00000160: 6365 2f52 6573 6561 7263 680d 0a09 546f  ce/Research...To
-00000170: 7069 6320 3a3a 2053 6369 656e 7469 6669  pic :: Scientifi
-00000180: 632f 456e 6769 6e65 6572 696e 6720 3a3a  c/Engineering ::
-00000190: 2043 6865 6d69 7374 7279 0d0a 0945 6e76   Chemistry...Env
-000001a0: 6972 6f6e 6d65 6e74 203a 3a20 436f 6e73  ironment :: Cons
-000001b0: 6f6c 650d 0a09 4465 7665 6c6f 706d 656e  ole...Developmen
-000001c0: 7420 5374 6174 7573 203a 3a20 3420 2d20  t Status :: 4 - 
-000001d0: 4265 7461 0d0a 0950 726f 6772 616d 6d69  Beta...Programmi
-000001e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001f0: 7974 686f 6e20 3a3a 2033 0d0a 094c 6963  ython :: 3...Lic
-00000200: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-00000210: 6f76 6564 203a 3a20 4253 4420 4c69 6365  oved :: BSD Lice
-00000220: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
-00000230: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000240: 6570 656e 6465 6e74 0d0a 0d0a 5b6f 7074  ependent....[opt
-00000250: 696f 6e73 5d0d 0a70 7974 686f 6e5f 7265  ions]..python_re
-00000260: 7175 6972 6573 203d 203e 3d33 2e38 0d0a  quires = >=3.8..
-00000270: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
-00000280: 6461 7461 203d 2054 7275 650d 0a70 6163  data = True..pac
-00000290: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a0d  kages = find:...
-000002a0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-000002b0: 6573 2e66 696e 645d 0d0a 696e 636c 7564  es.find]..includ
-000002c0: 6520 3d20 7368 656c 7866 696c 650d 0a09  e = shelxfile...
-000002d0: 7368 656c 7866 696c 652e 2a0d 0a65 7863  shelxfile.*..exc
-000002e0: 6c75 6465 203d 2073 6372 6970 7473 0d0a  lude = scripts..
-000002f0: 0974 6573 7473 0d0a 0974 6573 7473 2e2a  .tests...tests.*
-00000300: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000310: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000320: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 7368 656c 7866 696c 650a 7665 7273  = shelxfile.vers
+00000020: 696f 6e20 3d20 390a 6175 7468 6f72 203d  ion = 9.author =
+00000030: 2044 616e 6965 6c20 4b72 6174 7a65 7274   Daniel Kratzert
+00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
+00000050: 646b 7261 747a 6572 7440 676d 782e 6465  dkratzert@gmx.de
+00000060: 0a6c 6963 656e 7365 203d 2042 6565 7277  .license = Beerw
+00000070: 6172 6520 4c69 6365 6e73 650a 6465 7363  are License.desc
+00000080: 7269 7074 696f 6e20 3d20 4120 7061 7273  ription = A pars
+00000090: 6572 2066 6f72 2053 4845 4c58 4c20 7265  er for SHELXL re
+000000a0: 7375 6c74 7320 6669 6c65 732e 0a75 726c  sults files..url
+000000b0: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+000000c0: 622e 636f 6d2f 646b 7261 747a 6572 742f  b.com/dkratzert/
+000000d0: 5368 656c 5846 696c 650a 6c6f 6e67 5f64  ShelXFile.long_d
+000000e0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
+000000f0: 653a 2052 4541 444d 452e 6d64 0a6c 6f6e  e: README.md.lon
+00000100: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
+00000110: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
+00000120: 742f 6d61 726b 646f 776e 0a63 6c61 7373  t/markdown.class
+00000130: 6966 6965 7273 203d 200a 0949 6e74 656e  ifiers = ..Inten
+00000140: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+00000150: 5363 6965 6e63 652f 5265 7365 6172 6368  Science/Research
+00000160: 0a09 546f 7069 6320 3a3a 2053 6369 656e  ..Topic :: Scien
+00000170: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
+00000180: 6720 3a3a 2043 6865 6d69 7374 7279 0a09  g :: Chemistry..
+00000190: 456e 7669 726f 6e6d 656e 7420 3a3a 2043  Environment :: C
+000001a0: 6f6e 736f 6c65 0a09 4465 7665 6c6f 706d  onsole..Developm
+000001b0: 656e 7420 5374 6174 7573 203a 3a20 3420  ent Status :: 4 
+000001c0: 2d20 4265 7461 0a09 5072 6f67 7261 6d6d  - Beta..Programm
+000001d0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000001e0: 5079 7468 6f6e 203a 3a20 330a 094c 6963  Python :: 3..Lic
+000001f0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000200: 6f76 6564 203a 3a20 4253 4420 4c69 6365  oved :: BSD Lice
+00000210: 6e73 650a 094f 7065 7261 7469 6e67 2053  nse..Operating S
+00000220: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+00000230: 7065 6e64 656e 740a 0a5b 6f70 7469 6f6e  pendent..[option
+00000240: 735d 0a70 7974 686f 6e5f 7265 7175 6972  s].python_requir
+00000250: 6573 203d 203e 3d33 2e38 0a69 6e63 6c75  es = >=3.8.inclu
+00000260: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
+00000270: 3d20 5472 7565 0a70 6163 6b61 6765 7320  = True.packages 
+00000280: 3d20 6669 6e64 3a0a 0a5b 6f70 7469 6f6e  = find:..[option
+00000290: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+000002a0: 0a69 6e63 6c75 6465 203d 2073 6865 6c78  .include = shelx
+000002b0: 6669 6c65 0a09 7368 656c 7866 696c 652e  file..shelxfile.
+000002c0: 2a0a 6578 636c 7564 6520 3d20 7363 7269  *.exclude = scri
+000002d0: 7074 730a 0974 6573 7473 0a09 7465 7374  pts..tests..test
+000002e0: 732e 2a0a 0a5b 6567 675f 696e 666f 5d0a  s.*..[egg_info].
+000002f0: 7461 675f 6275 696c 6420 3d20 0a74 6167  tag_build = .tag
+00000300: 5f64 6174 6520 3d20 300a 0a              _date = 0..
```

### Comparing `shelxfile-8/shelxfile/atoms/atoms.py` & `shelxfile-9/shelxfile/atoms/atoms.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,224 +1,252 @@
-from math import acos, sqrt, degrees
-from typing import Union, List
-
-from shelxfile.atoms.atom import Atom
-from shelxfile.misc.dsrmath import atomic_distance, Array
-from shelxfile.misc.misc import DEBUG
-
-"""
-TODO:
-
-"""
-
-
-class Atoms():
-    """
-    All atoms from a SHELXL file with their properties.
-    """
-
-    def __init__(self, shx):
-        self.shx = shx
-        self.all_atoms: List[Atom] = []
-
-    def append(self, atom: 'Atom') -> None:
-        """
-        Adds a new atom to the list of atoms. Using append is essential.
-        """
-        self.all_atoms.append(atom)
-
-    @property
-    def nameslist(self):
-        return [at.fullname.upper() for at in self.all_atoms]
-
-    def __repr__(self) -> str:
-        if self.all_atoms:
-            return '\n'.join([str(x) for x in self.all_atoms])
-        else:
-            return 'No Atoms in file.'
-
-    def __iter__(self):
-        return iter(x for x in self.all_atoms)
-
-    def __getitem__(self, item: int) -> 'Atom':
-        return self.get_atom_by_id(item)
-
-    def __len__(self) -> int:
-        return len(self.all_atoms)
-
-    def __delitem__(self, key):
-        """
-        Delete an atom by its atomid:
-        del atoms[4]
-        """
-        for n, at in enumerate(self.all_atoms):
-            if key == at.atomid:
-                if DEBUG:
-                    print("deleting atom", at.fullname)
-                del self.all_atoms[n]
-                del self.shx._reslist[self.shx._reslist.index(at)]
-        # if DEBUG:
-        #    print('Could not delete atom {}'.format(self.get_atom_by_id(key.atomid).fullname))
-
-    @property
-    def atomsdict(self):
-        return dict((atom.fullname, atom) for atom in self.all_atoms)
-
-    @property
-    def number(self) -> int:
-        """
-        The number of atoms in the current SHELX file.
-        """
-        return len(self.all_atoms)
-
-    def get_atom_by_id(self, aid: int) -> Union['Atom', None]:
-        """
-        Returns the atom objext with atomId id.
-        """
-        for a in self.all_atoms:
-            if aid == a.atomid:
-                return a
-
-    def has_atom(self, atom_name: str) -> bool:
-        """
-        Returns true if shelx file has atom.
-        """
-        if '_' not in atom_name:
-            atom_name += '_0'
-        if atom_name.upper() in self.nameslist:
-            return True
-        else:
-            return False
-
-    def get_atom_by_name(self, atom_name: str) -> Union['Atom', None]:
-        """
-        Returns an Atom object using an atom name with residue number like C1, C1_0, F2_4, etc.
-        C1 means atom C1 in residue 0.
-        """
-        if '_' not in atom_name:
-            if atom_name == ">" or atom_name == "<":
-                return None
-            atom_name += '_0'
-        try:
-            at = self.atomsdict[atom_name.upper()]
-        except KeyError:
-            print("Atom {} not found in atom list.".format(atom_name))
-            return None
-        return at
-
-    def get_multi_atnames(self, atom_name, residue_class):
-        atoms = []
-        if residue_class:
-            for num in self.shx.residues.residue_classes[residue_class]:
-                if '_' not in atom_name:
-                    atom_name += '_0'
-                else:
-                    atom_name += '_{}'.format(num)
-                try:
-                    atoms.append(self.atomsdict[atom_name.upper()])
-                except KeyError:
-                    pass
-        else:
-            try:
-                atoms.append(self.atomsdict[atom_name.upper()])
-            except KeyError:
-                return None
-        return atoms
-
-    def get_all_atomcoordinates(self) -> dict:
-        """
-        Returns a dictionary {'C1': ['1.123', '0.7456', '3.245'], 'C2_2': ...}
-        """
-        atdict = {}
-        for at in self.all_atoms:
-            # if at.qpeak:
-            #    atdict[at.name] = at.frac_coords
-            # else:
-            atdict[at.name.upper() + '_' + str(at.resinum)] = at.frac_coords
-        return atdict
-
-    def get_frag_fend_atoms(self) -> list:
-        """
-        Returns a list of atoms with cartesian coordinates. Atom names and sfac are ignored. They come from AFIX 17x.
-        [[0.5316439256202359, 7.037351406500001, 10.112963255220803],
-        [-1.7511017452002604, 5.461541059000001, 10.01187984858907]]
-        """
-        atoms = []
-        for at in self.all_atoms:
-            if at.frag_atom:
-                atoms.append([at.xc, at.yc, at.zc])
-        return atoms
-
-    @property
-    def residues(self) -> list:
-        """
-        Returns a list of the residue numbers in the shelx file.
-        """
-        return list(set([x.resinum for x in self.all_atoms]))
-
-    @property
-    def q_peaks(self) -> list:
-        r"""
-        Returns a list of q-peaks in the file.
-        """
-        return [x for x in self.all_atoms if x.qpeak]
-
-    def distance(self, atom1: str, atom2: str) -> float:
-        """
-        Calculates the (shortest) distance of two atoms given as text names e.g. C1_3.
-        """
-        a1 = self.get_atom_by_name(atom1)
-        a2 = self.get_atom_by_name(atom2)
-        try:
-            return atomic_distance([a1.xc, a1.yc, a1.zc], [a2.xc, a2.yc, a2.zc])
-        except AttributeError:
-            return 0.0
-
-    def angle(self, at1: 'Atom', at2: 'Atom', at3: 'Atom') -> float:
-        """
-        Calculates the angle between three atoms.
-        """
-        ac1 = Array(at1.cart_coords)
-        ac2 = Array(at2.cart_coords)
-        ac3 = Array(at3.cart_coords)
-        vec1 = ac2 - ac1
-        vec2 = ac2 - ac3
-        return vec1.angle(vec2)
-
-    def torsion_angle(self, at1: 'Atom', at2: 'Atom', at3: 'Atom', at4: 'Atom') -> float:
-        """
-        Calculates the torsion angle (dieder angle) between four atoms.
-
-        From the book of Camelo Giacovazzo:
-        For a sequence of four atoms A, B, C, D, the torsion angle w(ABCD) is
-        defined as the angle between the normals to the planes ABC and BCD.
-        By convention w is positive if the sense of rotation from BA to
-        CD, viewed down BC, is clockwise, otherwise it is negative.
-        """
-        ac1 = Array(at1.cart_coords)
-        ac2 = Array(at2.cart_coords)
-        ac3 = Array(at3.cart_coords)
-        ac4 = Array(at4.cart_coords)
-        # Three vectors between four atoms:
-        v1 = ac2 - ac1
-        v2 = ac3 - ac2
-        v3 = ac4 - ac3
-        # cross product:
-        a = v1.cross(v2)
-        b = v2.cross(v3)
-        # If direction > 0, angle is positive, else negative:
-        direction = v1[0] * v2[1] * v3[2] - v1[2] * v1[1] * v3[0] + v1[2] * v2[0] * v3[1] - v1[0] \
-                    * v2[2] * v3[1] + v1[1] * v2[2] * v3[0] - v1[1] * v2[0] * v3[2]
-        # angle between plane normals:
-        ang = acos((a[0] * b[0] + a[1] * b[1] + a[2] * b[2]) / (
-                sqrt(a[0] * a[0] + a[1] * a[1] + a[2] * a[2]) * sqrt(b[0] * b[0] + b[1] * b[1] + b[2] * b[2])))
-        return degrees(ang) if direction > 0 else degrees(-ang)
-
-    def atoms_in_class(self, name: str) -> list:
-        """
-        Returns a list of atoms in residue class 'name'
-        """
-        atoms = []
-        for x in self.all_atoms:
-            if x.resiclass == name and x.name not in atoms:
-                atoms.append(x.name)
-        return atoms
+from math import acos, sqrt, degrees
+from typing import Union, List
+
+from shelxfile.atoms.atom import Atom
+from shelxfile.misc.dsrmath import atomic_distance, Array
+from shelxfile.misc.misc import DEBUG
+
+"""
+TODO:
+
+"""
+
+
+class Atoms():
+    """
+    All atoms from a SHELXL file with their properties.
+    """
+
+    def __init__(self, shx):
+        self.shx = shx
+        self.all_atoms: List[Atom] = []
+
+    def append(self, atom: 'Atom') -> None:
+        """
+        Adds a new atom to the list of atoms. Using append is essential.
+        """
+        self.all_atoms.append(atom)
+
+    @property
+    def nameslist(self):
+        return [at.fullname.upper() for at in self.all_atoms]
+
+    def __repr__(self) -> str:
+        if self.all_atoms:
+            return '\n'.join([str(x) for x in self.all_atoms])
+        else:
+            return 'No Atoms in file.'
+
+    def __iter__(self):
+        return iter(x for x in self.all_atoms)
+
+    def __getitem__(self, item: int) -> 'Atom':
+        return self.get_atom_by_id(item)
+
+    def __len__(self) -> int:
+        return len(self.all_atoms)
+
+    def __delitem__(self, key):
+        """
+        Delete an atom by its atomid:
+        del atoms[4]
+        """
+        for n, at in enumerate(self.all_atoms):
+            if key == at.atomid:
+                if DEBUG:
+                    print("deleting atom", at.fullname)
+                del self.all_atoms[n]
+                del self.shx._reslist[self.shx._reslist.index(at)]
+        # if DEBUG:
+        #    print('Could not delete atom {}'.format(self.get_atom_by_id(key.atomid).fullname))
+
+    @property
+    def atomsdict(self):
+        return dict((atom.fullname, atom) for atom in self.all_atoms)
+
+    @property
+    def number(self) -> int:
+        """
+        The number of atoms in the current SHELX file.
+        """
+        return len(self.all_atoms)
+
+    def get_atom_by_id(self, aid: int) -> Union['Atom', None]:
+        """
+        Returns the atom objext with atomId id.
+        """
+        for a in self.all_atoms:
+            if aid == a.atomid:
+                return a
+
+    def has_atom(self, atom_name: str) -> bool:
+        """
+        Returns true if shelx file has atom.
+        """
+        if '_' not in atom_name:
+            atom_name += '_0'
+        if atom_name.upper() in self.nameslist:
+            return True
+        else:
+            return False
+
+    def get_atom_by_name(self, atom_name: str) -> Union['Atom', None]:
+        """
+        Returns an Atom object using an atom name with residue number like C1, C1_0, F2_4, etc.
+        C1 means atom C1 in residue 0.
+        """
+        if '_' not in atom_name:
+            if atom_name == ">" or atom_name == "<":
+                return None
+            atom_name += '_0'
+        try:
+            at = self.atomsdict[atom_name.upper()]
+        except KeyError:
+            print("Atom {} not found in atom list.".format(atom_name))
+            return None
+        return at
+
+    def get_multi_atnames(self, atom_name, residue_class):
+        atoms = []
+        if residue_class:
+            for num in self.shx.residues.residue_classes[residue_class]:
+                if '_' not in atom_name:
+                    atom_name += '_0'
+                else:
+                    atom_name += '_{}'.format(num)
+                try:
+                    atoms.append(self.atomsdict[atom_name.upper()])
+                except KeyError:
+                    pass
+        else:
+            try:
+                atoms.append(self.atomsdict[atom_name.upper()])
+            except KeyError:
+                return None
+        return atoms
+
+    def get_all_atomcoordinates(self) -> dict:
+        """
+        Returns a dictionary {'C1': ['1.123', '0.7456', '3.245'], 'C2_2': ...}
+        """
+        atdict = {}
+        for at in self.all_atoms:
+            # if at.qpeak:
+            #    atdict[at.name] = at.frac_coords
+            # else:
+            atdict[at.name.upper() + '_' + str(at.resinum)] = at.frac_coords
+        return atdict
+
+    def get_frag_fend_atoms(self) -> list:
+        """
+        Returns a list of atoms with cartesian coordinates. Atom names and sfac are ignored. They come from AFIX 17x.
+        [[0.5316439256202359, 7.037351406500001, 10.112963255220803],
+        [-1.7511017452002604, 5.461541059000001, 10.01187984858907]]
+        """
+        atoms = []
+        for at in self.all_atoms:
+            if at.frag_atom:
+                atoms.append([at.xc, at.yc, at.zc])
+        return atoms
+
+    @property
+    def hydrogen_atoms(self) -> List[Atom]:
+        return [x for x in self.shx.atoms.all_atoms if x.is_hydrogen]
+
+    @property
+    def n_hydrogen_atoms(self) -> int:
+        return len(self.hydrogen_atoms)
+
+    @property
+    def n_anisotropic_atoms(self) -> int:
+        return len([x for x in self.all_atoms if sum(x.uvals[1:]) > 0.00001])
+
+    @property
+    def n_isotropic_atoms(self) -> int:
+        return len([x for x in self.all_atoms if sum(x.uvals[1:]) == 0.0])
+
+    @property
+    def n_anisotropic_hydrogen_atoms(self) -> int:
+        return len([x for x in self.hydrogen_atoms if sum(x.uvals[1:]) > 0.0001])
+
+    @property
+    def n_hydrogen_atoms_with_constr_u_val(self) -> int:
+        return len([x for x in self.hydrogen_atoms if x.uvals[0] < -1.0])
+
+    @property
+    def riding_atoms(self) -> List[Atom]:
+        return [x for x in self.hydrogen_atoms if x.afix]
+
+    @property
+    def residues(self) -> list:
+        """
+        Returns a list of the residue numbers in the shelx file.
+        """
+        return list(set([x.resinum for x in self.all_atoms]))
+
+    @property
+    def q_peaks(self) -> list:
+        r"""
+        Returns a list of q-peaks in the file.
+        """
+        return [x for x in self.all_atoms if x.qpeak]
+
+    def distance(self, atom1: str, atom2: str) -> float:
+        """
+        Calculates the (shortest) distance of two atoms given as text names e.g. C1_3.
+        """
+        a1 = self.get_atom_by_name(atom1)
+        a2 = self.get_atom_by_name(atom2)
+        try:
+            return atomic_distance([a1.xc, a1.yc, a1.zc], [a2.xc, a2.yc, a2.zc])
+        except AttributeError:
+            return 0.0
+
+    def angle(self, at1: 'Atom', at2: 'Atom', at3: 'Atom') -> float:
+        """
+        Calculates the angle between three atoms.
+        """
+        ac1 = Array(at1.cart_coords)
+        ac2 = Array(at2.cart_coords)
+        ac3 = Array(at3.cart_coords)
+        vec1 = ac2 - ac1
+        vec2 = ac2 - ac3
+        return vec1.angle(vec2)
+
+    def torsion_angle(self, at1: 'Atom', at2: 'Atom', at3: 'Atom', at4: 'Atom') -> float:
+        """
+        Calculates the torsion angle (dieder angle) between four atoms.
+
+        From the book of Camelo Giacovazzo:
+        For a sequence of four atoms A, B, C, D, the torsion angle w(ABCD) is
+        defined as the angle between the normals to the planes ABC and BCD.
+        By convention w is positive if the sense of rotation from BA to
+        CD, viewed down BC, is clockwise, otherwise it is negative.
+        """
+        ac1 = Array(at1.cart_coords)
+        ac2 = Array(at2.cart_coords)
+        ac3 = Array(at3.cart_coords)
+        ac4 = Array(at4.cart_coords)
+        # Three vectors between four atoms:
+        v1 = ac2 - ac1
+        v2 = ac3 - ac2
+        v3 = ac4 - ac3
+        # cross product:
+        a = v1.cross(v2)
+        b = v2.cross(v3)
+        # If direction > 0, angle is positive, else negative:
+        direction = v1[0] * v2[1] * v3[2] - v1[2] * v1[1] * v3[0] + v1[2] * v2[0] * v3[1] - v1[0] \
+                    * v2[2] * v3[1] + v1[1] * v2[2] * v3[0] - v1[1] * v2[0] * v3[2]
+        # angle between plane normals:
+        ang = acos((a[0] * b[0] + a[1] * b[1] + a[2] * b[2]) / (
+                sqrt(a[0] * a[0] + a[1] * a[1] + a[2] * a[2]) * sqrt(b[0] * b[0] + b[1] * b[1] + b[2] * b[2])))
+        return degrees(ang) if direction > 0 else degrees(-ang)
+
+    def atoms_in_class(self, name: str) -> list:
+        """
+        Returns a list of atoms in residue class 'name'
+        """
+        atoms = []
+        for x in self.all_atoms:
+            if x.resiclass == name and x.name not in atoms:
+                atoms.append(x.name)
+        return atoms
```

### Comparing `shelxfile-8/shelxfile/draw/draw_molecule.py` & `shelxfile-9/shelxfile/draw/draw_molecule.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-from __future__ import division
-
-import sys
-import time
-from math import sin, cos, pi, sqrt
-
-from shelxfile import Shelxfile
-from shelxfile.atoms.atoms import Atoms
-
-"""
-This module is a fork from https://github.com/des4maisons/molecule-viewer
-"""
-
-
-class Coordinate2D(object):
-    def __init__(self, x, y):
-        self.x = x
-        self.y = y
-
-    def __mul__(self, const):
-        return Coordinate2D(self.x * const, self.y * const)
-
-    def __add__(self, coor):
-        return Coordinate2D(self.x + coor.x, self.y + coor.y)
-
-    def __sub__(self, coor):
-        return self + coor * (-1)
-
-    def __truediv__(self, const):
-        return self * (1 / const)
-
-    def __repr__(self):
-        return "(%.02f, %.02f)" % (self.x, self.y)
-
-    def __str__(self):
-        return self.__repr__()
-
-
-class Atom(object):
-    def __init__(self, x, y, z, symbol, id):
-        self.coordinate = Coordinate(x, y, z)
-        self.symbol = symbol
-        self.id = int(id)
-
-    def __repr__(self):
-        return str((self.symbol, self.id, self.coordinate))
-
-    def __str__(self):
-        return self.__repr__()
-
-    def flatten(self, plane=None):
-        return self.coordinate.flatten(plane)
-
-    # Ugly! return symbol in a randomish ansi colour
-    def coloured_symbol(self):
-        return "\x1b[" + str(31 + (self.id % 7)) + "m" + self.symbol
-
-
-class Coordinate(object):
-    def __init__(self, x, y, z):
-        self.x, self.y, self.z = [x, y, z]
-
-    def __repr__(self):
-        return "(%.02f, %.02f, %.02f)" % (self.x, self.y, self.z)
-
-    def __str__(self):
-        return self.__repr__()
-
-    def __truediv__(self, const):
-        return self * (1 / const)
-
-    def __mul__(self, const):
-        return Coordinate(self.x * const, self.y * const, self.z * const)
-
-    def __add__(self, coor):
-        return Coordinate(self.x + coor.x, self.y + coor.y, self.z + coor.z)
-
-    # regular dot product
-    def dot(self, vector):
-        return self.x * vector.x + self.y * vector.y + self.z * vector.z
-
-    def length(self):
-        return sqrt((self.x ** 2) + (self.y ** 2) + (self.z ** 2))
-
-    # project self onto 'onto'
-    def project(self, onto):
-        length = onto.length()
-        scale_factor = self.dot(onto) / (length ** 2)
-        return onto * scale_factor
-
-    # cross product
-    def cross(self, vector):
-        a1, a2, a3 = [self.x, self.y, self.z]
-        b1, b2, b3 = [vector.x, vector.y, vector.z]
-        return Coordinate(a2 * b3 - a3 * b2,
-                          a3 * b1 - a1 * b3,
-                          a1 * b2 - a2 * b1)
-
-    # flatten takes a 2-element list of coordinates. When interpreted as vectors,
-    # these define a plane in 3-dim'l space
-    def flatten(self, plane=None):
-        if plane is None:  # defaults to x-y plane
-            plane = [Coordinate(1, 0, 0), Coordinate(0, 1, 0)]
-        # copy the list
-        plane = list(plane)
-        # get 2 perpendicular vectors that define the same plane
-        perp = plane[0].cross(plane[1])
-        plane[0] = perp.cross(plane[1])
-        # make them unit vectors
-        plane[0] = plane[0] / (plane[0].length())
-        plane[1] = plane[1] / (plane[1].length())
-
-        proj0 = self.project(plane[0])
-        proj1 = self.project(plane[1])
-        ratio0 = None
-        ratio1 = None
-        # the (signed) number of times the unit vector fits into the projection
-        # is the 2 dimensional coordinate we want
-        # so (2,0) == 2 * (1,0), 2 is what we want. don't divide by zero.
-        for component in ["x", "y", "z"]:
-            val = getattr(plane[0], component)
-            if val != 0:
-                ratio0 = getattr(proj0, component) / val
-            val = getattr(plane[1], component)
-            if val != 0:
-                ratio1 = getattr(proj1, component) / val
-        if ratio0 is None or ratio1 is None:  # if either are 0
-            raise ValueError("plane defined with zero vector")
-        return Coordinate2D(ratio0, ratio1)
-
-
-class Molecule(object):
-    def __init__(self, shx_atoms: Atoms):
-        self.atoms = []
-        for at in shx_atoms:
-            self.atoms.append(Atom(at.x, at.y, at.z, at.name, at.resinum))
-
-    def parse_atom(self, str):
-        atype, seqnum, elt, one, x, y, z, who, cares = str.split()
-        self.atoms.append(Atom(float(x), float(y), float(z), elt, int(seqnum)))
-
-    # dimensions is 2-tuple of the number of characters on x and y axis
-    def draw(self, plane=None, dimensions=None):
-        if dimensions is None:
-            dimensions = (80, 29)
-        screen = Screen(dimensions)
-        flattened = [a.flatten(plane) for a in self.atoms]
-        max_extreme = Coordinate2D(max([coor.x for coor in flattened]),
-                                   max([coor.y for coor in flattened]))
-        min_extreme = Coordinate2D(min([coor.x for coor in flattened]),
-                                   min([coor.y for coor in flattened]))
-        span = max_extreme - min_extreme
-        # make everything fit in our dimensions while maintaining proportions
-        scale_factor = min((screen.width - 1) / span.x, (screen.height - 1) / span.y)
-        extra_space = Coordinate2D(screen.width - 1, screen.height - 1) - span * scale_factor
-        offset = extra_space / 2
-        for atom in self.atoms:
-            # shift to be in the 1st quadrant (positive coordinates) close to (0,0)
-            screen_index = (atom.flatten(plane) - min_extreme) * scale_factor
-            screen_index = screen_index + offset
-            screen_index = (int(round(screen_index.x)), int(round(screen_index.y)))
-            screen.set(screen_index, atom.coloured_symbol())
-        screen.show()
-
-
-class Screen(list):
-    def __init__(self, widthheight):
-        list.__init__(self)
-        self.width = widthheight[1]
-        self.height = widthheight[0]
-        for i in range(self.width):
-            self.append([])
-            for _ in range(self.height):
-                self[i].append(" ")
-
-    def set(self, index, val):
-        x = index[0]
-        y = index[1]
-        self[x][y] = val
-
-    def show(self):
-        for row in self:
-            print("".join(row))
-
-
-if __name__ == "__main__":
-    shx = Shelxfile()
-    shx.read_file('./tests/resources/p21c.res')
-    try:
-        width = sys.argv[2]
-        height = sys.argv[3]
-        dims = (int(width), int(height) - 1)
-    except IndexError:
-        dims = None
-    angle = 0
-    angle_incr = (2 * pi) * (1 / 40)  # 40th of a circle
-    while True:
-        Molecule(shx.atoms).draw(plane=[Coordinate(0, 1, 0), Coordinate(sin(angle), 0, cos(angle))], dimensions=dims)
-        angle = angle + angle_incr
-        time.sleep(0.5)
-        print("\33[H")
+from __future__ import division
+
+import sys
+import time
+from math import sin, cos, pi, sqrt
+
+from shelxfile import Shelxfile
+from shelxfile.atoms.atoms import Atoms
+
+"""
+This module is a fork from https://github.com/des4maisons/molecule-viewer
+"""
+
+
+class Coordinate2D(object):
+    def __init__(self, x, y):
+        self.x = x
+        self.y = y
+
+    def __mul__(self, const):
+        return Coordinate2D(self.x * const, self.y * const)
+
+    def __add__(self, coor):
+        return Coordinate2D(self.x + coor.x, self.y + coor.y)
+
+    def __sub__(self, coor):
+        return self + coor * (-1)
+
+    def __truediv__(self, const):
+        return self * (1 / const)
+
+    def __repr__(self):
+        return "(%.02f, %.02f)" % (self.x, self.y)
+
+    def __str__(self):
+        return self.__repr__()
+
+
+class Atom(object):
+    def __init__(self, x, y, z, symbol, id):
+        self.coordinate = Coordinate(x, y, z)
+        self.symbol = symbol
+        self.id = int(id)
+
+    def __repr__(self):
+        return str((self.symbol, self.id, self.coordinate))
+
+    def __str__(self):
+        return self.__repr__()
+
+    def flatten(self, plane=None):
+        return self.coordinate.flatten(plane)
+
+    # Ugly! return symbol in a randomish ansi colour
+    def coloured_symbol(self):
+        return "\x1b[" + str(31 + (self.id % 7)) + "m" + self.symbol
+
+
+class Coordinate(object):
+    def __init__(self, x, y, z):
+        self.x, self.y, self.z = [x, y, z]
+
+    def __repr__(self):
+        return "(%.02f, %.02f, %.02f)" % (self.x, self.y, self.z)
+
+    def __str__(self):
+        return self.__repr__()
+
+    def __truediv__(self, const):
+        return self * (1 / const)
+
+    def __mul__(self, const):
+        return Coordinate(self.x * const, self.y * const, self.z * const)
+
+    def __add__(self, coor):
+        return Coordinate(self.x + coor.x, self.y + coor.y, self.z + coor.z)
+
+    # regular dot product
+    def dot(self, vector):
+        return self.x * vector.x + self.y * vector.y + self.z * vector.z
+
+    def length(self):
+        return sqrt((self.x ** 2) + (self.y ** 2) + (self.z ** 2))
+
+    # project self onto 'onto'
+    def project(self, onto):
+        length = onto.length()
+        scale_factor = self.dot(onto) / (length ** 2)
+        return onto * scale_factor
+
+    # cross product
+    def cross(self, vector):
+        a1, a2, a3 = [self.x, self.y, self.z]
+        b1, b2, b3 = [vector.x, vector.y, vector.z]
+        return Coordinate(a2 * b3 - a3 * b2,
+                          a3 * b1 - a1 * b3,
+                          a1 * b2 - a2 * b1)
+
+    # flatten takes a 2-element list of coordinates. When interpreted as vectors,
+    # these define a plane in 3-dim'l space
+    def flatten(self, plane=None):
+        if plane is None:  # defaults to x-y plane
+            plane = [Coordinate(1, 0, 0), Coordinate(0, 1, 0)]
+        # copy the list
+        plane = list(plane)
+        # get 2 perpendicular vectors that define the same plane
+        perp = plane[0].cross(plane[1])
+        plane[0] = perp.cross(plane[1])
+        # make them unit vectors
+        plane[0] = plane[0] / (plane[0].length())
+        plane[1] = plane[1] / (plane[1].length())
+
+        proj0 = self.project(plane[0])
+        proj1 = self.project(plane[1])
+        ratio0 = None
+        ratio1 = None
+        # the (signed) number of times the unit vector fits into the projection
+        # is the 2 dimensional coordinate we want
+        # so (2,0) == 2 * (1,0), 2 is what we want. don't divide by zero.
+        for component in ["x", "y", "z"]:
+            val = getattr(plane[0], component)
+            if val != 0:
+                ratio0 = getattr(proj0, component) / val
+            val = getattr(plane[1], component)
+            if val != 0:
+                ratio1 = getattr(proj1, component) / val
+        if ratio0 is None or ratio1 is None:  # if either are 0
+            raise ValueError("plane defined with zero vector")
+        return Coordinate2D(ratio0, ratio1)
+
+
+class Molecule(object):
+    def __init__(self, shx_atoms: Atoms):
+        self.atoms = []
+        for at in shx_atoms:
+            self.atoms.append(Atom(at.x, at.y, at.z, at.name, at.resinum))
+
+    def parse_atom(self, str):
+        atype, seqnum, elt, one, x, y, z, who, cares = str.split()
+        self.atoms.append(Atom(float(x), float(y), float(z), elt, int(seqnum)))
+
+    # dimensions is 2-tuple of the number of characters on x and y axis
+    def draw(self, plane=None, dimensions=None):
+        if dimensions is None:
+            dimensions = (80, 29)
+        screen = Screen(dimensions)
+        flattened = [a.flatten(plane) for a in self.atoms]
+        max_extreme = Coordinate2D(max([coor.x for coor in flattened]),
+                                   max([coor.y for coor in flattened]))
+        min_extreme = Coordinate2D(min([coor.x for coor in flattened]),
+                                   min([coor.y for coor in flattened]))
+        span = max_extreme - min_extreme
+        # make everything fit in our dimensions while maintaining proportions
+        scale_factor = min((screen.width - 1) / span.x, (screen.height - 1) / span.y)
+        extra_space = Coordinate2D(screen.width - 1, screen.height - 1) - span * scale_factor
+        offset = extra_space / 2
+        for atom in self.atoms:
+            # shift to be in the 1st quadrant (positive coordinates) close to (0,0)
+            screen_index = (atom.flatten(plane) - min_extreme) * scale_factor
+            screen_index = screen_index + offset
+            screen_index = (int(round(screen_index.x)), int(round(screen_index.y)))
+            screen.set(screen_index, atom.coloured_symbol())
+        screen.show()
+
+
+class Screen(list):
+    def __init__(self, widthheight):
+        list.__init__(self)
+        self.width = widthheight[1]
+        self.height = widthheight[0]
+        for i in range(self.width):
+            self.append([])
+            for _ in range(self.height):
+                self[i].append(" ")
+
+    def set(self, index, val):
+        x = index[0]
+        y = index[1]
+        self[x][y] = val
+
+    def show(self):
+        for row in self:
+            print("".join(row))
+
+
+if __name__ == "__main__":
+    shx = Shelxfile()
+    shx.read_file('./tests/resources/p21c.res')
+    try:
+        width = sys.argv[2]
+        height = sys.argv[3]
+        dims = (int(width), int(height) - 1)
+    except IndexError:
+        dims = None
+    angle = 0
+    angle_incr = (2 * pi) * (1 / 40)  # 40th of a circle
+    while True:
+        Molecule(shx.atoms).draw(plane=[Coordinate(0, 1, 0), Coordinate(sin(angle), 0, cos(angle))], dimensions=dims)
+        angle = angle + angle_incr
+        time.sleep(0.5)
+        print("\33[H")
```

### Comparing `shelxfile-8/shelxfile/misc/dsrmath.py` & `shelxfile-9/shelxfile/misc/dsrmath.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,853 +1,853 @@
-# -*- encoding: utf-8 -*-
-# möp
-#
-# ----------------------------------------------------------------------------
-# "THE BEER-WARE LICENSE" (Revision 42):
-# <dkratzert@gmx.de> wrote this file. As long as you retain
-# this notice you can do whatever you want with this stuff. If we meet some day,
-# and you think this stuff is worth it, you can buy me a beer in return.
-# Daniel Kratzert
-# ----------------------------------------------------------------------------
-#
-import random
-import string
-from math import sqrt, radians, cos, sin, acos, degrees, floor, tan
-from operator import sub, add
-from typing import List, Union
-
-from shelxfile.misc.misc import flatten, determinante
-
-
-class Array(object):
-    """
-    MIT License
-
-    Copyright (c) 2018 Jens Luebben
-
-    Permission is hereby granted, free of charge, to any person obtaining a copy
-    of this software and associated documentation files (the "Software"), to deal
-    in the Software without restriction, including without limitation the rights
-    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-    copies of the Software, and to permit persons to whom the Software is
-    furnished to do so, subject to the following conditions:
-
-    The above copyright notice and this permission notice shall be included in all
-    copies or substantial portions of the Software.
-    """
-    __slots__ = ['values']
-
-    def __init__(self, values: Union[list, tuple]):
-        self.values = values
-
-    def __iter__(self) -> iter:
-        for v in self.values:
-            yield v
-
-    def __len__(self) -> int:
-        return len(self.values)
-
-    def __hash__(self):
-        return hash(self.values)
-
-    def __add__(self, other: (list, 'Array')) -> 'Array':
-        """
-        This method is optimized for speed.
-        """
-        if isinstance(other, Array):
-            return Array(list(map(add, self.values, other)))
-        elif type(other) == float or type(other) == int:
-            # return Array( list(map(lambda x: x - other, self.values)) )
-            return Array([i + other for i in self.values])
-        else:
-            raise TypeError('Cannot add type Array to type {}.'.format(str(type(other))))
-
-    def __iadd__(self, other):
-        return self.__add__(other)
-
-    def __eq__(self, other):
-        """
-        Test for equality.
-        """
-        return all([a == b for (a, b) in zip(self.values, other.values)])
-
-    def __sub__(self, other):
-        """
-        Subtracts eiter an Array or a value from the self Array.
-        This method is optimized for speed.
-        """
-        if isinstance(other, Array):
-            return Array(list(map(sub, self.values, other)))  # slightly faster
-        elif isinstance(other, float) or isinstance(other, int):
-            return Array([i - other for i in self.values])
-        else:
-            raise TypeError('Cannot add type Array to type {}.'.format(str(type(other))))
-
-    def __imul__(self, other):
-        """
-        Currently supports multiplication by a number.
-        __imul__ means a *= b
-        """
-        if isinstance(other, (int, float)):
-            self.values = [v * other for v in self.values]
-            return self
-        else:
-            raise TypeError('Unsupported operation.')
-
-    def __mul__(self, other: ('Array', 'Matrix')) -> (float, 'Array'):
-        """
-        Calculates: a * b = axbx + ayby + azbz
-        """
-        if isinstance(other, Matrix):
-            # Array() * Matrix()
-            a = other[0]
-            b = other[1]
-            c = other[2]
-            x = self.values[0] * a[0] + self.values[1] * b[0] + self.values[2] * c[0]
-            y = self.values[0] * a[1] + self.values[1] * b[1] + self.values[2] * c[1]
-            z = self.values[0] * a[2] + self.values[1] * b[2] + self.values[2] * c[2]
-            return Array([x, y, z])
-        else:
-            return self.dot(other)
-
-    def __repr__(self):
-        return 'Array({})'.format(str(self.values))
-
-    def __getitem__(self, val):
-        """
-        Get one item from the array.
-        """
-        return self.values[val]
-
-    def __setitem__(self, pos, val):
-        """
-        Get one item from the array.
-        """
-        self.values[pos] = val
-
-    def norm(self):
-        """
-        The squared lenght of an array
-        """
-        return sum([n ** 2 for n in self.values])
-
-    def normalized(self):
-        """
-        Euclidean norm (straight-line distance) of a vector array.
-        """
-        return sqrt(self.norm())
-
-    @staticmethod
-    def zero(m: int) -> 'Array':
-        """
-        Create zero Array of dimension m
-        """
-        return Array([0.0 for _ in range(m)])
-
-    @staticmethod
-    def randarray(m: int) -> 'Array':
-        """
-        Create random Array of dimension m
-        """
-        return Array([random.randint(1, 9) for _ in range(m)])
-
-    @property
-    def floor(self):
-        return Array(list(map(floor, self.values)))
-
-    def dot(self, other: 'Array') -> float:
-        """
-        Dot product of an array in kartesian space.
-        """
-        if len(self) != len(other):
-            raise ValueError('Vector sizes must match')
-        return sum([i * j for i, j in zip(self, other)])
-
-    def cross(self, other: 'Array') -> 'Array':
-        """
-        Cross product of the Array (currently only for 3D vectors).
-        """
-        if len(self) != len(other) != 3:
-            raise ValueError('For 3D vectors only')
-        a1, a2, a3 = self
-        b1, b2, b3 = other
-        return Array([(a2 * b3 - a3 * b2), (a3 * b1 - a1 * b3), (a1 * b2 - a2 * b1)])
-
-    def angle(self, other: 'Array') -> float:
-        """
-        Calculates the angle between two vectors.
-        """
-        return round(degrees(acos(self.dot(other) / (self.normalized() * other.normalized()))), 9)
-
-
-class Matrix(object):
-    """
-    MIT License
-
-    Copyright (c) 2018 Jens Luebben
-
-    Permission is hereby granted, free of charge, to any person obtaining a copy
-    of this software and associated documentation files (the "Software"), to deal
-    in the Software without restriction, including without limitation the rights
-    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-    copies of the Software, and to permit persons to whom the Software is
-    furnished to do so, subject to the following conditions:
-
-    The above copyright notice and this permission notice shall be included in all
-    copies or substantial portions of the Software.
-
-    DK: Missing: inverse, eigenvalues
-    """
-    __slots__ = ['values', 'shape']
-
-    def __init__(self, values):
-        self.shape = (len(values[0]), len(values))
-        self.values = values
-
-    def __getitem__(self, val):
-        """
-        """
-        if isinstance(val, (tuple, list)):
-            if len(val) == 1:
-                return self.values[val[0]]
-            return self.values[val[1]][val[0]]
-        else:
-            return self.values[val]
-
-    def __repr__(self):
-        rows = ''
-        for row in self.values:
-            rows += '|' + ' '.join(['{:>7.4f}'.format(float(x)) for x in row]) + '|' + '\n'
-        return rows
-
-    def __add__(self, other: (list, 'Matrix')) -> 'Matrix':
-        """
-        Matrix addition
-        """
-        if isinstance(other, Array):
-            if not len(self) == len(other):
-                raise ValueError('Matrix and Array are not of equal length.')
-            return Matrix(
-                [[sum(e1, e2) for e1, e2 in zip(row1, row2)] for row1, row2 in zip(self.values, other.values)])
-        elif isinstance(other, (float, int)):
-            return Matrix([[x + other for x in i] for i in self.values])
-        elif isinstance(other, Matrix):
-            return Matrix([[e1 + e2 for e1, e2 in zip(row1, row2)] for row1, row2 in zip(self.values, other.values)])
-        else:
-            raise TypeError('Cannot add type {} Array to Matrix.'.format(str(type(other))))
-
-    def __mul__(self, other: ('Matrix', 'Array', int, float)) -> ('Matrix', 'Array'):
-        """
-        a * b operation
-        """
-        if isinstance(other, (int, float)):
-            return Matrix([[v * other for v in row] for row in self.values])
-        elif isinstance(other, (Matrix, OrthogonalMatrix)):
-            return Matrix([[sum(ea * eb for ea, eb in zip(a, b)) for b in other.values] for a in self.values])
-        elif isinstance(other, Array):
-            return Array([sum([b * x for (b, x) in zip(other.values, row)]) for row in self.values])
-        else:
-            raise TypeError('Cannot add type {} to Matrix.'.format(str(type(other))))
-
-    def __len__(self):
-        return self.shape[1]
-
-    def __iter__(self) -> list:
-        return [n for n in self.values]
-
-    def __eq__(self, other):
-        """
-        Test for equality.
-        """
-        return all([b == x for (b, x) in zip(other.values, self.values)])
-
-    def __sub__(self, other):
-        """
-        Substract two matrices.
-        """
-        output = []
-        for idx in range(len(self)):
-            tmp = []
-            for val_a, val_b in zip(self[idx], other[idx]):
-                tmp.append(val_a - val_b)
-            output.append(tmp[:])
-        return output[:]
-
-    def __truediv__(self, other):
-        """
-        #>>> Matrix([[1, 2, 3], [1, 2, 3], [1, 2, 3]]) / Matrix([[1, 2, 3], [1, 2, 3], [1, 2, 3]])
-        A / B = A * A^-1
-        """
-        return NotImplementedError
-
-    def __setitem__(self, key, value):
-        # TODO: Implement setitem
-        pass
-
-    @property
-    def T(self):
-        return self.transposed
-
-    @property
-    def transposed(self) -> 'Matrix':
-        """
-        transposes a matrix
-        """
-        return Matrix(list(zip(*self.values)))
-
-    def transpose_alt(self):
-        """
-        Transposes the current matrix.
-        """
-        rows = []
-        for i in range(self.shape[0]):
-            rows.append([r[i] for r in self.values])
-        return Matrix(rows)
-
-    def dot(self, other):
-        """
-        Dot product of two matrices.
-        """
-        new_a = []
-        for i, col in enumerate(self.transposed.values):
-            s = sum([v * o for v, o in zip(col, other)])
-            new_a.append(s)
-        return Matrix(new_a)
-
-    @staticmethod
-    def zero(m: int, n: int) -> 'Matrix':
-        """
-        Create zero matrix of dimension m,n
-        """
-        return Matrix([[0.0 for _ in range(n)] for _ in range(m)])
-
-    @staticmethod
-    def randmat(m: int, n: int) -> 'Matrix':
-        """
-        Create random matrix of dimension m, n
-
-        #>>> Matrix.randmat(5, 3)
-        |  2.000   1.000   2.000|
-        |  8.000   1.000   2.000|
-        |  3.000   5.000   1.000|
-        |  4.000   1.000   9.000|
-        |  2.000   8.000   4.000|
-        <BLANKLINE>
-        """
-        return Matrix([[random.randint(1, 9) for y in range(n)] for x in range(m)])
-
-    def cholesky(self) -> 'Matrix':
-        """
-        """
-        L = Matrix.zero(*self.shape)
-        for i, (ai, li) in enumerate(zip(self.values, L.values)):
-            for j, lj in enumerate(L.values[:i + 1]):
-                s = sum(li[k] * lj[k] for k in range(j))
-                li[j] = sqrt(ai[i] - s) if (i == j) else (1.0 / lj[j] * (ai[j] - s))
-        return L
-
-    def norm(self):
-        return self.det
-
-    @property
-    def inversed(self) -> 'Matrix':
-        """
-        Inversion of 3 × 3 matrices
-         -0.812500    0.125000    0.187500
-          0.125000   -0.250000    0.125000
-          0.520833    0.125000   -0.145833
-        """
-        if self.shape != (3, 3):
-            raise ValueError('Inversion is only valid for 3x3 Matrix.')
-        d = self.det
-        m1, m2, m3, m4, m5, m6, m7, m8, m9 = flatten(self.values)
-        inv = Matrix([[(m5 * m9 - m6 * m8) / d, (m3 * m8 - m2 * m9) / d, (m2 * m6 - m3 * m5) / d],
-                      [(m6 * m7 - m4 * m9) / d, (m1 * m9 - m3 * m7) / d, (m3 * m4 - m1 * m6) / d],
-                      [(m4 * m8 - m5 * m7) / d, (m2 * m7 - m1 * m8) / d, (m1 * m5 - m2 * m4) / d]])
-        return inv
-
-    @property
-    def det(self):
-        """
-        Return determinant of 3x3 matrix.
-        """
-        return determinante(self.values)
-
-    def power_iteration(self, num_simulations=10):
-        """
-        Eigenvalue algorythm from https://en.wikipedia.org/wiki/Power_iteration
-        """
-        # Ideally choose a random vector
-        # To decrease the chance that our vector
-        # Is orthogonal to the eigenvector
-        b_k = Array.randarray(self.shape[1])
-
-        for _ in range(num_simulations):
-            # calculate the matrix-by-vector product Ab
-            b_k1 = self.dot(b_k)
-
-            # calculate the norm
-            b_k1_norm = b_k1.det
-
-            # re normalize the vector
-            b_k = b_k1 / b_k1_norm
-
-        return b_k
-
-
-class SymmetryElement(object):
-    """
-    Class representing a symmetry operation.
-    """
-    symm_id = 1
-    __slots__ = ['centric', 'symms', 'ID', 'matrix', 'trans', 'matrix_iter', 'trans_iter']
-
-    def __init__(self, symms, centric=False):
-        """
-        Constructor.
-        """
-        self.centric = centric
-        self.symms = symms
-        self.ID = SymmetryElement.symm_id
-        SymmetryElement.symm_id += 1
-        lines = []
-        trans = []
-        for symm in self.symms:
-            line, t = self._parse_line(symm)
-            lines.append(line)
-            trans.append(t)
-        self.matrix = Matrix(lines).transposed
-        self.trans = Array(trans)
-        self.matrix_iter = Matrix(lines).transposed.values
-        self.trans_iter = Array(trans).values
-        if centric:
-            self.matrix *= -1
-            self.trans *= -1
-
-    def __str__(self):
-        string = "|{aa:2} {ab:2} {ac:2}|   |{v:>4.2}|\n" \
-                 "|{ba:2} {bb:2} {bc:2}| + |{vv:>4.2}|\n" \
-                 "|{ca:2} {cb:2} {cc:2}|   |{vvv:>4.2}|\n".format(aa=self.matrix[0, 0],
-                                                                  ab=self.matrix[0, 1],
-                                                                  ac=self.matrix[0, 2],
-                                                                  ba=self.matrix[1, 0],
-                                                                  bb=self.matrix[1, 1],
-                                                                  bc=self.matrix[1, 2],
-                                                                  ca=self.matrix[2, 0],
-                                                                  cb=self.matrix[2, 1],
-                                                                  cc=self.matrix[2, 2],
-                                                                  v=float(self.trans[0]),
-                                                                  vv=float(self.trans[1]),
-                                                                  vvv=float(self.trans[2]))
-        return string
-
-    def __repr__(self):
-        return self.to_shelxl()
-
-    def __eq__(self, other):
-        """
-        Check two SymmetryElement instances for equivalence.
-        Note that differences in lattice translation are ignored.
-        :param other: SymmetryElement instance
-        :return: True/False
-        """
-        m = (self.matrix == other.matrix)
-        t1 = Array([v % 1 for v in self.trans])
-        t2 = Array([v % 1 for v in other.trans])
-        t = (t1 == t2)
-        return m and t
-
-    def __sub__(self, other):
-        """
-        Computes and returns the translational difference between two SymmetryElements. Returns 999.0 if the elements
-        cannot be superimposed via an integer shift of the translational parts.
-        :param other: SymmetryElement instance
-        :return: float
-        """
-        if not self == other:
-            return 999.
-        return self.trans - other.trans
-
-    def apply_latt_symm(self, latt_symm):
-        """
-        Copies SymmetryElement instance and returns the copy after applying the translational part of 'lattSymm'.
-        :param latt_symm: SymmetryElement.
-        :return: SymmetryElement.
-        """
-        new_symm = SymmetryElement(self.to_shelxl().split(','))
-        new_symm.trans = Array([(self.trans[0] + latt_symm.trans[0]) / 1,
-                                (self.trans[1] + latt_symm.trans[1]) / 1,
-                                (self.trans[2] + latt_symm.trans[2]) / 1])
-        new_symm.centric = self.centric
-        return new_symm
-
-    def to_shelxl(self):
-        """
-        Generate and return string representation of Symmetry Operation in Shelxl syntax.
-        :return: string.
-        """
-        axes = ['X', 'Y', 'Z']
-        lines = []
-        for i in range(3):
-            text = str(self.trans[i]) if self.trans[i] else ''
-            for j in range(3):
-                s = '' if not self.matrix[i, j] else axes[j]
-                if self.matrix[i, j] < 0:
-                    s = '-' + s
-                elif s:
-                    s = '+' + s
-                text += s
-            lines.append(text)
-        return ', '.join(lines)
-
-    def _parse_line(self, symm):
-        symm = symm.upper().replace(' ', '')
-        chars = ['X', 'Y', 'Z']
-        line = []
-        for char in chars:
-            element, symm = self._partition(symm, char)
-            line.append(element)
-        if symm:
-            trans = self._float(symm)
-        else:
-            trans = 0
-        return line, trans
-
-    def _float(self, string):
-        try:
-            return float(string)
-        except ValueError:
-            if '/' in string:
-                string = string.replace('/', './') + '.'
-                return eval('{}'.format(string))
-
-    def _partition(self, symm, char):
-        parts = symm.partition(char)
-        if parts[1]:
-            if parts[0]:
-                sign = parts[0][-1]
-            else:
-                sign = '+'
-            if sign == '-':
-                return -1, ''.join((parts[0][:-1], parts[2]))
-            else:
-                return 1, ''.join((parts[0], parts[2])).replace('+', '')
-        else:
-            return 0, symm
-
-
-# End of work by Jens Lübben #############
-
-
-def my_isnumeric(value: str):
-    """
-    Determines if a string can be converted to a number.
-    """
-    try:
-        float(value)
-    except ValueError:
-        return False
-    return True
-
-
-def mean(values):
-    """
-    returns mean value of a list of numbers
-    """
-    return sum(values) / float(len(values))
-
-
-def median(nums):
-    """
-    calculates the median of a list of numbers
-    """
-    ls = sorted(nums)
-    n = len(ls)
-    if n == 0:
-        raise ValueError("Need a non-empty iterable")
-    # for uneven list length:
-    elif n % 2 == 1:
-        # // is floordiv:
-        return ls[n // 2]
-    else:
-        return sum(ls[int(int(n) / 2 - 1):int(int(n) / 2 + 1)]) / 2.0
-
-
-def std_dev(data: List) -> float:
-    """
-    returns standard deviation of values rounded to pl decimal places
-    S = sqrt( (sum(x-xm)^2) / n-1 )
-    xm = sum(x)/n
-    :param data: list with integer or float values
-    """
-    if len(data) == 0:
-        return 0
-    K = data[0]
-    n = 0
-    summ = 0
-    sum_sqr = 0
-    for x in data:
-        n += 1
-        summ += x - K
-        sum_sqr += (x - K) * (x - K)
-    variance = (sum_sqr - (summ * summ) / n) / (n - 1)
-    # use n instead of (n-1) if want to compute the exact variance of the given data
-    # use (n-1) if data are samples of a larger population
-    return sqrt(variance)
-
-
-def nalimov_test(data):
-    """
-    returns a index list of outliers base on the Nalimov test for data.
-    Modified implementation of:
-    "R. Kaiser, G. Gottschalk, Elementare Tests zur Beurteilung von Messdaten
-    Bibliographisches Institut, Mannheim 1972."
-    """
-    # q-values for degrees of freedom:
-    f = {1 : 1.409, 2: 1.645, 3: 1.757, 4: 1.814, 5: 1.848, 6: 1.870, 7: 1.885, 8: 1.895,
-         9 : 1.903, 10: 1.910, 11: 1.916, 12: 1.920, 13: 1.923, 14: 1.926, 15: 1.928,
-         16: 1.931, 17: 1.933, 18: 1.935, 19: 1.936, 20: 1.937, 30: 1.945}
-    fact = sqrt(float(len(data)) / (len(data) - 1))
-    fval = len(data) - 2
-    if fval < 2:
-        return []
-    outliers = []
-    if fval in f:
-        # less strict than the original:
-        q_crit = f[fval]
-    else:
-        q_crit = 1.95
-    for num, i in enumerate(data):
-        q = abs(((i - median(data)) / std_dev(data)) * fact)
-        if q > q_crit:
-            outliers.append(num)
-    return outliers
-
-
-def id_generator(size=6, chars=string.ascii_uppercase + string.digits):
-    """
-    returns a random ID like 'L5J74W'
-    :param size: length of the string
-    :type size: integer
-    :param chars: characters used for the ID
-    :type chars: string
-    """
-    return ''.join(random.choice(chars) for _ in range(size))
-
-
-def atomic_distance(p1: list, p2: list, cell=None, shortest_dist=False):
-    """
-    p1 and p2 are x, y , z coordinates as list ['x', 'y', 'z']
-    cell are the cell parameters as list: ['a', 'b', 'c', 'alpha', 'beta', 'gamma']
-
-    Returns the distance between the two points (Atoms). If shortest_dist is True, the
-    shortest distance ignoring translation is computed.
-    """
-    a, b, c, al, be, ga = 1, 1, 1, 1, 1, 1
-    if cell:
-        a, b, c = cell[:3]
-        al = radians(cell[3])
-        be = radians(cell[4])
-        ga = radians(cell[5])
-    if shortest_dist:
-        x1, y1, z1 = [x + 99.5 for x in p1]
-        x2, y2, z2 = [x + 99.5 for x in p2]
-        dx = (x1 - x2) % 1 - 0.5
-        dy = (y1 - y2) % 1 - 0.5
-        dz = (z1 - z2) % 1 - 0.5
-    else:
-        x1, y1, z1 = p1
-        x2, y2, z2 = p2
-        dx = (x1 - x2)
-        dy = (y1 - y2)
-        dz = (z1 - z2)
-    if cell:
-        return sqrt((a * dx) ** 2 + (b * dy) ** 2 + (c * dz) ** 2 + 2 * b * c * cos(al) * dy * dz +
-                    2 * dx * dz * a * c * cos(be) + 2 * dx * dy * a * b * cos(ga))
-    else:
-        return sqrt(dx ** 2 + dy ** 2 + dz ** 2)
-
-
-def dice_coefficient(a, b, case_insens=True):
-    """
-    :type a: str
-    :type b: str
-    :type case_insens: bool
-    dice coefficient 2nt/na + nb.
-    https://en.wikibooks.org/wiki/Algorithm_Implementation/Strings/Dice%27s_coefficient#Python
-    """
-    if case_insens:
-        a = a.lower()
-        b = b.lower()
-    if not len(a) or not len(b):
-        return 0.0
-    if len(a) == 1:
-        a = a + u'.'
-    if len(b) == 1:
-        b = b + u'.'
-    a_bigram_list = []
-    for i in range(len(a) - 1):
-        a_bigram_list.append(a[i:i + 2])
-    b_bigram_list = []
-    for i in range(len(b) - 1):
-        b_bigram_list.append(b[i:i + 2])
-    a_bigrams = set(a_bigram_list)
-    b_bigrams = set(b_bigram_list)
-    overlap = len(a_bigrams & b_bigrams)
-    dice_coeff = overlap * 2.0 / (len(a_bigrams) + len(b_bigrams))
-    return round(dice_coeff, 6)
-
-
-def dice_coefficient2(a, b, case_insens=True):
-    """
-    :type a: str
-    :type b: str
-    :type case_insens: bool
-    duplicate bigrams in a word should be counted distinctly
-    (per discussion), otherwise 'AA' and 'AAAA' would have a
-    dice coefficient of 1...
-    https://en.wikibooks.org/wiki/Algorithm_Implementation/Strings/Dice%27s_coefficient#Python
-
-    This implementation is reverse. 1 means not hit, 0 means best match
-    """
-    if case_insens:
-        a = a.lower()
-        b = b.lower()
-    if not len(a) or not len(b):
-        return 1.0
-    # quick case for true duplicates
-    if a == b:
-        return 0.0
-    # if a != b, and a or b are single chars, then they can't possibly match
-    if len(a) == 1 or len(b) == 1:
-        return 1.0
-    # use python list comprehension, preferred over list.append()
-    a_bigram_list = [a[i:i + 2] for i in range(len(a) - 1)]
-    b_bigram_list = [b[i:i + 2] for i in range(len(b) - 1)]
-    a_bigram_list.sort()
-    b_bigram_list.sort()
-    # assignments to save function calls
-    lena = len(a_bigram_list)
-    lenb = len(b_bigram_list)
-    # initialize match counters
-    matches = i = j = 0
-    while i < lena and j < lenb:
-        if a_bigram_list[i] == b_bigram_list[j]:
-            matches += 2
-            i += 1
-            j += 1
-        elif a_bigram_list[i] < b_bigram_list[j]:
-            i += 1
-        else:
-            j += 1
-    score = float(matches) / float(lena + lenb)
-    score = 1 - score
-    return round(score, 6)
-
-
-def levenshtein(s1, s2):
-    """
-    The levensteins distance of two strings.
-    """
-    s1 = s1.lower()
-    s2 = s2.lower()
-    if len(s1) < len(s2):
-        return levenshtein(s2, s1)
-    if len(s2) == 0:
-        return len(s1)
-    previous_row = list(range(len(s2) + 1))
-    for i, c1 in enumerate(s1):
-        current_row = [i + 1]
-        for j, c2 in enumerate(s2):
-            # j+1 instead of j since previous_row and current_row are one character longer:
-            insertions = previous_row[j + 1] + 1
-            deletions = current_row[j] + 1  # than s2
-            substitutions = previous_row[j] + (c1 != c2)
-            current_row.append(min(insertions, deletions, substitutions))
-        previous_row = current_row
-    return previous_row[-1]
-
-
-def distance(x1, y1, z1, x2, y2, z2, round_out=False):
-    """
-    distance between two points in space for orthogonal axes.
-    """
-    import math as m
-    d = m.sqrt((x1 - x2) ** 2 + (y1 - y2) ** 2 + (z1 - z2) ** 2)
-    if round_out:
-        return round(d, round_out)
-    else:
-        return d
-
-
-def vol_unitcell(a, b, c, al, be, ga):
-    """
-    calculates the volume of a unit cell
-    """
-    ca, cb, cg = cos(radians(al)), cos(radians(be)), cos(radians(ga))
-    v = a * b * c * sqrt(1 + 2 * ca * cb * cg - ca ** 2 - cb ** 2 - cg ** 2)
-    return v
-
-
-class OrthogonalMatrix():
-
-    def __init__(self, a, b, c, alpha, beta, gamma):
-        """
-        Converts von fractional to cartesian and vice versa.
-
-        >>> cell = [10.5086, 20.9035, 20.5072, 90, 94.13, 90]
-        >>> coord = [-0.186843,   0.282708,   0.526803]
-        >>> ort = OrthogonalMatrix(*cell)
-        >>> [ round(x, 6) for x in (ort * Array(coord)).values ]
-        [-2.741505, 5.909587, 10.775201]
-        >>> c_coord = [-2.741505423999065, 5.909586678000002, 10.775200700893732]
-        >>> [ round(x, 6) for x in (ort.inversed * Array(c_coord)).values]
-        [-0.186843, 0.282708, 0.526803]
-        """
-        self.a, self.b, self.c = a, b, c
-        self.V = vol_unitcell(a, b, c, alpha, beta, gamma)
-        self.alpha = radians(alpha)
-        self.beta = radians(beta)
-        self.gamma = radians(gamma)
-        phi = sqrt(1 - cos(self.alpha) ** 2 - cos(self.beta) ** 2 - cos(self.gamma) ** 2 +
-                   2 * cos(self.alpha) * cos(self.beta) * cos(self.gamma))
-        self.m = Matrix([[self.a, self.b * cos(self.gamma), self.c * cos(self.beta)],
-                         [0, self.b * sin(self.gamma),
-                          (self.c * (cos(self.alpha) - cos(self.beta) * cos(self.gamma)) / sin(self.gamma))],
-                         [0, 0, self.V / (self.a * self.b * sin(self.gamma))]])
-
-        # The inverted matrix:
-        self.mi = \
-            Matrix([[1.0 / self.a, -1.0 / (self.a * tan(self.gamma)),
-                     (cos(self.alpha) * cos(self.gamma) - cos(self.beta)) / (self.a * phi * sin(self.gamma))],
-                    [0.0, 1 / (self.b * sin(self.gamma)), (cos(self.beta) * cos(self.gamma) - cos(self.alpha)) /
-                     self.b * phi * sin(self.gamma)],
-                    [0.0, 0.0, sin(self.gamma) / (self.c * phi)]])
-
-    def __mul__(self, other: Array) -> Array:
-        """
-        To convert from fractional to cartesian.
-        """
-        return self.m * other
-
-    @property
-    def inversed(self):
-        """
-        To convert from cartesian to fractional.
-        """
-        return self.mi
-
-    @property
-    def transposed(self):
-        return self.m.transposed
-
-    @property
-    def T(self):
-        return self.m.transposed
-
-
-def almost_equal(a: Union[int, float], b: Union[int, float], places=3) -> float:
-    """
-    Returns True or False if the number a and b are are equal inside the
-    decimal places "places".
-    """
-    return round(abs(a - b), places) == 0
+# -*- encoding: utf-8 -*-
+# möp
+#
+# ----------------------------------------------------------------------------
+# "THE BEER-WARE LICENSE" (Revision 42):
+# <dkratzert@gmx.de> wrote this file. As long as you retain
+# this notice you can do whatever you want with this stuff. If we meet some day,
+# and you think this stuff is worth it, you can buy me a beer in return.
+# Daniel Kratzert
+# ----------------------------------------------------------------------------
+#
+import random
+import string
+from math import sqrt, radians, cos, sin, acos, degrees, floor, tan
+from operator import sub, add
+from typing import List, Union
+
+from shelxfile.misc.misc import flatten, determinante
+
+
+class Array(object):
+    """
+    MIT License
+
+    Copyright (c) 2018 Jens Luebben
+
+    Permission is hereby granted, free of charge, to any person obtaining a copy
+    of this software and associated documentation files (the "Software"), to deal
+    in the Software without restriction, including without limitation the rights
+    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+    copies of the Software, and to permit persons to whom the Software is
+    furnished to do so, subject to the following conditions:
+
+    The above copyright notice and this permission notice shall be included in all
+    copies or substantial portions of the Software.
+    """
+    __slots__ = ['values']
+
+    def __init__(self, values: Union[list, tuple]):
+        self.values = values
+
+    def __iter__(self) -> iter:
+        for v in self.values:
+            yield v
+
+    def __len__(self) -> int:
+        return len(self.values)
+
+    def __hash__(self):
+        return hash(self.values)
+
+    def __add__(self, other: (list, 'Array')) -> 'Array':
+        """
+        This method is optimized for speed.
+        """
+        if isinstance(other, Array):
+            return Array(list(map(add, self.values, other)))
+        elif type(other) == float or type(other) == int:
+            # return Array( list(map(lambda x: x - other, self.values)) )
+            return Array([i + other for i in self.values])
+        else:
+            raise TypeError('Cannot add type Array to type {}.'.format(str(type(other))))
+
+    def __iadd__(self, other):
+        return self.__add__(other)
+
+    def __eq__(self, other):
+        """
+        Test for equality.
+        """
+        return all([a == b for (a, b) in zip(self.values, other.values)])
+
+    def __sub__(self, other):
+        """
+        Subtracts eiter an Array or a value from the self Array.
+        This method is optimized for speed.
+        """
+        if isinstance(other, Array):
+            return Array(list(map(sub, self.values, other)))  # slightly faster
+        elif isinstance(other, float) or isinstance(other, int):
+            return Array([i - other for i in self.values])
+        else:
+            raise TypeError('Cannot add type Array to type {}.'.format(str(type(other))))
+
+    def __imul__(self, other):
+        """
+        Currently supports multiplication by a number.
+        __imul__ means a *= b
+        """
+        if isinstance(other, (int, float)):
+            self.values = [v * other for v in self.values]
+            return self
+        else:
+            raise TypeError('Unsupported operation.')
+
+    def __mul__(self, other: ('Array', 'Matrix')) -> (float, 'Array'):
+        """
+        Calculates: a * b = axbx + ayby + azbz
+        """
+        if isinstance(other, Matrix):
+            # Array() * Matrix()
+            a = other[0]
+            b = other[1]
+            c = other[2]
+            x = self.values[0] * a[0] + self.values[1] * b[0] + self.values[2] * c[0]
+            y = self.values[0] * a[1] + self.values[1] * b[1] + self.values[2] * c[1]
+            z = self.values[0] * a[2] + self.values[1] * b[2] + self.values[2] * c[2]
+            return Array([x, y, z])
+        else:
+            return self.dot(other)
+
+    def __repr__(self):
+        return 'Array({})'.format(str(self.values))
+
+    def __getitem__(self, val):
+        """
+        Get one item from the array.
+        """
+        return self.values[val]
+
+    def __setitem__(self, pos, val):
+        """
+        Get one item from the array.
+        """
+        self.values[pos] = val
+
+    def norm(self):
+        """
+        The squared lenght of an array
+        """
+        return sum([n ** 2 for n in self.values])
+
+    def normalized(self):
+        """
+        Euclidean norm (straight-line distance) of a vector array.
+        """
+        return sqrt(self.norm())
+
+    @staticmethod
+    def zero(m: int) -> 'Array':
+        """
+        Create zero Array of dimension m
+        """
+        return Array([0.0 for _ in range(m)])
+
+    @staticmethod
+    def randarray(m: int) -> 'Array':
+        """
+        Create random Array of dimension m
+        """
+        return Array([random.randint(1, 9) for _ in range(m)])
+
+    @property
+    def floor(self):
+        return Array(list(map(floor, self.values)))
+
+    def dot(self, other: 'Array') -> float:
+        """
+        Dot product of an array in kartesian space.
+        """
+        if len(self) != len(other):
+            raise ValueError('Vector sizes must match')
+        return sum([i * j for i, j in zip(self, other)])
+
+    def cross(self, other: 'Array') -> 'Array':
+        """
+        Cross product of the Array (currently only for 3D vectors).
+        """
+        if len(self) != len(other) != 3:
+            raise ValueError('For 3D vectors only')
+        a1, a2, a3 = self
+        b1, b2, b3 = other
+        return Array([(a2 * b3 - a3 * b2), (a3 * b1 - a1 * b3), (a1 * b2 - a2 * b1)])
+
+    def angle(self, other: 'Array') -> float:
+        """
+        Calculates the angle between two vectors.
+        """
+        return round(degrees(acos(self.dot(other) / (self.normalized() * other.normalized()))), 9)
+
+
+class Matrix(object):
+    """
+    MIT License
+
+    Copyright (c) 2018 Jens Luebben
+
+    Permission is hereby granted, free of charge, to any person obtaining a copy
+    of this software and associated documentation files (the "Software"), to deal
+    in the Software without restriction, including without limitation the rights
+    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+    copies of the Software, and to permit persons to whom the Software is
+    furnished to do so, subject to the following conditions:
+
+    The above copyright notice and this permission notice shall be included in all
+    copies or substantial portions of the Software.
+
+    DK: Missing: inverse, eigenvalues
+    """
+    __slots__ = ['values', 'shape']
+
+    def __init__(self, values):
+        self.shape = (len(values[0]), len(values))
+        self.values = values
+
+    def __getitem__(self, val):
+        """
+        """
+        if isinstance(val, (tuple, list)):
+            if len(val) == 1:
+                return self.values[val[0]]
+            return self.values[val[1]][val[0]]
+        else:
+            return self.values[val]
+
+    def __repr__(self):
+        rows = ''
+        for row in self.values:
+            rows += '|' + ' '.join(['{:>7.4f}'.format(float(x)) for x in row]) + '|' + '\n'
+        return rows
+
+    def __add__(self, other: (list, 'Matrix')) -> 'Matrix':
+        """
+        Matrix addition
+        """
+        if isinstance(other, Array):
+            if not len(self) == len(other):
+                raise ValueError('Matrix and Array are not of equal length.')
+            return Matrix(
+                [[sum(e1, e2) for e1, e2 in zip(row1, row2)] for row1, row2 in zip(self.values, other.values)])
+        elif isinstance(other, (float, int)):
+            return Matrix([[x + other for x in i] for i in self.values])
+        elif isinstance(other, Matrix):
+            return Matrix([[e1 + e2 for e1, e2 in zip(row1, row2)] for row1, row2 in zip(self.values, other.values)])
+        else:
+            raise TypeError('Cannot add type {} Array to Matrix.'.format(str(type(other))))
+
+    def __mul__(self, other: ('Matrix', 'Array', int, float)) -> ('Matrix', 'Array'):
+        """
+        a * b operation
+        """
+        if isinstance(other, (int, float)):
+            return Matrix([[v * other for v in row] for row in self.values])
+        elif isinstance(other, (Matrix, OrthogonalMatrix)):
+            return Matrix([[sum(ea * eb for ea, eb in zip(a, b)) for b in other.values] for a in self.values])
+        elif isinstance(other, Array):
+            return Array([sum([b * x for (b, x) in zip(other.values, row)]) for row in self.values])
+        else:
+            raise TypeError('Cannot add type {} to Matrix.'.format(str(type(other))))
+
+    def __len__(self):
+        return self.shape[1]
+
+    def __iter__(self) -> list:
+        return [n for n in self.values]
+
+    def __eq__(self, other):
+        """
+        Test for equality.
+        """
+        return all([b == x for (b, x) in zip(other.values, self.values)])
+
+    def __sub__(self, other):
+        """
+        Substract two matrices.
+        """
+        output = []
+        for idx in range(len(self)):
+            tmp = []
+            for val_a, val_b in zip(self[idx], other[idx]):
+                tmp.append(val_a - val_b)
+            output.append(tmp[:])
+        return output[:]
+
+    def __truediv__(self, other):
+        """
+        #>>> Matrix([[1, 2, 3], [1, 2, 3], [1, 2, 3]]) / Matrix([[1, 2, 3], [1, 2, 3], [1, 2, 3]])
+        A / B = A * A^-1
+        """
+        return NotImplementedError
+
+    def __setitem__(self, key, value):
+        # TODO: Implement setitem
+        pass
+
+    @property
+    def T(self):
+        return self.transposed
+
+    @property
+    def transposed(self) -> 'Matrix':
+        """
+        transposes a matrix
+        """
+        return Matrix(list(zip(*self.values)))
+
+    def transpose_alt(self):
+        """
+        Transposes the current matrix.
+        """
+        rows = []
+        for i in range(self.shape[0]):
+            rows.append([r[i] for r in self.values])
+        return Matrix(rows)
+
+    def dot(self, other):
+        """
+        Dot product of two matrices.
+        """
+        new_a = []
+        for i, col in enumerate(self.transposed.values):
+            s = sum([v * o for v, o in zip(col, other)])
+            new_a.append(s)
+        return Matrix(new_a)
+
+    @staticmethod
+    def zero(m: int, n: int) -> 'Matrix':
+        """
+        Create zero matrix of dimension m,n
+        """
+        return Matrix([[0.0 for _ in range(n)] for _ in range(m)])
+
+    @staticmethod
+    def randmat(m: int, n: int) -> 'Matrix':
+        """
+        Create random matrix of dimension m, n
+
+        #>>> Matrix.randmat(5, 3)
+        |  2.000   1.000   2.000|
+        |  8.000   1.000   2.000|
+        |  3.000   5.000   1.000|
+        |  4.000   1.000   9.000|
+        |  2.000   8.000   4.000|
+        <BLANKLINE>
+        """
+        return Matrix([[random.randint(1, 9) for y in range(n)] for x in range(m)])
+
+    def cholesky(self) -> 'Matrix':
+        """
+        """
+        L = Matrix.zero(*self.shape)
+        for i, (ai, li) in enumerate(zip(self.values, L.values)):
+            for j, lj in enumerate(L.values[:i + 1]):
+                s = sum(li[k] * lj[k] for k in range(j))
+                li[j] = sqrt(ai[i] - s) if (i == j) else (1.0 / lj[j] * (ai[j] - s))
+        return L
+
+    def norm(self):
+        return self.det
+
+    @property
+    def inversed(self) -> 'Matrix':
+        """
+        Inversion of 3 × 3 matrices
+         -0.812500    0.125000    0.187500
+          0.125000   -0.250000    0.125000
+          0.520833    0.125000   -0.145833
+        """
+        if self.shape != (3, 3):
+            raise ValueError('Inversion is only valid for 3x3 Matrix.')
+        d = self.det
+        m1, m2, m3, m4, m5, m6, m7, m8, m9 = flatten(self.values)
+        inv = Matrix([[(m5 * m9 - m6 * m8) / d, (m3 * m8 - m2 * m9) / d, (m2 * m6 - m3 * m5) / d],
+                      [(m6 * m7 - m4 * m9) / d, (m1 * m9 - m3 * m7) / d, (m3 * m4 - m1 * m6) / d],
+                      [(m4 * m8 - m5 * m7) / d, (m2 * m7 - m1 * m8) / d, (m1 * m5 - m2 * m4) / d]])
+        return inv
+
+    @property
+    def det(self):
+        """
+        Return determinant of 3x3 matrix.
+        """
+        return determinante(self.values)
+
+    def power_iteration(self, num_simulations=10):
+        """
+        Eigenvalue algorythm from https://en.wikipedia.org/wiki/Power_iteration
+        """
+        # Ideally choose a random vector
+        # To decrease the chance that our vector
+        # Is orthogonal to the eigenvector
+        b_k = Array.randarray(self.shape[1])
+
+        for _ in range(num_simulations):
+            # calculate the matrix-by-vector product Ab
+            b_k1 = self.dot(b_k)
+
+            # calculate the norm
+            b_k1_norm = b_k1.det
+
+            # re normalize the vector
+            b_k = b_k1 / b_k1_norm
+
+        return b_k
+
+
+class SymmetryElement(object):
+    """
+    Class representing a symmetry operation.
+    """
+    symm_id = 1
+    __slots__ = ['centric', 'symms', 'ID', 'matrix', 'trans', 'matrix_iter', 'trans_iter']
+
+    def __init__(self, symms, centric=False):
+        """
+        Constructor.
+        """
+        self.centric = centric
+        self.symms = symms
+        self.ID = SymmetryElement.symm_id
+        SymmetryElement.symm_id += 1
+        lines = []
+        trans = []
+        for symm in self.symms:
+            line, t = self._parse_line(symm)
+            lines.append(line)
+            trans.append(t)
+        self.matrix = Matrix(lines).transposed
+        self.trans = Array(trans)
+        self.matrix_iter = Matrix(lines).transposed.values
+        self.trans_iter = Array(trans).values
+        if centric:
+            self.matrix *= -1
+            self.trans *= -1
+
+    def __str__(self):
+        string = "|{aa:2} {ab:2} {ac:2}|   |{v:>4.2}|\n" \
+                 "|{ba:2} {bb:2} {bc:2}| + |{vv:>4.2}|\n" \
+                 "|{ca:2} {cb:2} {cc:2}|   |{vvv:>4.2}|\n".format(aa=self.matrix[0, 0],
+                                                                  ab=self.matrix[0, 1],
+                                                                  ac=self.matrix[0, 2],
+                                                                  ba=self.matrix[1, 0],
+                                                                  bb=self.matrix[1, 1],
+                                                                  bc=self.matrix[1, 2],
+                                                                  ca=self.matrix[2, 0],
+                                                                  cb=self.matrix[2, 1],
+                                                                  cc=self.matrix[2, 2],
+                                                                  v=float(self.trans[0]),
+                                                                  vv=float(self.trans[1]),
+                                                                  vvv=float(self.trans[2]))
+        return string
+
+    def __repr__(self):
+        return self.to_shelxl()
+
+    def __eq__(self, other):
+        """
+        Check two SymmetryElement instances for equivalence.
+        Note that differences in lattice translation are ignored.
+        :param other: SymmetryElement instance
+        :return: True/False
+        """
+        m = (self.matrix == other.matrix)
+        t1 = Array([v % 1 for v in self.trans])
+        t2 = Array([v % 1 for v in other.trans])
+        t = (t1 == t2)
+        return m and t
+
+    def __sub__(self, other):
+        """
+        Computes and returns the translational difference between two SymmetryElements. Returns 999.0 if the elements
+        cannot be superimposed via an integer shift of the translational parts.
+        :param other: SymmetryElement instance
+        :return: float
+        """
+        if not self == other:
+            return 999.
+        return self.trans - other.trans
+
+    def apply_latt_symm(self, latt_symm):
+        """
+        Copies SymmetryElement instance and returns the copy after applying the translational part of 'lattSymm'.
+        :param latt_symm: SymmetryElement.
+        :return: SymmetryElement.
+        """
+        new_symm = SymmetryElement(self.to_shelxl().split(','))
+        new_symm.trans = Array([(self.trans[0] + latt_symm.trans[0]) / 1,
+                                (self.trans[1] + latt_symm.trans[1]) / 1,
+                                (self.trans[2] + latt_symm.trans[2]) / 1])
+        new_symm.centric = self.centric
+        return new_symm
+
+    def to_shelxl(self):
+        """
+        Generate and return string representation of Symmetry Operation in Shelxl syntax.
+        :return: string.
+        """
+        axes = ['X', 'Y', 'Z']
+        lines = []
+        for i in range(3):
+            text = str(self.trans[i]) if self.trans[i] else ''
+            for j in range(3):
+                s = '' if not self.matrix[i, j] else axes[j]
+                if self.matrix[i, j] < 0:
+                    s = '-' + s
+                elif s:
+                    s = '+' + s
+                text += s
+            lines.append(text)
+        return ', '.join(lines)
+
+    def _parse_line(self, symm):
+        symm = symm.upper().replace(' ', '')
+        chars = ['X', 'Y', 'Z']
+        line = []
+        for char in chars:
+            element, symm = self._partition(symm, char)
+            line.append(element)
+        if symm:
+            trans = self._float(symm)
+        else:
+            trans = 0
+        return line, trans
+
+    def _float(self, string):
+        try:
+            return float(string)
+        except ValueError:
+            if '/' in string:
+                string = string.replace('/', './') + '.'
+                return eval('{}'.format(string))
+
+    def _partition(self, symm, char):
+        parts = symm.partition(char)
+        if parts[1]:
+            if parts[0]:
+                sign = parts[0][-1]
+            else:
+                sign = '+'
+            if sign == '-':
+                return -1, ''.join((parts[0][:-1], parts[2]))
+            else:
+                return 1, ''.join((parts[0], parts[2])).replace('+', '')
+        else:
+            return 0, symm
+
+
+# End of work by Jens Lübben #############
+
+
+def my_isnumeric(value: str):
+    """
+    Determines if a string can be converted to a number.
+    """
+    try:
+        float(value)
+    except ValueError:
+        return False
+    return True
+
+
+def mean(values):
+    """
+    returns mean value of a list of numbers
+    """
+    return sum(values) / float(len(values))
+
+
+def median(nums):
+    """
+    calculates the median of a list of numbers
+    """
+    ls = sorted(nums)
+    n = len(ls)
+    if n == 0:
+        raise ValueError("Need a non-empty iterable")
+    # for uneven list length:
+    elif n % 2 == 1:
+        # // is floordiv:
+        return ls[n // 2]
+    else:
+        return sum(ls[int(int(n) / 2 - 1):int(int(n) / 2 + 1)]) / 2.0
+
+
+def std_dev(data: List) -> float:
+    """
+    returns standard deviation of values rounded to pl decimal places
+    S = sqrt( (sum(x-xm)^2) / n-1 )
+    xm = sum(x)/n
+    :param data: list with integer or float values
+    """
+    if len(data) == 0:
+        return 0
+    K = data[0]
+    n = 0
+    summ = 0
+    sum_sqr = 0
+    for x in data:
+        n += 1
+        summ += x - K
+        sum_sqr += (x - K) * (x - K)
+    variance = (sum_sqr - (summ * summ) / n) / (n - 1)
+    # use n instead of (n-1) if want to compute the exact variance of the given data
+    # use (n-1) if data are samples of a larger population
+    return sqrt(variance)
+
+
+def nalimov_test(data):
+    """
+    returns a index list of outliers base on the Nalimov test for data.
+    Modified implementation of:
+    "R. Kaiser, G. Gottschalk, Elementare Tests zur Beurteilung von Messdaten
+    Bibliographisches Institut, Mannheim 1972."
+    """
+    # q-values for degrees of freedom:
+    f = {1 : 1.409, 2: 1.645, 3: 1.757, 4: 1.814, 5: 1.848, 6: 1.870, 7: 1.885, 8: 1.895,
+         9 : 1.903, 10: 1.910, 11: 1.916, 12: 1.920, 13: 1.923, 14: 1.926, 15: 1.928,
+         16: 1.931, 17: 1.933, 18: 1.935, 19: 1.936, 20: 1.937, 30: 1.945}
+    fact = sqrt(float(len(data)) / (len(data) - 1))
+    fval = len(data) - 2
+    if fval < 2:
+        return []
+    outliers = []
+    if fval in f:
+        # less strict than the original:
+        q_crit = f[fval]
+    else:
+        q_crit = 1.95
+    for num, i in enumerate(data):
+        q = abs(((i - median(data)) / std_dev(data)) * fact)
+        if q > q_crit:
+            outliers.append(num)
+    return outliers
+
+
+def id_generator(size=6, chars=string.ascii_uppercase + string.digits):
+    """
+    returns a random ID like 'L5J74W'
+    :param size: length of the string
+    :type size: integer
+    :param chars: characters used for the ID
+    :type chars: string
+    """
+    return ''.join(random.choice(chars) for _ in range(size))
+
+
+def atomic_distance(p1: List, p2: List, cell=None, shortest_dist=False):
+    """
+    p1 and p2 are x, y , z coordinates as list ['x', 'y', 'z']
+    cell are the cell parameters as list: ['a', 'b', 'c', 'alpha', 'beta', 'gamma']
+
+    Returns the distance between the two points (Atoms). If shortest_dist is True, the
+    shortest distance ignoring translation is computed.
+    """
+    a, b, c, al, be, ga = 1, 1, 1, 1, 1, 1
+    if cell:
+        a, b, c = cell[:3]
+        al = radians(cell[3])
+        be = radians(cell[4])
+        ga = radians(cell[5])
+    if shortest_dist:
+        x1, y1, z1 = [x + 99.5 for x in p1]
+        x2, y2, z2 = [x + 99.5 for x in p2]
+        dx = (x1 - x2) % 1 - 0.5
+        dy = (y1 - y2) % 1 - 0.5
+        dz = (z1 - z2) % 1 - 0.5
+    else:
+        x1, y1, z1 = p1
+        x2, y2, z2 = p2
+        dx = (x1 - x2)
+        dy = (y1 - y2)
+        dz = (z1 - z2)
+    if cell:
+        return sqrt((a * dx) ** 2 + (b * dy) ** 2 + (c * dz) ** 2 + 2 * b * c * cos(al) * dy * dz +
+                    2 * dx * dz * a * c * cos(be) + 2 * dx * dy * a * b * cos(ga))
+    else:
+        return sqrt(dx ** 2 + dy ** 2 + dz ** 2)
+
+
+def dice_coefficient(a, b, case_insens=True):
+    """
+    :type a: str
+    :type b: str
+    :type case_insens: bool
+    dice coefficient 2nt/na + nb.
+    https://en.wikibooks.org/wiki/Algorithm_Implementation/Strings/Dice%27s_coefficient#Python
+    """
+    if case_insens:
+        a = a.lower()
+        b = b.lower()
+    if not len(a) or not len(b):
+        return 0.0
+    if len(a) == 1:
+        a = a + u'.'
+    if len(b) == 1:
+        b = b + u'.'
+    a_bigram_list = []
+    for i in range(len(a) - 1):
+        a_bigram_list.append(a[i:i + 2])
+    b_bigram_list = []
+    for i in range(len(b) - 1):
+        b_bigram_list.append(b[i:i + 2])
+    a_bigrams = set(a_bigram_list)
+    b_bigrams = set(b_bigram_list)
+    overlap = len(a_bigrams & b_bigrams)
+    dice_coeff = overlap * 2.0 / (len(a_bigrams) + len(b_bigrams))
+    return round(dice_coeff, 6)
+
+
+def dice_coefficient2(a, b, case_insens=True):
+    """
+    :type a: str
+    :type b: str
+    :type case_insens: bool
+    duplicate bigrams in a word should be counted distinctly
+    (per discussion), otherwise 'AA' and 'AAAA' would have a
+    dice coefficient of 1...
+    https://en.wikibooks.org/wiki/Algorithm_Implementation/Strings/Dice%27s_coefficient#Python
+
+    This implementation is reverse. 1 means not hit, 0 means best match
+    """
+    if case_insens:
+        a = a.lower()
+        b = b.lower()
+    if not len(a) or not len(b):
+        return 1.0
+    # quick case for true duplicates
+    if a == b:
+        return 0.0
+    # if a != b, and a or b are single chars, then they can't possibly match
+    if len(a) == 1 or len(b) == 1:
+        return 1.0
+    # use python list comprehension, preferred over list.append()
+    a_bigram_list = [a[i:i + 2] for i in range(len(a) - 1)]
+    b_bigram_list = [b[i:i + 2] for i in range(len(b) - 1)]
+    a_bigram_list.sort()
+    b_bigram_list.sort()
+    # assignments to save function calls
+    lena = len(a_bigram_list)
+    lenb = len(b_bigram_list)
+    # initialize match counters
+    matches = i = j = 0
+    while i < lena and j < lenb:
+        if a_bigram_list[i] == b_bigram_list[j]:
+            matches += 2
+            i += 1
+            j += 1
+        elif a_bigram_list[i] < b_bigram_list[j]:
+            i += 1
+        else:
+            j += 1
+    score = float(matches) / float(lena + lenb)
+    score = 1 - score
+    return round(score, 6)
+
+
+def levenshtein(s1, s2):
+    """
+    The levensteins distance of two strings.
+    """
+    s1 = s1.lower()
+    s2 = s2.lower()
+    if len(s1) < len(s2):
+        return levenshtein(s2, s1)
+    if len(s2) == 0:
+        return len(s1)
+    previous_row = list(range(len(s2) + 1))
+    for i, c1 in enumerate(s1):
+        current_row = [i + 1]
+        for j, c2 in enumerate(s2):
+            # j+1 instead of j since previous_row and current_row are one character longer:
+            insertions = previous_row[j + 1] + 1
+            deletions = current_row[j] + 1  # than s2
+            substitutions = previous_row[j] + (c1 != c2)
+            current_row.append(min(insertions, deletions, substitutions))
+        previous_row = current_row
+    return previous_row[-1]
+
+
+def distance(x1, y1, z1, x2, y2, z2, round_out=False):
+    """
+    distance between two points in space for orthogonal axes.
+    """
+    import math as m
+    d = m.sqrt((x1 - x2) ** 2 + (y1 - y2) ** 2 + (z1 - z2) ** 2)
+    if round_out:
+        return round(d, round_out)
+    else:
+        return d
+
+
+def vol_unitcell(a, b, c, al, be, ga):
+    """
+    calculates the volume of a unit cell
+    """
+    ca, cb, cg = cos(radians(al)), cos(radians(be)), cos(radians(ga))
+    v = a * b * c * sqrt(1 + 2 * ca * cb * cg - ca ** 2 - cb ** 2 - cg ** 2)
+    return v
+
+
+class OrthogonalMatrix():
+
+    def __init__(self, a, b, c, alpha, beta, gamma):
+        """
+        Converts von fractional to cartesian and vice versa.
+
+        >>> cell = [10.5086, 20.9035, 20.5072, 90, 94.13, 90]
+        >>> coord = [-0.186843,   0.282708,   0.526803]
+        >>> ort = OrthogonalMatrix(*cell)
+        >>> [ round(x, 6) for x in (ort * Array(coord)).values ]
+        [-2.741505, 5.909587, 10.775201]
+        >>> c_coord = [-2.741505423999065, 5.909586678000002, 10.775200700893732]
+        >>> [ round(x, 6) for x in (ort.inversed * Array(c_coord)).values]
+        [-0.186843, 0.282708, 0.526803]
+        """
+        self.a, self.b, self.c = a, b, c
+        self.V = vol_unitcell(a, b, c, alpha, beta, gamma)
+        self.alpha = radians(alpha)
+        self.beta = radians(beta)
+        self.gamma = radians(gamma)
+        phi = sqrt(1 - cos(self.alpha) ** 2 - cos(self.beta) ** 2 - cos(self.gamma) ** 2 +
+                   2 * cos(self.alpha) * cos(self.beta) * cos(self.gamma))
+        self.m = Matrix([[self.a, self.b * cos(self.gamma), self.c * cos(self.beta)],
+                         [0, self.b * sin(self.gamma),
+                          (self.c * (cos(self.alpha) - cos(self.beta) * cos(self.gamma)) / sin(self.gamma))],
+                         [0, 0, self.V / (self.a * self.b * sin(self.gamma))]])
+
+        # The inverted matrix:
+        self.mi = \
+            Matrix([[1.0 / self.a, -1.0 / (self.a * tan(self.gamma)),
+                     (cos(self.alpha) * cos(self.gamma) - cos(self.beta)) / (self.a * phi * sin(self.gamma))],
+                    [0.0, 1 / (self.b * sin(self.gamma)), (cos(self.beta) * cos(self.gamma) - cos(self.alpha)) /
+                     self.b * phi * sin(self.gamma)],
+                    [0.0, 0.0, sin(self.gamma) / (self.c * phi)]])
+
+    def __mul__(self, other: Array) -> Array:
+        """
+        To convert from fractional to cartesian.
+        """
+        return self.m * other
+
+    @property
+    def inversed(self):
+        """
+        To convert from cartesian to fractional.
+        """
+        return self.mi
+
+    @property
+    def transposed(self):
+        return self.m.transposed
+
+    @property
+    def T(self):
+        return self.m.transposed
+
+
+def almost_equal(a: Union[int, float], b: Union[int, float], places=3) -> float:
+    """
+    Returns True or False if the number a and b are are equal inside the
+    decimal places "places".
+    """
+    return round(abs(a - b), places) == 0
```

### Comparing `shelxfile-8/shelxfile/misc/misc.py` & `shelxfile-9/shelxfile/misc/misc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,529 +1,519 @@
-# -*- encoding: utf-8 -*-
-# möpß
-#
-# ----------------------------------------------------------------------------
-# "THE BEER-WARE LICENSE" (Revision 42):
-# <dkratzert@gmx.de> wrote this file. As long as you retain
-# this notice you can do whatever you want with this stuff. If we meet some day,
-# and you think this stuff is worth it, you can buy me a beer in return.
-# Daniel Kratzert
-# ----------------------------------------------------------------------------
-#
-import os
-import re
-import textwrap
-from math import radians, cos, sin, sqrt
-from shutil import get_terminal_size
-
-# TODO: Add verbose mode that doesn't fail but gives output like debug mode.
-# Without DEBUG, the parser should only fail if the file is realy damaged. With DEBUG enabled, the parser
-# fails even in harmless cases.
-from time import time, perf_counter
-
-DEBUG = False
-PROFILE = False
-
-dsr_regex = re.compile(r'^rem\s+DSR\s+(PUT|REPLACE).*', re.IGNORECASE)
-
-
-class ParseOrderError(Exception):
-    def __init__(self, arg=None):
-        if DEBUG:
-            if arg:
-                print(arg)
-            else:
-                print("*** WRONG ODER of INSTRUCTIONS ***")
-
-
-class ParseNumError(Exception):
-    def __init__(self, arg=None):
-        if DEBUG:
-            if arg:
-                print(arg)
-            print("*** WRONG NUMBER OF NUMERICAL PARAMETERS ***")
-
-
-class ParseParamError(Exception):
-    def __init__(self, arg=None):
-        if DEBUG:
-            if arg:
-                print(arg)
-            print("*** WRONG NUMBER OF PARAMETERS ***")
-
-
-class ParseUnknownParam(Exception):
-    def __init__(self, arg=None):
-        if DEBUG:
-            if arg:
-                print(arg)
-            print("*** UNKNOWN PARAMETER ***")
-
-
-class ParseSyntaxError(Exception):
-    def __init__(self):
-        if DEBUG:
-            print("*** Syntax Error ***")
-
-
-try:
-    width, height = get_terminal_size()  # @UnusedVariable
-except():
-    width = 80
-sep_line = (width - 1) * '-'
-
-
-def remove_file(filename, exit_dsr=False):
-    """
-    removes the file "filename" from disk
-    program exits when exit is true
-    platon gets terminated if terminate is true
-    """
-    if os.path.isfile(filename):
-        try:
-            os.remove(filename)
-        except(IOError, OSError):
-            return False
-        return True
-
-
-def find_line(inputlist: list, regex: str, start: int = None) -> int:
-    """
-    returns the index number of the line where regex is found in the inputlist
-    if stop is true, stop searching with first line found
-    :param inputlist: list of strings
-    :type inputlist: list
-    :param regex: regular expression to search
-    :type regex: string
-    :param start: line number where to start the search
-    :param start: start searching at line start
-    :type start: string or int
-    >>> inp = ['Hallo blub', 'foo bar blub', '123', '1 blub 2 3 4']
-    >>> find_line(inp, '.*blub.*')
-    0
-    >>> inp = [['foo'],['bar']]
-    >>> find_line(inp, '.*blub.*') #doctest: +REPORT_NDIFF +NORMALIZE_WHITESPACE +ELLIPSIS
-    Traceback (most recent call last):
-        ...
-    TypeError: expected string or ...
-    """
-    if start:
-        start = int(start)
-        inputlist_slice = inputlist[start:]
-        for i, string in enumerate(inputlist_slice, start):
-            if re.match(regex, string, re.IGNORECASE):
-                return i  # returns the index number if regex found
-    else:
-        for i, string in enumerate(inputlist):
-            if re.match(regex, string, re.IGNORECASE):
-                return i  # returns the index number if regex found
-    return -1  # returns -1 if no regex found
-
-
-def which(name: str, flags=os.X_OK, exts=None) -> list:
-    """
-    Search PATH for executable files with the given name.
-
-    On MS-Windows the only flag that has any meaning is os.F_OK. Any other
-    flags will be ignored.
-    """
-    if exts is None:
-        exts = ['.exe', '.EXE', '.bat']
-    result = []
-    # exts = filter(None, os.environ.get('PATHEXT', '').split(os.pathsep))
-    path = os.getenv('PATH', None)
-    if path is None:
-        return []
-    for p in os.getenv('PATH', '').split(os.pathsep):
-        p = os.path.join(p, name)
-        if os.access(p, flags):
-            result.append(p)
-        for e in exts:
-            pext = p + e
-            if os.access(pext, flags):
-                result.append(pext)
-    return result
-
-
-def split_fvar_and_parameter(parameter: float) -> tuple:
-    """
-    Returns the free variable and value of a given parameter e.g. 30.5 for the occupancy.
-    :return (fvar: int, value: float)
-
-    >>> split_fvar_and_parameter(30.5)
-    (3, 0.5)
-    >>> split_fvar_and_parameter(31.0)
-    (3, 1.0)
-    >>> split_fvar_and_parameter(-30.5)
-    (-3, -0.5)
-    >>> split_fvar_and_parameter(11.0)
-    (1, 1.0)
-    >>> split_fvar_and_parameter(-11.0)
-    (-1, -1.0)
-    >>> split_fvar_and_parameter(-10.33333333)
-    (-1, -0.33333333)
-    """
-    fvar = abs(int(str(parameter).split('.')[0])) // 10  # The free variable number e.g. 2
-    value = abs(float(parameter)) % 10  # The value with which the free variable was multiplied e.g. 0.5
-    if parameter < 0:
-        value *= -1
-        fvar *= -1
-    return fvar, round(value, 8)
-
-
-def flatten(lis):
-    """
-    Given a list, possibly nested to any level, return it flattened.
-    From: http://code.activestate.com/recipes/578948-flattening-an-arbitrarily-nested-list-in-python/
-
-    >>> flatten([['wer', 234, 'brdt5'], ['dfg'], [[21, 34,5], ['fhg', 4]]])
-    ['wer', 234, 'brdt5', 'dfg', 21, 34, 5, 'fhg', 4]
-    """
-    new_lis = []
-    for item in lis:
-        if isinstance(item, list):
-            new_lis.extend(flatten(item))
-        else:
-            new_lis.append(item)
-    return new_lis
-
-
-def vol_tetrahedron(a, b, c, d, cell=None):
-    """
-    Returns the volume of a terahedron spanned by four points.
-
-    No cell is needed for orthogonal coordinates.
-
-    e.g. A = (3, 2, 1), B = (1, 2, 4), C = (4, 0, 3), D = (1, 1, 7)
-            |u1 u2 u3|
-    v = 1/6*|v1 v2 v3|
-            |w1 w2 w3|
-    AB = (1-3, 2-2, 4-1) = (-2, 0, 3)
-    AC = ...
-    AD = ...
-    V = 1/6[u,v,w]
-              |-2,  0, 3|
-    [u,v,w] = | 1, -2, 2| = 24-3-12 = 5
-              |-2, -1, 6|
-    V = 1/6*5
-    >>> cell = (10.5086, 20.9035, 20.5072, 90, 94.13, 90)
-    >>> a = (0.838817,   0.484526,   0.190081) # a ist um 0.01 ausgelenkt
-    >>> b = (0.875251,   0.478410,   0.256955)
-    >>> c = (0.789290,   0.456520,   0.301616)
-    >>> d = (0.674054,   0.430194,   0.280727)
-    >>> print('volume of Benzene ring atoms:')
-    volume of Benzene ring atoms:
-    >>> print(round(vol_tetrahedron(a, b, c, d, cell), 7))
-    0.0633528
-    """
-    A = [float(i) for i in a]
-    B = [float(i) for i in b]
-    C = [float(i) for i in c]
-    D = [float(i) for i in d]
-    if cell:
-        A = frac_to_cart(a, cell)
-        B = frac_to_cart(b, cell)
-        C = frac_to_cart(c, cell)
-        D = frac_to_cart(d, cell)
-    AB = subtract_vect(A, B)
-    AC = subtract_vect(A, C)
-    AD = subtract_vect(A, D)
-    D = determinante([AB, AC, AD])
-    return abs((D / 6))
-
-
-def time_this_method(f):
-    """
-    Rather promitive way of timing a method. More advanced would be the profilehooks module.
-    """
-    if PROFILE:
-        from functools import wraps
-
-        @wraps(f)
-        def wrapper(*args, **kwargs):
-            t1 = perf_counter()
-            result = f(*args, **kwargs)
-            t2 = perf_counter()
-            if PROFILE:
-                print('Time for "{}": {:5.3} ms\n'.format(f.__name__ + '()', (t2 - t1) * 1000))
-            return result
-    else:
-        wrapper = f
-    return wrapper
-
-
-def chunks(l: list, n: int) -> list:
-    """
-    returns successive n-sized chunks from l.
-    """
-    return [l[i:i + n] for i in range(0, len(l), n)]
-
-
-def multiline_test(line: str) -> bool:
-    """
-    test if the current line is a multiline with "=" at the end
-    :param line: 'O1 3 -0.01453 1.66590 0.10966 11.00 0.05 ='
-    """
-    if line.rfind('=') > -1:
-        # A '=' character in a rem line is not a line break!
-        if line.startswith("REM") and not dsr_regex.match(line):
-            return False
-        return True
-    else:
-        return False
-
-
-class TextLine:
-    def __init__(self, initdata):
-        """
-        #>>> t = TextLine('foo')
-        #>>> t.id
-        """
-        self.data = initdata
-        self.next = None
-        self.id = time()
-
-    def get_data(self):
-        return self.data
-
-    def get_next(self):
-        return self.next
-
-    def set_data(self, newdata):
-        self.data = newdata
-
-    def set_next(self, newnext):
-        self.next = newnext
-
-
-class ResList():
-    """
-    Contains the lines of the res file as unordered linked list.
-    """
-
-    def __init__(self):
-        """
-        >>> res = ResList()
-        >>> res
-        <BLANKLINE>
-        >>> res.append('zweiter')
-        >>> res.add('erster')
-        >>> res.add('dritter')
-        >>> res.append('vierter')
-        >>> res.size
-        4
-        >>> res.tail.get_data()
-        'vierter'
-        >>> res
-        dritter
-        erster
-        zweiter
-        vierter
-        """
-        self.head = None
-        self.tail = None
-        self.size = 0
-
-    def __repr__(self):
-        current = self.head
-        datalist = []
-        if not self.head:
-            return ''
-        while current != self.tail:
-            datalist.append(current.get_data())
-            current = current.get_next()
-        datalist.append(self.tail.get_data())
-        return "\n".join(datalist)
-
-    def is_empty(self):
-        return self.head is None
-
-    def add(self, item):
-        temp = TextLine(item)
-        temp.set_next(self.head)
-        self.head = temp
-        self.size += 1
-
-    def search(self, item):
-        current = self.head
-        found = False
-        while current is not None and not found:
-            if current.get_data() == item:
-                found = True
-            else:
-                current = current.get_next()
-        return found
-
-    def remove(self, item):
-        current = self.head
-        previous = None
-        found = False
-        while not found:
-            if current.get_data() == item:
-                found = True
-            else:
-                previous = current
-                current = current.get_next()
-        if previous is None:
-            self.head = current.get_next()
-        else:
-            previous.setNext(current.get_next())
-        self.size -= 1
-
-    def append(self, item):
-        temp = TextLine(item)
-        if not self.head:
-            self.head = temp
-        else:
-            last = self.tail
-            last.set_next(temp)
-        self.tail = temp
-        self.size += 1
-
-
-def wrap_line(line: str) -> str:
-    """
-    Wraps long lines according to SHELXL syntax with = at end and space characters before the next line.
-    The wrapping will only be at whitespace, not inside words.
-    """
-    maxlen = 79
-    if len(line) < maxlen:
-        line = ''.join(line)
-        return line
-    line = textwrap.wrap(line, maxlen, subsequent_indent='  ', drop_whitespace=False, replace_whitespace=False)
-    if len(line) > 1:
-        newline = []
-        for n, ln in enumerate(line):
-            if n < len(line) - 1:
-                ln += ' =\n'
-            newline.append(ln)
-        line = ' '.join(newline)
-    else:
-        line = ''.join(line)
-    return line
-
-
-def range_resolver(atoms_range: list, atom_names: list) -> list:
-    """
-    Resolves the atom names of ranges like "C1 > C5"
-    and works for each restraint line separately.
-    :param atoms_range: atoms with a range definition
-    :param atom_names: names of atoms in the fragment
-    """
-    # dict with lists of positions of the > or < sign:
-    rightleft = {'>': [], '<': []}
-    for rl in rightleft:
-        for num, i in enumerate(atoms_range):
-            i = i.upper()
-            if rl == i:
-                # fill the dictionary:
-                rightleft[rl].append(num)
-    for rl in rightleft:
-        # for each sign:
-        for i in rightleft[rl]:
-            # for each position of < or >:
-            if rl == '>':
-                # forward range
-                left = atom_names.index(atoms_range[i - 1]) + 1
-                right = atom_names.index(atoms_range[i + 1])
-                atoms_range[i:i + 1] = atom_names[left:right]
-            else:
-                # backward range
-                left = atom_names.index(atoms_range[i - 1])
-                right = atom_names.index(atoms_range[i + 1]) + 1
-                names = atom_names[right:left]
-                names.reverse()  # counting backwards
-                atoms_range[i:i + 1] = names
-    return atoms_range
-
-
-def walkdir(rootdir, include="", exclude=""):
-    """
-    Returns a list of files in all subdirectories with full path.
-    :param rootdir: base path from which walk should start
-    :param filter: list of file endings to include only e.g. ['.py', '.res']
-    :return: list of files
-
-    #>>> walkdir("../docs") #doctest: +REPORT_NDIFF +NORMALIZE_WHITESPACE +ELLIPSIS
-    #['../docs/test.txt']
-    #>>> walkdir("../setup/modpath.iss")
-    #['../setup/modpath.iss']
-    #>>> walkdir("../setup/modpath.iss", exclude=['.iss'])
-    #[]
-    #>>> walkdir("../docs", exclude=['.txt']) #doctest: +REPORT_NDIFF +NORMALIZE_WHITESPACE +ELLIPSIS
-    #[]
-    """
-    results = []
-    if not os.path.isdir(rootdir):
-        if os.path.splitext(rootdir)[1] in exclude:
-            return []
-        return [rootdir]
-    for root, sub_folders, files in os.walk(rootdir):
-        for file in files:
-            fullfilepath = os.path.join(root, file)
-            if exclude and os.path.splitext(fullfilepath)[1] in exclude:
-                continue
-            if include:
-                if os.path.splitext(fullfilepath)[1] in include:
-                    results.append(os.path.normpath(fullfilepath).replace('\\', '/'))
-            else:
-                results.append(os.path.normpath(fullfilepath).replace('\\', '/'))
-    return results
-
-
-def frac_to_cart(frac_coord: (list, tuple), cell: list) -> list:
-    """
-    Converts fractional coordinates to cartesian coodinates
-    :param frac_coord: [float, float, float]
-    :param cell:       [float, float, float, float, float, float]
-    """
-    a, b, c, alpha, beta, gamma = cell
-    x, y, z = frac_coord
-    alpha = radians(alpha)
-    beta = radians(beta)
-    gamma = radians(gamma)
-    cosastar = (cos(beta) * cos(gamma) - cos(alpha)) / (sin(beta) * sin(gamma))
-    sinastar = sqrt(1 - cosastar ** 2)
-    xc = a * x + (b * cos(gamma)) * y + (c * cos(beta)) * z
-    yc = 0 + (b * sin(gamma)) * y + (-c * sin(beta) * cosastar) * z
-    zc = 0 + 0 + (c * sin(beta) * sinastar) * z
-    return [xc, yc, zc]
-
-
-def cart_to_frac(cart_coord: list, cell: list) -> tuple:
-    """
-    converts cartesian coordinates to fractional coordinates
-    :param cart_coord: [float, float, float]
-    :param cell:       [float, float, float, float, float, float]
-    """
-    a, b, c, alpha, beta, gamma = cell
-    xc, yc, zc = cart_coord
-    alpha = radians(alpha)
-    beta = radians(beta)
-    gamma = radians(gamma)
-    cosastar = (cos(beta) * cos(gamma) - cos(alpha)) / (sin(beta) * sin(gamma))
-    sinastar = sqrt(1 - cosastar ** 2)
-    z = zc / (c * sin(beta) * sinastar)
-    y = (yc - (-c * sin(beta) * cosastar) * z) / (b * sin(gamma))
-    x = (xc - (b * cos(gamma)) * y - (c * cos(beta)) * z) / a
-    return x, y, z
-
-
-def determinante(a):
-    """
-    return determinant of 3x3 matrix
-    """
-    return (a[0][0] * (a[1][1] * a[2][2] - a[2][1] * a[1][2])
-            - a[1][0] * (a[0][1] * a[2][2] - a[2][1] * a[0][2])
-            + a[2][0] * (a[0][1] * a[1][2] - a[1][1] * a[0][2]))
-
-
-def subtract_vect(a, b):
-    """
-    subtract vector b from vector a
-    Deprecated, use mpmath instead!!!
-    :param a: [float, float, float]
-    :param b: [float, float, float]
-    """
-    return (a[0] - b[0],
-            a[1] - b[1],
-            a[2] - b[2])
+# -*- encoding: utf-8 -*-
+# möpß
+#
+# ----------------------------------------------------------------------------
+# "THE BEER-WARE LICENSE" (Revision 42):
+# <dkratzert@gmx.de> wrote this file. As long as you retain
+# this notice you can do whatever you want with this stuff. If we meet some day,
+# and you think this stuff is worth it, you can buy me a beer in return.
+# Daniel Kratzert
+# ----------------------------------------------------------------------------
+#
+import os
+import re
+import textwrap
+from math import radians, cos, sin, sqrt
+from shutil import get_terminal_size
+
+from time import time, perf_counter
+from typing import List
+
+DEBUG = False
+PROFILE = False
+
+dsr_regex = re.compile(r'^rem\s+DSR\s+(PUT|REPLACE).*', re.IGNORECASE)
+
+
+class ParseOrderError(Exception):
+    def __init__(self, arg=None):
+        if DEBUG:
+            if arg:
+                print(arg)
+            else:
+                print("*** WRONG ODER of INSTRUCTIONS ***")
+
+
+class ParseNumError(Exception):
+    def __init__(self, arg=None):
+        if DEBUG:
+            if arg:
+                print(arg)
+            print("*** WRONG NUMBER OF NUMERICAL PARAMETERS ***")
+
+
+class ParseParamError(Exception):
+    def __init__(self, arg=None):
+        if DEBUG:
+            if arg:
+                print(arg)
+            print("*** WRONG NUMBER OF PARAMETERS ***")
+
+
+class ParseUnknownParam(Exception):
+    def __init__(self, arg=None):
+        if DEBUG:
+            if arg:
+                print(arg)
+            print("*** UNKNOWN PARAMETER ***")
+
+
+class ParseSyntaxError(Exception):
+    def __init__(self):
+        if DEBUG:
+            print("*** Syntax Error ***")
+
+
+try:
+    width, height = get_terminal_size()  # @UnusedVariable
+except():
+    width = 80
+sep_line = (width - 1) * '-'
+
+
+def remove_file(filename, exit_dsr=False):
+    """
+    removes the file "filename" from disk
+    program exits when exit is true
+    platon gets terminated if terminate is true
+    """
+    if os.path.isfile(filename):
+        try:
+            os.remove(filename)
+        except(IOError, OSError):
+            return False
+        return True
+
+
+def find_line(inputlist: List, regex: str, start: int = None) -> int:
+    """
+    returns the index number of the line where regex is found in the inputlist
+    if stop is true, stop searching with first line found
+    :param inputlist: list of strings
+    :type inputlist: list
+    :param regex: regular expression to search
+    :type regex: string
+    :param start: line number where to start the search
+    :param start: start searching at line start
+    :type start: string or int
+    """
+    if start:
+        start = int(start)
+        inputlist_slice = inputlist[start:]
+        for i, string in enumerate(inputlist_slice, start):
+            if re.match(regex, string, re.IGNORECASE):
+                return i  # returns the index number if regex found
+    else:
+        for i, string in enumerate(inputlist):
+            if re.match(regex, string, re.IGNORECASE):
+                return i  # returns the index number if regex found
+    return -1  # returns -1 if no regex found
+
+
+def which(name: str, flags=os.X_OK, exts=None) -> list:
+    """
+    Search PATH for executable files with the given name.
+
+    On MS-Windows the only flag that has any meaning is os.F_OK. Any other
+    flags will be ignored.
+    """
+    if exts is None:
+        exts = ['.exe', '.EXE', '.bat']
+    result = []
+    # exts = filter(None, os.environ.get('PATHEXT', '').split(os.pathsep))
+    path = os.getenv('PATH', None)
+    if path is None:
+        return []
+    for p in os.getenv('PATH', '').split(os.pathsep):
+        p = os.path.join(p, name)
+        if os.access(p, flags):
+            result.append(p)
+        for e in exts:
+            pext = p + e
+            if os.access(pext, flags):
+                result.append(pext)
+    return result
+
+
+def split_fvar_and_parameter(parameter: float) -> tuple:
+    """
+    Returns the free variable and value of a given parameter e.g. 30.5 for the occupancy.
+    :return (fvar: int, value: float)
+
+    >>> split_fvar_and_parameter(30.5)
+    (3, 0.5)
+    >>> split_fvar_and_parameter(31.0)
+    (3, 1.0)
+    >>> split_fvar_and_parameter(-30.5)
+    (-3, -0.5)
+    >>> split_fvar_and_parameter(11.0)
+    (1, 1.0)
+    >>> split_fvar_and_parameter(-11.0)
+    (-1, -1.0)
+    >>> split_fvar_and_parameter(-10.33333333)
+    (-1, -0.33333333)
+    """
+    fvar = abs(int(str(parameter).split('.')[0])) // 10  # The free variable number e.g. 2
+    value = abs(float(parameter)) % 10  # The value with which the free variable was multiplied e.g. 0.5
+    if parameter < 0:
+        value *= -1
+        fvar *= -1
+    return fvar, round(value, 8)
+
+
+def flatten(lis):
+    """
+    Given a list, possibly nested to any level, return it flattened.
+    From: http://code.activestate.com/recipes/578948-flattening-an-arbitrarily-nested-list-in-python/
+
+    >>> flatten([['wer', 234, 'brdt5'], ['dfg'], [[21, 34,5], ['fhg', 4]]])
+    ['wer', 234, 'brdt5', 'dfg', 21, 34, 5, 'fhg', 4]
+    """
+    new_lis = []
+    for item in lis:
+        if isinstance(item, list):
+            new_lis.extend(flatten(item))
+        else:
+            new_lis.append(item)
+    return new_lis
+
+
+def vol_tetrahedron(a, b, c, d, cell=None):
+    """
+    Returns the volume of a terahedron spanned by four points.
+
+    No cell is needed for orthogonal coordinates.
+
+    e.g. A = (3, 2, 1), B = (1, 2, 4), C = (4, 0, 3), D = (1, 1, 7)
+            |u1 u2 u3|
+    v = 1/6*|v1 v2 v3|
+            |w1 w2 w3|
+    AB = (1-3, 2-2, 4-1) = (-2, 0, 3)
+    AC = ...
+    AD = ...
+    V = 1/6[u,v,w]
+              |-2,  0, 3|
+    [u,v,w] = | 1, -2, 2| = 24-3-12 = 5
+              |-2, -1, 6|
+    V = 1/6*5
+    >>> cell = (10.5086, 20.9035, 20.5072, 90, 94.13, 90)
+    >>> a = (0.838817,   0.484526,   0.190081) # a ist um 0.01 ausgelenkt
+    >>> b = (0.875251,   0.478410,   0.256955)
+    >>> c = (0.789290,   0.456520,   0.301616)
+    >>> d = (0.674054,   0.430194,   0.280727)
+    >>> print('volume of Benzene ring atoms:')
+    volume of Benzene ring atoms:
+    >>> print(round(vol_tetrahedron(a, b, c, d, cell), 7))
+    0.0633528
+    """
+    A = [float(i) for i in a]
+    B = [float(i) for i in b]
+    C = [float(i) for i in c]
+    D = [float(i) for i in d]
+    if cell:
+        A = frac_to_cart(a, cell)
+        B = frac_to_cart(b, cell)
+        C = frac_to_cart(c, cell)
+        D = frac_to_cart(d, cell)
+    AB = subtract_vect(A, B)
+    AC = subtract_vect(A, C)
+    AD = subtract_vect(A, D)
+    D = determinante([AB, AC, AD])
+    return abs((D / 6))
+
+
+def time_this_method(f):
+    """
+    Rather promitive way of timing a method. More advanced would be the profilehooks module.
+    """
+    if PROFILE:
+        from functools import wraps
+
+        @wraps(f)
+        def wrapper(*args, **kwargs):
+            t1 = perf_counter()
+            result = f(*args, **kwargs)
+            t2 = perf_counter()
+            if PROFILE:
+                print('Time for "{}": {:5.3} ms\n'.format(f.__name__ + '()', (t2 - t1) * 1000))
+            return result
+    else:
+        wrapper = f
+    return wrapper
+
+
+def chunks(l: list, n: int) -> list:
+    """
+    returns successive n-sized chunks from l.
+    """
+    return [l[i:i + n] for i in range(0, len(l), n)]
+
+
+def multiline_test(line: str) -> bool:
+    """
+    test if the current line is a multiline with "=" at the end
+    :param line: 'O1 3 -0.01453 1.66590 0.10966 11.00 0.05 ='
+    """
+    if line.rfind('=') > -1:
+        # A '=' character in a rem line is not a line break!
+        if line.startswith("REM") and not dsr_regex.match(line):
+            return False
+        return True
+    else:
+        return False
+
+
+class TextLine:
+    def __init__(self, initdata):
+        """
+        #>>> t = TextLine('foo')
+        #>>> t.id
+        """
+        self.data = initdata
+        self.next = None
+        self.id = time()
+
+    def get_data(self):
+        return self.data
+
+    def get_next(self):
+        return self.next
+
+    def set_data(self, newdata):
+        self.data = newdata
+
+    def set_next(self, newnext):
+        self.next = newnext
+
+
+class ResList():
+    """
+    Contains the lines of the res file as unordered linked list.
+    """
+
+    def __init__(self):
+        """
+        >>> res = ResList()
+        >>> res
+        <BLANKLINE>
+        >>> res.append('zweiter')
+        >>> res.add('erster')
+        >>> res.add('dritter')
+        >>> res.append('vierter')
+        >>> res.size
+        4
+        >>> res.tail.get_data()
+        'vierter'
+        >>> res
+        dritter
+        erster
+        zweiter
+        vierter
+        """
+        self.head = None
+        self.tail = None
+        self.size = 0
+
+    def __repr__(self):
+        current = self.head
+        datalist = []
+        if not self.head:
+            return ''
+        while current != self.tail:
+            datalist.append(current.get_data())
+            current = current.get_next()
+        datalist.append(self.tail.get_data())
+        return "\n".join(datalist)
+
+    def is_empty(self):
+        return self.head is None
+
+    def add(self, item):
+        temp = TextLine(item)
+        temp.set_next(self.head)
+        self.head = temp
+        self.size += 1
+
+    def search(self, item):
+        current = self.head
+        found = False
+        while current is not None and not found:
+            if current.get_data() == item:
+                found = True
+            else:
+                current = current.get_next()
+        return found
+
+    def remove(self, item):
+        current = self.head
+        previous = None
+        found = False
+        while not found:
+            if current.get_data() == item:
+                found = True
+            else:
+                previous = current
+                current = current.get_next()
+        if previous is None:
+            self.head = current.get_next()
+        else:
+            previous.setNext(current.get_next())
+        self.size -= 1
+
+    def append(self, item):
+        temp = TextLine(item)
+        if not self.head:
+            self.head = temp
+        else:
+            last = self.tail
+            last.set_next(temp)
+        self.tail = temp
+        self.size += 1
+
+
+def wrap_line(line: str) -> str:
+    """
+    Wraps long lines according to SHELXL syntax with = at end and space characters before the next line.
+    The wrapping will only be at whitespace, not inside words.
+    """
+    maxlen = 79
+    if len(line) < maxlen:
+        line = ''.join(line)
+        return line
+    line = textwrap.wrap(line, maxlen, subsequent_indent='  ', drop_whitespace=False, replace_whitespace=False)
+    if len(line) > 1:
+        newline = []
+        for n, ln in enumerate(line):
+            if n < len(line) - 1:
+                ln += ' =\n'
+            newline.append(ln)
+        line = ' '.join(newline)
+    else:
+        line = ''.join(line)
+    return line
+
+
+def range_resolver(atoms_range: list, atom_names: list) -> list:
+    """
+    Resolves the atom names of ranges like "C1 > C5"
+    and works for each restraint line separately.
+    :param atoms_range: atoms with a range definition
+    :param atom_names: names of atoms in the fragment
+    """
+    # dict with lists of positions of the > or < sign:
+    rightleft = {'>': [], '<': []}
+    for rl in rightleft:
+        for num, i in enumerate(atoms_range):
+            i = i.upper()
+            if rl == i:
+                # fill the dictionary:
+                rightleft[rl].append(num)
+    for rl in rightleft:
+        # for each sign:
+        for i in rightleft[rl]:
+            # for each position of < or >:
+            if rl == '>':
+                # forward range
+                left = atom_names.index(atoms_range[i - 1]) + 1
+                right = atom_names.index(atoms_range[i + 1])
+                atoms_range[i:i + 1] = atom_names[left:right]
+            else:
+                # backward range
+                left = atom_names.index(atoms_range[i - 1])
+                right = atom_names.index(atoms_range[i + 1]) + 1
+                names = atom_names[right:left]
+                names.reverse()  # counting backwards
+                atoms_range[i:i + 1] = names
+    return atoms_range
+
+
+def walkdir(rootdir, include="", exclude=""):
+    """
+    Returns a list of files in all subdirectories with full path.
+    :param rootdir: base path from which walk should start
+    :param filter: list of file endings to include only e.g. ['.py', '.res']
+    :return: list of files
+
+    #>>> walkdir("../docs") #doctest: +REPORT_NDIFF +NORMALIZE_WHITESPACE +ELLIPSIS
+    #['../docs/test.txt']
+    #>>> walkdir("../setup/modpath.iss")
+    #['../setup/modpath.iss']
+    #>>> walkdir("../setup/modpath.iss", exclude=['.iss'])
+    #[]
+    #>>> walkdir("../docs", exclude=['.txt']) #doctest: +REPORT_NDIFF +NORMALIZE_WHITESPACE +ELLIPSIS
+    #[]
+    """
+    results = []
+    if not os.path.isdir(rootdir):
+        if os.path.splitext(rootdir)[1] in exclude:
+            return []
+        return [rootdir]
+    for root, sub_folders, files in os.walk(rootdir):
+        for file in files:
+            fullfilepath = os.path.join(root, file)
+            if exclude and os.path.splitext(fullfilepath)[1] in exclude:
+                continue
+            if include:
+                if os.path.splitext(fullfilepath)[1] in include:
+                    results.append(os.path.normpath(fullfilepath).replace('\\', '/'))
+            else:
+                results.append(os.path.normpath(fullfilepath).replace('\\', '/'))
+    return results
+
+
+def frac_to_cart(frac_coord: (list, tuple), cell: list) -> list:
+    """
+    Converts fractional coordinates to cartesian coodinates
+    :param frac_coord: [float, float, float]
+    :param cell:       [float, float, float, float, float, float]
+    """
+    a, b, c, alpha, beta, gamma = cell
+    x, y, z = frac_coord
+    alpha = radians(alpha)
+    beta = radians(beta)
+    gamma = radians(gamma)
+    cosastar = (cos(beta) * cos(gamma) - cos(alpha)) / (sin(beta) * sin(gamma))
+    sinastar = sqrt(1 - cosastar ** 2)
+    xc = a * x + (b * cos(gamma)) * y + (c * cos(beta)) * z
+    yc = 0 + (b * sin(gamma)) * y + (-c * sin(beta) * cosastar) * z
+    zc = 0 + 0 + (c * sin(beta) * sinastar) * z
+    return [xc, yc, zc]
+
+
+def cart_to_frac(cart_coord: list, cell: list) -> tuple:
+    """
+    converts cartesian coordinates to fractional coordinates
+    :param cart_coord: [float, float, float]
+    :param cell:       [float, float, float, float, float, float]
+    """
+    a, b, c, alpha, beta, gamma = cell
+    xc, yc, zc = cart_coord
+    alpha = radians(alpha)
+    beta = radians(beta)
+    gamma = radians(gamma)
+    cosastar = (cos(beta) * cos(gamma) - cos(alpha)) / (sin(beta) * sin(gamma))
+    sinastar = sqrt(1 - cosastar ** 2)
+    z = zc / (c * sin(beta) * sinastar)
+    y = (yc - (-c * sin(beta) * cosastar) * z) / (b * sin(gamma))
+    x = (xc - (b * cos(gamma)) * y - (c * cos(beta)) * z) / a
+    return x, y, z
+
+
+def determinante(a):
+    """
+    return determinant of 3x3 matrix
+    """
+    return (a[0][0] * (a[1][1] * a[2][2] - a[2][1] * a[1][2])
+            - a[1][0] * (a[0][1] * a[2][2] - a[2][1] * a[0][2])
+            + a[2][0] * (a[0][1] * a[1][2] - a[1][1] * a[0][2]))
+
+
+def subtract_vect(a, b):
+    """
+    subtract vector b from vector a
+    Deprecated, use mpmath instead!!!
+    :param a: [float, float, float]
+    :param b: [float, float, float]
+    """
+    return (a[0] - b[0],
+            a[1] - b[1],
+            a[2] - b[2])
```

### Comparing `shelxfile-8/shelxfile/refine/refine.py` & `shelxfile-9/shelxfile/refine/refine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,307 +1,307 @@
-# -*- encoding: utf-8 -*-
-# möp
-#
-# ----------------------------------------------------------------------------
-# "THE BEER-WARE LICENSE" (Revision 42):
-# <dkratzert@gmx.de> wrote this file. As long as you retain
-# this notice you can do whatever you want with this stuff. If we meet some day,
-# and you think this stuff is worth it, you can buy me a beer in return.
-# Daniel Kratzert
-# ----------------------------------------------------------------------------
-#
-from __future__ import print_function
-
-import os
-import re
-import subprocess
-import sys
-from contextlib import suppress
-from pathlib import Path
-from shutil import which, copyfile
-
-with suppress(ImportError):
-    from shelxfile import Shelxfile
-from shelxfile.misc.misc import remove_file, sep_line, find_line
-from shelxfile.shelx.cards import ACTA
-
-
-def get_xl_version_string(exe: str) -> str:
-    """
-    Extracts the version string from a SHELXL executable.
-    This is fast and needs no hashes etc.
-    :type exe: str
-    :param exe: path to SHELXL executable
-    """
-    try:
-        with open(exe, 'rb') as f:
-            binary = f.read()
-            position = binary.find(b'Version 201')
-            if position > 0:
-                f.seek(position + 8, 0)  # seek to version string
-                version = f.read(6)  # read version string
-                return version.decode('ascii')
-            else:
-                return ''
-    except IOError:
-        print("Could not determine SHELXL version. Refinement might fail to run.")
-        return ''
-
-
-def find_shelxl_exe(shelxpath=None) -> str:
-    """
-    returns the appropriate shelxl executable
-    """
-    names = ['shelxl', 'xl']
-    download = 'You can download SHELXL at http://shelx.uni-goettingen.de'
-    exe = ''
-    if shelxpath:
-        return shelxpath
-    for name in names:
-        exe = which(name)
-        if not exe:
-            continue
-        version = get_xl_version_string(exe)
-        if not version:
-            print('Your SHELXL version', exe, 'is too old for this Program')
-            print('Please use SHELXL 2017 or above!')
-            print(download)
-        version = version.split('/')
-        if int(version[0]) < 2017:
-            print('Your SHELXL version is too old. Please use SHELXL 2017 or above!')
-            print(download)
-        else:
-            return exe
-    return exe
-
-
-class ShelxlRefine():
-    """
-    A class to do a shelxl refinement. It is only for shelxl 2017 and above!
-    The resfilename should be without ending.
-    """
-
-    def __init__(self, shx: 'Shelxfile', resfile_path: Path, shelxpath: str = None):
-        self.shx = shx
-        self.shelxpath = shelxpath
-        self.resfile_name = resfile_path.stem
-        self._shelx_command = find_shelxl_exe(shelxpath)
-        self.backup_file = os.path.abspath(str(self.resfile_name + '.shx-bak'))
-        self._acta_card = ''  # stores the ACTA values if acta is removed before refinement
-
-        if not self._shelx_command:
-            print('\nSHELXL executable not found in system path.\n')
-            print('You can download SHELXL at http://shelx.uni-goettingen.de\n')
-
-    def get_b_array(self):
-        """
-        Approximates the B array size to ensure refinement.
-        """
-        number_of_atoms = self.shx.atoms.number
-        # This is a rough aproximation, but it works until you have a really high number of processors:
-        barray = number_of_atoms * 8
-        if barray <= 3000:
-            barray = 3000
-        return barray
-
-    def remove_acta_card(self, acta_card):
-        """
-        Removes ACTA x from reslist and stores value in self._acta_card.
-        """
-        if not acta_card:
-            return
-        self._acta_card = acta_card._textline.strip('\r\n')[:]
-        del self.shx._reslist[self.shx.index_of(acta_card)]
-        # acta_index = self.shx.index_of(acta_card)
-        # self.shx.delete_on_write.update([acta_index])
-        self.shx.acta = None
-
-    def restore_acta_card(self):
-        """
-        Place ACTA after UNIT
-        """
-        if not self._acta_card:
-            return
-        acta = ACTA(self.shx, self._acta_card.split())
-        self.shx._reslist.insert(self.shx.unit.index + 1, ' ')
-        self.shx.acta = self.shx.assign_card(acta, self.shx.unit.index + 1)
-
-    def backup_shx_file(self):
-        """
-        makes a copy of the res file
-        make backup in shxsaves before every fragment fit.
-        name: self.resfile_name-date-time-seconds.res
-        """
-        import datetime
-        now = datetime.datetime.now()
-        timestamp = (str(now.year) + '_' + str(now.month) + '_' + str(now.day) + '_' +
-                     str(now.hour) + '-' + str(now.minute) + '-' + str(now.second))
-        resfile = os.path.abspath(str(self.resfile_name + '.res'))
-        bakup_dir = os.path.abspath(os.path.dirname(resfile)) + os.path.sep + os.path.relpath('shxsaves')
-        try:
-            copyfile(resfile, self.backup_file)
-        except IOError:
-            print('*** Unable to make backup file from {}. ***'.format(resfile))
-            sys.exit()
-        if not os.path.exists(bakup_dir):
-            try:
-                os.makedirs(bakup_dir)
-            except(IOError, OSError):
-                print('*** Unable to create backup directory {}. ***'.format(bakup_dir))
-        try:
-            copyfile(resfile,
-                     bakup_dir + os.path.sep + os.path.split(self.resfile_name)[1] + '_' + timestamp + '.res')
-        except IOError:
-            print('\n*** Unable to make backup file from {} in shxsaves. ***'.format(resfile))
-
-    def restore_shx_file(self):
-        """
-        restores filename from backup
-        """
-        resfile = os.path.abspath(str(self.resfile_name + '.res'))
-        try:
-            print('*** Restoring previous res file. ***')
-            copyfile(self.backup_file, resfile)
-        except IOError:
-            print('Unable to restore res file from {}.'.format(self.backup_file))
-        try:
-            remove_file(self.backup_file)
-        except IOError:
-            print('Unable to delete backup file {}.'.format(self.backup_file))
-
-    def pretty_shx_output(self, out: str):
-        """
-        selectively prints the output from shelx
-        """
-        if out.startswith(' +  Copyright(C)'):
-            print(' SHELXL {}'.format(' '.join(out.split()[6:8])), end='')
-        if out.startswith(' R1'):
-            line = out[:].split()
-            print(' {}   {} {:>6}'.format(line[0], line[1], line[2][:6]), end='')
-        if re.match(r'.*CANNOT RESOLVE (SAME|RIGU|SIMU|DELU)', out):
-            print('\nWarning: Are you sure that all atoms are in the correct order?\n')
-        if re.match(r'.*CANNOT\s+OPEN\s+FILE.*hkl.*', out):
-            print('*** No hkl file found! ***')
-            print('*** You need a proper hkl file to run SHELXL! ***')
-            sys.exit()
-        if re.match(r'.*\*\* Extinction \(EXTI\) or solvent.*', out):
-            return
-        if re.match(r'.*\*\* MERG code changed to 0', out):
-            return
-        if re.match(r'.*\*\* Bond\(s\) to .* ignored', out):
-            return
-        if re.match(r'.*\*\*.*', out):
-            print('\n SHELXL says:')
-            print(' {}'.format(out.strip('\n\r')), end='')
-        if 'before cycle' in out:
-            print(out, end='')
-        if 'finished at' in out:
-            print(out, end='')
-
-    def run_shelxl(self, anis: bool = False, backup_before: bool = True) -> None:
-        """
-        This method runs shelxl 2013 on the res file self.resfile_name
-        """
-        if not self._shelx_command:
-            print('Unable to refine.')
-            return
-        if anis:
-            self.shx.insert_anis()
-        status = True
-        resfile = self.resfile_name + '.res'
-        hklfile = self.resfile_name + '.hkl'
-        current_path = Path('.').resolve()
-        # Go into path of resfile:
-        os.chdir(Path(resfile).parent)
-        if not os.path.exists(hklfile):
-            print('You need a proper hkl file to run SHELXL.')
-            sys.exit()
-        command_line = ['{}'.format(self._shelx_command), "-b{}".format(self.get_b_array()),
-                        '{}'.format(self.resfile_name)]
-        if backup_before:
-            self.backup_shx_file()
-        print(sep_line)
-        print(' Running SHELXL with "{}" and "{}"'.format(' '.join(command_line), self.shx.cycles))
-        with subprocess.Popen(command_line, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, bufsize=1,
-                              universal_newlines=True) as p:
-            for line in p.stdout:
-                # output only the most importand things from shelxl:
-                self.pretty_shx_output(line)
-        os.chdir(current_path)
-        if p.returncode != 0:
-            status = False
-        if os.stat(resfile).st_size < 10:
-            # status is False if shelx was unsecessful
-            status = False
-        if not status:
-            print(sep_line)
-            print('\nError: SHELXL terminated unexpectedly.')
-            print('Check for errors in your SHELX input file!\n')
-            self.restore_shx_file()
-            sys.exit()
-
-    def check_refinement_results(self, list_file):
-        """
-        Does some checks if the refinement makes sense e.g. if the data to parameter
-        ratio is in an acceptable range.
-        """
-        is_resfile_there = os.path.exists(self.resfile_name + '.res')
-        if is_resfile_there and is_resfile_there == 'zero':
-            print('Something failed in SHELXL. Please check your .ins and .lst file!')
-            self.restore_shx_file()
-            try:
-                remove_file(self.backup_file)
-            except IOError:
-                print('Unable to delete backup file {}.'.format(self.backup_file))
-            sys.exit()
-        if not is_resfile_there:
-            print('Something failed in SHELXL. Please check your .ins and .lst file!')
-            self.restore_shx_file()
-            try:
-                remove_file(self.backup_file)
-            except IOError:
-                print('Unable to delete backup file {}.'.format(self.backup_file))
-            sys.exit()
-        regex_final = r' Final Structure Factor Calculation.*\n'
-        final_results = find_line(list_file, regex_final)
-        # find data and parameters:
-        try:
-            dataobj = re.search(r'[0-9]+\s+data', list_file[final_results + 4])
-            data = float(dataobj.group(0).split()[0])
-            parameterobj = re.search(r'[0-9]+\s+parameters', list_file[final_results + 4])
-            parameters = float(parameterobj.group(0).split()[0])
-            restrobj = re.search(r'[0-9]+\s+restraints', list_file[find_line(list_file, r" GooF = S =.*")])
-            restraints = float(restrobj.group(0).split()[0])
-        except AttributeError:
-            return False
-        try:
-            data_to_parameter_ratio = data / parameters
-            restr_ratio = ((data + restraints) / parameters)
-        except ZeroDivisionError:
-            return False
-        lattline = find_line(list_file, r'^ LATT.*')
-        centro = None
-        if lattline:
-            try:
-                latt = int(list_file[lattline].split()[1])
-            except ValueError:
-                latt = 1
-            if latt > 0:
-                centro = True
-            else:
-                centro = False
-        if centro and data_to_parameter_ratio < 10:
-            print('*** Warning! The data/parameter ratio is getting low (ratio = {:.1f})! ***'
-                  '\n*** but consider (data+restraints)/parameter = {:.1f} ***'
-                  .format(data_to_parameter_ratio, restr_ratio))
-        if not centro and data_to_parameter_ratio < 7.5:
-            print('*** Warning! The data/parameter ratio is getting low (ratio = {:.1f})! ***'
-                  '\n*** but consider (data+restraints)/parameter = {:.1f} ***'
-                  .format(data_to_parameter_ratio, restr_ratio))
-        try:
-            remove_file(self.backup_file)
-        except IOError:
-            print('Unable to delete backup file {}.'.format(self.backup_file))
-
-
-if __name__ == '__main__':
-    pass
+# -*- encoding: utf-8 -*-
+# möp
+#
+# ----------------------------------------------------------------------------
+# "THE BEER-WARE LICENSE" (Revision 42):
+# <dkratzert@gmx.de> wrote this file. As long as you retain
+# this notice you can do whatever you want with this stuff. If we meet some day,
+# and you think this stuff is worth it, you can buy me a beer in return.
+# Daniel Kratzert
+# ----------------------------------------------------------------------------
+#
+from __future__ import print_function
+
+import os
+import re
+import subprocess
+import sys
+from contextlib import suppress
+from pathlib import Path
+from shutil import which, copyfile
+
+with suppress(ImportError):
+    from shelxfile import Shelxfile
+from shelxfile.misc.misc import remove_file, sep_line, find_line
+from shelxfile.shelx.cards import ACTA
+
+
+def get_xl_version_string(exe: str) -> str:
+    """
+    Extracts the version string from a SHELXL executable.
+    This is fast and needs no hashes etc.
+    :type exe: str
+    :param exe: path to SHELXL executable
+    """
+    try:
+        with open(exe, 'rb') as f:
+            binary = f.read()
+            position = binary.find(b'Version 201')
+            if position > 0:
+                f.seek(position + 8, 0)  # seek to version string
+                version = f.read(6)  # read version string
+                return version.decode('ascii')
+            else:
+                return ''
+    except IOError:
+        print("Could not determine SHELXL version. Refinement might fail to run.")
+        return ''
+
+
+def find_shelxl_exe(shelxpath=None) -> str:
+    """
+    returns the appropriate shelxl executable
+    """
+    names = ['shelxl', 'xl']
+    download = 'You can download SHELXL at http://shelx.uni-goettingen.de'
+    exe = ''
+    if shelxpath:
+        return shelxpath
+    for name in names:
+        exe = which(name)
+        if not exe:
+            continue
+        version = get_xl_version_string(exe)
+        if not version:
+            print('Your SHELXL version', exe, 'is too old for this Program')
+            print('Please use SHELXL 2017 or above!')
+            print(download)
+        version = version.split('/')
+        if int(version[0]) < 2017:
+            print('Your SHELXL version is too old. Please use SHELXL 2017 or above!')
+            print(download)
+        else:
+            return exe
+    return exe
+
+
+class ShelxlRefine():
+    """
+    A class to do a shelxl refinement. It is only for shelxl 2017 and above!
+    The resfilename should be without ending.
+    """
+
+    def __init__(self, shx: 'Shelxfile', resfile_path: Path, shelxpath: str = None):
+        self.shx = shx
+        self.shelxpath = shelxpath
+        self.resfile_name = resfile_path.stem
+        self._shelx_command = find_shelxl_exe(shelxpath)
+        self.backup_file = os.path.abspath(str(self.resfile_name + '.shx-bak'))
+        self._acta_card = ''  # stores the ACTA values if acta is removed before refinement
+
+        if not self._shelx_command:
+            print('\nSHELXL executable not found in system path.\n')
+            print('You can download SHELXL at http://shelx.uni-goettingen.de\n')
+
+    def get_b_array(self):
+        """
+        Approximates the B array size to ensure refinement.
+        """
+        number_of_atoms = self.shx.atoms.number
+        # This is a rough aproximation, but it works until you have a really high number of processors:
+        barray = number_of_atoms * 8
+        if barray <= 3000:
+            barray = 3000
+        return barray
+
+    def remove_acta_card(self, acta_card):
+        """
+        Removes ACTA x from reslist and stores value in self._acta_card.
+        """
+        if not acta_card:
+            return
+        self._acta_card = acta_card._textline.strip('\r\n')[:]
+        del self.shx._reslist[self.shx.index_of(acta_card)]
+        # acta_index = self.shx.index_of(acta_card)
+        # self.shx.delete_on_write.update([acta_index])
+        self.shx.acta = None
+
+    def restore_acta_card(self):
+        """
+        Place ACTA after UNIT
+        """
+        if not self._acta_card:
+            return
+        acta = ACTA(self.shx, self._acta_card.split())
+        self.shx._reslist.insert(self.shx.unit.index + 1, ' ')
+        self.shx.acta = self.shx._assign_card(acta, self.shx.unit.index + 1)
+
+    def backup_shx_file(self):
+        """
+        makes a copy of the res file
+        make backup in shxsaves before every fragment fit.
+        name: self.resfile_name-date-time-seconds.res
+        """
+        import datetime
+        now = datetime.datetime.now()
+        timestamp = (str(now.year) + '_' + str(now.month) + '_' + str(now.day) + '_' +
+                     str(now.hour) + '-' + str(now.minute) + '-' + str(now.second))
+        resfile = os.path.abspath(str(self.resfile_name + '.res'))
+        bakup_dir = os.path.abspath(os.path.dirname(resfile)) + os.path.sep + os.path.relpath('shxsaves')
+        try:
+            copyfile(resfile, self.backup_file)
+        except IOError:
+            print('*** Unable to make backup file from {}. ***'.format(resfile))
+            sys.exit()
+        if not os.path.exists(bakup_dir):
+            try:
+                os.makedirs(bakup_dir)
+            except(IOError, OSError):
+                print('*** Unable to create backup directory {}. ***'.format(bakup_dir))
+        try:
+            copyfile(resfile,
+                     bakup_dir + os.path.sep + os.path.split(self.resfile_name)[1] + '_' + timestamp + '.res')
+        except IOError:
+            print('\n*** Unable to make backup file from {} in shxsaves. ***'.format(resfile))
+
+    def restore_shx_file(self):
+        """
+        restores filename from backup
+        """
+        resfile = os.path.abspath(str(self.resfile_name + '.res'))
+        try:
+            print('*** Restoring previous res file. ***')
+            copyfile(self.backup_file, resfile)
+        except IOError:
+            print('Unable to restore res file from {}.'.format(self.backup_file))
+        try:
+            remove_file(self.backup_file)
+        except IOError:
+            print('Unable to delete backup file {}.'.format(self.backup_file))
+
+    def pretty_shx_output(self, out: str):
+        """
+        selectively prints the output from shelx
+        """
+        if out.startswith(' +  Copyright(C)'):
+            print(' SHELXL {}'.format(' '.join(out.split()[6:8])), end='')
+        if out.startswith(' R1'):
+            line = out[:].split()
+            print(' {}   {} {:>6}'.format(line[0], line[1], line[2][:6]), end='')
+        if re.match(r'.*CANNOT RESOLVE (SAME|RIGU|SIMU|DELU)', out):
+            print('\nWarning: Are you sure that all atoms are in the correct order?\n')
+        if re.match(r'.*CANNOT\s+OPEN\s+FILE.*hkl.*', out):
+            print('*** No hkl file found! ***')
+            print('*** You need a proper hkl file to run SHELXL! ***')
+            sys.exit()
+        if re.match(r'.*\*\* Extinction \(EXTI\) or solvent.*', out):
+            return
+        if re.match(r'.*\*\* MERG code changed to 0', out):
+            return
+        if re.match(r'.*\*\* Bond\(s\) to .* ignored', out):
+            return
+        if re.match(r'.*\*\*.*', out):
+            print('\n SHELXL says:')
+            print(' {}'.format(out.strip('\n\r')), end='')
+        if 'before cycle' in out:
+            print(out, end='')
+        if 'finished at' in out:
+            print(out, end='')
+
+    def run_shelxl(self, anis: bool = False, backup_before: bool = True) -> None:
+        """
+        This method runs shelxl 2013 on the res file self.resfile_name
+        """
+        if not self._shelx_command:
+            print('Unable to refine.')
+            return
+        if anis:
+            self.shx.insert_anis()
+        status = True
+        resfile = self.resfile_name + '.res'
+        hklfile = self.resfile_name + '.hkl'
+        current_path = Path('.').resolve()
+        # Go into path of resfile:
+        os.chdir(Path(resfile).parent)
+        if not os.path.exists(hklfile):
+            print('You need a proper hkl file to run SHELXL.')
+            sys.exit()
+        command_line = ['{}'.format(self._shelx_command), "-b{}".format(self.get_b_array()),
+                        '{}'.format(self.resfile_name)]
+        if backup_before:
+            self.backup_shx_file()
+        print(sep_line)
+        print(' Running SHELXL with "{}" and "{}"'.format(' '.join(command_line), self.shx.cycles))
+        with subprocess.Popen(command_line, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, bufsize=1,
+                              universal_newlines=True) as p:
+            for line in p.stdout:
+                # output only the most importand things from shelxl:
+                self.pretty_shx_output(line)
+        os.chdir(current_path)
+        if p.returncode != 0:
+            status = False
+        if os.stat(resfile).st_size < 10:
+            # status is False if shelx was unsecessful
+            status = False
+        if not status:
+            print(sep_line)
+            print('\nError: SHELXL terminated unexpectedly.')
+            print('Check for errors in your SHELX input file!\n')
+            self.restore_shx_file()
+            sys.exit()
+
+    def check_refinement_results(self, list_file):
+        """
+        Does some checks if the refinement makes sense e.g. if the data to parameter
+        ratio is in an acceptable range.
+        """
+        is_resfile_there = os.path.exists(self.resfile_name + '.res')
+        if is_resfile_there and is_resfile_there == 'zero':
+            print('Something failed in SHELXL. Please check your .ins and .lst file!')
+            self.restore_shx_file()
+            try:
+                remove_file(self.backup_file)
+            except IOError:
+                print('Unable to delete backup file {}.'.format(self.backup_file))
+            sys.exit()
+        if not is_resfile_there:
+            print('Something failed in SHELXL. Please check your .ins and .lst file!')
+            self.restore_shx_file()
+            try:
+                remove_file(self.backup_file)
+            except IOError:
+                print('Unable to delete backup file {}.'.format(self.backup_file))
+            sys.exit()
+        regex_final = r' Final Structure Factor Calculation.*\n'
+        final_results = find_line(list_file, regex_final)
+        # find data and parameters:
+        try:
+            dataobj = re.search(r'[0-9]+\s+data', list_file[final_results + 4])
+            data = float(dataobj.group(0).split()[0])
+            parameterobj = re.search(r'[0-9]+\s+parameters', list_file[final_results + 4])
+            parameters = float(parameterobj.group(0).split()[0])
+            restrobj = re.search(r'[0-9]+\s+restraints', list_file[find_line(list_file, r" GooF = S =.*")])
+            restraints = float(restrobj.group(0).split()[0])
+        except AttributeError:
+            return False
+        try:
+            data_to_parameter_ratio = data / parameters
+            restr_ratio = ((data + restraints) / parameters)
+        except ZeroDivisionError:
+            return False
+        lattline = find_line(list_file, r'^ LATT.*')
+        centro = None
+        if lattline:
+            try:
+                latt = int(list_file[lattline].split()[1])
+            except ValueError:
+                latt = 1
+            if latt > 0:
+                centro = True
+            else:
+                centro = False
+        if centro and data_to_parameter_ratio < 10:
+            print('*** Warning! The data/parameter ratio is getting low (ratio = {:.1f})! ***'
+                  '\n*** but consider (data+restraints)/parameter = {:.1f} ***'
+                  .format(data_to_parameter_ratio, restr_ratio))
+        if not centro and data_to_parameter_ratio < 7.5:
+            print('*** Warning! The data/parameter ratio is getting low (ratio = {:.1f})! ***'
+                  '\n*** but consider (data+restraints)/parameter = {:.1f} ***'
+                  .format(data_to_parameter_ratio, restr_ratio))
+        try:
+            remove_file(self.backup_file)
+        except IOError:
+            print('Unable to delete backup file {}.'.format(self.backup_file))
+
+
+if __name__ == '__main__':
+    pass
```

### Comparing `shelxfile-8/shelxfile/shelx/cards.py` & `shelxfile-9/shelxfile/shelx/cards.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1871 +1,1902 @@
-import re
-from math import cos, radians, sqrt
-from typing import List
-
-from shelxfile.misc.dsrmath import my_isnumeric, SymmetryElement
-from shelxfile.misc.misc import chunks, ParseParamError, ParseNumError, \
-    ParseOrderError, DEBUG, ParseSyntaxError
-
-"""
-SHELXL cards:
-
-ABIN n1 n2
-ACTA 2θfull[#]
-AFIX mn d[#] sof[11] U[10.08]
-ANIS n
-ANIS names
-ANSC six coefficients
-ANSR anres[0.001]
-BASF scale factors
-BIND atom1 atom2
-BIND m n
-BLOC n1 n2 atomnames
-BOND atomnames
-BUMP s [0.02]
-CELL λ a b c α β γ
-CGLS nls[0] nrf[0] nextra[0]
-CHIV V[0] s[0.1] atomnames
-CONF atomnames max_d[1.9] max_a[170]
-CONN bmax[12] r[#] atomnames or CONN bmax[12]
-DAMP damp[0.7] limse[15]
-DANG d s[0.04] atom pairs
-DEFS sd[0.02] sf[0.1] su[0.01] ss[0.04] maxsof[1]
-DELU s1[0.01] s2[0.01] atomnames
-DFIX d s[0.02] atom pairs
-DISP E f' f"[#] mu[#]
-EADP atomnames
-END
-EQIV $n symmetry operation
-EXTI x[0]
-EXYZ atomnames
-FEND
-FLAT s[0.1] four or more atoms
-FMAP code[2] axis[#] nl[53]
-FRAG code[17] a[1] b[1] c[1] α[90] β[90] γ[90]
-FREE atom1 atom2
-FVAR osf[1] free variables
-GRID sl[#] sa[#] sd[#] dl[#] da[#] dd[#]
-HFIX mn U[#] d[#] atomnames
-HKLF N[0] S[1] r11...r33[1 0 0 0 1 0 0 0 1] sm[1] m[0]
-HTAB dh[2.0]
-HTAB donor-atom acceptor-atom
-ISOR s[0.1] st[0.2] atomnames
-LATT N[1]
-LAUE E
-LIST m[#] mult[1]
-L.S. nls[0] nrf[0] nextra[0]
-MERG n[2]
-MORE m[1]
-MOVE dx[0] dy[0] dz[0] sign[1]
-MPLA na atomnames
-NCSY DN sd[0.1] su[0.05] atoms
-NEUT
-OMIT atomnames
-OMIT s[-2] 2θ(lim)[180]
-OMIT h k l
-PART n sof
-PLAN npeaks[20] d1[#] d2[#]
-PRIG p[#]
-REM
-RESI class[ ] number[0] alias
-RIGU s1[0.004] s2[0.004] atomnames
-RTAB codename atomnames
-SADI s[0.02] pairs of atoms
-SAME s1[0.02] s2[0.04] atomnames
-SFAC elements
-SFAC E a1 b1 a2 b2 a3 b3 a4 b4 c f' f" mu r wt
-SHEL lowres[infinite] highres[0]
-SIMU s[0.04] st[0.08] dmax[2.0] atomnames
-SIZE dx dy dz
-SPEC del[0.2]
-STIR sres step[0.01]
-SUMP c sigma c1 m1 c2 m2 ...
-SWAT g[0] U[2]
-SYMM symmetry operation
-TEMP T[20]
-TITL [ ]
-TWIN 3x3 matrix [-1 0 0 0 -1 0 0 0 -1] N[2]
-TWST N[0]
-UNIT n1 n2 ...
-WGHT a[0.1] b[0] c[0] d[0] e[0] f[.33333]
-WIGL del[0.2] dU[0.2]
-WPDB n[1]
-XNPD Umin[-0.001]
-ZERR Z esd(a) esd(b) esd(c) esd(α) esd(β) esd(γ)
-"""
-
-
-class Residue():
-    def __init__(self):
-        self.shx = None
-        self._spline = None
-
-    @property
-    def residue_number(self):
-        if '_' in self._spline[0]:
-            _, suffix = self._spline[0].upper().split('_')
-            if any([x.isalpha() for x in suffix]):
-                self.residue_class = suffix
-            else:
-                # TODO: implement _+, _- and _*
-                if '*' in suffix:
-                    return list(self.shx.residues.residue_numbers.keys())
-                else:
-                    return [int(suffix)]
-        return [0]
-
-
-class Restraint(Residue):
-
-    def __init__(self, shx, spline: list):
-        """
-        Base class for parsing restraints.
-        TODO: resolve ranges like SADI_CCF3 O1 > F9
-        """
-        super().__init__()
-        self.shx = shx
-        self.residue_class = ''  # '' is the default class (with residue number 0)
-        self.textline = ' '.join(spline)
-        self.name = None
-        self.atoms = []
-
-    @property
-    def index(self):
-        return self.shx.index_of(self)
-
-    def _parse_line(self, spline, pairs=False):
-        """
-        Residues may be referenced by any instruction that allows atom names; the reference takes
-        the form of the character '_' followed by either the residue class or number without intervening
-        spaces.
-        Individual atom names in an instruction may be followed by '_' and a residue number, but not by '_* ' or '_'
-        and a residue class. If an atom name is not followed by a residue number, the current residue is
-        assumed (unless overridden by a global residue number or class appended to the instruction
-        codeword).
-        """
-        self._spline = spline
-        # TODO: check if suffix is a residue class and set instance variable accordingly
-        if '_' in spline[0]:
-            self.name, suffix = spline[0].upper().split('_')
-        else:
-            self.name = spline[0].upper()
-        self.set_defs_values()
-        self.check_if_class_name_fits_to_command()
-        params = []
-        atoms = []
-        for x in spline[1:]:
-            if my_isnumeric(x):
-                params.append(float(x))
-            else:
-                atoms.append(x)
-        if pairs:
-            return params, chunks(atoms, 2)
-        else:
-            return params, atoms
-
-    def check_if_class_name_fits_to_command(self):
-        if DEBUG and self.__class__.__name__ != self.name:
-            print('*** Trying to parse restraint with wrong class ***')
-            raise ParseSyntaxError
-
-    def set_defs_values(self):
-        # Beware! DEFS changes only the non-defined default values:
-        # DEFS sd[0.02] sf[0.1] su[0.01] ss[0.04] maxsof[1]
-        if self.shx.defs:  # and self.shx.defs.active:
-            if self.name == 'DFIX':
-                self.s = self.shx.defs.sd
-            if self.name == 'SAME':
-                self.s1 = self.shx.defs.sd
-                self.s2 = self.shx.defs.sd * 2
-            if self.name == 'SADI':
-                self.s = self.shx.defs.sd
-            if self.name == 'CHIV':
-                self.s = self.shx.defs.sf
-            if self.name == 'FLAT':
-                self.s = self.shx.defs.sf
-            if self.name == 'DELU':
-                self.s1 = self.shx.defs.su
-                self.s2 = self.shx.defs.su
-            if self.name == 'SIMU':
-                self.s = self.shx.defs.ss
-                self.st = self.shx.defs.ss * 2
-
-    def _paircheck(self):
-        if not self.atoms:
-            return
-        if len(self.atoms[-1]) != 2 and DEBUG:
-            print('*** Wrong number of numerical parameters ***')
-            print('Instruction: {}'.format(self.textline))
-            raise ParseNumError
-
-    def __iter__(self):
-        for x in self.textline.split():
-            yield x
-
-    def __repr__(self):
-        return self.textline
-
-    def __str__(self):
-        return self.textline
-
-    def split(self):
-        return self.textline.split()
-
-
-class Command():
-    """
-    A class to parse all general commands except restraints.
-    """
-
-    def __init__(self, shx, spline: list):
-        self._shx = shx
-        self._spline = spline
-        self.residue_class = ''
-        self._textline = ' '.join(spline)
-
-    def _parse_line(self, spline, intnums=False):
-        """
-        :param spline: Splitted shelxl line
-        :param intnums: if numerical parameters should be integer
-        :return: numerical parameters and words
-        """
-        if '_' in spline[0]:
-            self._card_name, suffix = spline[0].upper().split('_')
-        else:
-            self._card_name = spline[0].upper()
-        numparams = []
-        words = []
-        for x in spline[1:]:  # all values after SHELX card
-            if str.isdigit(x[0]) or x[0] in '+-':
-                if intnums:
-                    numparams.append(int(x))
-                else:
-                    numparams.append(float(x))
-            else:
-                words.append(x)
-        return numparams, words
-
-    @property
-    def index(self):
-        return self._shx.index_of(self)
-
-    @property
-    def position(self) -> int:
-        return self.index
-
-    def __iter__(self):
-        for x in self.__repr__().split():
-            yield x
-
-    def split(self):
-        return self._textline.split()
-
-    def __str__(self):
-        return self._textline
-
-    def __repr__(self):
-        return self._textline
-
-
-class ABIN(Command):
-
-    def __init__(self, shx, spline):
-        """
-        ABIN n1 n2
-        """
-        super(ABIN, self).__init__(shx, spline)
-        p, _ = self._parse_line(spline)
-        if len(p) > 0:
-            self.n1 = p[0]
-        if len(p) > 1:
-            self.n2 = p[1]
-
-
-class ANIS(Command):
-
-    def __init__(self, shx, spline: List):
-        """
-        ANIS n
-        ANIS names
-        """
-        super(ANIS, self).__init__(shx, spline)
-        p, self.atoms = self._parse_line(spline)
-        self.over_all = True
-        if len(p) > 0:
-            self.over_all = False
-            self.n = p[0]
-        if len(self.atoms) > 0:
-            self.over_all = False
-
-    def __bool__(self):
-        return True
-
-
-class MPLA(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        MPLA na atomnames
-        """
-        super(MPLA, self).__init__(shx, spline)
-        p, self.atoms = self._parse_line(spline, intnums=True)
-        if len(p) > 0:
-            self.na = p[0]
-
-
-class MORE(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        MORE m[1]
-        """
-        super(MORE, self).__init__(shx, spline)
-        self.m = 1
-        p, _ = self._parse_line(spline, intnums=True)
-        self.m = p[0]
-
-
-class CELL(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        CELL λ a b c α β γ
-        """
-        super(CELL, self).__init__(shx, spline)
-        p, _ = self._parse_line(spline)
-        self._cell_list = []
-        if len(p) > 0:
-            self.wavelen = float(p[0])
-        if len(p) > 6:
-            self._cell_list = p[1:]
-            self.a = p[1]
-            self.b = p[2]
-            self.c = p[3]
-            self.alpha = p[4]
-            self.beta = p[5]
-            self.gamma = p[6]
-            self.cosal = cos(radians(self.alpha))
-            self.cosbe = cos(radians(self.beta))
-            self.cosga = cos(radians(self.gamma))
-        else:
-            raise ParseSyntaxError
-
-    @property
-    def volume(self) -> float:
-        """
-        calculates the volume of a unit cell
-        """
-        try:
-            ca, cb, cg = cos(radians(self.alpha)), cos(radians(self.beta)), cos(radians(self.gamma))
-            v = self.a * self.b * self.c * sqrt(1 + 2 * ca * cb * cg - ca ** 2 - cb ** 2 - cg ** 2)
-        except AttributeError:
-            # No valid celll
-            v = 0.0
-        return v
-
-    @property
-    def V(self) -> float:
-        return self.volume
-
-    def __iter__(self):
-        return iter(self._cell_list)
-
-    def __getitem__(self, item):
-        return self._cell_list[item]
-
-
-class ZERR(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        ZERR Z esd(a) esd(b) esd(c) esd(α) esd(β) esd(γ)
-        """
-        super(ZERR, self).__init__(shx, spline)
-        p, _ = self._parse_line(spline)
-        self.Z = 1
-        if len(p) > 0:
-            self.Z = p[0]
-        if len(p) > 6:
-            self.esd_list = p[1:]
-            self.esd_a = p[0]
-            self.esd_b = p[1]
-            self.esd_c = p[2]
-            self.esd_al = p[3]
-            self.esd_be = p[4]
-            self.esd_ga = p[5]
-
-
-class AFIX(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        AFIX mn d[#] sof[11] U[10.08]
-        """
-        super(AFIX, self).__init__(shx, spline)
-        p, _ = self._parse_line(spline)
-        self.U = 10.08
-        self.sof = 11.0
-        if len(p) > 0:
-            self.mn = int(p[0])
-        if len(p) > 1:
-            self.d = p[1]
-        if len(p) > 2:
-            self.sof = p[2]
-        if len(p) > 3:
-            self.U = p[3]
-
-    def __bool__(self):
-        if self.mn > 0:
-            return True
-        else:
-            return False
-
-
-class Residues():
-
-    def __init__(self, shx):
-        self.shx = shx
-        self.all_residues = []
-        self.residue_classes = {}  # class: numbers
-        # self.residue_numbers = {}  # number: class
-
-    def append(self, resi: 'RESI') -> None:
-        """
-        Adds a new residues to the list of residues.
-        """
-        self.all_residues.append(resi)
-        # Collect dict with class: numbers
-        if resi.residue_class in self.residue_classes:
-            self.residue_classes[resi.residue_class].append(resi.residue_number)
-        else:
-            self.residue_classes[resi.residue_class] = [resi.residue_number]
-        """
-        # Collect dict with number: classes
-        if resi.residue_number in self.residue_numbers:
-            if DEBUG:
-                print('*** Duplicate residue number {} found! ***'.format(resi.residue_number))
-        else:
-            self.residue_numbers[resi.residue_number] = resi.residue_class
-        """
-
-    @property
-    def residue_numbers(self):
-        return dict((x.residue_number, x.residue_class) for x in self.shx.residues.all_residues)
-
-
-class RESI():
-
-    def __init__(self, shx, spline: list):
-        """
-        RESI class[ ] number[0] alias
-        """
-        self.shx = shx
-        self.residue_class = ''
-        self.residue_number = 0
-        self.alias = None
-        self.chain_id = None
-        self.textline = ' '.join(spline)
-        if len(spline) < 2 and DEBUG:
-            print('*** Wrong RESI definition found! Check your RESI instructions ***')
-            raise ParseParamError
-        self.get_resi_definition(spline)
-        if self.residue_number < -999 or self.residue_number > 9999:
-            print('*** Invalid residue number given. ****')
-            raise ParseSyntaxError
-
-    def get_resi_definition(self, resi: list) -> tuple:
-        """
-        RESI class[ ] number[0] alias
-
-        Returns the residue number and class of a string like 'RESI TOL 1'
-        or 'RESI 1 TOL'
-
-        Residue names may now begin with a digit.
-        They must however contain at least one letter
-
-        Allowed residue numbers is now from -999 to 9999 (2017/1)
-        """
-        alpha = re.compile('[a-zA-Z]')
-        for x in resi:
-            if alpha.search(x):
-                if ':' in x:
-                    # contains ":" thus must be a chain-id+number
-                    self.chain_id, self.residue_number = x.split(':')[0], int(x.split(':')[1])
-                else:
-                    # contains letters, must be a name (class)
-                    self.residue_class = x
-            else:
-                # everything else can only be a number
-                if self.residue_number > 0:
-                    self.alias = int(x)
-                else:
-                    try:
-                        self.residue_number = int(x)
-                    except ValueError:
-                        self.residue_number = 0
-        return self.residue_class, self.residue_number, self.chain_id, self.alias
-
-    def _parse_line(self, spline, intnums=False):
-        """
-        :param spline: Splitted shelxl line
-        :param intnums: if numerical parameters should be integer
-        :return: numerical parameters and words
-        """
-        if '_' in spline[0]:
-            self.card_name, suffix = spline[0].upper().split('_')
-            if any([x.isalpha() for x in suffix]):
-                self.residue_class = suffix
-            else:
-                # TODO: implement _+, _- and _*
-                self.residue_number = int(suffix)
-        else:
-            self.card_name = spline[0].upper()
-        numparams = []
-        words = []
-        for x in spline[1:]:  # all values after SHELX card
-            if str.isdigit(x[0]) or x[0] in '+-':
-                if intnums:
-                    numparams.append(int(x))
-                else:
-                    numparams.append(float(x))
-            else:
-                words.append(x)
-        return numparams, words
-
-    @property
-    def index(self):
-        return self.shx.index_of(self)
-
-    def __iter__(self):
-        for x in self.__repr__().split():
-            yield x
-
-    def split(self):
-        return self.textline.split()
-
-    def __str__(self):
-        return self.textline
-
-    def __repr__(self):
-        return self.textline
-
-    def __bool__(self):
-        if self.residue_number > 0:
-            return True
-        else:
-            return False
-
-
-class PART(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        PART n sof
-        """
-        super(PART, self).__init__(shx, spline)
-        p, _ = self._parse_line(spline)
-        self.sof = 11.0
-        self.n = 0
-        try:
-            self.n = int(p[0])
-        except(ValueError, IndexError):
-            if DEBUG:
-                print('*** Wrong PART definition in line {} found! '
-                      'Check your PART instructions ***'.format(shx.error_line_num))
-                raise
-            self.n = 0
-        if len(p) > 1:
-            self.sof = float(p[1])
-
-    def __bool__(self):
-        if self.n > 0:
-            return True
-        else:
-            return False
-
-
-class XNPD(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        XNPD Umin[-0.001]
-        """
-        super(XNPD, self).__init__(shx, spline)
-        p, _ = self._parse_line(spline)
-        self.Umin = -0.001
-        if len(p) > 0:
-            self.Umin = p[0]
-
-
-class SIZE(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        SIZE dx dy dz
-        """
-        super(SIZE, self).__init__(shx, spline)
-        self.dx, self.dy, self.dz = None, None, None
-        p, _ = self._parse_line(spline)
-        if len(p) > 0:
-            self.dx = p[0]
-        if len(p) > 1:
-            self.dy = p[1]
-        if len(p) > 2:
-            self.dz = p[2]
-
-    def _as_text(self):
-        if all([self.dx, self.dy, self.dz]):
-            return "SIZE {:,g} {:,g} {:,g}".format(self.dx, self.dy, self.dz)
-        else:
-            return ""
-
-    def __repr__(self):
-        return self._as_text()
-
-    def __str__(self):
-        return self._as_text()
-
-
-class SHEL(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        SHEL lowres[infinite] highres[0]
-        """
-        super(SHEL, self).__init__(shx, spline)
-        params, _ = self._parse_line(spline)
-        if len(params) > 0:
-            self.lowres = params[0]
-        if len(params) > 1:
-            self.highres = params[1]
-
-
-class WIGL(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        WIGL del[0.2] dU[0.2]
-        """
-        super(WIGL, self).__init__(shx, spline)
-        p, _ = self._parse_line(spline)
-        self.d = 0.2
-        self.dU = 0.2
-        if len(p) > 0:
-            self.d = p[0]
-        if len(p) > 1:
-            self.dU = p[1]
-
-
-class WPDB(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        WPDB n[1]
-        """
-        super(WPDB, self).__init__(shx, spline)
-        p, _ = self._parse_line(spline)
-        self.n = 1
-        if len(p) > 0:
-            self.n = p[0]
-
-
-class SPEC(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        SPEC d[0.2]
-        """
-        super(SPEC, self).__init__(shx, spline)
-        p, _ = self._parse_line(spline)
-        if len(p) > 0:
-            self.d = p[0]
-
-
-class STIR(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        STIR sres step[0.01]
-        """
-        super(STIR, self).__init__(shx, spline)
-        p, _ = self._parse_line(spline)
-        self.step = 0.01
-        if len(p) > 0:
-            self.sres = p[0]
-        if len(p) > 1:
-            self.step = p[1]
-
-    def __repr__(self):
-        return "STIR {} {}".format(self.sres if self.sres else '', self.step)
-
-    def __str__(self):
-        return "STIR {} {}".format(self.sres if self.sres else '', self.step)
-
-
-class TWST(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        TWST N[0] (N[1] after SHELXL-2018/3)
-        Twin component number to be used for the completeness and Friedel completeness statistics.
-        """
-        super(TWST, self).__init__(shx, spline)
-        p, _ = self._parse_line(spline)
-        self.N = 1
-        if len(p) > 0:
-            self.N = p[0]
-
-
-class RTAB(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        RTAB codename atomnames
-        """
-        super(RTAB, self).__init__(shx, spline)
-        self.code = spline.pop(1)
-        _, self.atoms = self._parse_line(spline)
-
-
-class PRIG(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        PRIG p[#]
-        """
-        super(PRIG, self).__init__(shx, spline)
-        params, _ = self._parse_line(spline)
-        if len(params) > 0:
-            self.p = params[0]
-
-
-class PLAN(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        PLAN npeaks[20] d1[#] d2[#]
-        """
-        super(PLAN, self).__init__(shx, spline)
-        params, _ = self._parse_line(spline)
-        if len(params) > 0:
-            self.npeaks = params[0]
-        if len(params) > 1:
-            self.d1 = params[1]
-        if len(params) > 2:
-            self.d2 = params[2]
-
-
-class FRAG(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        FRAG code[17] a[1] b[1] c[1] α[90] β[90] γ[90]
-        """
-        super(FRAG, self).__init__(shx, spline)
-        params, _ = self._parse_line(spline)
-        self.code = params[0]
-        self.cell = params[1:7]
-
-
-class FREE(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        FREE atom1 atom2
-        """
-        super(FREE, self).__init__(shx, spline)
-        _, atoms = self._parse_line(spline)
-        try:
-            self.atom1 = atoms[0]
-            self.atom2 = atoms[1]
-        except IndexError:
-            raise ParseParamError
-
-
-class FMAP(Command):
-    """
-    FMAP code[2] axis[#] nl[53]
-    """
-
-    def __init__(self, shx, spline: list):
-        super(FMAP, self).__init__(shx, spline)
-        params, _ = self._parse_line(spline)
-        if len(params) > 0:
-            self.code = params[0]
-        if len(params) > 1:
-            self.axis = params[1]
-        if len(params) > 2:
-            self.axis = params[2]
-
-
-class MOVE(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        MOVE dx[0] dy[0] dz[0] sign[1]
-        """
-        super(MOVE, self).__init__(shx, spline)
-        params, _ = self._parse_line(spline)
-        if len(params) > 2:
-            self.dxdydz = params[:3]
-        if len(params) > 3:
-            self.sign = params[3]
-
-
-class MERG(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        MERG n[2]
-        """
-        super(MERG, self).__init__(shx, spline)
-        self.n = None
-        _n, _ = self._parse_line(spline)
-        if len(_n) > 0:
-            self.n = _n[0]
-
-
-class HTAB(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        HTAB dh[2.0]
-        HTAB donor-atom acceptor-atom
-        """
-        super(HTAB, self).__init__(shx, spline)
-        self.dh = None
-        dh, atoms = self._parse_line(spline)
-        if dh:
-            self.dh = dh[0]
-        if len(atoms) == 2:
-            self.donor = atoms[0]
-            self.acceptor = atoms[1]
-
-
-class GRID(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        GRID sl[#] sa[#] sd[#] dl[#] da[#] dd[#]
-        """
-        super(GRID, self).__init__(shx, spline)
-        params, _ = self._parse_line(spline)
-        if len(params) > 0:
-            self.sl = params[0]
-        if len(params) > 1:
-            self.sa = params[1]
-        if len(params) > 2:
-            self.sd = params[2]
-        if len(params) > 3:
-            self.dl = params[3]
-        if len(params) > 4:
-            self.da = params[4]
-        if len(params) > 5:
-            self.dd = params[5]
-
-
-class ACTA(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        ACTA 2θfull[#]
-        """
-        super(ACTA, self).__init__(shx, spline)
-        self.twotheta, _ = self._parse_line(spline)
-        self.shx = shx
-
-    def _as_str(self):
-        if self.twotheta:
-            return "ACTA {:,g}".format(self.twotheta[0])
-        else:
-            return "ACTA"
-
-    def __repr__(self):
-        return self._as_str()
-
-    def __str__(self):
-        return self._as_str()
-
-
-class BLOC(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        BLOC n1 n2 atomnames
-        """
-        super(BLOC, self).__init__(shx, spline)
-        params, self.atoms = self._parse_line(spline)
-        if len(params) > 1:
-            self.n2 = params[1]
-        if len(params) > 0:
-            self.n1 = params[0]
-        self.shx = shx
-
-
-class FVAR():
-    def __init__(self, number: int = 1, value: float = 0.0):
-        """
-        FVAR osf[1] free variables
-        """
-        self.fvar_value = value  # value
-        self.number = number  # occurence inside of FVAR instructions
-        self.usage = 1
-
-    def __str__(self):
-        return str(float(self.fvar_value))
-
-    def __repr__(self):
-        return str(float(self.fvar_value))
-
-
-class FVARs():
-    def __init__(self, shx):
-        super(FVARs, self).__init__()
-        self.fvars = []  # free variables
-        self.shx = shx
-        self._fvarline = 0
-
-    def __iter__(self):
-        """
-        Must be defined for __repr__() to work.
-        """
-        for x in self.fvars:
-            yield x
-
-    def __getitem__(self, item: int) -> str:
-        # SHELXL counts fvars from 1 to x:
-        item = abs(item) - 1
-        return self.fvars[item].fvar_value
-
-    def __setitem__(self, key, fvar_value):
-        self.fvars[key] = fvar_value
-
-    def __len__(self) -> int:
-        return len(self.fvars)
-
-    def __str__(self) -> str:
-        # returnes FVAR as list of FVAR instructions with seven numbers in one line
-        lines = chunks(self.as_stringlist, 7)
-        fvars = ['   '.join(i) for i in lines]
-        fvars = ['FVAR   ' + i for i in fvars]
-        return "\n".join(fvars)
-
-    def __repr__(self):
-        return str([x for x in self.fvars])
-
-    @property
-    def position(self) -> int:
-        return self.shx.index_of(self)
-
-    def set_free_variables(self, fvar: int, dummy_fvar: float = 0.5):
-        """
-        Inserts additional free variables according to the fvar number.
-        """
-        if fvar > 99:
-            print('*** SHELXL allows only 99 free variables! ***')
-            raise ParseParamError
-        varlen = len(self.fvars)
-        difference = (abs(fvar) - varlen)
-        if difference > 0:
-            for n in range(int(difference)):
-                fv = FVAR(varlen + n, dummy_fvar)
-                self.fvars.append(fv)
-
-    def append(self, fvar) -> None:
-        self.fvars.append(fvar)
-
-    def set_fvar_usage(self, fvarnum: int, times: int = 1) -> None:
-        """
-        Incerements the usage count of a free variable by times.
-        """
-        fvarnum = abs(fvarnum)
-        if len(self.fvars) >= abs(fvarnum):
-            self.fvars[fvarnum - 1].usage += times
-        elif fvarnum > 1 and DEBUG:
-            print('*** Free variable {} is not defined but used! ***'.format(fvarnum))
-
-    def get_fvar_usage(self, fvarnum):
-        """
-        Returns the usage (count) of a certain free variable.
-        """
-        try:
-            usage = self.fvars[fvarnum - 1].usage
-        except IndexError:
-            return 0
-        return usage
-
-    def fvars_used(self):
-        """
-        Retruns a dictionary with the usage of all free variables.
-        """
-        used = {}
-        for num, fv in enumerate(self.fvars):
-            used[num + 1] = fv.usage
-        return used
-
-    @property
-    def as_stringlist(self):
-        return [str(x.fvar_value) for x in self.fvars]
-
-
-class CONF(Command):
-
-    def __init__(self, shx, spline: list) -> None:
-        """
-        CONF atomnames max_d[1.9] max_a[170]
-        """
-        super(CONF, self).__init__(shx, spline)
-
-
-class CONN(Command):
-
-    def __init__(self, shx, spline: list) -> None:
-        """
-        CONN bmax[12] r[#] atomnames or CONN bmax[12]
-        """
-        super(CONN, self).__init__(shx, spline)
-
-
-class REM(Command):
-
-    def __init__(self, shx, spline: list) -> None:
-        """
-        Parses REM lines
-        """
-        super(REM, self).__init__(shx, spline)
-
-
-class BIND(Command):
-
-    def __init__(self, shx, spline: list) -> None:
-        """
-        BIND atom1 atom2
-        BIND m n
-        """
-        super(BIND, self).__init__(shx, spline)
-        self.parts, self.atoms = self._parse_line(spline)
-
-
-class BOND(Command):
-
-    def __init__(self, shx, spline: list) -> None:
-        """
-        BOND atomnames
-        """
-        super(BOND, self).__init__(shx, spline)
-        _, self.atoms = self._parse_line(spline)
-
-
-class DISP(Command):
-    """
-    DISP E f' f"[#] mu[#]
-    """
-
-    def __init__(self, shx, spline: list) -> None:
-        super(DISP, self).__init__(shx, spline)
-        self.element, self.parameter = self._parse_line(spline)
-
-
-class Restraints():
-    """
-    Base class for the list of restraints.
-    :type _restraints: List[Restraint]
-    """
-
-    def __init__(self):
-        """
-        """
-        self._restraints = []
-
-    def append(self, restr):
-        self._restraints.append(restr)
-
-    def __iter__(self):
-        for x in self._restraints:
-            yield x
-
-    def __getitem__(self, item):
-        return self._restraints[item]
-
-    def __repr__(self):
-        if self._restraints:
-            return "\n".join([str(x) for x in self._restraints])
-        else:
-            return 'No Restraints in file.'
-
-    @staticmethod
-    def _resolve_atoms(shx, restr: Restraint):
-        atoms = restr.atoms
-        for atnum, ap in enumerate(atoms):
-            if not isinstance(ap, (list, tuple)):
-                # ignores all ranges: ['O1', '>', 'F9']
-                try:
-                    atoms[atnum] = shx.atoms.get_atom_by_name(ap)
-                except TypeError:
-                    continue
-                continue
-            for num, atname in enumerate(ap):
-                # without range: [['O1', 'C1'], ...]
-                try:
-                    atoms[atnum][num] = shx.atoms.get_atom_by_name(atname)
-                except TypeError:
-                    continue
-
-
-class DEFS(Restraint):
-
-    def __init__(self, shx, spline: list):
-        """
-        DEFS sd[0.02] sf[0.1] su[0.01] ss[0.04] maxsof[1]
-        Changes the *default* effective standard deviations for the following
-        DFIX, SAME, SADI, CHIV, FLAT, DELU and SIMU restraints.
-        """
-        super(DEFS, self).__init__(shx, spline)
-        self.sf = 0.1
-        self.su = 0.01
-        self.ss = 0.04
-        self.maxsof = 1
-        self.sd = 0.02
-        self.active = True
-        p, _ = self._parse_line(spline)
-        if _:
-            raise ParseParamError
-        if len(p) > 0:
-            self.sd = p[0]
-        if len(p) > 1:
-            self.sf = p[1]
-        if len(p) > 2:
-            self.su = p[2]
-        if len(p) > 3:
-            self.ss = p[3]
-        if len(p) > 4:
-            self.maxsof = p[4]
-
-    @property
-    def all(self):
-        return self.sd, self.sf, self.su, self.ss, self.maxsof
-
-
-class NCSY(Restraint):
-    """
-    NCSY DN sd[0.1] su[0.05] atoms
-    """
-
-    def __init__(self, shx, spline: list):
-        super(NCSY, self).__init__(shx, spline)
-        self.sd = 0.1
-        self.su = 0.05
-        self.DN = None
-        p, self.atoms = self._parse_line(spline, pairs=False)
-        if len(p) > 0:
-            self.DN = p[0]
-        if len(p) > 1:
-            self.sd = p[1]
-        if len(p) > 2:
-            self.su = p[2]
-        if not self.DN:
-            raise ParseNumError
-
-
-class ISOR(Restraint):
-
-    def __init__(self, shx, spline: list):
-        """
-        ISOR s[0.1] st[0.2] atomnames
-        """
-        super(ISOR, self).__init__(shx, spline)
-        self.s = 0.1
-        self.st = 0.2
-        p, self.atoms = self._parse_line(spline, pairs=False)
-        if len(p) > 0:
-            self.s = p[0]
-        if len(p) > 1:
-            self.st = p[1]
-
-
-class FLAT(Restraint):
-    """
-    FLAT s[0.1] four or more atoms
-    """
-
-    def __init__(self, shx, spline: list):
-        super(FLAT, self).__init__(shx, spline)
-        self.s = 0.1
-        p, self.atoms = self._parse_line(spline, pairs=False)
-        if len(p) > 0:
-            self.s = p[0]
-        # TODO: Have to resolve ranges first:
-        # if len(self.atoms) < 4:
-        #    raise ParseParamError
-
-
-class BUMP(Restraint):
-
-    def __init__(self, shx, spline):
-        """
-        BUMP s [0.02]
-        """
-        super(BUMP, self).__init__(shx, spline)
-        self.s = 0.02
-        p, _ = self._parse_line(spline, pairs=False)
-        if len(p) > 0:
-            self.s = p[0]
-        if _:
-            raise ParseParamError
-
-
-class DFIX(Restraint):
-
-    def __init__(self, shx, spline):
-        """
-        DFIX d s[0.02] atom pairs
-        """
-        super(DFIX, self).__init__(shx, spline)
-        self.s = 0.02
-        p, self.atoms = self._parse_line(spline, pairs=True)
-        if len(p) > 0:
-            self.d = p[0]
-        if len(p) > 1:
-            self.s = p[1]
-        self._paircheck()
-        if not self.d:
-            raise ParseNumError
-        if DEBUG and 0.0001 < self.d <= self.s:
-            print('*** WRONG ODER of INSTRUCTIONS. d is smaller than s ***')
-            print("{}".format(self.textline))
-
-
-class DANG(Restraint):
-
-    def __init__(self, shx, spline):
-        """
-        DANG d s[0.04] atom pairs
-        """
-        super(DANG, self).__init__(shx, spline)
-        self.s = 0.04
-        p, self.atoms = self._parse_line(spline, pairs=True)
-        if len(p) > 0:
-            self.d = p[0]
-        if len(p) > 1:
-            self.s = p[1]
-        self._paircheck()
-        if not self.d:
-            raise ParseNumError
-        if 0.0001 < self.d <= self.s:  # Raise exception if d is smaller than s
-            raise ParseOrderError
-
-
-class SADI(Restraint):
-
-    def __init__(self, shx, spline):
-        """
-        SADI s[0.02] pairs of atoms
-        Instructions with only two atoms are ignored by SHELXL: SADI C3 C4
-        SADI_3 C3 C4 C3_4 C4_4 creates SADI C3_3 C4_3  C3_4 C4_4
-        SADI_CCF3 C3 C4 C3_4 C4_4 creates SADI C3_1 C4_1  C3_2 C4_2  C3_4 C4_4 if there are residues 1, 2 and 4
-        """
-        super(SADI, self).__init__(shx, spline)
-        self.s = 0.02
-        p, self.atoms = self._parse_line(spline, pairs=True)
-        if len(p) > 0:
-            self.s = p[0]
-        self._paircheck()
-
-
-class SAME(Restraint):
-
-    def __init__(self, shx, spline):
-        """
-        SAME s1[0.02] s2[0.04] atomnames
-        """
-        super(SAME, self).__init__(shx, spline)
-        self.s1 = 0.02
-        self.s2 = 0.04
-        p, self.atoms = self._parse_line(spline, pairs=False)
-        if len(p) > 0:
-            self.s1 = p[0]
-        if len(p) > 1:
-            self.s2 = p[1]
-
-
-class RIGU(Restraint):
-
-    def __init__(self, shx, spline: list):
-        """
-        RIGU s1[0.004] s2[0.004] atomnames
-        """
-        super(RIGU, self).__init__(shx, spline)
-        self.s1 = 0.004
-        self.s2 = 0.004
-        p, self.atoms = self._parse_line(spline, pairs=False)
-        if len(p) > 0:
-            self.s1 = p[0]
-        if len(p) > 1:
-            self.s2 = p[1]
-
-
-class SIMU(Restraint):
-
-    def __init__(self, shx, spline: list):
-        """
-        SIMU s[0.04] st[0.08] dmax[2.0] atomnames
-        """
-        super(SIMU, self).__init__(shx, spline)
-        self.s = 0.04
-        self.st = 0.08
-        self.dmax = 2.0
-        p, self.atoms = self._parse_line(spline, pairs=False)
-        if len(p) > 0:
-            self.s = p[0]
-        if len(p) > 1:
-            self.st = p[1]
-        if len(p) > 2:
-            self.dmax = p[2]
-
-
-class DELU(Restraint):
-
-    def __init__(self, shx, spline: list):
-        """
-        DELU s1[0.01] s2[0.01] atomnames
-        """
-        super(DELU, self).__init__(shx, spline)
-        self.s1 = 0.01
-        self.s2 = 0.01
-        p, self.atoms = self._parse_line(spline, pairs=False)
-        if len(p) > 0:
-            self.s1 = p[0]
-        if len(p) > 1:
-            self.s2 = p[1]
-
-
-class CHIV(Restraint):
-
-    def __init__(self, shx, spline: list):
-        """
-        CHIV V[0] s[0.1] atomnames
-        """
-        super(CHIV, self).__init__(shx, spline)
-        self.s = 0.1
-        self.V = 0.0
-        p, self.atoms = self._parse_line(spline, pairs=False)
-        if len(p) > 0:
-            self.V = p[0]
-        if len(p) > 1:
-            self.s = p[1]
-
-
-class EADP(Restraint):
-    """
-    EADP atomnames
-    """
-
-    def __init__(self, shx, spline: list) -> None:
-        super(EADP, self).__init__(shx, spline)
-        _, self.atoms = self._parse_line(spline, pairs=False)
-
-
-class EXYZ(Restraint):
-    """
-    EADP atomnames
-    """
-
-    def __init__(self, shx, spline: list) -> None:
-        super(EXYZ, self).__init__(shx, spline)
-        _, self.atoms = self._parse_line(spline, pairs=False)
-
-
-class DAMP(Command):
-    """
-    DAMP damp[0.7] limse[15]
-    """
-
-    def __init__(self, shx, spline: list):
-        super(DAMP, self).__init__(shx, spline)
-        values, _ = self._parse_line(spline, intnums=False)
-        self.damp, self.limse = 0, 0
-        if len(values) > 0:
-            self.damp = values[0]
-        if len(values) > 1:
-            self.damp, self.limse = values
-
-    def __repr__(self) -> str:
-        if self.limse == 0:
-            return "DAMP  {:,g}".format(self.damp)
-        else:
-            return "DAMP  {:,g} {:,g}".format(self.damp, self.limse)
-
-
-class HFIX(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        HFIX mn U[#] d[#] atomnames
-        """
-        super(HFIX, self).__init__(shx, spline)
-        self.params, self.atoms = self._parse_line(spline, intnums=True)
-
-    def __repr__(self):
-        return "HFIX {} {}".format(" ".join([str(x) for x in self.params]) if self.params else '',
-                                   " ".join(self.atoms) if self.atoms else '')
-
-
-class HKLF(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        HKLF N[0] S[1] r11...r33[1 0 0 0 1 0 0 0 1] sm[1] m[0]
-        """
-        super(HKLF, self).__init__(shx, spline)
-        p, _ = self._parse_line(spline)
-        self.n = 0
-        self.s = 1
-        self.matrix = [1, 0, 0, 0, 1, 0, 0, 0, 1]
-        self.sm = 1
-        self.m = 0
-        if len(p) > 0:
-            self.n = int(p[0])
-        if len(p) > 1:
-            self.s = p[1]
-        if len(p) > 10:
-            self.matrix = p[3:11]
-        if len(p) > 11:
-            self.sm = p[12]
-        if len(p) > 12:
-            self.m = p[13]
-
-    def __repr__(self):
-        return "HKLF {:,g} {:,g}  {}  {:,g} {:,g}".format(self.n, self.s, ' '.join([str(i) for i in self.matrix]),
-                                                          self.sm, self.m)
-
-
-class SUMP(Command):
-    """
-    SUMP for linear equation eypressions with free variables.
-    SUMP c sigma c1 m1 c2 m2 ...
-    """
-
-    def __init__(self, shx, spline: list):
-        super(SUMP, self).__init__(shx, spline)
-        p, _ = self._parse_line(spline)
-        self.c = p.pop(0)
-        self.fvars = {}
-        self.sigma = p.pop(0)
-        # this is to have integer free variables
-        fvars = [int(x) for x in p[1::2]]
-        times = [x for x in p[0::2]]
-        self.fvars = [[x, y] for x, y in zip(times, fvars)]
-
-    def __getitem__(self, item):
-        return self.fvars[item]
-
-
-class LATT(Command):
-    lattdict = {1: [],  # Primitive
-                2: [SymmetryElement(['0.5', '0.5', '0.5'])],  # I-centered
-                3: [SymmetryElement(['1/3', '2/3', '2/3']),  # Rhombohedral
-                    SymmetryElement(['2/3', '1/3', '1/3'])],
-                4: [SymmetryElement(['0.0', '0.5', '0.5']),  # F-centered
-                    SymmetryElement(['0.5', '0.0', '0.5']),
-                    SymmetryElement(['0.5', '0.5', '0.0'])],
-                5: [SymmetryElement(['0.0', '0.5', '0.5'])],  # A-centered
-                6: [SymmetryElement(['0.5', '0.0', '0.5'])],  # B-centered
-                7: [SymmetryElement(['0.5', '0.5', '0.0'])]}  # C-centered
-
-    lattint_to_str = {1: 'P', 2: 'I', 3: 'R', 4: 'F', 5: 'A', 6: 'B', 7: 'C'}
-
-    def __init__(self, shx, spline: list):
-        """
-        LATT N[1]
-        """
-        super(LATT, self).__init__(shx, spline)
-        p, _ = self._parse_line(spline)
-        self.centric = False
-        try:
-            self.N = int(p[0])
-        except ValueError:
-            self.N = -1
-        self.N_str = self.lattint_to_str[abs(self.N)]
-        if self.N > 0:  # centrosymmetric space group:
-            self.centric = True
-        self.latt_ops = LATT.lattdict[abs(self.N)]
-
-
-class SYMM(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        SYMM symmetry operation
-        """
-        super(SYMM, self).__init__(shx, spline)
-        self.symmcard = self._parse_line(spline)
-
-    def _parse_line(self, spline: list, intnums: bool = False) -> list:
-        symmcard = ''.join(spline[1:]).split(',')  # removes whitespace
-        return symmcard
-
-    def _as_str(self):
-        return "SYMM  " + ", ".join(self.symmcard)
-
-    def __repr__(self):
-        return self._as_str()
-
-    def __str__(self) -> str:
-        return self._as_str()
-
-
-class SymmCards():
-    """
-    Contains the list of SYMM cards
-    """
-
-    def __init__(self, shx):
-        self.shx = shx
-        self._symmcards = [SymmetryElement(['X', 'Y', 'Z'])]
-        self.latt_ops = []
-
-    def _as_str(self) -> str:
-        return "\n".join([str(x) for x in self._symmcards])
-
-    def __repr__(self) -> str:
-        return self._as_str()
-
-    def __str__(self) -> str:
-        return self._as_str()
-
-    def __getitem__(self, item):
-        return self._symmcards[item]
-
-    def __iter__(self):
-        for x in self._symmcards:
-            yield x
-
-    def append(self, symm_data: list) -> None:
-        """
-        Add the content of a Shelxl SYMM command to generate the appropriate SymmetryElement instance.
-        :param symm_data: list of strings. eg.['1/2+X', '1/2+Y', '1/2+Z']
-        :return: None
-        """
-        new_symm = SymmetryElement(symm_data)
-        self._symmcards.append(new_symm)
-        for symm in self.shx.latt.latt_ops:
-            latt_symm = new_symm.apply_latt_symm(symm)
-            if latt_symm not in self._symmcards:
-                self._symmcards.append(latt_symm)
-        if self.shx.latt.centric:
-            self._symmcards.append(SymmetryElement(symm_data, centric=True))
-            for symm in self.shx.latt.latt_ops:
-                latt_symm = new_symm.apply_latt_symm(symm)
-                latt_symm.centric = True
-                self._symmcards.append(latt_symm)
-
-    def set_centric(self, value: bool):
-        """
-        Defines the instance as representing a centrosymmetric structure. Generates the appropriate SymmetryElement
-        instances automatically if called before adding further SYMM commands via self.addSymm().
-        """
-        self.shx.latt.centric = value
-        self._symmcards.append(SymmetryElement(['-X', '-Y', '-Z']))
-        self._symmcards[-1].centric = True
-
-    def set_latt_ops(self, lattops: list) -> None:
-        """
-        Adds lattice operations. If called before adding SYMM commands, the appropriate lattice operations are used
-        automatically to generate further SymmetryElements.
-        :param lattops: list of SymmetryElement instances.
-        """
-        self.latt_ops = lattops
-
-
-class LSCycles(Command):
-    def __init__(self, shx, spline: list):
-        """
-        L.S. nls[0] nrf[0] nextra[0]
-        #TODO: support nls parameter
-        If nrf is positive, it is the number of these cycles that should be performed before applying ANIS.
-        Negative nrf indicates which reflections should be ignored during the refinement but used instead for
-        the calculation of free R-factors in the final structure factor summation.
-        nextra is the number of additional parameters that were derived from the data when 'squeezing' the
-        structure etc.
-        """
-        super(LSCycles, self).__init__(shx, spline)
-        p, _ = self._parse_line(spline)
-        self._shx = shx
-        self.cgls = False
-        self._cycles = 0
-        self._nrf = ''
-        self._nextra = ''
-        try:
-            self._cycles = int(p[0])
-        except (IndexError, NameError, ValueError):
-            raise ParseNumError
-        try:
-            self._nrf = int(p[1])
-        except IndexError:
-            pass
-        try:
-            self._nextra = int(p[2])
-        except IndexError:
-            pass
-        if spline[0].upper() == 'CGLS':
-            self.cgls = True
-
-    @property
-    def number(self):
-        return self._cycles
-
-    @number.setter
-    def number(self, n: int) -> None:
-        self._cycles = int(n)
-        self.__init__(self._shx, self._as_str().split())
-
-    def set_refine_cycles(self, number: int) -> None:
-        """
-        Sets the number of refinement cycles for the current res file.
-        """
-        self.number = int(number)
-
-    @property
-    def text(self) -> str:
-        """
-        'CGLS 10 2 '
-        """
-        return self.__repr__()
-
-    def __iter__(self):
-        for x in self.__repr__().split():
-            yield x
-
-    def _as_str(self):
-        return '{} {} {} {}'.format('CGLS' if self.cgls else 'L.S.', self._cycles,
-                                    self._nrf if self._nrf else '', self._nextra if self._nextra else '').strip()
-
-    def __repr__(self):
-        return self._as_str()
-
-
-class SFACTable():
-    def __init__(self, shx):
-        """
-        Holds the information of SFAC instructions. Either with default values and only elements
-        SFAC elements
-        or as explicit scattering factor in the form of an exponential series, followed by real and
-        imaginary dispersion terms, linear absorption coefficient, covalent radius and atomic weight.
-
-        SFAC elements  or  SFAC E a1 b1 a2 b2 a3 b3 a4 b4 c f' f" mu r wt
-        """
-        self.sfac_table = []
-        self.shx = shx
-        self.elements_list = []
-
-    def __iter__(self):
-        for x in self.sfac_table:
-            yield x['element'].capitalize()
-
-    def __repr__(self):
-        sftext = ''
-        elements = []
-        for sf in self.sfac_table:
-            if not self.is_exp(sf) and sf['element'].capitalize() not in elements:
-                elements.append(sf['element'].capitalize())
-            else:
-                if elements:
-                    sftext = self._extend_sfac_text(elements, sftext)
-                    elements = []
-                values = []
-                for x in ('element', 'a1', 'b1', 'a2', 'b2', 'a3', 'b3', 'a4', 'b4', 'c',
-                          'fprime', 'fdprime', 'mu', 'r', 'wt'):
-                    values.append(sf[x])
-                sftext += "\nSFAC " + "  ".join(values)
-        if elements:
-            sftext = self._extend_sfac_text(elements, sftext)
-        return sftext[1:]
-
-    def _extend_sfac_text(self, elements: List[str], sftext: str) -> str:
-        sftext += "\nSFAC " + "  ".join(elements)
-        return sftext
-
-    def __getitem__(self, index: int):
-        """
-        Returns the n-th element in the sfac table, beginning with 1.
-        """
-        if index == 0:
-            raise IndexError
-        if index < 0:
-            index = len(self.sfac_table) + index + 1
-        return self.sfac_table[index - 1]['element'].capitalize()
-
-    def parse_element_line(self, spline: list):
-        """
-        Adds a new SFAC card to the list of cards.
-        """
-        if not ''.join(spline[1:]).isalpha():  # joining, because space is not alphabetical
-            # Excplicit with all values
-            sfdic = {}
-            for n, x in enumerate(['element', 'a1', 'b1', 'a2', 'b2', 'a3', 'b3', 'a4', 'b4', 'c',
-                                   'fprime', 'fdprime', 'mu', 'r', 'wt']):
-                if n == 0:
-                    self.elements_list.append(spline[n + 1].upper())
-                try:
-                    sfdic[x] = spline[n + 1]
-                except IndexError:
-                    raise ParseNumError()
-            self.sfac_table.append(sfdic)
-        else:
-            # Just the elements
-            for x in spline[1:]:
-                self.elements_list.append(x.upper())
-                self.sfac_table.append({'element': x.upper()})
-
-    def has_element(self, element):
-        return element.upper() in self.elements_list
-
-    @staticmethod
-    def is_exp(item):
-        return 'a1' in item
-
-    def add_element(self, element: str):
-        """
-        Adds an element to the SFAC list.
-        """
-        if self.has_element(element):
-            return
-        self.elements_list.append(element.upper())
-        self.sfac_table.append({'element': element.upper(), 'line_number': None})
-        self.shx.unit.add_number(1.0)
-
-    def remove_element(self, element: str):
-        del self.sfac_table[self.shx.elem2sfac(element.upper()) - 1]
-        del self.elements_list[self.elements_list.index(element.upper())]
-
-
-class UNIT(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        UNIT n1 n2 ...
-        """
-        super(UNIT, self).__init__(shx, spline)
-        self.values, _ = self._parse_line(spline)
-
-    def add_number(self, number: float):
-        self.values.append(number)
-
-    def __iter__(self):
-        yield [x for x in self.values]
-
-    def __repr__(self):
-        return "UNIT " + "  ".join(["{:,g}".format(x) for x in self.values])
-
-    def __str__(self):
-        return self.__repr__()
-
-    def __setitem__(self, key, value):
-        self.values[key] = value
-
-    def __getitem__(self, item):
-        return self.values[item]
-
-    def __add__(self, other):
-        self.values.append(other)
-
-
-class BASF(Command):
-    """
-    BASF scale factors
-    BASF can occour in multiple lines.
-    """
-
-    def __init__(self, shx, spline):
-        super(BASF, self).__init__(shx, spline)
-        self.scale_factors, _ = self._parse_line(spline)
-
-    def __iter__(self):
-        yield self.scale_factors
-
-
-class TWIN(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        TWIN 3x3 matrix [-1 0 0 0 -1 0 0 0 -1] N[2]
-        +N     -N  m = |N|
-        m-1 to 2m-1
-        m-1   (2*abs(m)/2)-1
-        """
-        super(TWIN, self).__init__(shx, spline)
-        self.matrix = [-1, 0, 0, 0, -1, 0, 0, 0, -1]
-        self.allowed_N = 2
-        self.n_value = 2
-        if len(spline) > 1:
-            p, _ = self._parse_line(spline, intnums=False)
-            if len(p) == 9:
-                self.matrix = p
-            elif len(p) == 10:
-                self.matrix = p[:9]
-                self.n_value = int(p[9])
-            else:
-                raise ParseNumError("*** Check TWIN instruction. ***")
-        m = abs(self.n_value) / 2
-        if self.n_value > 0:
-            self.allowed_N = abs(self.n_value) - 1
-        else:
-            self.allowed_N = (2 * m) - 1
-
-
-class WGHT(Command):
-
-    def __init__(self, shx, spline: list):
-        """
-        The weighting scheme is defined as follows:
-        w = q / [ σ²(Fo²) + (a*P)² + b*P + d + e*sin(θ)/$lambda; ]
-
-        WGHT a[0.1] b[0] c[0] d[0] e[0] f[.33333]
-        Usually only WGHT a b
-        """
-        super(WGHT, self).__init__(shx, spline)
-        self.shx = shx
-        self.a = 0.1
-        self.b = 0.0
-        self.c = 0.0
-        self.d = 0.0
-        self.e = 0.0
-        self.f = 0.33333
-        p, _ = self._parse_line(spline)
-        if len(p) > 0:
-            self.a = p[0]
-        if len(p) > 1:
-            self.b = p[1]
-        if len(p) > 2:
-            self.c = p[2]
-        if len(p) > 3:
-            self.d = p[3]
-        if len(p) > 4:
-            self.e = p[4]
-        if len(p) > 5:
-            self.f = p[5]
-
-    def _as_string(self):
-        wght = 'WGHT   {} {}'.format(self.a, self.b)
-        # It is very unlikely that someone changes other parameter than a and b:
-        if (self.c + self.d + self.e + self.f) != 0.33333:
-            wght += ' {} {} {} {}'.format(self.c, self.d, self.e, self.f)
-        return wght
-
-    def difference(self) -> List[float]:
-        """
-        Returns a list with the weight differences of the parameters a and b.
-        """
-        try:
-            adiff = abs(self.shx.wght.a - self.shx.wght_suggested.a)
-            bdiff = abs(self.shx.wght.b - self.shx.wght_suggested.b)
-        except AttributeError:
-            print("No suggested weighting scheme found. Unable to proceed.")
-            return [0.0, 0.0]
-        return [round(adiff, 3), round(bdiff, 3)]
-
-    def __repr__(self):
-        return self._as_string()
-
-    def __str__(self):
-        return self._as_string()
+import re
+from math import cos, radians, sqrt
+from typing import List, Union
+
+from shelxfile.misc.dsrmath import my_isnumeric, SymmetryElement
+from shelxfile.misc.misc import chunks, ParseParamError, ParseNumError, \
+    ParseOrderError, DEBUG, ParseSyntaxError
+
+"""
+SHELXL cards:
+
+ABIN n1 n2
+ACTA 2θfull[#]
+AFIX mn d[#] sof[11] U[10.08]
+ANIS n
+ANIS names
+ANSC six coefficients
+ANSR anres[0.001]
+BASF scale factors
+BIND atom1 atom2
+BIND m n
+BLOC n1 n2 atomnames
+BOND atomnames
+BUMP s [0.02]
+CELL λ a b c α β γ
+CGLS nls[0] nrf[0] nextra[0]
+CHIV V[0] s[0.1] atomnames
+CONF atomnames max_d[1.9] max_a[170]
+CONN bmax[12] r[#] atomnames or CONN bmax[12]
+DAMP damp[0.7] limse[15]
+DANG d s[0.04] atom pairs
+DEFS sd[0.02] sf[0.1] su[0.01] ss[0.04] maxsof[1]
+DELU s1[0.01] s2[0.01] atomnames
+DFIX d s[0.02] atom pairs
+DISP E f' f"[#] mu[#]
+EADP atomnames
+END
+EQIV $n symmetry operation
+EXTI x[0]
+EXYZ atomnames
+FEND
+FLAT s[0.1] four or more atoms
+FMAP code[2] axis[#] nl[53]
+FRAG code[17] a[1] b[1] c[1] α[90] β[90] γ[90]
+FREE atom1 atom2
+FVAR osf[1] free variables
+GRID sl[#] sa[#] sd[#] dl[#] da[#] dd[#]
+HFIX mn U[#] d[#] atomnames
+HKLF N[0] S[1] r11...r33[1 0 0 0 1 0 0 0 1] sm[1] m[0]
+HTAB dh[2.0]
+HTAB donor-atom acceptor-atom
+ISOR s[0.1] st[0.2] atomnames
+LATT N[1]
+LAUE E
+LIST m[#] mult[1]
+L.S. nls[0] nrf[0] nextra[0]
+MERG n[2]
+MORE m[1]
+MOVE dx[0] dy[0] dz[0] sign[1]
+MPLA na atomnames
+NCSY DN sd[0.1] su[0.05] atoms
+NEUT
+OMIT atomnames
+OMIT s[-2] 2θ(lim)[180]
+OMIT h k l
+PART n sof
+PLAN npeaks[20] d1[#] d2[#]
+PRIG p[#]
+REM
+RESI class[ ] number[0] alias
+RIGU s1[0.004] s2[0.004] atomnames
+RTAB codename atomnames
+SADI s[0.02] pairs of atoms
+SAME s1[0.02] s2[0.04] atomnames
+SFAC elements
+SFAC E a1 b1 a2 b2 a3 b3 a4 b4 c f' f" mu r wt
+SHEL lowres[infinite] highres[0]
+SIMU s[0.04] st[0.08] dmax[2.0] atomnames
+SIZE dx dy dz
+SPEC del[0.2]
+STIR sres step[0.01]
+SUMP c sigma c1 m1 c2 m2 ...
+SWAT g[0] U[2]
+SYMM symmetry operation
+TEMP T[20]
+TITL [ ]
+TWIN 3x3 matrix [-1 0 0 0 -1 0 0 0 -1] N[2]
+TWST N[0]
+UNIT n1 n2 ...
+WGHT a[0.1] b[0] c[0] d[0] e[0] f[.33333]
+WIGL del[0.2] dU[0.2]
+WPDB n[1]
+XNPD Umin[-0.001]
+ZERR Z esd(a) esd(b) esd(c) esd(α) esd(β) esd(γ)
+"""
+
+
+class Residue():
+    def __init__(self):
+        self.shx = None
+        self._spline = None
+
+    @property
+    def residue_number(self):
+        if '_' in self._spline[0]:
+            _, suffix = self._spline[0].upper().split('_')
+            if any([x.isalpha() for x in suffix]):
+                self.residue_class = suffix
+            else:
+                # TODO: implement _+, _- and _*
+                if '*' in suffix:
+                    return list(self.shx.residues.residue_numbers.keys())
+                else:
+                    return [int(suffix)]
+        return [0]
+
+
+class Restraint(Residue):
+
+    def __init__(self, shx, spline: list):
+        """
+        Base class for parsing restraints.
+        TODO: resolve ranges like SADI_CCF3 O1 > F9
+        """
+        super().__init__()
+        self.shx = shx
+        self.residue_class = ''  # '' is the default class (with residue number 0)
+        self.textline = ' '.join(spline)
+        self.name = None
+        self.atoms = []
+
+    @property
+    def index(self):
+        return self.shx.index_of(self)
+
+    def _parse_line(self, spline, pairs=False):
+        """
+        Residues may be referenced by any instruction that allows atom names; the reference takes
+        the form of the character '_' followed by either the residue class or number without intervening
+        spaces.
+        Individual atom names in an instruction may be followed by '_' and a residue number, but not by '_* ' or '_'
+        and a residue class. If an atom name is not followed by a residue number, the current residue is
+        assumed (unless overridden by a global residue number or class appended to the instruction
+        codeword).
+        """
+        self._spline = spline
+        # TODO: check if suffix is a residue class and set instance variable accordingly
+        if '_' in spline[0]:
+            self.name, suffix = spline[0].upper().split('_')
+        else:
+            self.name = spline[0].upper()
+        self.set_defs_values()
+        self.check_if_class_name_fits_to_command()
+        params = []
+        atoms = []
+        for x in spline[1:]:
+            if my_isnumeric(x):
+                params.append(float(x))
+            else:
+                atoms.append(x)
+        if pairs:
+            return params, chunks(atoms, 2)
+        else:
+            return params, atoms
+
+    def check_if_class_name_fits_to_command(self):
+        if DEBUG and self.__class__.__name__ != self.name:
+            print('*** Trying to parse restraint with wrong class ***')
+            raise ParseSyntaxError
+
+    def set_defs_values(self):
+        # Beware! DEFS changes only the non-defined default values:
+        # DEFS sd[0.02] sf[0.1] su[0.01] ss[0.04] maxsof[1]
+        if self.shx.defs:  # and self.shx.defs.active:
+            if self.name == 'DFIX':
+                self.s = self.shx.defs.sd
+            if self.name == 'SAME':
+                self.s1 = self.shx.defs.sd
+                self.s2 = self.shx.defs.sd * 2
+            if self.name == 'SADI':
+                self.s = self.shx.defs.sd
+            if self.name == 'CHIV':
+                self.s = self.shx.defs.sf
+            if self.name == 'FLAT':
+                self.s = self.shx.defs.sf
+            if self.name == 'DELU':
+                self.s1 = self.shx.defs.su
+                self.s2 = self.shx.defs.su
+            if self.name == 'SIMU':
+                self.s = self.shx.defs.ss
+                self.st = self.shx.defs.ss * 2
+
+    def _paircheck(self):
+        if not self.atoms:
+            return
+        if len(self.atoms[-1]) != 2 and DEBUG:
+            print('*** Wrong number of numerical parameters ***')
+            print('Instruction: {}'.format(self.textline))
+            raise ParseNumError
+
+    def __iter__(self):
+        for x in self.textline.split():
+            yield x
+
+    def __repr__(self):
+        return self.textline
+
+    def __str__(self):
+        return self.textline
+
+    def split(self):
+        return self.textline.split()
+
+
+class Command():
+    """
+    A class to parse all general commands except restraints.
+    """
+
+    def __init__(self, shx, spline: list):
+        self._shx = shx
+        self._spline = spline
+        self.residue_class = ''
+        self._textline = ' '.join(spline)
+
+    def _parse_line(self, spline, intnums=False):
+        """
+        :param spline: Splitted shelxl line
+        :param intnums: if numerical parameters should be integer
+        :return: numerical parameters and words
+        """
+        if '_' in spline[0]:
+            self._card_name, suffix = spline[0].upper().split('_')
+        else:
+            self._card_name = spline[0].upper()
+        numparams = []
+        words = []
+        for x in spline[1:]:  # all values after SHELX card
+            if str.isdigit(x[0]) or x[0] in '+-':
+                if intnums:
+                    numparams.append(int(x))
+                else:
+                    numparams.append(float(x))
+            else:
+                words.append(x)
+        return numparams, words
+
+    def set(self, value):
+        self.__init__(self._shx, value.split())
+
+    @property
+    def index(self):
+        return self._shx.index_of(self)
+
+    @property
+    def position(self) -> int:
+        return self.index
+
+    def __iter__(self):
+        for x in self.__repr__().split():
+            yield x
+
+    def split(self):
+        return self._textline.split()
+
+    def __str__(self):
+        return self._textline
+
+    def __repr__(self):
+        return self._textline
+
+
+class ABIN(Command):
+
+    def __init__(self, shx, spline):
+        """
+        ABIN n1 n2
+        """
+        super(ABIN, self).__init__(shx, spline)
+        p, _ = self._parse_line(spline)
+        if len(p) > 0:
+            self.n1 = p[0]
+        if len(p) > 1:
+            self.n2 = p[1]
+
+
+class ANIS(Command):
+
+    def __init__(self, shx, spline: List):
+        """
+        ANIS n
+        ANIS names
+        """
+        super(ANIS, self).__init__(shx, spline)
+        p, self.atoms = self._parse_line(spline)
+        self.over_all = True
+        if len(p) > 0:
+            self.over_all = False
+            self.n = p[0]
+        if len(self.atoms) > 0:
+            self.over_all = False
+
+    def __bool__(self):
+        return True
+
+
+class MPLA(Command):
+
+    def __init__(self, shx, spline: List):
+        """
+        MPLA na atomnames
+        """
+        super(MPLA, self).__init__(shx, spline)
+        p, self.atoms = self._parse_line(spline, intnums=True)
+        if len(p) > 0:
+            self.na = p[0]
+
+
+class MORE(Command):
+
+    def __init__(self, shx, spline: List):
+        """
+        MORE m[1]
+        """
+        super(MORE, self).__init__(shx, spline)
+        self.m = 1
+        p, _ = self._parse_line(spline, intnums=True)
+        self.m = p[0]
+
+
+class CELL(Command):
+
+    def __init__(self, shx, spline: List):
+        """
+        CELL λ a b c α β γ
+        """
+        super(CELL, self).__init__(shx, spline)
+        p, _ = self._parse_line(spline)
+        self._cell_list = []
+        if len(p) > 0:
+            self.wavelen = float(p[0])
+        if len(p) > 6:
+            self._cell_list = p[1:]
+            self.a = p[1]
+            self.b = p[2]
+            self.c = p[3]
+            self.alpha = p[4]
+            self.beta = p[5]
+            self.gamma = p[6]
+            self.cosal = cos(radians(self.alpha))
+            self.cosbe = cos(radians(self.beta))
+            self.cosga = cos(radians(self.gamma))
+        else:
+            raise ParseSyntaxError
+
+    @property
+    def volume(self) -> float:
+        """
+        calculates the volume of a unit cell
+        """
+        try:
+            ca, cb, cg = cos(radians(self.alpha)), cos(radians(self.beta)), cos(radians(self.gamma))
+            v = self.a * self.b * self.c * sqrt(1 + 2 * ca * cb * cg - ca ** 2 - cb ** 2 - cg ** 2)
+        except AttributeError:
+            # No valid celll
+            v = 0.0
+        return v
+
+    @property
+    def V(self) -> float:
+        return self.volume
+
+    def __iter__(self):
+        return iter(self._cell_list)
+
+    def __getitem__(self, item):
+        return self._cell_list[item]
+
+
+class ZERR(Command):
+
+    def __init__(self, shx, spline: List):
+        """
+        ZERR Z esd(a) esd(b) esd(c) esd(α) esd(β) esd(γ)
+        """
+        super(ZERR, self).__init__(shx, spline)
+        p, _ = self._parse_line(spline)
+        self.Z = 1
+        if len(p) > 0:
+            self.Z = p[0]
+        if len(p) > 6:
+            self.esd_list = p[1:]
+            self.esd_a = p[0]
+            self.esd_b = p[1]
+            self.esd_c = p[2]
+            self.esd_al = p[3]
+            self.esd_be = p[4]
+            self.esd_ga = p[5]
+
+
+class AFIX(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        AFIX mn d[#] sof[11] U[10.08]
+        """
+        super(AFIX, self).__init__(shx, spline)
+        p, _ = self._parse_line(spline)
+        self.U = 10.08
+        self.sof = 11.0
+        self.mn = None
+        self.d = None
+        if len(p) > 0:
+            self.mn = int(p[0])
+        if len(p) > 1:
+            self.d = p[1]
+        if len(p) > 2:
+            self.sof = p[2]
+        if len(p) > 3:
+            self.U = p[3]
+
+    def __bool__(self):
+        if self.mn and self.mn > 0:
+            return True
+        else:
+            return False
+
+
+class Residues():
+
+    def __init__(self, shx):
+        self.shx = shx
+        self.all_residues = []
+        self.residue_classes = {}  # class: numbers
+        # self.residue_numbers = {}  # number: class
+
+    def append(self, resi: 'RESI') -> None:
+        """
+        Adds a new residues to the list of residues.
+        """
+        self.all_residues.append(resi)
+        # Collect dict with class: numbers
+        if resi.residue_class in self.residue_classes:
+            self.residue_classes[resi.residue_class].append(resi.residue_number)
+        else:
+            self.residue_classes[resi.residue_class] = [resi.residue_number]
+        """
+        # Collect dict with number: classes
+        if resi.residue_number in self.residue_numbers:
+            if DEBUG:
+                print('*** Duplicate residue number {} found! ***'.format(resi.residue_number))
+        else:
+            self.residue_numbers[resi.residue_number] = resi.residue_class
+        """
+
+    @property
+    def residue_numbers(self):
+        return dict((x.residue_number, x.residue_class) for x in self.shx.residues.all_residues)
+
+
+class RESI():
+
+    def __init__(self, shx, spline: list):
+        """
+        RESI class[ ] number[0] alias
+        """
+        self.shx = shx
+        self.residue_class = ''
+        self.residue_number = 0
+        self.alias = None
+        self.chain_id = None
+        self.textline = ' '.join(spline)
+        if len(spline) < 2 and DEBUG:
+            print('*** Wrong RESI definition found! Check your RESI instructions ***')
+            raise ParseParamError
+        self.get_resi_definition(spline)
+        if self.residue_number < -999 or self.residue_number > 9999:
+            print('*** Invalid residue number given. ****')
+            raise ParseSyntaxError
+
+    def get_resi_definition(self, resi: list) -> tuple:
+        """
+        RESI class[ ] number[0] alias
+
+        Returns the residue number and class of a string like 'RESI TOL 1'
+        or 'RESI 1 TOL'
+
+        Residue names may now begin with a digit.
+        They must however contain at least one letter
+
+        Allowed residue numbers is now from -999 to 9999 (2017/1)
+        """
+        alpha = re.compile('[a-zA-Z]')
+        for x in resi:
+            if alpha.search(x):
+                if ':' in x:
+                    # contains ":" thus must be a chain-id+number
+                    self.chain_id, self.residue_number = x.split(':')[0], int(x.split(':')[1])
+                else:
+                    # contains letters, must be a name (class)
+                    self.residue_class = x
+            else:
+                # everything else can only be a number
+                if self.residue_number > 0:
+                    self.alias = int(x)
+                else:
+                    try:
+                        self.residue_number = int(x)
+                    except ValueError:
+                        self.residue_number = 0
+        return self.residue_class, self.residue_number, self.chain_id, self.alias
+
+    def _parse_line(self, spline, intnums=False):
+        """
+        :param spline: Splitted shelxl line
+        :param intnums: if numerical parameters should be integer
+        :return: numerical parameters and words
+        """
+        if '_' in spline[0]:
+            self.card_name, suffix = spline[0].upper().split('_')
+            if any([x.isalpha() for x in suffix]):
+                self.residue_class = suffix
+            else:
+                # TODO: implement _+, _- and _*
+                self.residue_number = int(suffix)
+        else:
+            self.card_name = spline[0].upper()
+        numparams = []
+        words = []
+        for x in spline[1:]:  # all values after SHELX card
+            if str.isdigit(x[0]) or x[0] in '+-':
+                if intnums:
+                    numparams.append(int(x))
+                else:
+                    numparams.append(float(x))
+            else:
+                words.append(x)
+        return numparams, words
+
+    @property
+    def index(self):
+        return self.shx.index_of(self)
+
+    def __iter__(self):
+        for x in self.__repr__().split():
+            yield x
+
+    def split(self):
+        return self.textline.split()
+
+    def __str__(self):
+        return self.textline
+
+    def __repr__(self):
+        return self.textline
+
+    def __bool__(self):
+        if self.residue_number > 0:
+            return True
+        else:
+            return False
+
+
+class PART(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        PART n sof
+        """
+        super(PART, self).__init__(shx, spline)
+        p, _ = self._parse_line(spline)
+        self.sof = 11.0
+        self.n = 0
+        try:
+            self.n = int(p[0])
+        except(ValueError, IndexError):
+            if DEBUG:
+                print('*** Wrong PART definition in line {} found! '
+                      'Check your PART instructions ***'.format(shx.error_line_num))
+                raise
+            self.n = 0
+        if len(p) > 1:
+            self.sof = float(p[1])
+
+    def __bool__(self):
+        if self.n > 0:
+            return True
+        else:
+            return False
+
+
+class XNPD(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        XNPD Umin[-0.001]
+        """
+        super(XNPD, self).__init__(shx, spline)
+        p, _ = self._parse_line(spline)
+        self.Umin = -0.001
+        if len(p) > 0:
+            self.Umin = p[0]
+
+
+class SIZE(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        SIZE dx dy dz
+        """
+        super(SIZE, self).__init__(shx, spline)
+        self.dx, self.dy, self.dz = None, None, None
+        p, _ = self._parse_line(spline)
+        if len(p) > 0:
+            self.dx = p[0]
+        if len(p) > 1:
+            self.dy = p[1]
+        if len(p) > 2:
+            self.dz = p[2]
+
+    def _as_text(self):
+        if all([self.dx, self.dy, self.dz]):
+            return "SIZE {:,g} {:,g} {:,g}".format(self.dx, self.dy, self.dz)
+        else:
+            return ""
+
+    def __repr__(self):
+        return self._as_text()
+
+    def __str__(self):
+        return self._as_text()
+
+
+class SHEL(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        SHEL lowres[infinite] highres[0]
+        """
+        super(SHEL, self).__init__(shx, spline)
+        params, _ = self._parse_line(spline)
+        self.lowres = None
+        self.highres = None
+        if len(params) > 0:
+            self.lowres = params[0]
+        if len(params) > 1:
+            self.highres = params[1]
+
+
+class WIGL(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        WIGL del[0.2] dU[0.2]
+        """
+        super(WIGL, self).__init__(shx, spline)
+        p, _ = self._parse_line(spline)
+        self.d = 0.2
+        self.dU = 0.2
+        if len(p) > 0:
+            self.d = p[0]
+        if len(p) > 1:
+            self.dU = p[1]
+
+
+class WPDB(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        WPDB n[1]
+        """
+        super(WPDB, self).__init__(shx, spline)
+        p, _ = self._parse_line(spline)
+        self.n = 1
+        if len(p) > 0:
+            self.n = p[0]
+
+
+class SPEC(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        SPEC d[0.2]
+        """
+        super(SPEC, self).__init__(shx, spline)
+        self.d = None
+        p, _ = self._parse_line(spline)
+        if len(p) > 0:
+            self.d = p[0]
+
+
+class STIR(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        STIR sres step[0.01]
+        """
+        super(STIR, self).__init__(shx, spline)
+        p, _ = self._parse_line(spline)
+        self.step = 0.01
+        self.sres = None
+        if len(p) > 0:
+            self.sres = p[0]
+        if len(p) > 1:
+            self.step = p[1]
+
+    def __repr__(self):
+        return "STIR {} {}".format(self.sres if self.sres else '', self.step)
+
+    def __str__(self):
+        return "STIR {} {}".format(self.sres if self.sres else '', self.step)
+
+
+class TWST(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        TWST N[0] (N[1] after SHELXL-2018/3)
+        Twin component number to be used for the completeness and Friedel completeness statistics.
+        """
+        super(TWST, self).__init__(shx, spline)
+        p, _ = self._parse_line(spline)
+        self.N = 1
+        if len(p) > 0:
+            self.N = p[0]
+
+
+class RTAB(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        RTAB codename atomnames
+        """
+        super(RTAB, self).__init__(shx, spline)
+        self.code = spline.pop(1)
+        _, self.atoms = self._parse_line(spline)
+
+
+class PRIG(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        PRIG p[#]
+        """
+        super(PRIG, self).__init__(shx, spline)
+        params, _ = self._parse_line(spline)
+        if len(params) > 0:
+            self.p = params[0]
+
+
+class PLAN(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        PLAN npeaks[20] d1[#] d2[#]
+        """
+        self.shx = shx
+        super(PLAN, self).__init__(shx, spline)
+        self.npeaks = 20
+        self.d1 = None
+        self.d2 = None
+        params, _ = self._parse_line(spline)
+        if len(params) > 0:
+            self.npeaks = int(params[0])
+        if len(params) > 1:
+            self.d1 = params[1]
+        if len(params) > 2:
+            self.d2 = params[2]
+
+    def __repr__(self):
+        return f'PLAN {self.npeaks:,g}{" " if self.d1 else ""}{self.d1 if self.d1 is not None else ""}' \
+               f'{" " if self.d2 else ""}{self.d2 if self.d2 is not None else ""}'
+
+
+class FRAG(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        FRAG code[17] a[1] b[1] c[1] α[90] β[90] γ[90]
+        """
+        super(FRAG, self).__init__(shx, spline)
+        params, _ = self._parse_line(spline)
+        self.code = params[0]
+        self.cell = params[1:7]
+
+
+class FREE(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        FREE atom1 atom2
+        """
+        super(FREE, self).__init__(shx, spline)
+        _, atoms = self._parse_line(spline)
+        self.atom1 = None
+        self.atom2 = None
+        try:
+            self.atom1 = atoms[0]
+            self.atom2 = atoms[1]
+        except IndexError:
+            raise ParseParamError
+
+
+class FMAP(Command):
+    """
+    FMAP code[2] axis[#] nl[53]
+    """
+
+    def __init__(self, shx, spline: list):
+        super(FMAP, self).__init__(shx, spline)
+        params, _ = self._parse_line(spline)
+        self.code = None
+        self.axis = None
+        self.nl = None
+        if len(params) > 0:
+            self.code = params[0]
+        if len(params) > 1:
+            self.axis = params[1]
+        if len(params) > 2:
+            self.nl = params[2]
+
+
+class MOVE(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        MOVE dx[0] dy[0] dz[0] sign[1]
+        """
+        super(MOVE, self).__init__(shx, spline)
+        params, _ = self._parse_line(spline)
+        self.dxdydz = None
+        self.sign = None
+        if len(params) > 2:
+            self.dxdydz = params[:3]
+        if len(params) > 3:
+            self.sign = params[3]
+
+
+class MERG(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        MERG n[2]
+        """
+        super(MERG, self).__init__(shx, spline)
+        self.n = None
+        _n, _ = self._parse_line(spline)
+        if len(_n) > 0:
+            self.n = _n[0]
+
+
+class HTAB(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        HTAB dh[2.0]
+        HTAB donor-atom acceptor-atom
+        """
+        super(HTAB, self).__init__(shx, spline)
+        self.dh = None
+        self.donor = None
+        self.acceptor = None
+        dh, atoms = self._parse_line(spline)
+        if dh:
+            self.dh = dh[0]
+        if len(atoms) == 2:
+            self.donor = atoms[0]
+            self.acceptor = atoms[1]
+
+
+class GRID(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        GRID sl[#] sa[#] sd[#] dl[#] da[#] dd[#]
+        """
+        super(GRID, self).__init__(shx, spline)
+        params, _ = self._parse_line(spline)
+        if len(params) > 0:
+            self.sl = params[0]
+        if len(params) > 1:
+            self.sa = params[1]
+        if len(params) > 2:
+            self.sd = params[2]
+        if len(params) > 3:
+            self.dl = params[3]
+        if len(params) > 4:
+            self.da = params[4]
+        if len(params) > 5:
+            self.dd = params[5]
+
+
+class ACTA(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        ACTA 2θfull[#]
+        """
+        super(ACTA, self).__init__(shx, spline)
+        self.twotheta, _ = self._parse_line(spline)
+        self.shx = shx
+
+    def _as_str(self):
+        if self.twotheta:
+            return f"ACTA {self.twotheta[0]:,g}"
+        else:
+            return "ACTA"
+
+    def __repr__(self):
+        return self._as_str()
+
+    def __str__(self):
+        return self._as_str()
+
+
+class BLOC(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        BLOC n1 n2 atomnames
+        """
+        super(BLOC, self).__init__(shx, spline)
+        params, self.atoms = self._parse_line(spline)
+        self.n1 = None
+        self.n2 = None
+        if len(params) > 0:
+            self.n1 = params[0]
+        if len(params) > 1:
+            self.n2 = params[1]
+        self.shx = shx
+
+
+class FVAR():
+    def __init__(self, number: int = 1, value: float = 0.0):
+        """
+        FVAR osf[1] free variables
+        """
+        self.fvar_value = value  # value
+        self.number = number  # occurence inside of FVAR instructions
+        self.usage = 1
+
+    def __str__(self):
+        return str(float(self.fvar_value))
+
+    def __repr__(self):
+        return str(float(self.fvar_value))
+
+
+class FVARs():
+    def __init__(self, shx):
+        super(FVARs, self).__init__()
+        self.fvars = []  # free variables
+        self.shx = shx
+        self._fvarline = 0
+
+    def __iter__(self):
+        """
+        Must be defined for __repr__() to work.
+        """
+        for x in self.fvars:
+            yield x
+
+    def __getitem__(self, item: int) -> str:
+        # SHELXL counts fvars from 1 to x:
+        item = abs(item) - 1
+        return self.fvars[item].fvar_value
+
+    def __setitem__(self, key, fvar_value):
+        self.fvars[key] = fvar_value
+
+    def __len__(self) -> int:
+        return len(self.fvars)
+
+    def __str__(self) -> str:
+        # returnes FVAR as list of FVAR instructions with seven numbers in one line
+        lines = chunks(self.as_stringlist, 7)
+        fvars = ['   '.join(i) for i in lines]
+        fvars = ['FVAR   ' + i for i in fvars]
+        return "\n".join(fvars)
+
+    def __repr__(self):
+        return str([x for x in self.fvars])
+
+    @property
+    def position(self) -> int:
+        return self.shx.index_of(self)
+
+    def set_free_variables(self, fvar: int, dummy_fvar: float = 0.5):
+        """
+        Inserts additional free variables according to the fvar number.
+        """
+        if fvar > 99:
+            print('*** SHELXL allows only 99 free variables! ***')
+            raise ParseParamError
+        varlen = len(self.fvars)
+        difference = (abs(fvar) - varlen)
+        if difference > 0:
+            for n in range(int(difference)):
+                fv = FVAR(varlen + n, dummy_fvar)
+                self.fvars.append(fv)
+
+    def append(self, fvar) -> None:
+        self.fvars.append(fvar)
+
+    def set_fvar_usage(self, fvarnum: int, times: int = 1) -> None:
+        """
+        Incerements the usage count of a free variable by times.
+        """
+        fvarnum = abs(fvarnum)
+        if len(self.fvars) >= abs(fvarnum):
+            self.fvars[fvarnum - 1].usage += times
+        elif fvarnum > 1 and DEBUG:
+            print('*** Free variable {} is not defined but used! ***'.format(fvarnum))
+
+    def get_fvar_usage(self, fvarnum):
+        """
+        Returns the usage (count) of a certain free variable.
+        """
+        try:
+            usage = self.fvars[fvarnum - 1].usage
+        except IndexError:
+            return 0
+        return usage
+
+    def fvars_used(self):
+        """
+        Retruns a dictionary with the usage of all free variables.
+        """
+        used = {}
+        for num, fv in enumerate(self.fvars):
+            used[num + 1] = fv.usage
+        return used
+
+    @property
+    def as_stringlist(self):
+        return [str(x.fvar_value) for x in self.fvars]
+
+
+class CONF(Command):
+
+    def __init__(self, shx, spline: list) -> None:
+        """
+        CONF atomnames max_d[1.9] max_a[170]
+        """
+        super(CONF, self).__init__(shx, spline)
+
+
+class CONN(Command):
+
+    def __init__(self, shx, spline: list) -> None:
+        """
+        CONN bmax[12] r[#] atomnames or CONN bmax[12]
+        """
+        super(CONN, self).__init__(shx, spline)
+
+
+class REM(Command):
+
+    def __init__(self, shx, spline: list) -> None:
+        """
+        Parses REM lines
+        """
+        super(REM, self).__init__(shx, spline)
+
+
+class BIND(Command):
+
+    def __init__(self, shx, spline: list) -> None:
+        """
+        BIND atom1 atom2
+        BIND m n
+        """
+        super(BIND, self).__init__(shx, spline)
+        self.parts, self.atoms = self._parse_line(spline)
+
+
+class BOND(Command):
+
+    def __init__(self, shx, spline: list) -> None:
+        """
+        BOND atomnames
+        """
+        super(BOND, self).__init__(shx, spline)
+        _, self.atoms = self._parse_line(spline)
+
+
+class DISP(Command):
+    """
+    DISP E f' f"[#] mu[#]
+    """
+
+    def __init__(self, shx, spline: list) -> None:
+        super(DISP, self).__init__(shx, spline)
+        self.element, self.parameter = self._parse_line(spline)
+
+
+class Restraints():
+    """
+    Base class for the list of restraints.
+    :type _restraints: List[Restraint]
+    """
+
+    def __init__(self):
+        """
+        """
+        self._restraints = []
+
+    def append(self, restr):
+        self._restraints.append(restr)
+
+    def __iter__(self):
+        for x in self._restraints:
+            yield x
+
+    def __getitem__(self, item):
+        return self._restraints[item]
+
+    def __repr__(self):
+        if self._restraints:
+            return "\n".join([str(x) for x in self._restraints])
+        else:
+            return 'No Restraints in file.'
+
+    @staticmethod
+    def _resolve_atoms(shx, restr: Restraint):
+        atoms = restr.atoms
+        for atnum, ap in enumerate(atoms):
+            if not isinstance(ap, (list, tuple)):
+                # ignores all ranges: ['O1', '>', 'F9']
+                try:
+                    atoms[atnum] = shx.atoms.get_atom_by_name(ap)
+                except TypeError:
+                    continue
+                continue
+            for num, atname in enumerate(ap):
+                # without range: [['O1', 'C1'], ...]
+                try:
+                    atoms[atnum][num] = shx.atoms.get_atom_by_name(atname)
+                except TypeError:
+                    continue
+
+
+class DEFS(Restraint):
+
+    def __init__(self, shx, spline: list):
+        """
+        DEFS sd[0.02] sf[0.1] su[0.01] ss[0.04] maxsof[1]
+        Changes the *default* effective standard deviations for the following
+        DFIX, SAME, SADI, CHIV, FLAT, DELU and SIMU restraints.
+        """
+        super(DEFS, self).__init__(shx, spline)
+        self.sf = 0.1
+        self.su = 0.01
+        self.ss = 0.04
+        self.maxsof = 1
+        self.sd = 0.02
+        self.active = True
+        p, _ = self._parse_line(spline)
+        if _:
+            raise ParseParamError
+        if len(p) > 0:
+            self.sd = p[0]
+        if len(p) > 1:
+            self.sf = p[1]
+        if len(p) > 2:
+            self.su = p[2]
+        if len(p) > 3:
+            self.ss = p[3]
+        if len(p) > 4:
+            self.maxsof = p[4]
+
+    @property
+    def all(self):
+        return self.sd, self.sf, self.su, self.ss, self.maxsof
+
+
+class NCSY(Restraint):
+    """
+    NCSY DN sd[0.1] su[0.05] atoms
+    """
+
+    def __init__(self, shx, spline: list):
+        super(NCSY, self).__init__(shx, spline)
+        self.sd = 0.1
+        self.su = 0.05
+        self.DN = None
+        p, self.atoms = self._parse_line(spline, pairs=False)
+        if len(p) > 0:
+            self.DN = p[0]
+        if len(p) > 1:
+            self.sd = p[1]
+        if len(p) > 2:
+            self.su = p[2]
+        if not self.DN:
+            raise ParseNumError
+
+
+class ISOR(Restraint):
+
+    def __init__(self, shx, spline: list):
+        """
+        ISOR s[0.1] st[0.2] atomnames
+        """
+        super(ISOR, self).__init__(shx, spline)
+        self.s = 0.1
+        self.st = 0.2
+        p, self.atoms = self._parse_line(spline, pairs=False)
+        if len(p) > 0:
+            self.s = p[0]
+        if len(p) > 1:
+            self.st = p[1]
+
+
+class FLAT(Restraint):
+    """
+    FLAT s[0.1] four or more atoms
+    """
+
+    def __init__(self, shx, spline: list):
+        super(FLAT, self).__init__(shx, spline)
+        self.s = 0.1
+        p, self.atoms = self._parse_line(spline, pairs=False)
+        if len(p) > 0:
+            self.s = p[0]
+        # TODO: Have to resolve ranges first:
+        # if len(self.atoms) < 4:
+        #    raise ParseParamError
+
+
+class BUMP(Restraint):
+
+    def __init__(self, shx, spline):
+        """
+        BUMP s [0.02]
+        """
+        super(BUMP, self).__init__(shx, spline)
+        self.s = 0.02
+        p, _ = self._parse_line(spline, pairs=False)
+        if len(p) > 0:
+            self.s = p[0]
+        if _:
+            raise ParseParamError
+
+
+class DFIX(Restraint):
+
+    def __init__(self, shx, spline):
+        """
+        DFIX d s[0.02] atom pairs
+        """
+        super(DFIX, self).__init__(shx, spline)
+        self.s = 0.02
+        p, self.atoms = self._parse_line(spline, pairs=True)
+        if len(p) > 0:
+            self.d = p[0]
+        if len(p) > 1:
+            self.s = p[1]
+        self._paircheck()
+        if not self.d:
+            raise ParseNumError
+        if DEBUG and 0.0001 < self.d <= self.s:
+            print('*** WRONG ODER of INSTRUCTIONS. d is smaller than s ***')
+            print("{}".format(self.textline))
+
+
+class DANG(Restraint):
+
+    def __init__(self, shx, spline):
+        """
+        DANG d s[0.04] atom pairs
+        """
+        super(DANG, self).__init__(shx, spline)
+        self.s = 0.04
+        p, self.atoms = self._parse_line(spline, pairs=True)
+        if len(p) > 0:
+            self.d = p[0]
+        if len(p) > 1:
+            self.s = p[1]
+        self._paircheck()
+        if not self.d:
+            raise ParseNumError
+        if 0.0001 < self.d <= self.s:  # Raise exception if d is smaller than s
+            raise ParseOrderError
+
+
+class SADI(Restraint):
+
+    def __init__(self, shx, spline):
+        """
+        SADI s[0.02] pairs of atoms
+        Instructions with only two atoms are ignored by SHELXL: SADI C3 C4
+        SADI_3 C3 C4 C3_4 C4_4 creates SADI C3_3 C4_3  C3_4 C4_4
+        SADI_CCF3 C3 C4 C3_4 C4_4 creates SADI C3_1 C4_1  C3_2 C4_2  C3_4 C4_4 if there are residues 1, 2 and 4
+        """
+        super(SADI, self).__init__(shx, spline)
+        self.s = 0.02
+        p, self.atoms = self._parse_line(spline, pairs=True)
+        if len(p) > 0:
+            self.s = p[0]
+        self._paircheck()
+
+
+class SAME(Restraint):
+
+    def __init__(self, shx, spline):
+        """
+        SAME s1[0.02] s2[0.04] atomnames
+        """
+        super(SAME, self).__init__(shx, spline)
+        self.s1 = 0.02
+        self.s2 = 0.04
+        p, self.atoms = self._parse_line(spline, pairs=False)
+        if len(p) > 0:
+            self.s1 = p[0]
+        if len(p) > 1:
+            self.s2 = p[1]
+
+
+class RIGU(Restraint):
+
+    def __init__(self, shx, spline: list):
+        """
+        RIGU s1[0.004] s2[0.004] atomnames
+        """
+        super(RIGU, self).__init__(shx, spline)
+        self.s1 = 0.004
+        self.s2 = 0.004
+        p, self.atoms = self._parse_line(spline, pairs=False)
+        if len(p) > 0:
+            self.s1 = p[0]
+        if len(p) > 1:
+            self.s2 = p[1]
+
+
+class SIMU(Restraint):
+
+    def __init__(self, shx, spline: list):
+        """
+        SIMU s[0.04] st[0.08] dmax[2.0] atomnames
+        """
+        super(SIMU, self).__init__(shx, spline)
+        self.s = 0.04
+        self.st = 0.08
+        self.dmax = 2.0
+        p, self.atoms = self._parse_line(spline, pairs=False)
+        if len(p) > 0:
+            self.s = p[0]
+        if len(p) > 1:
+            self.st = p[1]
+        if len(p) > 2:
+            self.dmax = p[2]
+
+
+class DELU(Restraint):
+
+    def __init__(self, shx, spline: list):
+        """
+        DELU s1[0.01] s2[0.01] atomnames
+        """
+        super(DELU, self).__init__(shx, spline)
+        self.s1 = 0.01
+        self.s2 = 0.01
+        p, self.atoms = self._parse_line(spline, pairs=False)
+        if len(p) > 0:
+            self.s1 = p[0]
+        if len(p) > 1:
+            self.s2 = p[1]
+
+
+class CHIV(Restraint):
+
+    def __init__(self, shx, spline: list):
+        """
+        CHIV V[0] s[0.1] atomnames
+        """
+        super(CHIV, self).__init__(shx, spline)
+        self.s = 0.1
+        self.V = 0.0
+        p, self.atoms = self._parse_line(spline, pairs=False)
+        if len(p) > 0:
+            self.V = p[0]
+        if len(p) > 1:
+            self.s = p[1]
+
+
+class EADP(Restraint):
+    """
+    EADP atomnames
+    """
+
+    def __init__(self, shx, spline: list) -> None:
+        super(EADP, self).__init__(shx, spline)
+        _, self.atoms = self._parse_line(spline, pairs=False)
+
+
+class EXYZ(Restraint):
+    """
+    EADP atomnames
+    """
+
+    def __init__(self, shx, spline: list) -> None:
+        super(EXYZ, self).__init__(shx, spline)
+        _, self.atoms = self._parse_line(spline, pairs=False)
+
+
+class DAMP(Command):
+    """
+    DAMP damp[0.7] limse[15]
+    """
+
+    def __init__(self, shx, spline: list):
+        super(DAMP, self).__init__(shx, spline)
+        values, _ = self._parse_line(spline, intnums=False)
+        self.damp, self.limse = 0, 0
+        if len(values) > 0:
+            self.damp = values[0]
+        if len(values) > 1:
+            self.damp, self.limse = values
+
+    def __repr__(self) -> str:
+        if self.limse == 0:
+            return "DAMP  {:,g}".format(self.damp)
+        else:
+            return "DAMP  {:,g} {:,g}".format(self.damp, self.limse)
+
+
+class HFIX(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        HFIX mn U[#] d[#] atomnames
+        """
+        super(HFIX, self).__init__(shx, spline)
+        self.params, self.atoms = self._parse_line(spline, intnums=True)
+
+    def __repr__(self):
+        return f"HFIX {' '.join([str(x) for x in self.params]) if self.params else ''} " \
+               f"{' '.join(self.atoms) if self.atoms else ''}"
+
+
+class HKLF(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        HKLF N[0] S[1] r11...r33[1 0 0 0 1 0 0 0 1] sm[1] m[0]
+        """
+        super(HKLF, self).__init__(shx, spline)
+        p, _ = self._parse_line(spline)
+        self.n = 0
+        self.s = 1
+        self.matrix = [1, 0, 0, 0, 1, 0, 0, 0, 1]
+        self.sm = 1
+        self.m = 0
+        if len(p) > 0:
+            self.n = int(p[0])
+        if len(p) > 1:
+            self.s = p[1]
+        if len(p) > 10:
+            self.matrix = p[3:11]
+        if len(p) > 11:
+            self.sm = p[12]
+        if len(p) > 12:
+            self.m = p[13]
+
+    def __repr__(self):
+        return "HKLF {:,g} {:,g}  {}  {:,g} {:,g}".format(self.n, self.s, ' '.join([str(i) for i in self.matrix]),
+                                                          self.sm, self.m)
+
+
+class SUMP(Command):
+    """
+    SUMP for linear equation eypressions with free variables.
+    SUMP c sigma c1 m1 c2 m2 ...
+    """
+
+    def __init__(self, shx, spline: list):
+        super(SUMP, self).__init__(shx, spline)
+        p, _ = self._parse_line(spline)
+        self.c = p.pop(0)
+        self.fvars = {}
+        self.sigma = p.pop(0)
+        # this is to have integer free variables
+        fvars = [int(x) for x in p[1::2]]
+        times = [x for x in p[0::2]]
+        self.fvars = [[x, y] for x, y in zip(times, fvars)]
+
+    def __getitem__(self, item):
+        return self.fvars[item]
+
+
+class LATT(Command):
+    lattdict = {1: [],  # Primitive
+                2: [SymmetryElement(['0.5', '0.5', '0.5'])],  # I-centered
+                3: [SymmetryElement(['1/3', '2/3', '2/3']),  # Rhombohedral
+                    SymmetryElement(['2/3', '1/3', '1/3'])],
+                4: [SymmetryElement(['0.0', '0.5', '0.5']),  # F-centered
+                    SymmetryElement(['0.5', '0.0', '0.5']),
+                    SymmetryElement(['0.5', '0.5', '0.0'])],
+                5: [SymmetryElement(['0.0', '0.5', '0.5'])],  # A-centered
+                6: [SymmetryElement(['0.5', '0.0', '0.5'])],  # B-centered
+                7: [SymmetryElement(['0.5', '0.5', '0.0'])]}  # C-centered
+
+    lattint_to_str = {1: 'P', 2: 'I', 3: 'R', 4: 'F', 5: 'A', 6: 'B', 7: 'C'}
+
+    def __init__(self, shx, spline: list):
+        """
+        LATT N[1]
+        """
+        super(LATT, self).__init__(shx, spline)
+        p, _ = self._parse_line(spline)
+        self.centric = False
+        try:
+            self.N = int(p[0])
+        except ValueError:
+            self.N = -1
+        self.N_str = self.lattint_to_str[abs(self.N)]
+        if self.N > 0:  # centrosymmetric space group:
+            self.centric = True
+        self.latt_ops = LATT.lattdict[abs(self.N)]
+
+
+class SYMM(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        SYMM symmetry operation
+        """
+        super(SYMM, self).__init__(shx, spline)
+        self.symmcard = self._parse_line(spline)
+
+    def _parse_line(self, spline: list, intnums: bool = False) -> list:
+        symmcard = ''.join(spline[1:]).split(',')  # removes whitespace
+        return symmcard
+
+    def _as_str(self):
+        return "SYMM  " + ", ".join(self.symmcard)
+
+    def __repr__(self):
+        return self._as_str()
+
+    def __str__(self) -> str:
+        return self._as_str()
+
+
+class SymmCards():
+    """
+    Contains the list of SYMM cards
+    """
+
+    def __init__(self, shx):
+        self.shx = shx
+        self._symmcards = [SymmetryElement(['X', 'Y', 'Z'])]
+        self.latt_ops = []
+
+    def _as_str(self) -> str:
+        return "\n".join([str(x) for x in self._symmcards])
+
+    def __repr__(self) -> str:
+        return self._as_str()
+
+    def __str__(self) -> str:
+        return self._as_str()
+
+    def __getitem__(self, item):
+        return self._symmcards[item]
+
+    def __iter__(self):
+        for x in self._symmcards:
+            yield x
+
+    def append(self, symm_data: list) -> None:
+        """
+        Add the content of a Shelxl SYMM command to generate the appropriate SymmetryElement instance.
+        :param symm_data: list of strings. eg.['1/2+X', '1/2+Y', '1/2+Z']
+        :return: None
+        """
+        new_symm = SymmetryElement(symm_data)
+        self._symmcards.append(new_symm)
+        for symm in self.shx.latt.latt_ops:
+            latt_symm = new_symm.apply_latt_symm(symm)
+            if latt_symm not in self._symmcards:
+                self._symmcards.append(latt_symm)
+        if self.shx.latt.centric:
+            self._symmcards.append(SymmetryElement(symm_data, centric=True))
+            for symm in self.shx.latt.latt_ops:
+                latt_symm = new_symm.apply_latt_symm(symm)
+                latt_symm.centric = True
+                self._symmcards.append(latt_symm)
+
+    def set_centric(self, value: bool):
+        """
+        Defines the instance as representing a centrosymmetric structure. Generates the appropriate SymmetryElement
+        instances automatically if called before adding further SYMM commands via self.addSymm().
+        """
+        self.shx.latt.centric = value
+        self._symmcards.append(SymmetryElement(['-X', '-Y', '-Z']))
+        self._symmcards[-1].centric = True
+
+    def set_latt_ops(self, lattops: list) -> None:
+        """
+        Adds lattice operations. If called before adding SYMM commands, the appropriate lattice operations are used
+        automatically to generate further SymmetryElements.
+        :param lattops: list of SymmetryElement instances.
+        """
+        self.latt_ops = lattops
+
+
+class LSCycles(Command):
+    def __init__(self, shx, spline: list):
+        """
+        L.S. nls[0] nrf[0] nextra[0]
+        #TODO: support nls parameter
+        If nrf is positive, it is the number of these cycles that should be performed before applying ANIS.
+        Negative nrf indicates which reflections should be ignored during the refinement but used instead for
+        the calculation of free R-factors in the final structure factor summation.
+        nextra is the number of additional parameters that were derived from the data when 'squeezing' the
+        structure etc.
+        """
+        super(LSCycles, self).__init__(shx, spline)
+        p, _ = self._parse_line(spline)
+        self._shx = shx
+        self.cgls = False
+        self._cycles = 0
+        self._nrf = ''
+        self._nextra = ''
+        try:
+            self._cycles = int(p[0])
+        except (IndexError, NameError, ValueError):
+            raise ParseNumError
+        try:
+            self._nrf = int(p[1])
+        except IndexError:
+            pass
+        try:
+            self._nextra = int(p[2])
+        except IndexError:
+            pass
+        if spline[0].upper() == 'CGLS':
+            self.cgls = True
+
+    @property
+    def number(self):
+        return self._cycles
+
+    @number.setter
+    def number(self, n: int) -> None:
+        self._cycles = int(n)
+        self.__init__(self._shx, self._as_str().split())
+
+    def set_refine_cycles(self, number: int) -> None:
+        """
+        Sets the number of refinement cycles for the current res file.
+        """
+        self.number = int(number)
+
+    @property
+    def text(self) -> str:
+        """
+        'CGLS 10 2 '
+        """
+        return self.__repr__()
+
+    def __iter__(self):
+        for x in self.__repr__().split():
+            yield x
+
+    def _as_str(self):
+        return '{} {} {} {}'.format('CGLS' if self.cgls else 'L.S.', self._cycles,
+                                    self._nrf if self._nrf else '', self._nextra if self._nextra else '').strip()
+
+    def __repr__(self):
+        return self._as_str()
+
+
+class SFACTable():
+    def __init__(self, shx):
+        """
+        Holds the information of SFAC instructions. Either with default values and only elements
+        SFAC elements
+        or as explicit scattering factor in the form of an exponential series, followed by real and
+        imaginary dispersion terms, linear absorption coefficient, covalent radius and atomic weight.
+
+        SFAC elements  or  SFAC E a1 b1 a2 b2 a3 b3 a4 b4 c f' f" mu r wt
+        """
+        self.sfac_table = []
+        self.shx = shx
+        self.elements_list = []
+
+    def __iter__(self):
+        for x in self.sfac_table:
+            yield x['element'].capitalize()
+
+    def __repr__(self):
+        sftext = ''
+        elements = []
+        for sf in self.sfac_table:
+            if not self.is_exp(sf) and sf['element'].capitalize() not in elements:
+                elements.append(sf['element'].capitalize())
+            else:
+                if elements:
+                    sftext = self._extend_sfac_text(elements, sftext)
+                    elements = []
+                values = []
+                for x in ('element', 'a1', 'b1', 'a2', 'b2', 'a3', 'b3', 'a4', 'b4', 'c',
+                          'fprime', 'fdprime', 'mu', 'r', 'wt'):
+                    values.append(sf[x])
+                sftext += "\nSFAC " + "  ".join(values)
+        if elements:
+            sftext = self._extend_sfac_text(elements, sftext)
+        return sftext[1:]
+
+    def _extend_sfac_text(self, elements: List[str], sftext: str) -> str:
+        sftext += "\nSFAC " + "  ".join(elements)
+        return sftext
+
+    def __getitem__(self, index: int):
+        """
+        Returns the n-th element in the sfac table, beginning with 1.
+        """
+        if index == 0:
+            raise IndexError
+        if index < 0:
+            index = len(self.sfac_table) + index + 1
+        return self.sfac_table[index - 1]['element'].capitalize()
+
+    def parse_element_line(self, spline: list):
+        """
+        Adds a new SFAC card to the list of cards.
+        """
+        if not ''.join(spline[1:]).isalpha():  # joining, because space is not alphabetical
+            # Excplicit with all values
+            sfdic = {}
+            for n, x in enumerate(['element', 'a1', 'b1', 'a2', 'b2', 'a3', 'b3', 'a4', 'b4', 'c',
+                                   'fprime', 'fdprime', 'mu', 'r', 'wt']):
+                if n == 0:
+                    self.elements_list.append(spline[n + 1].upper())
+                try:
+                    sfdic[x] = spline[n + 1]
+                except IndexError:
+                    raise ParseNumError()
+            self.sfac_table.append(sfdic)
+        else:
+            # Just the elements
+            for x in spline[1:]:
+                self.elements_list.append(x.upper())
+                self.sfac_table.append({'element': x.upper()})
+
+    def has_element(self, element):
+        return element.upper() in self.elements_list
+
+    @staticmethod
+    def is_exp(item):
+        return 'a1' in item
+
+    def add_element(self, element: str):
+        """
+        Adds an element to the SFAC list.
+        """
+        if self.has_element(element):
+            return
+        self.elements_list.append(element.upper())
+        self.sfac_table.append({'element': element.upper(), 'line_number': None})
+        self.shx.unit.add_number(1.0)
+
+    def remove_element(self, element: str):
+        del self.sfac_table[self.shx.elem2sfac(element.upper()) - 1]
+        del self.elements_list[self.elements_list.index(element.upper())]
+
+
+class UNIT(Command):
+
+    values: List[Union[int, float]]
+
+    def __init__(self, shx, spline: List):
+        """
+        UNIT n1 n2 ...
+        """
+        super(UNIT, self).__init__(shx, spline)
+        self.values, _ = self._parse_line(spline)
+
+    def add_number(self, number: float):
+        self.values.append(number)
+
+    def __iter__(self):
+        yield [x for x in self.values]
+
+    def __repr__(self):
+        return "UNIT " + "  ".join(["{:,g}".format(x) for x in self.values])
+
+    def __str__(self):
+        return self.__repr__()
+
+    def __setitem__(self, key, value):
+        self.values[key] = value
+
+    def __getitem__(self, item):
+        return self.values[item]
+
+    def __add__(self, other):
+        self.values.append(other)
+
+
+class BASF(Command):
+    """
+    BASF scale factors
+    BASF can occour in multiple lines.
+    """
+    scale_factors: List[Union[int, float]]
+
+    def __init__(self, shx, spline):
+        super(BASF, self).__init__(shx, spline)
+        self.scale_factors, _ = self._parse_line(spline)
+
+    def __iter__(self):
+        yield self.scale_factors
+
+
+class TWIN(Command):
+
+    def __init__(self, shx, spline: List):
+        """
+        TWIN 3x3 matrix [-1 0 0 0 -1 0 0 0 -1] N[2]
+        +N     -N  m = |N|
+        m-1 to 2m-1
+        m-1   (2*abs(m)/2)-1
+        """
+        super(TWIN, self).__init__(shx, spline)
+        self.matrix = [-1, 0, 0, 0, -1, 0, 0, 0, -1]
+        self.allowed_N = 2
+        self.n_value = 2
+        if len(spline) > 1:
+            p, _ = self._parse_line(spline, intnums=False)
+            if len(p) == 9:
+                self.matrix = p
+            elif len(p) == 10:
+                self.matrix = p[:9]
+                self.n_value = int(p[9])
+            else:
+                raise ParseNumError("*** Check TWIN instruction. ***")
+        m = abs(self.n_value) / 2
+        if self.n_value > 0:
+            self.allowed_N = abs(self.n_value) - 1
+        else:
+            self.allowed_N = (2 * m) - 1
+
+
+class WGHT(Command):
+
+    def __init__(self, shx, spline: list):
+        """
+        The weighting scheme is defined as follows:
+        w = q / [ σ²(Fo²) + (a*P)² + b*P + d + e*sin(θ)/$lambda; ]
+
+        WGHT a[0.1] b[0] c[0] d[0] e[0] f[.33333]
+        Usually only 'WGHT a b' is used
+        """
+        super(WGHT, self).__init__(shx, spline)
+        self.shx = shx
+        self.a = 0.1
+        self.b = 0.0
+        self.c = 0.0
+        self.d = 0.0
+        self.e = 0.0
+        self.f = 0.33333
+        p, _ = self._parse_line(spline)
+        if len(p) > 0:
+            self.a = p[0]
+        if len(p) > 1:
+            self.b = p[1]
+        if len(p) > 2:
+            self.c = p[2]
+        if len(p) > 3:
+            self.d = p[3]
+        if len(p) > 4:
+            self.e = p[4]
+        if len(p) > 5:
+            self.f = p[5]
+
+    def _as_string(self):
+        wght = 'WGHT   {} {}'.format(self.a, self.b)
+        # It is very unlikely that someone changes other parameter than a and b:
+        if (self.c + self.d + self.e + self.f) != 0.33333:
+            wght += ' {} {} {} {}'.format(self.c, self.d, self.e, self.f)
+        return wght
+
+    def difference(self) -> List[float]:
+        """
+        Returns a list with the weight differences of the parameters a and b.
+        """
+        try:
+            adiff = abs(self.shx.wght.a - self.shx.wght_suggested.a)
+            bdiff = abs(self.shx.wght.b - self.shx.wght_suggested.b)
+        except AttributeError:
+            print("No suggested weighting scheme found. Unable to proceed.")
+            return [0.0, 0.0]
+        return [round(adiff, 3), round(bdiff, 3)]
+
+    def __repr__(self):
+        return self._as_string()
+
+    def __str__(self):
+        return self._as_string()
```

### Comparing `shelxfile-8/shelxfile/shelx/sdm.py` & `shelxfile-9/shelxfile/shelx/sdm.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,406 +1,406 @@
-# -*- encoding: utf-8 -*-
-# möp
-#
-# ----------------------------------------------------------------------------
-# "THE BEER-WARE LICENSE" (Revision 42):
-# <dkratzert@gmx.de> wrote this file. As long as you retain
-# this notice you can do whatever you want with this stuff. If we meet some day,
-# and you think this stuff is worth it, you can buy me a beer in return.
-# Daniel Kratzert
-# ----------------------------------------------------------------------------
-#
-import time
-from math import sqrt, radians, sin
-from pathlib import Path
-from string import ascii_letters
-
-from shelxfile.atoms.atom import Atom
-from shelxfile.misc.dsrmath import Array, Matrix, vol_unitcell
-from shelxfile.misc.misc import DEBUG, wrap_line
-from shelxfile.shelx.cards import AFIX, RESI
-
-
-class SDMItem(object):
-    __slots__ = ['dist', 'atom1', 'atom2', 'a1', 'a2', 'symmetry_number', 'covalent', 'dddd']
-
-    def __init__(self):
-        self.dist = 0.0
-        self.atom1 = None
-        self.a1 = 0
-        self.atom2 = None
-        self.a2 = 0
-        self.symmetry_number = 0
-        self.covalent = True
-        self.dddd = 0
-
-    def __lt__(self, a2):
-        return True if self.dist < a2.dist else False
-
-    def __eq__(self, other: 'SDMItem'):
-        if other.a1 == self.a2 and other.a2 == self.a1:
-            return True
-        return False
-
-    def __repr__(self):
-        return '{} {} dist: {:.6} coval: {} sn: {}  {}\n'.format(self.a1, self.a2,
-                                                                 self.dist, self.covalent,
-                                                                 self.symmetry_number, self.dddd)
-
-
-class SDM():
-    """
-    This class calculates the shortest distance matrix and creates a completed (grown) structure by crystal symmetry.
-    """
-
-    def __init__(self, shx: 'Shelxfile'):
-        self.shx = shx
-        self.cell = (
-            self.shx.cell.a, self.shx.cell.b, self.shx.cell.c, self.shx.cell.alpha, self.shx.cell.beta, self.shx.cell.gamma)
-        self.aga = self.shx.cell.a * self.shx.cell.b * self.shx.cell.cosga
-        self.bbe = self.shx.cell.a * self.shx.cell.c * self.shx.cell.cosbe
-        self.cal = self.shx.cell.b * self.shx.cell.c * self.shx.cell.cosal
-        self.sdm_list = []  # list of sdmitems
-        self.maxmol = 1
-        self.sdmtime = 0
-        self.bondlist = []
-        self.asq = self.shx.cell[0] ** 2
-        self.bsq = self.shx.cell[1] ** 2
-        self.csq = self.shx.cell[2] ** 2
-        # calculate reciprocal lattice vectors:
-        self.astar = (self.shx.cell.b * self.shx.cell.c * sin(radians(self.shx.cell.alpha))) / self.shx.cell.V
-        self.bstar = (self.shx.cell.c * self.shx.cell.a * sin(radians(self.shx.cell.beta))) / self.shx.cell.V
-        self.cstar = (self.shx.cell.a * self.shx.cell.b * sin(radians(self.shx.cell.gamma))) / self.shx.cell.V
-
-    def calc_sdm(self) -> list:
-        t1 = time.perf_counter()
-        all_atoms = self.shx.atoms.all_atoms
-        self.bondlist.clear()
-        for i, at1 in enumerate(all_atoms):
-            prime_array = [Array(at1.frac_coords) * symop.matrix + symop.trans for symop in self.shx.symmcards]
-            for j, at2 in enumerate(all_atoms):
-                mind = 1000000
-                hma = False
-                sdm_item = SDMItem()
-                for n, symop in enumerate(self.shx.symmcards):
-                    D = prime_array[n] - Array(at2.frac_coords) + 0.5
-                    dp = [v - 0.5 for v in D - D.floor]
-                    dk = self.vector_length(*dp)
-                    if dk > 5.3:
-                        continue
-                    if n:
-                        dk += 0.0001
-                    if (dk > 0.01) and (mind >= dk):
-                        mind = min(dk, mind)
-                        sdm_item.dist = mind
-                        sdm_item.atom1 = at1
-                        sdm_item.atom2 = at2
-                        sdm_item.a1 = i
-                        sdm_item.a2 = j
-                        sdm_item.symmetry_number = n
-                        hma = True
-                if not sdm_item.atom1:
-                    # Do not grow grown atoms:
-                    continue
-                if (not sdm_item.atom1.ishydrogen and not sdm_item.atom2.ishydrogen) and \
-                        sdm_item.atom1.part.n * sdm_item.atom2.part.n == 0 \
-                        or sdm_item.atom1.part.n == sdm_item.atom2.part.n:
-                    dddd = (at1.radius + at2.radius) * 1.2
-                    sdm_item.dddd = dddd
-                else:
-                    dddd = 0.0
-                if sdm_item.dist < dddd:
-                    if hma:
-                        # self.bondlist.append((i, j, sdm_item.atom1.name, sdm_item.atom2.name, sdm_item.dist))
-                        sdm_item.covalent = True
-                else:
-                    sdm_item.covalent = False
-                if hma:
-                    self.sdm_list.append(sdm_item)
-        t2 = time.perf_counter()
-        self.sdmtime = t2 - t1
-        if DEBUG:
-            print('Zeit sdm_calc:', self.sdmtime)
-        self.sdm_list.sort()
-        print(len(self.sdm_list))
-        self.calc_molindex(all_atoms)
-        need_symm = self.collect_needed_symmetry()
-        if DEBUG:
-            print("The asymmetric unit contains {} fragments.".format(self.maxmol))
-        return need_symm
-
-    def collect_needed_symmetry(self) -> list:
-        need_symm = []
-        # Collect needsymm list:
-        for sdm_item in self.sdm_list:
-            if sdm_item.covalent:
-                # all_atoms[sdm_item.a1].molindex < 1 ...
-                if sdm_item.atom1.molindex < 1 or sdm_item.atom1.molindex > 6:
-                    continue
-                for n, symop in enumerate(self.shx.symmcards):
-                    if sdm_item.atom1.part.n != 0 and sdm_item.atom2.part.n != 0 \
-                            and sdm_item.atom1.part.n != sdm_item.atom2.part.n:
-                        # both not part 0 and different part numbers
-                        continue
-                    # Both the same atomic number and number hydrogen:
-                    if sdm_item.atom1.an == sdm_item.atom2.an and sdm_item.atom1.ishydrogen:
-                        continue
-                    prime = Array(sdm_item.atom1.frac_coords) * symop.matrix + symop.trans
-                    D = prime - Array(sdm_item.atom2.frac_coords) + Array([0.5, 0.5, 0.5])
-                    floor_d = D.floor
-                    dp = D - floor_d - Array([0.5, 0.5, 0.5])
-                    if n == 0 and Array([0, 0, 0]) == floor_d:
-                        continue
-                    dk = self.vector_length(*dp)
-                    dddd = sdm_item.dist + 0.2
-                    if sdm_item.atom1.ishydrogen and sdm_item.atom2.ishydrogen:
-                        dddd = 1.8
-                    if (dk > 0.001) and (dddd >= dk):
-                        bs = [n + 1, (5 - floor_d[0]), (5 - floor_d[1]), (5 - floor_d[2]), sdm_item.atom1.molindex]
-                        if bs not in need_symm:
-                            need_symm.append(bs)
-        return need_symm
-
-    def calc_molindex(self, all_atoms):
-        # Start for George's "bring atoms together algorithm":
-        someleft = 1
-        nextmol = 1
-        for at in all_atoms:
-            at.molindex = -1
-        all_atoms[0].molindex = 1
-        while nextmol:
-            someleft = 1
-            nextmol = 0
-            while someleft:
-                someleft = 0
-                for sdm_item in self.sdm_list:
-                    if sdm_item.covalent and sdm_item.atom1.molindex * sdm_item.atom2.molindex < 0:
-                        sdm_item.atom1.molindex = self.maxmol
-                        sdm_item.atom2.molindex = self.maxmol
-                        someleft += 1
-            for ni, at in enumerate(all_atoms):
-                if not at.ishydrogen and at.molindex < 0:
-                    nextmol = ni
-                    break
-            if nextmol:
-                self.maxmol += 1
-                all_atoms[nextmol].molindex = self.maxmol
-
-    def vector_length(self, x: float, y: float, z: float) -> float:
-        """
-        Calculates the vector length given in fractional coordinates.
-        """
-        A = 2.0 * (x * y * self.aga + x * z * self.bbe + y * z * self.cal)
-        return sqrt(x ** 2 * self.asq + y ** 2 * self.bsq + z ** 2 * self.csq + A)
-
-    def packer(self, sdm: 'SDM', need_symm: list, with_qpeaks=False):
-        """
-        Packs atoms of the asymmetric unit to real molecules.
-        """
-        # t1 = time.perf_counter()
-        asymm = self.shx.atoms.all_atoms
-        if with_qpeaks:
-            showatoms = asymm[:]
-        else:
-            showatoms = [at for at in asymm if not at.qpeak]
-        for symm in need_symm:
-            symm_num, h, k, l, symmgroup = symm
-            h -= 5
-            k -= 5
-            l -= 5
-            symm_num -= 1
-            for atom in asymm:
-                if not with_qpeaks and atom.qpeak:
-                    continue
-                # Essential to have hydrogen atoms grown:
-                # if not atom.ishydrogen and atom.molindex == symmgroup:
-                if atom.molindex == symmgroup:
-                    new_atom = Atom(self.shx)
-                    if atom.qpeak:
-                        continue
-                    else:
-                        pass
-                        uvals = atom.uvals
-                        # TODO: Transform u values according to symmetry:
-                        # currently, the adps are directed in wrong directions after after applying symmetry to atoms.
-                        # uvals = self.transform_uvalues(uvals, symm_num)
-                    new_atom.set_atom_parameters(
-                        name=atom.name[:3] + ">>" + str(symm_num) + '_' + ascii_letters[atom.part.n],
-                        sfac_num=atom.sfac_num,
-                        coords=Array(atom.frac_coords) * self.shx.symmcards[symm_num].matrix
-                               + Array(self.shx.symmcards[symm_num].trans) + Array([h, k, l]),
-                        part=atom.part,
-                        afix=AFIX(self.shx, (atom.afix).split()) if atom.afix else None,
-                        resi=RESI(self.shx, ('RESI ' + atom.resinum + atom.resiclass).split()) if atom.resi else None,
-                        site_occupation=atom.sof,
-                        uvals=uvals,
-                        symmgen=True
-                    )
-                    isthere = False
-                    if new_atom.part.n >= 0:
-                        for atom in showatoms:
-                            if atom.part.n != new_atom.part.n:
-                                continue
-                            length = sdm.vector_length(new_atom.x - atom.x,
-                                                       new_atom.y - atom.y,
-                                                       new_atom.z - atom.z)
-                            if length < 0.2:
-                                isthere = True
-                    if not isthere:
-                        showatoms.append(new_atom)
-                # elif grow_qpeaks:
-                #    add q-peaks here
-        # t2 = time.perf_counter()
-        # print('packzeit:', t2-t1) # 0.04s
-        return showatoms
-
-    def transform_uvalues(self, uvals: (list, tuple), symm_num: int):
-        """
-        Transforms the Uij values according to local symmetry.
-        R. W. Grosse-Kunstleve, P. D. Adams (2002). J. Appl. Cryst. 35, 477–480.
-        http://dx.doi.org/10.1107/S0021889802008580
-
-        U(star) = N * U(cif) * N.T
-        U(star) = R * U(star) * R^t
-        U(cif) = N^-1 * U(star) * (N^-1).T
-
-        U(cart) = A * U(star) * A.T
-        U(frac) = A^1 * U(cart) * (A^1).t
-        U(star) = A^-1 * U(cart) * A^-1.t
-
-        R is the rotation part of a given symmetry operation
-
-        [ [U11, U12, U13]
-          [U12, U22, U23]
-          [U13, U23, U33]
-        ]
-        # Shelxl uses U* with a*,b*c*-parameterization
-        atomname sfac x y z sof[11] U[0.05] or U11 U22 U33 U23 U13 U12
-
-        Read:
-        X-Ray Analysis and the Structure of Organic Molecules Second Edition, Dunitz, P240
-
-        """
-        U11, U22, U33, U23, U13, U12 = uvals
-        U21 = U12
-        U32 = U23
-        U31 = U13
-        Ucif = Matrix([[U11, U12, U13], [U21, U22, U23], [U31, U32, U33]])
-        # matrix with the reciprocal lattice vectors:
-        N = Matrix([[self.astar, 0, 0],
-                    [0, self.bstar, 0],
-                    [0, 0, self.cstar]])
-        R = self.shx.symmcards[symm_num].matrix
-        R_t = self.shx.symmcards[symm_num].matrix.transposed
-        A = self.shx.orthogonal_matrix
-        # U(star) = N * U(cif) * N.T
-        # U(cart) = A * U(star) * A.T
-        # U(star) = R * U(star) * R^t
-        # U(cif) = N^-1 * U(star) * (N^-1).T
-        # U(star) = A^-1 * U(cart) * A^-1.T
-        Ustar = N * Ucif * N.T
-        Ustar = R * Ustar * R_t
-        Ucif = N.inversed * Ustar * N.inversed.T
-        uvals = Ucif
-        upper_diagonal = uvals.values[0][0], uvals.values[1][1], uvals.values[2][2], \
-                         uvals.values[1][2], uvals.values[0][2], \
-                         uvals.values[0][1]
-        return upper_diagonal
-
-
-def ufrac_to_ucart(A, cell, uvals):
-    """
-    #>>> uvals = [0.07243, 0.03058, 0.03216, -0.01057, -0.01708, 0.03014]
-    #>>> Ucart = Matrix([[ 0.0754483395556807,  0.030981701122469,  -0.0194466522033868], [  0.030981701122469,  0.03058, -0.01057], [-0.0194466522033868, -0.01057, 0.03216] ])
-    #>>> cell = (10.5086, 20.9035, 20.5072, 90, 94.13, 90)
-    #>>> from shelxfile.dsrmath import OrthogonalMatrix
-    #>>> A = OrthogonalMatrix(*cell)
-    #>>> ufrac_to_ucart(A, cell, uvals)
-    #TODO: test if this is right:
-    | 0.0740  0.0310 -0.0299|
-    | 0.0302  0.0306 -0.0148|
-    |-0.0171 -0.0106  0.0346|
-    <BLANKLINE>
-    """
-    U11, U22, U33, U23, U13, U12 = uvals
-    U21 = U12
-    U32 = U23
-    U31 = U13
-    Uij = Matrix([[U11, U12, U13], [U21, U22, U23], [U31, U32, U33]])
-    a, b, c, alpha, beta, gamma = cell
-    V = vol_unitcell(*cell)
-    # calculate reciprocal lattice vectors:
-    astar = (b * c * sin(radians(alpha))) / V
-    bstar = (c * a * sin(radians(beta))) / V
-    cstar = (a * b * sin(radians(gamma))) / V
-    # matrix with the reciprocal lattice vectors:
-    N = Matrix([[astar, 0, 0],
-                [0, bstar, 0],
-                [0, 0, cstar]])
-    # Finally transform Uij values from fractional to cartesian axis system:
-    Ucart = A * N * Uij * N.T * A.T
-    return Ucart
-
-
-if __name__ == "__main__":
-    from shelxfile.shelx.shelx import Shelxfile
-
-    shx = Shelxfile()
-    shx.read_file('shelxfile/tests/resources/p-31c.res')
-    t1 = time.perf_counter()
-    sdm = SDM(shx)
-    needsymm = sdm.calc_sdm()
-    print('sdmlist:', len(sdm.sdm_list))
-    print(needsymm)
-    packed_atoms = sdm.packer(sdm, needsymm)
-    print('Zeit für sdm:', round(time.perf_counter() - t1, 3), 's')
-    # p-31c: [[2, 6, 5, 5, 5], [3, 6, 6, 5, 5], [2, 6, 6, 5, 3], [3, 5, 6, 5, 3], [2, 5, 5, 5, 4], [3, 5, 5, 5, 4]]
-    # print(len(shx.atoms))
-    # print(len(packed_atoms))
-
-    head = """
-REM Solution 1  R1  0.081,  Alpha = 0.0146  in P31c
-REM Flack x = -0.072 ( 0.041 ) from Parsons' quotients
-REM C19.667 N2.667 P4
-TITL p-31c-neu in P-31c
-CELL  0.71073  12.5067  12.5067  24.5615   90.000   90.000  120.000
-ZERR   2   0.0043   0.0043   0.0085   0.000   0.000   0.000
-LATT -1
-SFAC C H N P Cl
-UNIT 120 186 14 12 12
-TEMP -173.000
-OMIT 0   0   2
-L.S. 10
-BOND $H
-ACTA
-CONF
-
-LIST 4
-FMAP 2
-PLAN 40
-WGHT    0.034600    0.643600
-FVAR       0.22604   0.76052   0.85152\n"""
-
-    tail = """\n
-HKLF 4
- 
-REM  p-31c-neu in P-31c
-REM R1 =  0.0308 for    4999 Fo > 4sig(Fo)  and  0.0343 for all    5352 data
-REM    287 parameters refined using    365 restraints
- 
-END 
- 
-WGHT      0.0348      0.6278 
-"""
-    for at in packed_atoms:
-        if at.qpeak:
-            continue
-        # print(wrap_line(str(at)))
-        head += wrap_line(str(at)) + '\n'
-    head += tail
-    p = Path('./test.res')
-    p.write_text(head)
-    print(len(shx.atoms))
-    print(len(packed_atoms))
-    print('Zeit für sdm:', round(sdm.sdmtime, 3), 's')
-    # print(sdm.bondlist)
-    # print(len(sdm.bondlist), '(170) Atome in p-31c.res, (208) in I-43d.res')
+# -*- encoding: utf-8 -*-
+# möp
+#
+# ----------------------------------------------------------------------------
+# "THE BEER-WARE LICENSE" (Revision 42):
+# <dkratzert@gmx.de> wrote this file. As long as you retain
+# this notice you can do whatever you want with this stuff. If we meet some day,
+# and you think this stuff is worth it, you can buy me a beer in return.
+# Daniel Kratzert
+# ----------------------------------------------------------------------------
+#
+import time
+from math import sqrt, radians, sin
+from pathlib import Path
+from string import ascii_letters
+
+from shelxfile.atoms.atom import Atom
+from shelxfile.misc.dsrmath import Array, Matrix, vol_unitcell
+from shelxfile.misc.misc import DEBUG, wrap_line
+from shelxfile.shelx.cards import AFIX, RESI
+
+
+class SDMItem(object):
+    __slots__ = ['dist', 'atom1', 'atom2', 'a1', 'a2', 'symmetry_number', 'covalent', 'dddd']
+
+    def __init__(self):
+        self.dist = 0.0
+        self.atom1 = None
+        self.a1 = 0
+        self.atom2 = None
+        self.a2 = 0
+        self.symmetry_number = 0
+        self.covalent = True
+        self.dddd = 0
+
+    def __lt__(self, a2):
+        return True if self.dist < a2.dist else False
+
+    def __eq__(self, other: 'SDMItem'):
+        if other.a1 == self.a2 and other.a2 == self.a1:
+            return True
+        return False
+
+    def __repr__(self):
+        return '{} {} dist: {:.6} coval: {} sn: {}  {}\n'.format(self.a1, self.a2,
+                                                                 self.dist, self.covalent,
+                                                                 self.symmetry_number, self.dddd)
+
+
+class SDM():
+    """
+    This class calculates the shortest distance matrix and creates a completed (grown) structure by crystal symmetry.
+    """
+
+    def __init__(self, shx: 'Shelxfile'):
+        self.shx = shx
+        self.cell = (
+            self.shx.cell.a, self.shx.cell.b, self.shx.cell.c, self.shx.cell.alpha, self.shx.cell.beta, self.shx.cell.gamma)
+        self.aga = self.shx.cell.a * self.shx.cell.b * self.shx.cell.cosga
+        self.bbe = self.shx.cell.a * self.shx.cell.c * self.shx.cell.cosbe
+        self.cal = self.shx.cell.b * self.shx.cell.c * self.shx.cell.cosal
+        self.sdm_list = []  # list of sdmitems
+        self.maxmol = 1
+        self.sdmtime = 0
+        self.bondlist = []
+        self.asq = self.shx.cell[0] ** 2
+        self.bsq = self.shx.cell[1] ** 2
+        self.csq = self.shx.cell[2] ** 2
+        # calculate reciprocal lattice vectors:
+        self.astar = (self.shx.cell.b * self.shx.cell.c * sin(radians(self.shx.cell.alpha))) / self.shx.cell.V
+        self.bstar = (self.shx.cell.c * self.shx.cell.a * sin(radians(self.shx.cell.beta))) / self.shx.cell.V
+        self.cstar = (self.shx.cell.a * self.shx.cell.b * sin(radians(self.shx.cell.gamma))) / self.shx.cell.V
+
+    def calc_sdm(self) -> list:
+        t1 = time.perf_counter()
+        all_atoms = self.shx.atoms.all_atoms
+        self.bondlist.clear()
+        for i, at1 in enumerate(all_atoms):
+            prime_array = [Array(at1.frac_coords) * symop.matrix + symop.trans for symop in self.shx.symmcards]
+            for j, at2 in enumerate(all_atoms):
+                mind = 1000000
+                hma = False
+                sdm_item = SDMItem()
+                for n, symop in enumerate(self.shx.symmcards):
+                    D = prime_array[n] - Array(at2.frac_coords) + 0.5
+                    dp = [v - 0.5 for v in D - D.floor]
+                    dk = self.vector_length(*dp)
+                    if dk > 5.3:
+                        continue
+                    if n:
+                        dk += 0.0001
+                    if (dk > 0.01) and (mind >= dk):
+                        mind = min(dk, mind)
+                        sdm_item.dist = mind
+                        sdm_item.atom1 = at1
+                        sdm_item.atom2 = at2
+                        sdm_item.a1 = i
+                        sdm_item.a2 = j
+                        sdm_item.symmetry_number = n
+                        hma = True
+                if not sdm_item.atom1:
+                    # Do not grow grown atoms:
+                    continue
+                if (not sdm_item.atom1.ishydrogen and not sdm_item.atom2.ishydrogen) and \
+                        sdm_item.atom1.part.n * sdm_item.atom2.part.n == 0 \
+                        or sdm_item.atom1.part.n == sdm_item.atom2.part.n:
+                    dddd = (at1.radius + at2.radius) * 1.2
+                    sdm_item.dddd = dddd
+                else:
+                    dddd = 0.0
+                if sdm_item.dist < dddd:
+                    if hma:
+                        # self.bondlist.append((i, j, sdm_item.atom1.name, sdm_item.atom2.name, sdm_item.dist))
+                        sdm_item.covalent = True
+                else:
+                    sdm_item.covalent = False
+                if hma:
+                    self.sdm_list.append(sdm_item)
+        t2 = time.perf_counter()
+        self.sdmtime = t2 - t1
+        if DEBUG:
+            print('Zeit sdm_calc:', self.sdmtime)
+        self.sdm_list.sort()
+        print(len(self.sdm_list))
+        self.calc_molindex(all_atoms)
+        need_symm = self.collect_needed_symmetry()
+        if DEBUG:
+            print("The asymmetric unit contains {} fragments.".format(self.maxmol))
+        return need_symm
+
+    def collect_needed_symmetry(self) -> list:
+        need_symm = []
+        # Collect needsymm list:
+        for sdm_item in self.sdm_list:
+            if sdm_item.covalent:
+                # all_atoms[sdm_item.a1].molindex < 1 ...
+                if sdm_item.atom1.molindex < 1 or sdm_item.atom1.molindex > 6:
+                    continue
+                for n, symop in enumerate(self.shx.symmcards):
+                    if sdm_item.atom1.part.n != 0 and sdm_item.atom2.part.n != 0 \
+                            and sdm_item.atom1.part.n != sdm_item.atom2.part.n:
+                        # both not part 0 and different part numbers
+                        continue
+                    # Both the same atomic number and number hydrogen:
+                    if sdm_item.atom1.an == sdm_item.atom2.an and sdm_item.atom1.ishydrogen:
+                        continue
+                    prime = Array(sdm_item.atom1.frac_coords) * symop.matrix + symop.trans
+                    D = prime - Array(sdm_item.atom2.frac_coords) + Array([0.5, 0.5, 0.5])
+                    floor_d = D.floor
+                    dp = D - floor_d - Array([0.5, 0.5, 0.5])
+                    if n == 0 and Array([0, 0, 0]) == floor_d:
+                        continue
+                    dk = self.vector_length(*dp)
+                    dddd = sdm_item.dist + 0.2
+                    if sdm_item.atom1.ishydrogen and sdm_item.atom2.ishydrogen:
+                        dddd = 1.8
+                    if (dk > 0.001) and (dddd >= dk):
+                        bs = [n + 1, (5 - floor_d[0]), (5 - floor_d[1]), (5 - floor_d[2]), sdm_item.atom1.molindex]
+                        if bs not in need_symm:
+                            need_symm.append(bs)
+        return need_symm
+
+    def calc_molindex(self, all_atoms):
+        # Start for George's "bring atoms together algorithm":
+        someleft = 1
+        nextmol = 1
+        for at in all_atoms:
+            at.molindex = -1
+        all_atoms[0].molindex = 1
+        while nextmol:
+            someleft = 1
+            nextmol = 0
+            while someleft:
+                someleft = 0
+                for sdm_item in self.sdm_list:
+                    if sdm_item.covalent and sdm_item.atom1.molindex * sdm_item.atom2.molindex < 0:
+                        sdm_item.atom1.molindex = self.maxmol
+                        sdm_item.atom2.molindex = self.maxmol
+                        someleft += 1
+            for ni, at in enumerate(all_atoms):
+                if not at.ishydrogen and at.molindex < 0:
+                    nextmol = ni
+                    break
+            if nextmol:
+                self.maxmol += 1
+                all_atoms[nextmol].molindex = self.maxmol
+
+    def vector_length(self, x: float, y: float, z: float) -> float:
+        """
+        Calculates the vector length given in fractional coordinates.
+        """
+        A = 2.0 * (x * y * self.aga + x * z * self.bbe + y * z * self.cal)
+        return sqrt(x ** 2 * self.asq + y ** 2 * self.bsq + z ** 2 * self.csq + A)
+
+    def packer(self, sdm: 'SDM', need_symm: list, with_qpeaks=False):
+        """
+        Packs atoms of the asymmetric unit to real molecules.
+        """
+        # t1 = time.perf_counter()
+        asymm = self.shx.atoms.all_atoms
+        if with_qpeaks:
+            showatoms = asymm[:]
+        else:
+            showatoms = [at for at in asymm if not at.qpeak]
+        for symm in need_symm:
+            symm_num, h, k, l, symmgroup = symm
+            h -= 5
+            k -= 5
+            l -= 5
+            symm_num -= 1
+            for atom in asymm:
+                if not with_qpeaks and atom.qpeak:
+                    continue
+                # Essential to have hydrogen atoms grown:
+                # if not atom.ishydrogen and atom.molindex == symmgroup:
+                if atom.molindex == symmgroup:
+                    new_atom = Atom(self.shx)
+                    if atom.qpeak:
+                        continue
+                    else:
+                        pass
+                        uvals = atom.uvals
+                        # TODO: Transform u values according to symmetry:
+                        # currently, the adps are directed in wrong directions after after applying symmetry to atoms.
+                        # uvals = self.transform_uvalues(uvals, symm_num)
+                    new_atom.set_atom_parameters(
+                        name=atom.name[:3] + ">>" + str(symm_num) + '_' + ascii_letters[atom.part.n],
+                        sfac_num=atom.sfac_num,
+                        coords=Array(atom.frac_coords) * self.shx.symmcards[symm_num].matrix
+                               + Array(self.shx.symmcards[symm_num].trans) + Array([h, k, l]),
+                        part=atom.part,
+                        afix=AFIX(self.shx, (atom.afix).split()) if atom.afix else None,
+                        resi=RESI(self.shx, ('RESI ' + atom.resinum + atom.resiclass).split()) if atom.resi else None,
+                        site_occupation=atom.sof,
+                        uvals=uvals,
+                        symmgen=True
+                    )
+                    isthere = False
+                    if new_atom.part.n >= 0:
+                        for atom in showatoms:
+                            if atom.part.n != new_atom.part.n:
+                                continue
+                            length = sdm.vector_length(new_atom.x - atom.x,
+                                                       new_atom.y - atom.y,
+                                                       new_atom.z - atom.z)
+                            if length < 0.2:
+                                isthere = True
+                    if not isthere:
+                        showatoms.append(new_atom)
+                # elif grow_qpeaks:
+                #    add q-peaks here
+        # t2 = time.perf_counter()
+        # print('packzeit:', t2-t1) # 0.04s
+        return showatoms
+
+    def transform_uvalues(self, uvals: (list, tuple), symm_num: int):
+        """
+        Transforms the Uij values according to local symmetry.
+        R. W. Grosse-Kunstleve, P. D. Adams (2002). J. Appl. Cryst. 35, 477–480.
+        http://dx.doi.org/10.1107/S0021889802008580
+
+        U(star) = N * U(cif) * N.T
+        U(star) = R * U(star) * R^t
+        U(cif) = N^-1 * U(star) * (N^-1).T
+
+        U(cart) = A * U(star) * A.T
+        U(frac) = A^1 * U(cart) * (A^1).t
+        U(star) = A^-1 * U(cart) * A^-1.t
+
+        R is the rotation part of a given symmetry operation
+
+        [ [U11, U12, U13]
+          [U12, U22, U23]
+          [U13, U23, U33]
+        ]
+        # Shelxl uses U* with a*,b*c*-parameterization
+        atomname sfac x y z sof[11] U[0.05] or U11 U22 U33 U23 U13 U12
+
+        Read:
+        X-Ray Analysis and the Structure of Organic Molecules Second Edition, Dunitz, P240
+
+        """
+        U11, U22, U33, U23, U13, U12 = uvals
+        U21 = U12
+        U32 = U23
+        U31 = U13
+        Ucif = Matrix([[U11, U12, U13], [U21, U22, U23], [U31, U32, U33]])
+        # matrix with the reciprocal lattice vectors:
+        N = Matrix([[self.astar, 0, 0],
+                    [0, self.bstar, 0],
+                    [0, 0, self.cstar]])
+        R = self.shx.symmcards[symm_num].matrix
+        R_t = self.shx.symmcards[symm_num].matrix.transposed
+        A = self.shx.orthogonal_matrix
+        # U(star) = N * U(cif) * N.T
+        # U(cart) = A * U(star) * A.T
+        # U(star) = R * U(star) * R^t
+        # U(cif) = N^-1 * U(star) * (N^-1).T
+        # U(star) = A^-1 * U(cart) * A^-1.T
+        Ustar = N * Ucif * N.T
+        Ustar = R * Ustar * R_t
+        Ucif = N.inversed * Ustar * N.inversed.T
+        uvals = Ucif
+        upper_diagonal = uvals.values[0][0], uvals.values[1][1], uvals.values[2][2], \
+                         uvals.values[1][2], uvals.values[0][2], \
+                         uvals.values[0][1]
+        return upper_diagonal
+
+
+def ufrac_to_ucart(A, cell, uvals):
+    """
+    #>>> uvals = [0.07243, 0.03058, 0.03216, -0.01057, -0.01708, 0.03014]
+    #>>> Ucart = Matrix([[ 0.0754483395556807,  0.030981701122469,  -0.0194466522033868], [  0.030981701122469,  0.03058, -0.01057], [-0.0194466522033868, -0.01057, 0.03216] ])
+    #>>> cell = (10.5086, 20.9035, 20.5072, 90, 94.13, 90)
+    #>>> from shelxfile.dsrmath import OrthogonalMatrix
+    #>>> A = OrthogonalMatrix(*cell)
+    #>>> ufrac_to_ucart(A, cell, uvals)
+    #TODO: test if this is right:
+    | 0.0740  0.0310 -0.0299|
+    | 0.0302  0.0306 -0.0148|
+    |-0.0171 -0.0106  0.0346|
+    <BLANKLINE>
+    """
+    U11, U22, U33, U23, U13, U12 = uvals
+    U21 = U12
+    U32 = U23
+    U31 = U13
+    Uij = Matrix([[U11, U12, U13], [U21, U22, U23], [U31, U32, U33]])
+    a, b, c, alpha, beta, gamma = cell
+    V = vol_unitcell(*cell)
+    # calculate reciprocal lattice vectors:
+    astar = (b * c * sin(radians(alpha))) / V
+    bstar = (c * a * sin(radians(beta))) / V
+    cstar = (a * b * sin(radians(gamma))) / V
+    # matrix with the reciprocal lattice vectors:
+    N = Matrix([[astar, 0, 0],
+                [0, bstar, 0],
+                [0, 0, cstar]])
+    # Finally transform Uij values from fractional to cartesian axis system:
+    Ucart = A * N * Uij * N.T * A.T
+    return Ucart
+
+
+if __name__ == "__main__":
+    from shelxfile.shelx.shelx import Shelxfile
+
+    shx = Shelxfile()
+    shx.read_file('shelxfile/tests/resources/p-31c.res')
+    t1 = time.perf_counter()
+    sdm = SDM(shx)
+    needsymm = sdm.calc_sdm()
+    print('sdmlist:', len(sdm.sdm_list))
+    print(needsymm)
+    packed_atoms = sdm.packer(sdm, needsymm)
+    print('Zeit für sdm:', round(time.perf_counter() - t1, 3), 's')
+    # p-31c: [[2, 6, 5, 5, 5], [3, 6, 6, 5, 5], [2, 6, 6, 5, 3], [3, 5, 6, 5, 3], [2, 5, 5, 5, 4], [3, 5, 5, 5, 4]]
+    # print(len(shx.atoms))
+    # print(len(packed_atoms))
+
+    head = """
+REM Solution 1  R1  0.081,  Alpha = 0.0146  in P31c
+REM Flack x = -0.072 ( 0.041 ) from Parsons' quotients
+REM C19.667 N2.667 P4
+TITL p-31c-neu in P-31c
+CELL  0.71073  12.5067  12.5067  24.5615   90.000   90.000  120.000
+ZERR   2   0.0043   0.0043   0.0085   0.000   0.000   0.000
+LATT -1
+SFAC C H N P Cl
+UNIT 120 186 14 12 12
+TEMP -173.000
+OMIT 0   0   2
+L.S. 10
+BOND $H
+ACTA
+CONF
+
+LIST 4
+FMAP 2
+PLAN 40
+WGHT    0.034600    0.643600
+FVAR       0.22604   0.76052   0.85152\n"""
+
+    tail = """\n
+HKLF 4
+ 
+REM  p-31c-neu in P-31c
+REM R1 =  0.0308 for    4999 Fo > 4sig(Fo)  and  0.0343 for all    5352 data
+REM    287 parameters refined using    365 restraints
+ 
+END 
+ 
+WGHT      0.0348      0.6278 
+"""
+    for at in packed_atoms:
+        if at.qpeak:
+            continue
+        # print(wrap_line(str(at)))
+        head += wrap_line(str(at)) + '\n'
+    head += tail
+    p = Path('./test.res')
+    p.write_text(head)
+    print(len(shx.atoms))
+    print(len(packed_atoms))
+    print('Zeit für sdm:', round(sdm.sdmtime, 3), 's')
+    # print(sdm.bondlist)
+    # print(len(sdm.bondlist), '(170) Atome in p-31c.res, (208) in I-43d.res')
```

### Comparing `shelxfile-8/shelxfile/shelx/sdm_rust.py` & `shelxfile-9/shelxfile/shelx/sdm_rust.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,316 +1,316 @@
-# -*- encoding: utf-8 -*-
-# möp
-#
-# ----------------------------------------------------------------------------
-# "THE BEER-WARE LICENSE" (Revision 42):
-# <dkratzert@gmx.de> wrote this file. As long as you retain
-# this notice you can do whatever you want with this stuff. If we meet some day,
-# and you think this stuff is worth it, you can buy me a beer in return.
-# Daniel Kratzert
-# ----------------------------------------------------------------------------
-#
-import time
-from dataclasses import dataclass
-from math import sqrt, radians, sin
-from string import ascii_letters
-from typing import Union
-
-# noinspection PyUnresolvedReferences
-from shelxfile.shelx.sdm_complete import calc_sdm
-
-from shelxfile.atoms.atom import Atom
-from shelxfile.misc.dsrmath import Array, Matrix, vol_unitcell
-from shelxfile.misc.misc import DEBUG
-from shelxfile.shelx.cards import AFIX, RESI
-
-
-@dataclass
-class RAtom:
-    name: str
-    x: float
-    y: float
-    z: float
-    element: str
-    part: int
-    symmgen: bool
-    molindex: int
-    qpeak: bool
-    radius: float
-
-
-class SDMR():
-    """
-    This class calculates the shortest distance matrix and creates a completed (grown) structure by crystal symmetry.
-    """
-
-    def __init__(self, shx: 'Shelxfile'):
-        self.shx = shx
-        # self.sdm_list: list[SDMItem]
-        self.all_atoms = self.get_atoms()
-        self.sdm_list = []  # list of sdmitems
-        self.maxmol: int = 1
-        self.cell = (
-            self.shx.cell.a, self.shx.cell.b, self.shx.cell.c, self.shx.cell.alpha, self.shx.cell.beta, self.shx.cell.gamma)
-        self.aga = self.shx.cell.a * self.shx.cell.b * self.shx.cell.cosga
-        self.bbe = self.shx.cell.a * self.shx.cell.c * self.shx.cell.cosbe
-        self.cal = self.shx.cell.b * self.shx.cell.c * self.shx.cell.cosal
-        self.maxmol = 1
-        self.sdmtime = 0
-        self.bondlist = []
-        self.asq = self.shx.cell[0] ** 2
-        self.bsq = self.shx.cell[1] ** 2
-        self.csq = self.shx.cell[2] ** 2
-        # calculate reciprocal lattice vectors:
-        self.astar = (self.shx.cell.b * self.shx.cell.c * sin(radians(self.shx.cell.alpha))) / self.shx.cell.V
-        self.bstar = (self.shx.cell.c * self.shx.cell.a * sin(radians(self.shx.cell.beta))) / self.shx.cell.V
-        self.cstar = (self.shx.cell.a * self.shx.cell.b * sin(radians(self.shx.cell.gamma))) / self.shx.cell.V
-
-    def get_atoms(self) -> tuple[Union[RAtom, RAtom], ...]:
-        atoms = []
-        for atom in self.shx.atoms:
-            atoms.append(
-                RAtom(name=atom.name, x=atom.x, y=atom.y, z=atom.z, element=atom.element, part=atom.part.n,
-                      symmgen=False, molindex=0, qpeak=atom.qpeak, radius=atom.radius))
-        return tuple(atoms)
-
-    def calc_sdm(self) -> list:
-        t1 = time.perf_counter()
-        symms = self.shx.symmcards._symmcards
-        self.sdm_list = calc_sdm(self.all_atoms, symms, self.shx.cell)
-        self.sdm_list.sort()
-        t2 = time.perf_counter()
-        print('Zeit für sdm:', round(t2 - t1, 3), 's')
-        self.sdmtime = t2 - t1
-        self.calc_molindex(self.shx.atoms.all_atoms)
-        need_symm = self.collect_needed_symmetry(self.shx.atoms.all_atoms)
-        if DEBUG:
-            print("The asymmetric unit contains {} fragments.".format(self.maxmol))
-        return need_symm
-
-    def collect_needed_symmetry(self, all_atoms) -> list:
-        need_symm = []
-        # Collect needsymm list:
-        for sdm_item in self.sdm_list:
-            if sdm_item.covalent:
-                at1: Atom = all_atoms[sdm_item.a1]
-                at2: Atom = all_atoms[sdm_item.a2]
-                if at1.molindex < 1 or at1.molindex > 6:
-                    continue
-                prime_array = [Array(at1.frac_coords) * symop.matrix + symop.trans for symop in self.shx.symmcards]
-                for n, symop in enumerate(self.shx.symmcards):
-                    if at1.part != 0 and at2.part != 0 and at1.part != at2.part:
-                        # both not part 0 and different part numbers
-                        continue
-                    # Both the same atomic number and number hydrogen:
-                    if at1.element == at2.element and at1.is_hydrogen:
-                        continue
-                    D = prime_array[n] - Array([at2.x, at2.y, at2.z]) + Array((0.5, 0.5, 0.5))
-                    floor_d = D.floor
-                    if n == 0 and D.floor.values == (0, 0, 0):
-                        continue
-                    dp = D - floor_d - Array((0.5, 0.5, 0.5))
-                    dk = self.vector_length(*dp)
-                    dddd = sdm_item.dist + 0.2
-                    if at1.is_hydrogen and at2.is_hydrogen:
-                        dddd = 1.8
-                    if (dk > 0.001) and (dddd >= dk):
-                        bs = [n + 1, (5 - floor_d[0]), (5 - floor_d[1]), (5 - floor_d[2]), at1.molindex]
-                        if bs not in need_symm:
-                            need_symm.append(bs)
-        return need_symm
-
-    def calc_molindex(self, all_atoms):
-        # Start for George's "bring atoms together algorithm":
-        someleft = 1
-        nextmol = 1
-        for at in all_atoms:
-            at.molindex = -1
-        all_atoms[0].molindex = 1
-        while nextmol:
-            someleft = 1
-            nextmol = 0
-            while someleft:
-                someleft = 0
-                for sdm_item in self.sdm_list:
-                    at1: Atom = all_atoms[sdm_item.a1]
-                    at2: Atom = all_atoms[sdm_item.a2]
-                    if sdm_item.covalent and at1.molindex * at2.molindex < 0:
-                        at1.molindex = self.maxmol
-                        at2.molindex = self.maxmol
-                        someleft += 1
-            for ni, at in enumerate(all_atoms):
-                if not at.is_hydrogen and at.molindex < 0:
-                    nextmol = ni
-                    break
-            if nextmol:
-                self.maxmol += 1
-                all_atoms[nextmol].molindex = self.maxmol
-
-    def vector_length(self, x: float, y: float, z: float) -> float:
-        """
-        Calculates the vector length given in fractional coordinates.
-        """
-        A = 2.0 * (x * y * self.aga + x * z * self.bbe + y * z * self.cal)
-        return sqrt(x ** 2 * self.asq + y ** 2 * self.bsq + z ** 2 * self.csq + A)
-
-    def packer(self, sdm: 'SDMR', need_symm: list, with_qpeaks=False):
-        """
-        Packs atoms of the asymmetric unit to real molecules.
-        """
-        asymm = self.shx.atoms.all_atoms
-        if with_qpeaks:
-            showatoms = asymm[:]
-        else:
-            showatoms = [at for at in asymm if not at.qpeak]
-        for symm in need_symm:
-            symm_num, h, k, l, symmgroup = symm
-            h -= 5
-            k -= 5
-            l -= 5
-            symm_num -= 1
-            for atom in asymm:
-                if not with_qpeaks and atom.qpeak:
-                    continue
-                # Essential to have hydrogen atoms grown:
-                # if not atom.ishydrogen and atom.molindex == symmgroup:
-                if atom.molindex == symmgroup:
-                    new_atom = Atom(self.shx)
-                    if atom.qpeak:
-                        continue
-                    else:
-                        uvals = atom.uvals
-                        # TODO: Transform u values according to symmetry:
-                        # currently, the adps are directed in wrong directions after after applying symmetry to atoms.
-                        # uvals = self.transform_uvalues(uvals, symm_num)
-                    new_atom.set_atom_parameters(
-                        name=atom.name[:3] + ">>" + str(symm_num) + '_' + ascii_letters[atom.part.n],
-                        sfac_num=atom.sfac_num,
-                        coords=Array(atom.frac_coords) * self.shx.symmcards[symm_num].matrix
-                               + Array(self.shx.symmcards[symm_num].trans) + Array([h, k, l]),
-                        part=atom.part,
-                        afix=AFIX(self.shx, (atom.afix).split()) if atom.afix else None,
-                        resi=RESI(self.shx, ('RESI ' + str(atom.resinum) + atom.resiclass).split()) if atom.resi else None,
-                        site_occupation=atom.sof,
-                        uvals=uvals,
-                        symmgen=True
-                    )
-                    isthere = False
-                    if new_atom.part.n >= 0:
-                        for atom in showatoms:
-                            if atom.part.n != new_atom.part.n:
-                                continue
-                            length = sdm.vector_length(new_atom.x - atom.x, new_atom.y - atom.y, new_atom.z - atom.z)
-                            if length < 0.2:
-                                isthere = True
-                    if not isthere:
-                        showatoms.append(new_atom)
-        return showatoms
-
-    def transform_uvalues(self, uvals: (list, tuple), symm_num: int):
-        """
-        Transforms the Uij values according to local symmetry.
-        R. W. Grosse-Kunstleve, P. D. Adams (2002). J. Appl. Cryst. 35, 477–480.
-        http://dx.doi.org/10.1107/S0021889802008580
-
-        U(star) = N * U(cif) * N.T
-        U(star) = R * U(star) * R^t
-        U(cif) = N^-1 * U(star) * (N^-1).T
-
-        U(cart) = A * U(star) * A.T
-        U(frac) = A^1 * U(cart) * (A^1).t
-        U(star) = A^-1 * U(cart) * A^-1.t
-
-        R is the rotation part of a given symmetry operation
-
-        [ [U11, U12, U13]
-          [U12, U22, U23]
-          [U13, U23, U33]
-        ]
-        # Shelxl uses U* with a*,b*c*-parameterization
-        atomname sfac x y z sof[11] U[0.05] or U11 U22 U33 U23 U13 U12
-
-        Read:
-        X-Ray Analysis and the Structure of Organic Molecules Second Edition, Dunitz, P240
-
-        """
-        U11, U22, U33, U23, U13, U12 = uvals
-        U21 = U12
-        U32 = U23
-        U31 = U13
-        Ucif = Matrix([[U11, U12, U13], [U21, U22, U23], [U31, U32, U33]])
-        # matrix with the reciprocal lattice vectors:
-        N = Matrix([[self.astar, 0, 0],
-                    [0, self.bstar, 0],
-                    [0, 0, self.cstar]])
-        R = self.shx.symmcards[symm_num].matrix
-        R_t = self.shx.symmcards[symm_num].matrix.transposed
-        A = self.shx.orthogonal_matrix
-        # U(star) = N * U(cif) * N.T
-        # U(cart) = A * U(star) * A.T
-        # U(star) = R * U(star) * R^t
-        # U(cif) = N^-1 * U(star) * (N^-1).T
-        # U(star) = A^-1 * U(cart) * A^-1.T
-        Ustar = N * Ucif * N.T
-        Ustar = R * Ustar * R_t
-        Ucif = N.inversed * Ustar * N.inversed.T
-        uvals = Ucif
-        upper_diagonal = uvals.values[0][0], uvals.values[1][1], uvals.values[2][2], \
-                         uvals.values[1][2], uvals.values[0][2], \
-                         uvals.values[0][1]
-        return upper_diagonal
-
-
-def ufrac_to_ucart(A, cell, uvals):
-    """
-    #>>> uvals = [0.07243, 0.03058, 0.03216, -0.01057, -0.01708, 0.03014]
-    #>>> Ucart = Matrix([[ 0.0754483395556807,  0.030981701122469,  -0.0194466522033868], [  0.030981701122469,  0.03058, -0.01057], [-0.0194466522033868, -0.01057, 0.03216] ])
-    #>>> cell = (10.5086, 20.9035, 20.5072, 90, 94.13, 90)
-    #>>> from shelxfile.dsrmath import OrthogonalMatrix
-    #>>> A = OrthogonalMatrix(*cell)
-    #>>> ufrac_to_ucart(A, cell, uvals)
-    #TODO: test if this is right:
-    | 0.0740  0.0310 -0.0299|
-    | 0.0302  0.0306 -0.0148|
-    |-0.0171 -0.0106  0.0346|
-    <BLANKLINE>
-    """
-    U11, U22, U33, U23, U13, U12 = uvals
-    U21 = U12
-    U32 = U23
-    U31 = U13
-    Uij = Matrix([[U11, U12, U13], [U21, U22, U23], [U31, U32, U33]])
-    a, b, c, alpha, beta, gamma = cell
-    V = vol_unitcell(*cell)
-    # calculate reciprocal lattice vectors:
-    astar = (b * c * sin(radians(alpha))) / V
-    bstar = (c * a * sin(radians(beta))) / V
-    cstar = (a * b * sin(radians(gamma))) / V
-    # matrix with the reciprocal lattice vectors:
-    N = Matrix([[astar, 0, 0],
-                [0, bstar, 0],
-                [0, 0, cstar]])
-    # Finally transform Uij values from fractional to cartesian axis system:
-    Ucart = A * N * Uij * N.T * A.T
-    return Ucart
-
-
-if __name__ == "__main__":
-    from shelxfile.shelx.shelx import Shelxfile
-
-    shx = Shelxfile()
-    shx.read_file('shelxfile/tests/resources/p-31c.res')
-    t1 = time.perf_counter()
-    sdm = SDMR(shx)
-    needsymm = sdm.calc_sdm()
-    print('Zeit für sdm:', round(time.perf_counter() - t1, 3), 's')
-    print(needsymm)
-    packed_atoms = sdm.packer(sdm, needsymm)
-    print(len(shx.atoms))
-    print(len(packed_atoms))
-    assert str(packed_atoms[90]) == 'H2>>1_b 2   0.557744    0.080938   0.300634   21.00000   -1.30000'
-    assert str(packed_atoms[
-                   129]) == 'C15>>2_a  1    1.145639    0.497216    0.299794    11.00000    0.01803    0.01661      0.03458    0.00038   -0.00408    0.01187'
-    # [[1, 5, 5, 5, 4], [1, 5, 5, 5, 5], [2, 6, 5, 5, 5], [3, 6, 6, 5, 5], [1, 5, 5, 5, 3], [2, 6, 6, 5, 3],
-    # 88
-    # 208
-
+# -*- encoding: utf-8 -*-
+# möp
+#
+# ----------------------------------------------------------------------------
+# "THE BEER-WARE LICENSE" (Revision 42):
+# <dkratzert@gmx.de> wrote this file. As long as you retain
+# this notice you can do whatever you want with this stuff. If we meet some day,
+# and you think this stuff is worth it, you can buy me a beer in return.
+# Daniel Kratzert
+# ----------------------------------------------------------------------------
+#
+import time
+from dataclasses import dataclass
+from math import sqrt, radians, sin
+from string import ascii_letters
+from typing import Union
+
+# noinspection PyUnresolvedReferences
+from shelxfile.shelx.sdm_complete import calc_sdm
+
+from shelxfile.atoms.atom import Atom
+from shelxfile.misc.dsrmath import Array, Matrix, vol_unitcell
+from shelxfile.misc.misc import DEBUG
+from shelxfile.shelx.cards import AFIX, RESI
+
+
+@dataclass
+class RAtom:
+    name: str
+    x: float
+    y: float
+    z: float
+    element: str
+    part: int
+    symmgen: bool
+    molindex: int
+    qpeak: bool
+    radius: float
+
+
+class SDMR():
+    """
+    This class calculates the shortest distance matrix and creates a completed (grown) structure by crystal symmetry.
+    """
+
+    def __init__(self, shx: 'Shelxfile'):
+        self.shx = shx
+        # self.sdm_list: list[SDMItem]
+        self.all_atoms = self.get_atoms()
+        self.sdm_list = []  # list of sdmitems
+        self.maxmol: int = 1
+        self.cell = (
+            self.shx.cell.a, self.shx.cell.b, self.shx.cell.c, self.shx.cell.alpha, self.shx.cell.beta, self.shx.cell.gamma)
+        self.aga = self.shx.cell.a * self.shx.cell.b * self.shx.cell.cosga
+        self.bbe = self.shx.cell.a * self.shx.cell.c * self.shx.cell.cosbe
+        self.cal = self.shx.cell.b * self.shx.cell.c * self.shx.cell.cosal
+        self.maxmol = 1
+        self.sdmtime = 0
+        self.bondlist = []
+        self.asq = self.shx.cell[0] ** 2
+        self.bsq = self.shx.cell[1] ** 2
+        self.csq = self.shx.cell[2] ** 2
+        # calculate reciprocal lattice vectors:
+        self.astar = (self.shx.cell.b * self.shx.cell.c * sin(radians(self.shx.cell.alpha))) / self.shx.cell.V
+        self.bstar = (self.shx.cell.c * self.shx.cell.a * sin(radians(self.shx.cell.beta))) / self.shx.cell.V
+        self.cstar = (self.shx.cell.a * self.shx.cell.b * sin(radians(self.shx.cell.gamma))) / self.shx.cell.V
+
+    def get_atoms(self) -> tuple[Union[RAtom, RAtom], ...]:
+        atoms = []
+        for atom in self.shx.atoms:
+            atoms.append(
+                RAtom(name=atom.name, x=atom.x, y=atom.y, z=atom.z, element=atom.element, part=atom.part.n,
+                      symmgen=False, molindex=0, qpeak=atom.qpeak, radius=atom.radius))
+        return tuple(atoms)
+
+    def calc_sdm(self) -> list:
+        t1 = time.perf_counter()
+        symms = self.shx.symmcards._symmcards
+        self.sdm_list = calc_sdm(self.all_atoms, symms, self.shx.cell)
+        self.sdm_list.sort()
+        t2 = time.perf_counter()
+        print('Zeit für sdm:', round(t2 - t1, 3), 's')
+        self.sdmtime = t2 - t1
+        self.calc_molindex(self.shx.atoms.all_atoms)
+        need_symm = self.collect_needed_symmetry(self.shx.atoms.all_atoms)
+        if DEBUG:
+            print("The asymmetric unit contains {} fragments.".format(self.maxmol))
+        return need_symm
+
+    def collect_needed_symmetry(self, all_atoms) -> list:
+        need_symm = []
+        # Collect needsymm list:
+        for sdm_item in self.sdm_list:
+            if sdm_item.covalent:
+                at1: Atom = all_atoms[sdm_item.a1]
+                at2: Atom = all_atoms[sdm_item.a2]
+                if at1.molindex < 1 or at1.molindex > 6:
+                    continue
+                prime_array = [Array(at1.frac_coords) * symop.matrix + symop.trans for symop in self.shx.symmcards]
+                for n, symop in enumerate(self.shx.symmcards):
+                    if at1.part != 0 and at2.part != 0 and at1.part != at2.part:
+                        # both not part 0 and different part numbers
+                        continue
+                    # Both the same atomic number and number hydrogen:
+                    if at1.element == at2.element and at1.is_hydrogen:
+                        continue
+                    D = prime_array[n] - Array([at2.x, at2.y, at2.z]) + Array((0.5, 0.5, 0.5))
+                    floor_d = D.floor
+                    if n == 0 and D.floor.values == (0, 0, 0):
+                        continue
+                    dp = D - floor_d - Array((0.5, 0.5, 0.5))
+                    dk = self.vector_length(*dp)
+                    dddd = sdm_item.dist + 0.2
+                    if at1.is_hydrogen and at2.is_hydrogen:
+                        dddd = 1.8
+                    if (dk > 0.001) and (dddd >= dk):
+                        bs = [n + 1, (5 - floor_d[0]), (5 - floor_d[1]), (5 - floor_d[2]), at1.molindex]
+                        if bs not in need_symm:
+                            need_symm.append(bs)
+        return need_symm
+
+    def calc_molindex(self, all_atoms):
+        # Start for George's "bring atoms together algorithm":
+        someleft = 1
+        nextmol = 1
+        for at in all_atoms:
+            at.molindex = -1
+        all_atoms[0].molindex = 1
+        while nextmol:
+            someleft = 1
+            nextmol = 0
+            while someleft:
+                someleft = 0
+                for sdm_item in self.sdm_list:
+                    at1: Atom = all_atoms[sdm_item.a1]
+                    at2: Atom = all_atoms[sdm_item.a2]
+                    if sdm_item.covalent and at1.molindex * at2.molindex < 0:
+                        at1.molindex = self.maxmol
+                        at2.molindex = self.maxmol
+                        someleft += 1
+            for ni, at in enumerate(all_atoms):
+                if not at.is_hydrogen and at.molindex < 0:
+                    nextmol = ni
+                    break
+            if nextmol:
+                self.maxmol += 1
+                all_atoms[nextmol].molindex = self.maxmol
+
+    def vector_length(self, x: float, y: float, z: float) -> float:
+        """
+        Calculates the vector length given in fractional coordinates.
+        """
+        A = 2.0 * (x * y * self.aga + x * z * self.bbe + y * z * self.cal)
+        return sqrt(x ** 2 * self.asq + y ** 2 * self.bsq + z ** 2 * self.csq + A)
+
+    def packer(self, sdm: 'SDMR', need_symm: list, with_qpeaks=False):
+        """
+        Packs atoms of the asymmetric unit to real molecules.
+        """
+        asymm = self.shx.atoms.all_atoms
+        if with_qpeaks:
+            showatoms = asymm[:]
+        else:
+            showatoms = [at for at in asymm if not at.qpeak]
+        for symm in need_symm:
+            symm_num, h, k, l, symmgroup = symm
+            h -= 5
+            k -= 5
+            l -= 5
+            symm_num -= 1
+            for atom in asymm:
+                if not with_qpeaks and atom.qpeak:
+                    continue
+                # Essential to have hydrogen atoms grown:
+                # if not atom.ishydrogen and atom.molindex == symmgroup:
+                if atom.molindex == symmgroup:
+                    new_atom = Atom(self.shx)
+                    if atom.qpeak:
+                        continue
+                    else:
+                        uvals = atom.uvals
+                        # TODO: Transform u values according to symmetry:
+                        # currently, the adps are directed in wrong directions after after applying symmetry to atoms.
+                        # uvals = self.transform_uvalues(uvals, symm_num)
+                    new_atom.set_atom_parameters(
+                        name=atom.name[:3] + ">>" + str(symm_num) + '_' + ascii_letters[atom.part.n],
+                        sfac_num=atom.sfac_num,
+                        coords=Array(atom.frac_coords) * self.shx.symmcards[symm_num].matrix
+                               + Array(self.shx.symmcards[symm_num].trans) + Array([h, k, l]),
+                        part=atom.part,
+                        afix=AFIX(self.shx, (atom.afix).split()) if atom.afix else None,
+                        resi=RESI(self.shx, ('RESI ' + str(atom.resinum) + atom.resiclass).split()) if atom.resi else None,
+                        site_occupation=atom.sof,
+                        uvals=uvals,
+                        symmgen=True
+                    )
+                    isthere = False
+                    if new_atom.part.n >= 0:
+                        for atom in showatoms:
+                            if atom.part.n != new_atom.part.n:
+                                continue
+                            length = sdm.vector_length(new_atom.x - atom.x, new_atom.y - atom.y, new_atom.z - atom.z)
+                            if length < 0.2:
+                                isthere = True
+                    if not isthere:
+                        showatoms.append(new_atom)
+        return showatoms
+
+    def transform_uvalues(self, uvals: (list, tuple), symm_num: int):
+        """
+        Transforms the Uij values according to local symmetry.
+        R. W. Grosse-Kunstleve, P. D. Adams (2002). J. Appl. Cryst. 35, 477–480.
+        http://dx.doi.org/10.1107/S0021889802008580
+
+        U(star) = N * U(cif) * N.T
+        U(star) = R * U(star) * R^t
+        U(cif) = N^-1 * U(star) * (N^-1).T
+
+        U(cart) = A * U(star) * A.T
+        U(frac) = A^1 * U(cart) * (A^1).t
+        U(star) = A^-1 * U(cart) * A^-1.t
+
+        R is the rotation part of a given symmetry operation
+
+        [ [U11, U12, U13]
+          [U12, U22, U23]
+          [U13, U23, U33]
+        ]
+        # Shelxl uses U* with a*,b*c*-parameterization
+        atomname sfac x y z sof[11] U[0.05] or U11 U22 U33 U23 U13 U12
+
+        Read:
+        X-Ray Analysis and the Structure of Organic Molecules Second Edition, Dunitz, P240
+
+        """
+        U11, U22, U33, U23, U13, U12 = uvals
+        U21 = U12
+        U32 = U23
+        U31 = U13
+        Ucif = Matrix([[U11, U12, U13], [U21, U22, U23], [U31, U32, U33]])
+        # matrix with the reciprocal lattice vectors:
+        N = Matrix([[self.astar, 0, 0],
+                    [0, self.bstar, 0],
+                    [0, 0, self.cstar]])
+        R = self.shx.symmcards[symm_num].matrix
+        R_t = self.shx.symmcards[symm_num].matrix.transposed
+        A = self.shx.orthogonal_matrix
+        # U(star) = N * U(cif) * N.T
+        # U(cart) = A * U(star) * A.T
+        # U(star) = R * U(star) * R^t
+        # U(cif) = N^-1 * U(star) * (N^-1).T
+        # U(star) = A^-1 * U(cart) * A^-1.T
+        Ustar = N * Ucif * N.T
+        Ustar = R * Ustar * R_t
+        Ucif = N.inversed * Ustar * N.inversed.T
+        uvals = Ucif
+        upper_diagonal = uvals.values[0][0], uvals.values[1][1], uvals.values[2][2], \
+                         uvals.values[1][2], uvals.values[0][2], \
+                         uvals.values[0][1]
+        return upper_diagonal
+
+
+def ufrac_to_ucart(A, cell, uvals):
+    """
+    #>>> uvals = [0.07243, 0.03058, 0.03216, -0.01057, -0.01708, 0.03014]
+    #>>> Ucart = Matrix([[ 0.0754483395556807,  0.030981701122469,  -0.0194466522033868], [  0.030981701122469,  0.03058, -0.01057], [-0.0194466522033868, -0.01057, 0.03216] ])
+    #>>> cell = (10.5086, 20.9035, 20.5072, 90, 94.13, 90)
+    #>>> from shelxfile.dsrmath import OrthogonalMatrix
+    #>>> A = OrthogonalMatrix(*cell)
+    #>>> ufrac_to_ucart(A, cell, uvals)
+    #TODO: test if this is right:
+    | 0.0740  0.0310 -0.0299|
+    | 0.0302  0.0306 -0.0148|
+    |-0.0171 -0.0106  0.0346|
+    <BLANKLINE>
+    """
+    U11, U22, U33, U23, U13, U12 = uvals
+    U21 = U12
+    U32 = U23
+    U31 = U13
+    Uij = Matrix([[U11, U12, U13], [U21, U22, U23], [U31, U32, U33]])
+    a, b, c, alpha, beta, gamma = cell
+    V = vol_unitcell(*cell)
+    # calculate reciprocal lattice vectors:
+    astar = (b * c * sin(radians(alpha))) / V
+    bstar = (c * a * sin(radians(beta))) / V
+    cstar = (a * b * sin(radians(gamma))) / V
+    # matrix with the reciprocal lattice vectors:
+    N = Matrix([[astar, 0, 0],
+                [0, bstar, 0],
+                [0, 0, cstar]])
+    # Finally transform Uij values from fractional to cartesian axis system:
+    Ucart = A * N * Uij * N.T * A.T
+    return Ucart
+
+
+if __name__ == "__main__":
+    from shelxfile.shelx.shelx import Shelxfile
+
+    shx = Shelxfile()
+    shx.read_file('shelxfile/tests/resources/p-31c.res')
+    t1 = time.perf_counter()
+    sdm = SDMR(shx)
+    needsymm = sdm.calc_sdm()
+    print('Zeit für sdm:', round(time.perf_counter() - t1, 3), 's')
+    print(needsymm)
+    packed_atoms = sdm.packer(sdm, needsymm)
+    print(len(shx.atoms))
+    print(len(packed_atoms))
+    assert str(packed_atoms[90]) == 'H2>>1_b 2   0.557744    0.080938   0.300634   21.00000   -1.30000'
+    assert str(packed_atoms[
+                   129]) == 'C15>>2_a  1    1.145639    0.497216    0.299794    11.00000    0.01803    0.01661      0.03458    0.00038   -0.00408    0.01187'
+    # [[1, 5, 5, 5, 4], [1, 5, 5, 5, 5], [2, 6, 5, 5, 5], [3, 6, 6, 5, 5], [1, 5, 5, 5, 3], [2, 6, 6, 5, 3],
+    # 88
+    # 208
+
```

### Comparing `shelxfile-8/shelxfile/shelx/shelx.py` & `shelxfile-9/shelxfile/shelx/shelx.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,1087 +1,1088 @@
-# -*- encoding: utf-8 -*-
-# möpß
-#
-# ----------------------------------------------------------------------------
-# "THE BEER-WARE LICENSE" (Revision 42):
-# <dkratzert@gmx.de> wrote this file. As long as you retain
-# this notice you can do whatever you want with this stuff. If we meet some day,
-# and you think this stuff is worth it, you can buy me a beer in return.
-# Daniel Kratzert
-# ----------------------------------------------------------------------------
-#
-from pathlib import Path
-from typing import Union, List
-
-from shelxfile.atoms.atom import Atom
-from shelxfile.atoms.atoms import Atoms
-from shelxfile.refine.refine import ShelxlRefine
-from shelxfile.shelx.sdm import SDM
-
-__doc__ = """
-This is a full implementation of the SHELXL file syntax. Additionally it is able to edit SHELX properties with Python.
-The implementation is Python3-only and supports SHELXL after 2017 (You should not use old versions anyway).
-
-The parser is quiet about the most errors unless you enable DEBUG in misc.py. The parser will try to read the 
-SHELX file even if it has syntax errors, but if for example, the SFAC and UNIT instruction is not consistent 
-it will fail. 
-"""
-
-import os
-import re
-import sys
-
-from shelxfile.shelx.cards import ACTA, FVAR, FVARs, REM, BOND, Restraints, DEFS, NCSY, ISOR, FLAT, \
-    BUMP, DFIX, DANG, SADI, SAME, RIGU, SIMU, DELU, CHIV, EADP, EXYZ, DAMP, HFIX, HKLF, SUMP, SYMM, LSCycles, \
-    SFACTable, UNIT, BASF, TWIN, WGHT, BLOC, SymmCards, CONN, CONF, BIND, DISP, GRID, HTAB, MERG, FRAG, FREE, FMAP, \
-    MOVE, PLAN, PRIG, RTAB, SHEL, SIZE, SPEC, STIR, TWST, WIGL, WPDB, XNPD, ZERR, CELL, LATT, MORE, MPLA, AFIX, PART, \
-    RESI, ABIN, ANIS, Residues
-from shelxfile.misc.dsrmath import Array, OrthogonalMatrix
-from shelxfile.misc.misc import DEBUG, ParseOrderError, ParseNumError, ParseUnknownParam, \
-    multiline_test, dsr_regex, wrap_line, ParseSyntaxError
-
-"""
-TODO:
-- Handle BEDE & LONE plus their results
-- Rotate ellipsoids with kabsch
-- kallall.Q, killall.C 
-- Q-peak printing is wrong: Q1    1   0.9828    1.1159    0.3148   11.00000  0.04      0.00  
-- Write out parts and afix in grow mode
-- Delete atoms (H) in AFIX -> delete entire afix group
-- Is backup file and reccovery from failed refinement working?
-- check if atoms in restraints are also in structure
-- restraints involved with an atom should also be part of the atoms properties
-------------------------------------------------------------
-- deleting atoms should also remove them from restraints
-- add remove_hydrogen_atoms(atom) method.
-- shx.remove_all_H([list of atoms], or all)
-- bond list
-- implement an add_afix(afixm, afixn, atoms, frag_fend=False, position=None, afix_options=None)
-  default position is directly behind FVAR or FRAG/FEND if enabled
-- will read in lst file after refinement to fill shx.lst_file properties.
-- shx.move_in_part([list of atoms])
-- shx.move_in_resi([list of atoms])
-- shx.sort.residue(3) (low priority)
-- shx.lst_file.residuals -> density, r-values, goof, movements, bad reflections
-   bad restraints, shelx *** errors
-- shx.unused_atom_name('C') -> get a carbon atom with unused number
-- shx.sort -> sort file (low priority)
-"""
-
-SHX_CARDS = ('TITL', 'CELL', 'ZERR', 'LATT', 'SYMM', 'SFAC', 'UNIT', 'LIST', 'L.S.', 'CGLS',
-             'BOND', 'FMAP', 'PLAN', 'TEMP', 'ACTA', 'CONF', 'SIMU', 'RIGU', 'WGHT', 'FVAR',
-             'DELU', 'SAME', 'DISP', 'LAUE', 'REM ', 'MORE', 'TIME', 'END ', 'HKLF', 'OMIT',
-             'SHEL', 'BASF', 'TWIN', 'EXTI', 'SWAT', 'HOPE', 'MERG', 'SPEC', 'RESI', 'MOVE',
-             'ANIS', 'AFIX', 'HFIX', 'FRAG', 'FEND', 'EXYZ', 'EADP', 'EQIV', 'CONN', 'BIND',
-             'FREE', 'DFIX', 'BUMP', 'SADI', 'CHIV', 'FLAT', 'DEFS', 'ISOR', 'NCSY', 'SUMP',
-             'BLOC', 'DAMP', 'STIR', 'MPLA', 'RTAB', 'HTAB', 'SIZE', 'WPDB', 'GRID', 'MOLE',
-             'XNPD', 'REST', 'CHAN', 'FLAP', 'RNUM', 'SOCC', 'PRIG', 'WIGL', 'RANG', 'TANG',
-             'ADDA', 'STAG', 'NEUT', 'ABIN', 'ANSC', 'ANSR', 'NOTR', 'TWST', 'PART', 'DANG',
-             'BEDE', 'LONE', 'REM', 'END')
-
-
-class Shelxfile():
-    """
-    Class for data from a SHELXL res file. Includes Atoms, cards and unit cell.
-
-    :type restraints: List[Restraint]
-    """
-    _r1_regex = re.compile(r'^REM\s+R1\s+=', re.IGNORECASE)
-    _wr2_regex = re.compile(r'^REM\s+wR2\s+=', re.IGNORECASE)
-    _parameters_regex = re.compile(r'^REM\s+\d+\s+parameters\s+refined', re.IGNORECASE)
-    _diff_peak_regex = re.compile(r'^REM\sHighest\sdifference', re.IGNORECASE)
-    _goof_regex = re.compile(r'^REM\swR2\s=\s.*,\sGooF', re.IGNORECASE)
-    _spgrp_regex = re.compile(r'^REM\s+\S+\s+in\s+\S+', re.IGNORECASE)
-
-    def __init__(self):
-        """
-        Reads the shelx file and extracts information.
-
-        :param resfile: file path
-        """
-        self.temp_in_kelvin = 0.0
-        self.shelx_max_line_length = 79  # maximum character lenth per line in SHELXL
-        self.nohkl = False
-        self._a, self._b, self._c, self._alpha, self._beta, self._gamma, self.V = \
-            None, None, None, None, None, None, None
-        self.cell: Union[CELL, None] = None
-        self.ansc: List[float] = []
-        self.abin: Union[None, ABIN] = None
-        self.acta: Union[None, ACTA] = None
-        self.fmap: Union[None, FMAP] = None
-        self.xnpd: Union[None, XNPD] = None
-        self.wpdb: Union[None, WPDB] = None
-        self.wigl: Union[None, WIGL] = None
-        self.temp: Union[int, float] = 20
-        # TODO: Implement swat class:
-        self.swat = None
-        self.stir: Union[None, STIR] = None
-        self.spec: Union[None, SPEC] = None
-        self.twst: Union[None, TWST] = None
-        self.plan: Union[None, PLAN] = None
-        self.prig: Union[None, PRIG] = None
-        self.merg: Union[None, MERG] = None
-        self.more: Union[None, MORE] = None
-        self.move: Union[None, MOVE] = None
-        self.defs: Union[None, DEFS] = None
-        self.zerr: Union[None, ZERR] = None
-        self.wght: Union[None, WGHT] = None
-        self.frag: Union[None, FRAG] = None
-        self.twin: Union[None, TWIN] = None
-        self.basf: Union[None, BASF] = None
-        self.latt: Union[None, LATT] = None
-        self.anis: Union[None, ANIS] = None
-        self.damp: Union[None, DAMP] = None
-        self.unit: Union[None, UNIT] = None
-        self.size: Union[None, SIZE] = None
-        self.htab: Union[None, HTAB] = None
-        self.shel: Union[None, SHEL] = None
-        self.mpla: Union[None, MPLA] = None
-        self.hklf: Union[None, HKLF] = None
-        self.grid: Union[None, GRID] = None
-        self.conn: Union[None, CONN] = None
-        self.conf: Union[None, CONF] = None
-        self.afix: Union[AFIX, None] = None
-        self.rtab: List[RTAB] = []
-        self.omit: List[str] = []
-        self.free: List[FREE] = []
-        self.eqiv: List[str] = []
-        self.bonds: List[BOND] = []
-        self.disp: List[BOND] = []
-        self.bind: List[BIND] = []
-        self.bloc: List[BLOC] = []
-        self.part: PART = PART(self, ['PART', '0'])
-        self.resi: RESI = RESI(self, ['RESI', '0'])
-        self.residues = Residues(self)
-        self.dsrlines: List[str] = []
-        self.dsrline_nums: List[int] = []
-        self.symmcards: SymmCards = SymmCards(self)
-        self.hfixes: List[HFIX] = []
-        self.sump: List[SUMP] = []
-        self.wght_suggested: Union[None, WGHT] = None
-        self.Z: int = 1
-        self.titl = ""
-        self.exti: float = 0.0
-        self.ansr: float = 0.001
-        self.rem: List[REM] = []
-        self.atoms: Atoms = Atoms(self)
-        self.fvars: FVARs = FVARs(self)
-        self.restraints: Restraints = Restraints()
-        self.sfac_table: SFACTable = SFACTable(self)
-        self.cycles: Union[None, LSCycles] = None
-        self.R1: Union[None, float] = None
-        self.wr2: Union[None, float] = None
-        self.goof: Union[None, float] = None
-        self.rgoof: Union[None, float] = None
-        self.space_group: Union[None, str] = None
-        self.data: Union[None, int] = None
-        self.parameters: Union[None, int] = None
-        self.dat_to_param: Union[None, float] = None
-        self.num_restraints: Union[None, int] = None
-        self.highest_peak: Union[None, float] = None
-        self.deepest_hole: Union[None, float] = None
-        self.end: bool = False
-        self.maxsof: float = 1.0
-        self.delete_on_write: set = set()
-        self.wavelen: float = 0.0
-        self.global_sadi: Union[None, int] = None
-        self.list: int = 0
-        self.theta_full: float = 0.0
-        self.error_line_num: int = -1  # Only used to tell the line number during an exception.
-        self.resfile: Union[Path, None] = None
-        self._reslist: List = []
-
-    def write_shelx_file(self, filename=None, verbose=False) -> None:
-        if not filename:
-            filename = self.resfile
-        with open(filename, 'w') as f:
-            for num, line in enumerate(self._reslist):
-                if num in self.delete_on_write:
-                    if DEBUG:
-                        # print('Deleted line {}'.format(num + 1))
-                        pass
-                    continue
-                if line == '':  # and self._reslist[num + 1] == '':
-                    continue
-                # Prevent wrapping long lines with \n breaks by splitting first:
-                line = "\n".join([wrap_line(x) for x in str(line).split("\n")])
-                f.write(str(line) + '\n')
-        if verbose or DEBUG:
-            print('File successfully written to {}'.format(os.path.abspath(filename)))
-
-    def read_file(self, resfile: Union[Path, str]) -> None:
-        """
-        Read input from a file path.
-        """
-        if isinstance(resfile, str):
-            resfile = Path(resfile)
-        self.resfile = resfile.resolve()
-        if DEBUG:
-            print('Resfile is:', resfile)
-        try:
-            self._reslist: List = resfile.read_text().splitlines(keepends=False)
-            self._test_if_file_is_valid(resfile)
-        except UnicodeDecodeError:
-            if DEBUG:
-                print('*** Unable to read file', resfile, '***')
-            return
-        self._find_included_files()
-        self.parse_cards()
-
-    def read_string(self, resfile_string: str):
-        """
-        Read input as string.
-        This will not read files included with "+filename" syntax!
-        """
-        self._reslist = resfile_string.splitlines(keepends=False)
-        self.parse_cards()
-
-    def parse_cards(self):
-        try:
-            self._parse_cards()
-        except Exception as e:
-            if DEBUG:
-                self.show_line_where_error_occured(e)
-                raise
-            else:
-                return
-
-    def _test_if_file_is_valid(self, resfile):
-        if len(self._reslist) < 20 and DEBUG:
-            print('*** Not a SHELXL file: {} ***'.format(resfile))
-            sys.exit()
-
-    def show_line_where_error_occured(self, e):
-        try:
-            print('Error near:\n', self._reslist[self.error_line_num])
-        except IndexError:
-            pass
-        print(e)
-        print("*** Syntax error found in file {}, line {} ***".format(self.resfile, self.error_line_num + 1))
-
-    def _find_included_files(self):
-        # Tracks the file names of included files in order to find recursive inclusion:
-        includefiles = []
-        for line_num, line in enumerate(self._reslist):
-            if line.startswith('+'):
-                try:
-                    file_included_in_includefile = self._read_included_file(includefiles, line)
-                    if file_included_in_includefile:
-                        for line_num_includefile, l in enumerate(file_included_in_includefile):
-                            reslist_position = line_num + 1 + line_num_includefile
-                            # '+filename' include files are not copied to res file,
-                            #  so I have to delete these lines on write.
-                            # '++filename' copies them to the .res file where appropriate
-                            # I leave this out, because I am not SHELXL:
-                            # if l.startswith('+') and l[:2] != '++':
-                            #    self.delete_on_write.update([lnum])
-                            self._reslist.insert(reslist_position, l)
-                        continue
-                except IndexError:
-                    if DEBUG:
-                        print('*** CANNOT READ INCLUDE FILE {} ***'.format(line))
-                    # Not sure if this is a good idea: del reslist[n]
-
-    def _read_included_file(self, includefiles: List[str], line: str):
-        include_filename: Path = self.resfile.resolve().parent.joinpath(line[1:])
-        # Detect recursive file inclusion:
-        if include_filename.name in includefiles:
-            raise ValueError('*** Recoursive include files detected! ***')
-        includefiles.append(include_filename.name)
-        try:
-            newfile = include_filename.read_text().splitlines(keepends=False)
-        except IOError as e:
-            if DEBUG:
-                print(e)
-                print('*** CANNOT OPEN NESTED INPUT FILE {} ***'.format(include_filename))
-            return []
-        return newfile
-
-    def reload(self):
-        """
-        Reloads the shelx file and parses it again.
-        """
-        if DEBUG:
-            print('loading file:', self.resfile)
-        self.read_file(self.resfile.resolve())
-
-    def _parse_cards(self):
-        lastcard = ''
-        fvarnum = 1
-        for line_num, line in enumerate(self._reslist):
-            self.error_line_num = line_num  # For exception during parsing.
-            list_of_lines = [line_num]  # list of lines where a card appears, e.g. for atoms with two lines
-            if line[:1] == ' ' or line == '':
-                continue
-            if not self.titl and line[:4] == 'TITL':
-                # TITL[]  ->  = and ! can be part of the TITL!
-                self.titl = line[5:76]
-                lastcard = 'TITL'
-                continue
-            wrapindex = 0
-            # This while loop makes wrapped lines look like they are not wrapped. The following lines are then
-            # beginning with a space character and thus are ignored. The 'lines' list holds the line nnumbers where
-            # 'line' is located ([line_num]) plus the wrapped lines.
-            if multiline_test(self._reslist[line_num]):
-                multiline = True
-            else:
-                multiline = False
-            while multiline:
-                # Glue together the two lines wrapped with "=":
-                wrapindex += 1
-                line = line.rpartition('=')[0] + self._reslist[line_num + wrapindex]
-                # self.delete_on_write.update([line_num + wrapindex])
-                list_of_lines.append(line_num + wrapindex)  # list containing the lines of a multiline command
-                # Do not activate this, otherwise, the unwrapping stops after two lines.
-                if multiline_test(self._reslist[line_num + wrapindex]):
-                    multiline = True
-                else:
-                    multiline = False
-                self._reslist[line_num + wrapindex] = ''
-            # The current line splitted:
-            spline = line.split('!')[0].split()  # Ignore comments with "!", see how this performes
-            # The current line as string:
-            line = line.upper().split('!')[0]  # Ignore comments with "!", see how this performes
-            word = line[:4]
-            # get RESI:
-            if line.startswith(('END', 'HKLF')) and self.resi:
-                self.resi.num = 0
-                if DEBUG:
-                    print('RESI in line {} was not closed'.format(line_num + 1))
-                # Do not continue here, otherwise HKLF is not parsed
-                # continue
-            if line.startswith('RESI'):
-                self.resi = RESI(self, spline)
-                self.assign_card(self.resi, line_num)
-                if self.resi.residue_number > 0:
-                    self.residues.append(self.resi)
-                continue
-            # Now collect the PART:
-            if line.startswith(('END', 'HKLF')) and self.part:
-                self.part.n = 0
-                if DEBUG:
-                    print('PART in line {} was not closed'.format(line_num + 1))
-                # Do not continue here, otherwise HKLF is not parsed
-                # continue
-            if line.startswith('PART'):
-                self.part = PART(self, spline)
-                self.assign_card(self.part, line_num)
-                continue
-            # collect AFIX:
-            if line.startswith(('END', 'HKLF')) and self.afix:
-                self.afix.mn = 0
-                if DEBUG:
-                    print('AFIX in line {} was not closed'.format(line_num + 1))
-            elif line.startswith('AFIX'):
-                self.afix = AFIX(self, spline)
-                self.assign_card(self.afix, line_num)
-            elif self.is_atom(line):
-                # A SHELXL atom:
-                # F9    4    0.395366   0.177026   0.601546  21.00000   0.03231  ( 0.03248 =
-                #            0.03649  -0.00522  -0.01212   0.00157 )
-                a = Atom(self)
-                a.parse_line(spline, list_of_lines, part=self.part, afix=self.afix, resi=self.resi)
-                self.append_card(self.atoms, a, line_num)
-            elif word == 'SADI':
-                # SADI s[0.02] pairs of atoms
-                # or SADI
-                if len(spline) == 1:
-                    self.global_sadi = line_num
-                self.append_card(self.restraints, SADI(self, spline), line_num)
-            elif word == 'DFIX':
-                # DFIX d s[0.02] atom pairs
-                self.append_card(self.restraints, DFIX(self, spline), line_num)
-            elif word == 'SIMU':
-                # SIMU s[0.04] st[0.08] dmax[2.0] atomnames
-                self.append_card(self.restraints, SIMU(self, spline), line_num)
-            elif word == 'DELU':
-                # DELU s1[0.01] s2[0.01] atomnames
-                self.append_card(self.restraints, DELU(self, spline), line_num)
-            elif word == 'RIGU':
-                # RIGU s1[0.004] s2[0.004] atomnames
-                self.append_card(self.restraints, RIGU(self, spline), line_num)
-            elif word == 'BASF':
-                # BASF scale factors
-                self.assign_card(BASF(self, spline), line_num)
-            elif word == 'HFIX':
-                # HFIX mn U[#] d[#] atomnames
-                self.append_card(self.hfixes, HFIX(self, spline), line_num)
-            elif word == 'DANG':
-                # DANG d s[0.04] atom pairs
-                self.append_card(self.restraints, DANG(self, spline), line_num)
-            elif word == 'EADP':
-                self.append_card(self.restraints, EADP(self, spline), line_num)
-            elif line[:3] == 'REM':
-                if dsr_regex.match(line):
-                    self.dsrlines.append(" ".join(spline))
-                    self.dsrline_nums.extend(list_of_lines)
-                self.append_card(self.rem, REM(self, spline), line_num)
-                self._get_residuals(spline, line)
-            elif word == 'AFIX':
-                # nothing to do
-                pass
-            elif word == 'CELL':
-                # CELL λ a b c α β γ
-                if not lastcard == 'TITL' and DEBUG:
-                    print('TITL is missing.')
-                self.cell = CELL(self, spline)
-                self.assign_card(self.cell, line_num)
-                self._a, self._b, self._c, self._alpha, self._beta, self._gamma = self.cell
-                self.orthogonal_matrix = OrthogonalMatrix(*self.cell)
-                self.wavelen = self.cell.wavelen
-                lastcard = 'CELL'
-            elif word == "ZERR":
-                # ZERR Z esd(a) esd(b) esd(c) esd(α) esd(β) esd(γ)
-                if not lastcard == 'CELL':
-                    if DEBUG:
-                        print('*** Invalid SHELX file!')
-                    raise ParseOrderError
-                if not self.cell:
-                    raise ParseOrderError('*** Cell parameters missing! ***')
-                if len(spline) >= 8:
-                    self.zerr = ZERR(self, spline)
-                    self.Z = self.zerr.Z
-                    if self.Z < 1:
-                        self.Z = 1
-                        if DEBUG:
-                            print('Z value is zero.')
-                    self.assign_card(self.zerr, line_num)
-                lastcard = 'ZERR'
-            elif word == "LATT":
-                # LATT N[1]
-                # 1=P, 2=I, 3=rhombohedral obverse on hexagonal axes, 4=F, 5=A, 6=B, 7=C.
-                # negative is non-centrosymmetric
-                self.latt = LATT(self, spline)
-                self.assign_card(self.latt, line_num)
-                if not lastcard == 'ZERR' and DEBUG:
-                    print('*** ZERR instruction is missing! ***')
-                if self.latt.centric:
-                    self.symmcards.set_centric(True)
-            elif word == "SYMM":
-                # SYMM symmetry operation
-                #  Being more greedy, because many files do this wrong:
-                # if not lastcard == 'ZERR':
-                #    raise ParseOrderError
-                # if not self.zerr:
-                #    raise ParseOrderError
-                s = SYMM(self, spline)
-                if not self.latt and DEBUG:
-                    print("*** LATT instruction is missing! ***")
-                    raise ParseSyntaxError
-                # Have to do this after parsing, because P-1 has no SYMM!
-                # if self.latt.centric:
-                #    self.symmcards.set_centric(True)
-                self.symmcards.append(s.symmcard)
-                if s not in self._reslist:
-                    self._reslist[line_num] = s
-                else:
-                    self.delete_on_write.update([line_num])
-                    self._reslist[line_num] = ' '
-                lastcard = 'SYMM'
-            elif word == 'SFAC':
-                # SFAC elements or
-                # SFAC E a1 b1 a2 b2 a3 b3 a4 b4 c f' f" mu r wt
-                # Being less strict to be able to parse files without cell errors:
-                # if not (lastcard == 'LATT' or lastcard == 'ZERR'):
-                #    raise ParseOrderError
-                # if not self.symmcards:
-                #    raise ParseOrderError
-                if len(spline) <= 1:
-                    continue
-                self.sfac_table.parse_element_line(spline)
-                if self.sfac_table not in self._reslist:
-                    self._reslist[line_num] = self.sfac_table
-                else:
-                    self.delete_on_write.update([line_num])
-                    self._reslist[line_num] = ' '
-                lastcard = 'SFAC'
-            elif word == 'UNIT':
-                # UNIT n1 n2 ...
-                # Number of atoms of each type in the unit-cell, in SFAC order.
-                if not lastcard == 'SFAC':
-                    raise ParseOrderError
-                if self.sfac_table:
-                    try:
-                        self.unit = self.assign_card(UNIT(self, spline), line_num)
-                    except ValueError:
-                        if DEBUG:
-                            print('*** Non-numeric value in SFAC instruction! ***')
-                        raise
-                else:
-                    raise ParseOrderError
-                if len(self.unit.values) != len(self.sfac_table.elements_list) and DEBUG:
-                    print('*** Number of UNIT and SFAC values differ! ***')
-                    raise ParseNumError
-                lastcard = 'UNIT'
-            elif word in ['L.S.', 'CGLS']:
-                # CGLS nls[0] nrf[0] nextra[0]
-                # L.S. nls[0] nrf[0] nextra[0]
-                self.cycles = self.assign_card(LSCycles(self, spline), line_num)
-            elif word == "LIST":
-                # LIST m[#] mult[1] (mult is for list 4 only)
-                self.list = int(spline[1])
-            elif word == "FVAR":
-                # FVAR osf[1] free variables
-                for fvvalue in spline[1:]:
-                    fvarnum += 1
-                    self.append_card(self.fvars, FVAR(fvarnum, float(fvvalue)), line_num)
-                    if self.fvars not in self._reslist:
-                        self._reslist[line_num] = self.fvars
-                    else:
-                        self.delete_on_write.update([line_num])
-            elif word == 'ANIS':
-                # ANIS n or ANIS names
-                # Must be before Atom(), to know which atom is anis.
-                self.anis = ANIS(self, spline)
-                self.assign_card(self.anis, line_num)
-            elif word == 'WGHT':
-                # WGHT a[0.1] b[0] c[0] d[0] e[0] f[.33333]
-                if self.end:
-                    self.wght_suggested = self.assign_card(WGHT(self, spline), line_num)
-                    continue
-                self.wght = self.assign_card(WGHT(self, spline), line_num)
-            elif word == 'ACTA':
-                # ACTA 2θfull[#] -> optional parameter NOHKL
-                self.acta = ACTA(self, spline)
-                self.assign_card(self.acta, line_num)
-            elif word == 'DAMP':
-                # DAMP damp[0.7] limse[15]
-                self.damp = DAMP(self, spline)
-                self.assign_card(self.damp, line_num)
-            elif word == 'ABIN':
-                # ABIN n1 n2
-                self.abin = ABIN(self, spline)
-                self.assign_card(self.abin, line_num)
-            elif word == 'ANSC':
-                # ANSC six coefficients
-                if len(spline) == 7:
-                    self.ansc = [float(x) for x in spline[:1]]
-            elif word == 'ANSR':
-                # ANSR anres[0.001]
-                if len(spline) == 2:
-                    self.ansr = float(spline[1])
-            elif word == 'BIND':
-                # BIND atom1 atom2
-                if len(spline) == 3:
-                    self.append_card(self.bind, BIND(self, spline), line_num)
-            elif word == 'BLOC':
-                # BLOC n1 n2 atomnames
-                self.append_card(self.bloc, BLOC(self, spline), line_num)
-            elif word == 'BOND':
-                # BOND atomnames
-                self.append_card(self.bonds, BOND(self, spline), line_num)
-            elif word == 'BUMP':
-                # BUMP s [0.02]
-                self.append_card(self.restraints, BUMP(self, spline), line_num)
-            elif word == 'CHIV':
-                # CHIV V[0] s[0.1] atomnames
-                self.append_card(self.restraints, CHIV(self, spline), line_num)
-            elif word == 'CONF':
-                # CONF atomnames max_d[1.9] max_a[170]
-                self.conf = CONF(self, spline)
-                self.assign_card(self.conf, line_num)
-            elif word == 'CONN':
-                # CONN bmax[12] r[#] atomnames or CONN bmax[12]
-                # bonded are d < (r1 + r2 + 0.5) Å
-                self.conn = CONN(self, spline)
-                self.assign_card(self.conn, line_num)
-            elif word == 'DEFS':
-                # DEFS sd[0.02] sf[0.1] su[0.01] ss[0.04] maxsof[1]
-                self.defs = DEFS(self, spline)
-                self.assign_card(self.defs, line_num)
-            elif word == 'DISP':
-                # DISP E f' f"[#] mu[#]
-                if not lastcard == 'SFAC':
-                    raise ParseOrderError
-                self.append_card(self.disp, DISP(self, spline), line_num)
-            elif word == 'EQIV':
-                # EQIV $n symmetry operation
-                # TODO: implement EQUIV class
-                if len(spline) > 1 and spline[1].startswith('$'):
-                    self.eqiv.append(spline[1:])
-            elif word == 'EXTI':
-                # EXTI x[0]
-                self.exti = float(spline[1])
-            elif word == 'EXYZ':
-                # EXYZ atomnames
-                self.append_card(self.restraints, EXYZ(self, spline), line_num)
-            elif word == 'FRAG':
-                # FRAG code[17] a[1] b[1] c[1] α[90] β[90] γ[90]
-                if len(spline) == 8:
-                    self.frag = FRAG(self, spline)
-                    self.assign_card(self.frag, line_num)
-            elif word == 'FEND':
-                # FEND (must follow FRAG)
-                if not self.frag:
-                    raise ParseOrderError
-                self.frag = None  # Turns frag mode off.
-            elif word == 'FLAT':
-                # FLAT s[0.1] four or more atoms
-                self.append_card(self.restraints, FLAT(self, spline), line_num)
-            elif word == 'FREE':
-                # FREE atom1 atom2
-                self.append_card(self.free, FREE(self, spline), line_num)
-            elif word == 'GRID':
-                # GRID sl[#] sa[#] sd[#] dl[#] da[#] dd[#]
-                self.grid = GRID(self, spline)
-                self.assign_card(self.grid, line_num)
-            elif word == 'HKLF':
-                # HKLF N[0] S[1] r11...r33[1 0 0 0 1 0 0 0 1] sm[1] m[0]
-                self.hklf = HKLF(self, spline)
-                self.assign_card(self.hklf, line_num)
-            elif line.startswith('END'):
-                # END (after HKLF or ends an include file)
-                self.end = True
-            elif word == 'HTAB':
-                # HTAB dh[2.0]  or  HTAB donor-atom acceptor-atom
-                self.htab = HTAB(self, spline)
-                self.assign_card(self.htab, line_num)
-            elif word == 'ISOR':
-                # ISOR s[0.1] st[0.2] atomnames
-                self.append_card(self.restraints, ISOR(self, spline), line_num)
-            elif word == 'LAUE':
-                # LAUE E
-                # I completely do not understand the LAUE instruction description in the manual!
-                continue
-            elif word == 'MERG':
-                # MERG n[2]
-                self.merg = MERG(self, spline)
-                self.assign_card(self.merg, line_num)
-            elif word == 'MORE':
-                # MORE m[1]
-                self.more = MORE(self, spline)
-                self.assign_card(self.more, line_num)
-            elif word == 'FMAP':
-                # FMAP code[2] axis[#] nl[53]
-                self.fmap = FMAP(self, spline)
-                self.assign_card(self.fmap, line_num)
-            elif word == 'MOVE':
-                # MOVE dx[0] dy[0] dz[0] sign[1]
-                self.move = MOVE(self, spline)
-                self.assign_card(self.move, line_num)
-            elif word == 'MPLA':
-                # MPLA na atomnames
-                self.mpla = MPLA(self, spline)
-                self.assign_card(self.mpla, line_num)
-            elif word == 'NCSY':
-                # NCSY DN sd[0.1] su[0.05] atoms
-                self.append_card(self.restraints, NCSY(self, spline), line_num)
-            elif word == 'NEUT':
-                # NEUT
-                if not lastcard == 'SYMM':
-                    raise ParseOrderError
-            elif word == 'OMIT':
-                # OMIT atomnames  or  OMIT s[-2] 2θ(lim)[180]  or  OMIT h k l
-                # TODO: Implement OMIT class
-                self.omit.append(spline[1:])
-            elif word == 'PLAN':
-                # PLAN npeaks[20] d1[#] d2[#]
-                self.plan = PLAN(self, spline)
-                self.assign_card(self.plan, line_num)
-            elif word == 'PRIG':
-                # PRIG p[#]
-                self.prig = PRIG(self, spline)
-                self.assign_card(self.prig, line_num)
-            elif word == 'RTAB':
-                # RTAB codename atomnames  -->  codename: e.g. 'omeg' gets tabualted in the lst
-                self.append_card(self.rtab, RTAB(self, spline), line_num)
-            elif word == 'SAME':
-                # SAME s1[0.02] s2[0.04] atomnames
-                self.append_card(self.restraints, SAME(self, spline), line_num)
-            elif word == 'SHEL':
-                # SHEL lowres[infinite] highres[0]
-                self.shel = SHEL(self, spline)
-                self.assign_card(self.shel, line_num)
-            elif word == 'SIZE':
-                # SIZE dx dy dz
-                self.size = SIZE(self, spline)
-                self.assign_card(self.size, line_num)
-            elif word == 'SPEC':
-                # SPEC del[0.2]
-                if len(spline) > 1:
-                    self.spec = SPEC(self, spline)
-                    self.assign_card(self.spec, line_num)
-            elif word == 'STIR':
-                # STIR sres step[0.01]   -> stepwise improvement in the resolution sres
-                self.stir = STIR(self, spline)
-                self.assign_card(self.stir, line_num)
-            elif word == 'SUMP':
-                # SUMP c sigma c1 m1 c2 m2 ...
-                self.append_card(self.sump, SUMP(self, spline), line_num)
-            elif word == 'SWAT':
-                # SWAT g[0] U[2]
-                self.swat = spline[1:]
-            elif word == 'TEMP':
-                # TEMP T[20]  -> in Celsius
-                self.temp = float(spline[1].split('(')[0])
-                self.temp_in_kelvin = self.temp + 273.15
-            elif word == 'TWIN':
-                # TWIN 3x3 matrix [-1 0 0 0 -1 0 0 0 -1] N[2]
-                self.twin = TWIN(self, spline)
-                self.assign_card(self.twin, line_num)
-            elif word == 'TWST':
-                # TWST N[0] (N[1] after SHELXL-2018/3)
-                if len(spline) > 1:
-                    self.twst = TWST(self, spline)
-                    self.assign_card(self.twst, line_num)
-            elif word == 'WIGL':
-                # WIGL del[0.2] dU[0.2]
-                self.wigl = WIGL(self, spline)
-                self.assign_card(self.wigl, line_num)
-            elif word == 'WPDB':
-                # WPDB n[1]
-                self.wpdb = WPDB(self, spline)
-                self.assign_card(self.wpdb, line_num)
-            elif word == 'XNPD':
-                # XNPD Umin[-0.001]
-                self.xnpd = XNPD(self, spline)
-                self.assign_card(self.xnpd, line_num)
-            elif word == 'BEDE':
-                # Later...
-                continue
-            elif word == 'LONE':
-                # Later...
-                continue
-            elif word == 'MOLE':
-                # print('*** MOLE is deprecated! Do not use it! ***')
-                pass
-            elif word == 'HOPE':
-                # print('*** HOPE is deprecated! Do not use it! ***')
-                pass
-            elif line[:1] == '+':
-                pass
-            else:
-                if not line.strip():
-                    continue
-                if DEBUG:
-                    print("Error in line: {} -> {}".format(line_num, line))
-                    raise ParseUnknownParam
-
-    def add_atom(self, name: str = None, coordinates: list = None, element='C', uvals: list = None, part: int = 0,
-                 sof: float = 11.0):
-        """
-        Adds an atom to the ShelxFile.atoms list. If no element is given, carbon atoms are assumed.
-        """
-        if uvals is None:
-            uvals = [0.04]
-        part = PART(self, 'PART {}'.format(part).split())
-        afix = AFIX(self, 'AFIX 0'.split())
-        resi = RESI(self, 'RESI 0'.split())
-        a = Atom(self)
-        sfac_num = self.elem2sfac(element)
-        a.set_atom_parameters(name=name, sfac_num=sfac_num, coords=coordinates,
-                              part=part, afix=afix, resi=resi, site_occupation=sof, uvals=uvals)
-        self.append_card(self.atoms, a, 0)
-
-    def frac_to_cart(self, coordinates: list) -> Array:
-        """
-        fractional to cartesian coordinates by applying the orthogonal matrix.
-        """
-        return self.orthogonal_matrix * Array(coordinates)
-
-    def __repr__(self):
-        """
-        Represents the shelxl object.
-        """
-        resl = []
-        for num, line in enumerate(self._reslist):
-            if num in self.delete_on_write:
-                continue
-            try:
-                if line == '' and self._reslist[num + 1] == '':
-                    continue
-            except IndexError:
-                pass
-            # Prevent wrapping long lines with \n breaks by splitting first:
-            line = "".join([wrap_line(x) for x in str(line).split("\n")])
-            resl.append(line)
-        return "\n".join(resl)
-
-    def grow(self, with_qpeaks: bool = False):
-        """
-        Returns a list of atoms that represent the complete molecules of the structure.
-        """
-        sdm = SDM(self)
-        needsymm = sdm.calc_sdm()
-        packed_atoms = sdm.packer(sdm, needsymm, with_qpeaks=with_qpeaks)
-        return packed_atoms
-
-    def refine(self, cycles: Union[int, None] = None, backup_before: bool = True) -> bool:
-        filen = self.resfile.stem
-        # Go into path of resfile:
-        os.chdir(self.resfile.parent)
-        # so that shelxl can use the filename as parameter only (It does not like long names)
-        if cycles is not None:
-            self.cycles.number = cycles
-        # shutil.copyfile(filen+'.res', filen+'.ins')
-        ref = ShelxlRefine(self, self.resfile)
-        ref.remove_acta_card(self.acta)
-        self.write_shelx_file(filen + '.ins')
-        ref.run_shelxl(backup_before=backup_before)
-        self.reload()
-        ref.restore_acta_card()
-        # self.write_shelx_file(filen + '.res')
-        return True
-
-    def refine_weight_convergence(self, stop_after: int = 10):
-        """
-        Tries to refine weigting sheme from SHELXL until it converged (self.weight_difference() is zero) or
-        stopt_after cycles are reached. 
-        """
-        for _ in range(stop_after):
-            difference = self.wght.difference()
-            print("Weighting difference = {} {}".format(*difference))
-            if self._weight_converged(difference):
-                return True
-            else:
-                self.update_weight()
-                self.refine(9)
-        print("Maximum number of refinement cycles reached, but no WGHT convergence.")
-        return False
-
-    def _weight_converged(self, diff):
-        return diff == [0.0, 0.0]
-
-    def append_card(self, obj, card, line_num):
-        """
-        Appends SHELX card to an object list, e.g. self.restraints and
-        assigns the line_num in reslist with the card instance.
-        """
-        obj.append(card)
-        self._reslist[line_num] = card
-        return card
-
-    def assign_card(self, card, line_num):
-        self._reslist[line_num] = card
-        return card
-
-    @staticmethod
-    def is_atom(atomline: str) -> bool:
-        """
-        Returns True is line contains an atom.
-        """
-        # no empty line, not in cards and not space at start:
-        if atomline[:4].upper() not in SHX_CARDS:  # exclude all non-atom cards
-            spline = atomline.split()
-            # Too few parameter for an atom:
-            if len(spline) < 5:
-                return False
-            # means sfac number is missing:
-            if '.' in spline[1]:
-                return False
-            if Shelxfile._coordinates_are_unrealistic(spline):
-                return False
-            # Exclude lone pairs:
-            if len(spline) > 5 and spline[5] == '!':
-                return False
-            return True
-        else:
-            return False
-
-    @staticmethod
-    def _coordinates_are_unrealistic(spline):
-        return any(float(y) > 4.0 for y in spline[2:5])
-
-    def elem2sfac(self, atom_type: str) -> int:
-        """
-        returns an sfac-number for the element given in "atom_type"
-        """
-        for num, element in enumerate(self.sfac_table, 1):
-            if atom_type.upper() == element.upper():
-                return num  # return sfac number
-
-    def sfac2elem(self, sfacnum: int) -> str:
-        """
-        returns an element and needs an sfac-number
-        :param sfacnum: string like '2'
-        """
-        try:
-            elem = self.sfac_table[int(sfacnum)]
-        except IndexError:
-            return ''
-        return elem
-
-    def add_line(self, linenum: int, obj):
-        """
-        Adds a new SHELX card to the reslist after linenum.
-        """
-        self._reslist.insert(linenum + 1, obj)
-
-    def replace_line(self, obj, new_line: str):
-        """
-        Replaces a single line in the res file with new_line.
-        """
-        self._reslist[self.index_of(obj)] = new_line
-
-    def index_of(self, obj):
-        return self._reslist.index(obj)
-
-    @property
-    def sum_formula(self) -> str:
-        """
-        The sum formula of the structure with regards of the UNIT instruction.
-        """
-        formstring = ''
-        try:
-            val = self.unit.values
-            eli = self.sfac_table.elements_list
-        except AttributeError:
-            return ''
-        if len(val) == len(eli):
-            for el, num in zip(self.sfac_table.elements_list, self.unit.values):
-                try:
-                    formstring += "{}{:,g} ".format(el, num / self.Z)
-                except ZeroDivisionError:
-                    return ''
-        return formstring.strip()
-
-    def update_weight(self):
-        try:
-            self.wght.a = self.wght_suggested.a
-            self.wght.b = self.wght_suggested.b
-            self.wght.c = self.wght_suggested.c
-            self.wght.d = self.wght_suggested.d
-            self.wght.e = self.wght_suggested.e
-            self.wght.f = self.wght_suggested.f
-        except AttributeError:
-            return
-
-    def insert_anis(self):
-        """
-        Inserts ANIS into a results file for refinement of anisotropic displacement parameters.
-        TODO: implement ANIS n and ANIS atoms
-        """
-        self.add_line(self.unit.position, 'ANIS')
-
-    @property
-    def sum_formula_exact(self) -> str:
-        """
-        The sum formula of the structure with all atom occupancies summed together as string.
-        """
-        formstring = ''
-        sumdict = self.sum_formula_ex_dict()
-        for el in sumdict:
-            formstring += "{}{:,g} ".format(el.capitalize(), round(sumdict[el], 2))
-        return formstring.strip()
-
-    def sum_formula_ex_dict(self) -> dict:
-        """
-        The sum formula of the structure with all atom occupancies summed together as dictionary.
-        """
-        sumdict = {}
-        for el in self.sfac_table.elements_list:
-            for atom in self.atoms:
-                if atom.element.upper() == el.upper() and not atom.qpeak:
-                    if el in sumdict:
-                        sumdict[el] += atom.occupancy
-                    else:
-                        sumdict[el] = atom.occupancy
-            if el not in sumdict:
-                sumdict[el] = 0.0
-        return sumdict
-
-    def insert_frag_fend_entry(self, dbatoms: list, cell: list):
-        """
-        Inserts the FRAG ... FEND entry in the res file.
-        :param dbatoms:   list of atoms in the database entry
-        :param cell:  string with "FRAG 17 cell" from the database entry
-        """
-        dblist = []
-        for line in dbatoms:
-            dblist.append("{:4} {:<4} {:>8}  {:>8}  {:>8}".format(*line))
-        dblines = ' The following is from DSR:\n'
-        dblines = dblines + 'FRAG 17 {} {} {} {} {} {}'.format(*cell) + '\n'
-        dblines = dblines + '\n'.join(dblist)
-        dblines = dblines + '\nFEND\n'
-        # insert the db entry right after FVAR
-        self.add_line(self.fvars.position, dblines)
-
-    def _get_residuals(self, spline, line):
-        if Shelxfile._r1_regex.match(line):
-            self._get_r1(spline)
-        if Shelxfile._wr2_regex.match(line):
-            self._get_wr2(spline)
-        if Shelxfile._parameters_regex.match(line):
-            self._get_params_and_restraints(spline)
-        if Shelxfile._diff_peak_regex.match(line):
-            self._get_peak_hole(spline)
-        if Shelxfile._goof_regex.match(line):
-            self._get_goof(spline)
-        if Shelxfile._spgrp_regex.match(line):
-            self._get_space_group(spline)
-
-    def _get_space_group(self, spline):
-        try:
-            self.space_group = spline[3]
-        except(IndexError, ValueError):
-            pass
-
-    def _get_goof(self, spline):
-        try:
-            self.goof = float(spline[8].split(',')[0])
-            self.rgoof = float(spline[12].split(',')[0])
-        except(IndexError, ValueError):
-            pass
-
-    def _get_peak_hole(self, spline):
-        # REM Highest difference peak  0.407,  deepest hole -0.691,  1-sigma level  0.073
-        try:
-            self.highest_peak = float(spline[4].split(",")[0])
-            self.deepest_hole = float(spline[7].split(",")[0])
-        except(IndexError, ValueError):
-            pass
-
-    def _get_params_and_restraints(self, spline):
-        try:
-            self.parameters = int(spline[1])
-            if self.data and self.parameters:
-                self.dat_to_param = float(self.data) / float(self.parameters)
-        except IndexError:
-            pass
-        try:
-            self.num_restraints = int(spline[-2])
-        except(IndexError, ValueError):
-            pass
-
-    def _get_wr2(self, spline):
-        try:
-            self.wr2 = float(spline[3].split(",")[0])
-        except(IndexError, ValueError):
-            pass
-
-    def _get_r1(self, spline):
-        try:
-            self.R1 = float(spline[3])
-        except(IndexError, ValueError):
-            pass
-        try:
-            self.data = int(spline[-2])
-        except(IndexError, ValueError):
-            pass
-
-
-if __name__ == "__main__":
-    print(Path('.').resolve())
-    # file = r'../shelxfile/tests/resources/p21c.res'
-    file = r'./shelxfile/tests/resources/p-31c.res'
-    shx = Shelxfile()
-    shx.read_file(file)
-    print(shx.atoms)
-    print(shx.sum_formula_exact)
-    print(shx.sum_formula)
-    print(shx.sum_formula_ex_dict())
-    print(shx.restraints)
-    sys.exit()
-
-    # noinspection PyUnreachableCode
-    """
-    #To get all available SHELX commands:
-    def get_shelx_commands():
-        url = "http://shelx.uni-goettingen.de/shelxl_html.php"
-        response = urlopen('{}/version.txt'.format(url))
-        html = response.read().decode('UTF-8')
-        #res = BeautifulSoup(html, "html5lib")
-        tags = res.findAll("p", {"class": 'instr'})
-        for l in tags:
-            if l:
-                print(str(l).split(">")[1].split("<")[0])
-    """
+# -*- encoding: utf-8 -*-
+# möpß
+#
+# ----------------------------------------------------------------------------
+# "THE BEER-WARE LICENSE" (Revision 42):
+# <dkratzert@gmx.de> wrote this file. As long as you retain
+# this notice you can do whatever you want with this stuff. If we meet some day,
+# and you think this stuff is worth it, you can buy me a beer in return.
+# Daniel Kratzert
+# ----------------------------------------------------------------------------
+#
+from pathlib import Path
+from typing import Union, List
+
+from shelxfile.atoms.atom import Atom
+from shelxfile.atoms.atoms import Atoms
+from shelxfile.refine.refine import ShelxlRefine
+from shelxfile.shelx.sdm import SDM
+
+__doc__ = """
+This is a full implementation of the SHELXL file syntax. Additionally it is able to edit SHELX properties with Python.
+The implementation is Python3-only and supports SHELXL after 2017 (You should not use old versions anyway).
+
+The parser is quiet about the most errors unless you enable DEBUG in misc.py. The parser will try to read the 
+SHELX file even if it has syntax errors, but if for example, the SFAC and UNIT instruction is not consistent 
+it will fail. 
+"""
+
+import os
+import re
+import sys
+
+from shelxfile.shelx.cards import ACTA, FVAR, FVARs, REM, BOND, Restraints, DEFS, NCSY, ISOR, FLAT, \
+    BUMP, DFIX, DANG, SADI, SAME, RIGU, SIMU, DELU, CHIV, EADP, EXYZ, DAMP, HFIX, HKLF, SUMP, SYMM, LSCycles, \
+    SFACTable, UNIT, BASF, TWIN, WGHT, BLOC, SymmCards, CONN, CONF, BIND, DISP, GRID, HTAB, MERG, FRAG, FREE, FMAP, \
+    MOVE, PLAN, PRIG, RTAB, SHEL, SIZE, SPEC, STIR, TWST, WIGL, WPDB, XNPD, ZERR, CELL, LATT, MORE, MPLA, AFIX, PART, \
+    RESI, ABIN, ANIS, Residues
+from shelxfile.misc.dsrmath import Array, OrthogonalMatrix
+from shelxfile.misc.misc import DEBUG, ParseOrderError, ParseNumError, ParseUnknownParam, \
+    multiline_test, dsr_regex, wrap_line, ParseSyntaxError
+
+"""
+TODO:
+- Handle BEDE & LONE plus their results
+- Rotate ellipsoids with kabsch
+- kallall.Q, killall.C 
+- Q-peak printing is wrong: Q1    1   0.9828    1.1159    0.3148   11.00000  0.04      0.00  
+- Write out parts and afix in grow mode
+- Delete atoms (H) in AFIX -> delete entire afix group
+- Is backup file and reccovery from failed refinement working?
+- check if atoms in restraints are also in structure
+- restraints involved with an atom should also be part of the atoms properties
+------------------------------------------------------------
+- deleting atoms should also remove them from restraints
+- add remove_hydrogen_atoms(atom) method.
+- shx.remove_all_H([list of atoms], or all)
+- bond list
+- implement an add_afix(afixm, afixn, atoms, frag_fend=False, position=None, afix_options=None)
+  default position is directly behind FVAR or FRAG/FEND if enabled
+- will read in lst file after refinement to fill shx.lst_file properties.
+- shx.move_in_part([list of atoms])
+- shx.move_in_resi([list of atoms])
+- shx.sort.residue(3) (low priority)
+- shx.lst_file.residuals -> density, r-values, goof, movements, bad reflections
+   bad restraints, shelx *** errors
+- shx.unused_atom_name('C') -> get a carbon atom with unused number
+- shx.sort -> sort file (low priority)
+"""
+
+SHX_CARDS = ('TITL', 'CELL', 'ZERR', 'LATT', 'SYMM', 'SFAC', 'UNIT', 'LIST', 'L.S.', 'CGLS',
+             'BOND', 'FMAP', 'PLAN', 'TEMP', 'ACTA', 'CONF', 'SIMU', 'RIGU', 'WGHT', 'FVAR',
+             'DELU', 'SAME', 'DISP', 'LAUE', 'REM ', 'MORE', 'TIME', 'END ', 'HKLF', 'OMIT',
+             'SHEL', 'BASF', 'TWIN', 'EXTI', 'SWAT', 'HOPE', 'MERG', 'SPEC', 'RESI', 'MOVE',
+             'ANIS', 'AFIX', 'HFIX', 'FRAG', 'FEND', 'EXYZ', 'EADP', 'EQIV', 'CONN', 'BIND',
+             'FREE', 'DFIX', 'BUMP', 'SADI', 'CHIV', 'FLAT', 'DEFS', 'ISOR', 'NCSY', 'SUMP',
+             'BLOC', 'DAMP', 'STIR', 'MPLA', 'RTAB', 'HTAB', 'SIZE', 'WPDB', 'GRID', 'MOLE',
+             'XNPD', 'REST', 'CHAN', 'FLAP', 'RNUM', 'SOCC', 'PRIG', 'WIGL', 'RANG', 'TANG',
+             'ADDA', 'STAG', 'NEUT', 'ABIN', 'ANSC', 'ANSR', 'NOTR', 'TWST', 'PART', 'DANG',
+             'BEDE', 'LONE', 'REM', 'END')
+
+
+class Shelxfile():
+    """
+    Class for data from a SHELXL res file. Includes Atoms, cards and unit cell.
+
+    :type restraints: List[Restraint]
+    """
+    _r1_regex = re.compile(r'^REM\s+R1\s+=', re.IGNORECASE)
+    _wr2_regex = re.compile(r'^REM\s+wR2\s+=', re.IGNORECASE)
+    _parameters_regex = re.compile(r'^REM\s+\d+\s+parameters\s+refined', re.IGNORECASE)
+    _diff_peak_regex = re.compile(r'^REM\sHighest\sdifference', re.IGNORECASE)
+    _goof_regex = re.compile(r'^REM\swR2\s=\s.*,\sGooF', re.IGNORECASE)
+    _spgrp_regex = re.compile(r'^REM\s+\S+\s+in\s+\S+', re.IGNORECASE)
+
+    def __init__(self):
+        """
+        Reads the shelx file and extracts information.
+
+        :param resfile: file path
+        """
+        self.temp_in_kelvin = 0.0
+        self.shelx_max_line_length = 79  # maximum character lenth per line in SHELXL
+        self.nohkl = False
+        self._a, self._b, self._c, self._alpha, self._beta, self._gamma, self.V = \
+            None, None, None, None, None, None, None
+        self.cell: Union[CELL, None] = None
+        self.ansc: List[float] = []
+        self.abin: Union[None, ABIN] = None
+        self.acta: Union[None, ACTA] = None
+        self.fmap: Union[None, FMAP] = None
+        self.xnpd: Union[None, XNPD] = None
+        self.wpdb: Union[None, WPDB] = None
+        self.wigl: Union[None, WIGL] = None
+        self.temp: Union[int, float] = 20
+        # TODO: Implement swat class:
+        self.swat = None
+        self.stir: Union[None, STIR] = None
+        self.spec: Union[None, SPEC] = None
+        self.twst: Union[None, TWST] = None
+        self.plan: Union[None, PLAN] = None
+        self.prig: Union[None, PRIG] = None
+        self.merg: Union[None, MERG] = None
+        self.more: Union[None, MORE] = None
+        self.move: Union[None, MOVE] = None
+        self.defs: Union[None, DEFS] = None
+        self.zerr: Union[None, ZERR] = None
+        self.wght: Union[None, WGHT] = None
+        self.frag: Union[None, FRAG] = None
+        self.twin: Union[None, TWIN] = None
+        self.basf: Union[None, BASF] = None
+        self.latt: Union[None, LATT] = None
+        self.anis: Union[None, ANIS] = None
+        self.damp: Union[None, DAMP] = None
+        self.unit: Union[None, UNIT] = None
+        self.size: Union[None, SIZE] = None
+        self.htab: Union[None, HTAB] = None
+        self.shel: Union[None, SHEL] = None
+        self.mpla: Union[None, MPLA] = None
+        self.hklf: Union[None, HKLF] = None
+        self.grid: Union[None, GRID] = None
+        self.conn: Union[None, CONN] = None
+        self.conf: Union[None, CONF] = None
+        self.afix: Union[AFIX, None] = None
+        self.rtab: List[RTAB] = []
+        self.omit: List[str] = []
+        self.free: List[FREE] = []
+        self.eqiv: List[str] = []
+        self.bonds: List[BOND] = []
+        self.disp: List[BOND] = []
+        self.bind: List[BIND] = []
+        self.bloc: List[BLOC] = []
+        self.part: PART = PART(self, ['PART', '0'])
+        self.resi: RESI = RESI(self, ['RESI', '0'])
+        self.residues = Residues(self)
+        self.dsrlines: List[str] = []
+        self.dsrline_nums: List[int] = []
+        self.symmcards: SymmCards = SymmCards(self)
+        self.hfixes: List[HFIX] = []
+        self.sump: List[SUMP] = []
+        self.wght_suggested: Union[None, WGHT] = None
+        self.Z: int = 1
+        self.titl = ""
+        self.exti: float = 0.0
+        self.ansr: float = 0.001
+        self.rem: List[REM] = []
+        self.atoms: Atoms = Atoms(self)
+        self.fvars: FVARs = FVARs(self)
+        self.restraints: Restraints = Restraints()
+        self.sfac_table: SFACTable = SFACTable(self)
+        self.cycles: Union[None, LSCycles] = None
+        self.R1: Union[None, float] = None
+        self.wr2: Union[None, float] = None
+        self.goof: Union[None, float] = None
+        self.rgoof: Union[None, float] = None
+        self.space_group: Union[None, str] = None
+        self.data: Union[None, int] = None
+        self.parameters: Union[None, int] = None
+        self.dat_to_param: Union[None, float] = None
+        self.num_restraints: Union[None, int] = None
+        self.highest_peak: Union[None, float] = None
+        self.deepest_hole: Union[None, float] = None
+        self.end: bool = False
+        self.maxsof: float = 1.0
+        self.delete_on_write: set = set()
+        self.wavelen: float = 0.0
+        self.global_sadi: Union[None, int] = None
+        self.list: int = 0
+        self.theta_full: float = 0.0
+        self.error_line_num: int = -1  # Only used to tell the line number during an exception.
+        self.resfile: Union[Path, None] = None
+        self._reslist: List = []
+
+    def write_shelx_file(self, filename=None, verbose=False) -> None:
+        if not filename:
+            filename = self.resfile
+        with open(filename, 'w') as f:
+            for num, line in enumerate(self._reslist):
+                if num in self.delete_on_write:
+                    if DEBUG:
+                        # print('Deleted line {}'.format(num + 1))
+                        pass
+                    continue
+                if line == '':  # and self._reslist[num + 1] == '':
+                    continue
+                # Prevent wrapping long lines with \n breaks by splitting first:
+                line = "\n".join([wrap_line(x) for x in str(line).split("\n")])
+                f.write(str(line) + '\n')
+        if verbose or DEBUG:
+            print('File successfully written to {}'.format(os.path.abspath(filename)))
+
+    def read_file(self, resfile: Union[Path, str]) -> None:
+        """
+        Read input from a file path.
+        """
+        if isinstance(resfile, str):
+            resfile = Path(resfile)
+        self.resfile = resfile.resolve()
+        if DEBUG:
+            print('Resfile is:', resfile)
+        try:
+            self._reslist: List = resfile.read_text().splitlines(keepends=False)
+            self._test_if_file_is_valid(resfile)
+        except UnicodeDecodeError:
+            if DEBUG:
+                print('*** Unable to read file', resfile, '***')
+            return
+        self._find_included_files()
+        self.parse_cards()
+
+    def read_string(self, resfile_string: str):
+        """
+        Read input as string.
+        This will not read files included with "+filename" syntax!
+        """
+        self._reslist = resfile_string.splitlines(keepends=False)
+        self.parse_cards()
+
+    def parse_cards(self):
+        try:
+            self._parse_cards()
+        except Exception as e:
+            if DEBUG:
+                self.show_line_where_error_occured(e)
+                raise
+            else:
+                return
+
+    def _test_if_file_is_valid(self, resfile):
+        if len(self._reslist) < 20 and DEBUG:
+            print('*** Not a SHELXL file: {} ***'.format(resfile))
+            sys.exit()
+
+    def show_line_where_error_occured(self, e):
+        try:
+            print('Error near:\n', self._reslist[self.error_line_num])
+        except IndexError:
+            pass
+        print(e)
+        print("*** Syntax error found in file {}, line {} ***".format(self.resfile, self.error_line_num + 1))
+
+    def _find_included_files(self):
+        # Tracks the file names of included files in order to find recursive inclusion:
+        includefiles = []
+        for line_num, line in enumerate(self._reslist):
+            if line.startswith('+'):
+                try:
+                    file_included_in_includefile = self._read_included_file(includefiles, line)
+                    if file_included_in_includefile:
+                        for line_num_includefile, l in enumerate(file_included_in_includefile):
+                            reslist_position = line_num + 1 + line_num_includefile
+                            # '+filename' include files are not copied to res file,
+                            #  so I have to delete these lines on write.
+                            # '++filename' copies them to the .res file where appropriate
+                            # I leave this out, because I am not SHELXL:
+                            # if l.startswith('+') and l[:2] != '++':
+                            #    self.delete_on_write.update([lnum])
+                            self._reslist.insert(reslist_position, l)
+                        continue
+                except IndexError:
+                    if DEBUG:
+                        print('*** CANNOT READ INCLUDE FILE {} ***'.format(line))
+                    # Not sure if this is a good idea: del reslist[n]
+
+    def _read_included_file(self, includefiles: List[str], line: str):
+        include_filename: Path = self.resfile.resolve().parent.joinpath(line[1:])
+        # Detect recursive file inclusion:
+        if include_filename.name in includefiles:
+            raise ValueError('*** Recoursive include files detected! ***')
+        includefiles.append(include_filename.name)
+        try:
+            newfile = include_filename.read_text().splitlines(keepends=False)
+        except IOError as e:
+            if DEBUG:
+                print(e)
+                print('*** CANNOT OPEN NESTED INPUT FILE {} ***'.format(include_filename))
+            return []
+        return newfile
+
+    def reload(self):
+        """
+        Reloads the shelx file and parses it again.
+        """
+        if DEBUG:
+            print('loading file:', self.resfile)
+        self.read_file(self.resfile.resolve())
+
+    def _parse_cards(self):
+        lastcard = ''
+        fvarnum = 1
+        for line_num, line in enumerate(self._reslist):
+            self.error_line_num = line_num  # For exception during parsing.
+            list_of_lines = [line_num]  # list of lines where a card appears, e.g. for atoms with two lines
+            if line[:1] == ' ' or line == '':
+                continue
+            if not self.titl and line[:4] == 'TITL':
+                # TITL[]  ->  = and ! can be part of the TITL!
+                self.titl = line[5:76]
+                lastcard = 'TITL'
+                continue
+            wrapindex = 0
+            # This while loop makes wrapped lines look like they are not wrapped. The following lines are then
+            # beginning with a space character and thus are ignored. The 'lines' list holds the line nnumbers where
+            # 'line' is located ([line_num]) plus the wrapped lines.
+            if multiline_test(self._reslist[line_num]):
+                multiline = True
+            else:
+                multiline = False
+            while multiline:
+                # Glue together the two lines wrapped with "=":
+                wrapindex += 1
+                line = line.rpartition('=')[0] + self._reslist[line_num + wrapindex]
+                # self.delete_on_write.update([line_num + wrapindex])
+                list_of_lines.append(line_num + wrapindex)  # list containing the lines of a multiline command
+                # Do not activate this, otherwise, the unwrapping stops after two lines.
+                if multiline_test(self._reslist[line_num + wrapindex]):
+                    multiline = True
+                else:
+                    multiline = False
+                self._reslist[line_num + wrapindex] = ''
+            # The current line splitted:
+            spline = line.split('!')[0].split()  # Ignore comments with "!", see how this performes
+            # The current line as string:
+            line = line.upper().split('!')[0]  # Ignore comments with "!", see how this performes
+            word = line[:4]
+            # get RESI:
+            if line.startswith(('END', 'HKLF')) and self.resi:
+                self.resi.num = 0
+                if DEBUG:
+                    print('RESI in line {} was not closed'.format(line_num + 1))
+                # Do not continue here, otherwise HKLF is not parsed
+                # continue
+            if line.startswith('RESI'):
+                self.resi = RESI(self, spline)
+                self._assign_card(self.resi, line_num)
+                if self.resi.residue_number > 0:
+                    self.residues.append(self.resi)
+                continue
+            # Now collect the PART:
+            if line.startswith(('END', 'HKLF')) and self.part:
+                self.part.n = 0
+                if DEBUG:
+                    print('PART in line {} was not closed'.format(line_num + 1))
+                # Do not continue here, otherwise HKLF is not parsed
+                # continue
+            if line.startswith('PART'):
+                self.part = PART(self, spline)
+                self._assign_card(self.part, line_num)
+                continue
+            # collect AFIX:
+            if line.startswith(('END', 'HKLF')) and self.afix:
+                self.afix.mn = 0
+                if DEBUG:
+                    print('AFIX in line {} was not closed'.format(line_num + 1))
+            elif line.startswith('AFIX'):
+                self.afix = AFIX(self, spline)
+                self._assign_card(self.afix, line_num)
+            elif self.is_atom(line):
+                # A SHELXL atom:
+                # F9    4    0.395366   0.177026   0.601546  21.00000   0.03231  ( 0.03248 =
+                #            0.03649  -0.00522  -0.01212   0.00157 )
+                a = Atom(self)
+                a.parse_line(spline, list_of_lines, part=self.part, afix=self.afix, resi=self.resi)
+                self._append_card(self.atoms, a, line_num)
+            elif word == 'SADI':
+                # SADI s[0.02] pairs of atoms
+                # or SADI
+                if len(spline) == 1:
+                    self.global_sadi = line_num
+                self._append_card(self.restraints, SADI(self, spline), line_num)
+            elif word == 'DFIX':
+                # DFIX d s[0.02] atom pairs
+                self._append_card(self.restraints, DFIX(self, spline), line_num)
+            elif word == 'SIMU':
+                # SIMU s[0.04] st[0.08] dmax[2.0] atomnames
+                self._append_card(self.restraints, SIMU(self, spline), line_num)
+            elif word == 'DELU':
+                # DELU s1[0.01] s2[0.01] atomnames
+                self._append_card(self.restraints, DELU(self, spline), line_num)
+            elif word == 'RIGU':
+                # RIGU s1[0.004] s2[0.004] atomnames
+                self._append_card(self.restraints, RIGU(self, spline), line_num)
+            elif word == 'BASF':
+                # BASF scale factors
+                self._assign_card(BASF(self, spline), line_num)
+            elif word == 'HFIX':
+                # HFIX mn U[#] d[#] atomnames
+                self._append_card(self.hfixes, HFIX(self, spline), line_num)
+            elif word == 'DANG':
+                # DANG d s[0.04] atom pairs
+                self._append_card(self.restraints, DANG(self, spline), line_num)
+            elif word == 'EADP':
+                self._append_card(self.restraints, EADP(self, spline), line_num)
+            elif line[:3] == 'REM':
+                if dsr_regex.match(line):
+                    self.dsrlines.append(" ".join(spline))
+                    self.dsrline_nums.extend(list_of_lines)
+                self._append_card(self.rem, REM(self, spline), line_num)
+                self._get_residuals(spline, line)
+            elif word == 'AFIX':
+                # nothing to do
+                pass
+            elif word == 'CELL':
+                # CELL λ a b c α β γ
+                if not lastcard == 'TITL' and DEBUG:
+                    print('TITL is missing.')
+                self.cell = CELL(self, spline)
+                self._assign_card(self.cell, line_num)
+                self._a, self._b, self._c, self._alpha, self._beta, self._gamma = self.cell
+                self.orthogonal_matrix = OrthogonalMatrix(*self.cell)
+                self.wavelen = self.cell.wavelen
+                lastcard = 'CELL'
+            elif word == "ZERR":
+                # ZERR Z esd(a) esd(b) esd(c) esd(α) esd(β) esd(γ)
+                if not lastcard == 'CELL':
+                    if DEBUG:
+                        print('*** Invalid SHELX file!')
+                    raise ParseOrderError
+                if not self.cell:
+                    raise ParseOrderError('*** Cell parameters missing! ***')
+                if len(spline) >= 8:
+                    self.zerr = ZERR(self, spline)
+                    self.Z = self.zerr.Z
+                    if self.Z < 1:
+                        self.Z = 1
+                        if DEBUG:
+                            print('Z value is zero.')
+                    self._assign_card(self.zerr, line_num)
+                lastcard = 'ZERR'
+            elif word == "LATT":
+                # LATT N[1]
+                # 1=P, 2=I, 3=rhombohedral obverse on hexagonal axes, 4=F, 5=A, 6=B, 7=C.
+                # negative is non-centrosymmetric
+                self.latt = LATT(self, spline)
+                self._assign_card(self.latt, line_num)
+                if not lastcard == 'ZERR' and DEBUG:
+                    print('*** ZERR instruction is missing! ***')
+                if self.latt.centric:
+                    self.symmcards.set_centric(True)
+            elif word == "SYMM":
+                # SYMM symmetry operation
+                #  Being more greedy, because many files do this wrong:
+                # if not lastcard == 'ZERR':
+                #    raise ParseOrderError
+                # if not self.zerr:
+                #    raise ParseOrderError
+                s = SYMM(self, spline)
+                if not self.latt and DEBUG:
+                    print("*** LATT instruction is missing! ***")
+                    raise ParseSyntaxError
+                # Have to do this after parsing, because P-1 has no SYMM!
+                # if self.latt.centric:
+                #    self.symmcards.set_centric(True)
+                self.symmcards.append(s.symmcard)
+                if s not in self._reslist:
+                    self._reslist[line_num] = s
+                else:
+                    self.delete_on_write.update([line_num])
+                    self._reslist[line_num] = ' '
+                lastcard = 'SYMM'
+            elif word == 'SFAC':
+                # SFAC elements or
+                # SFAC E a1 b1 a2 b2 a3 b3 a4 b4 c f' f" mu r wt
+                # Being less strict to be able to parse files without cell errors:
+                # if not (lastcard == 'LATT' or lastcard == 'ZERR'):
+                #    raise ParseOrderError
+                # if not self.symmcards:
+                #    raise ParseOrderError
+                if len(spline) <= 1:
+                    continue
+                self.sfac_table.parse_element_line(spline)
+                if self.sfac_table not in self._reslist:
+                    self._reslist[line_num] = self.sfac_table
+                else:
+                    self.delete_on_write.update([line_num])
+                    self._reslist[line_num] = ' '
+                lastcard = 'SFAC'
+            elif word == 'UNIT':
+                # UNIT n1 n2 ...
+                # Number of atoms of each type in the unit-cell, in SFAC order.
+                if not lastcard == 'SFAC':
+                    raise ParseOrderError
+                if self.sfac_table:
+                    try:
+                        self.unit = self._assign_card(UNIT(self, spline), line_num)
+                    except ValueError:
+                        if DEBUG:
+                            print('*** Non-numeric value in SFAC instruction! ***')
+                        raise
+                else:
+                    raise ParseOrderError
+                if len(self.unit.values) != len(self.sfac_table.elements_list) and DEBUG:
+                    print('*** Number of UNIT and SFAC values differ! ***')
+                    raise ParseNumError
+                lastcard = 'UNIT'
+            elif word in ['L.S.', 'CGLS']:
+                # CGLS nls[0] nrf[0] nextra[0]
+                # L.S. nls[0] nrf[0] nextra[0]
+                self.cycles = self._assign_card(LSCycles(self, spline), line_num)
+            elif word == "LIST":
+                # LIST m[#] mult[1] (mult is for list 4 only)
+                self.list = int(spline[1])
+            elif word == "FVAR":
+                # FVAR osf[1] free variables
+                for fvvalue in spline[1:]:
+                    fvarnum += 1
+                    self._append_card(self.fvars, FVAR(fvarnum, float(fvvalue)), line_num)
+                    if self.fvars not in self._reslist:
+                        self._reslist[line_num] = self.fvars
+                    else:
+                        self.delete_on_write.update([line_num])
+            elif word == 'ANIS':
+                # ANIS n or ANIS names
+                # Must be before Atom(), to know which atom is anis.
+                self.anis = ANIS(self, spline)
+                self._assign_card(self.anis, line_num)
+            elif word == 'WGHT':
+                # WGHT a[0.1] b[0] c[0] d[0] e[0] f[.33333]
+                if self.end:
+                    self.wght_suggested = self._assign_card(WGHT(self, spline), line_num)
+                    continue
+                self.wght = self._assign_card(WGHT(self, spline), line_num)
+            elif word == 'ACTA':
+                # ACTA 2θfull[#] -> optional parameter NOHKL
+                self.acta = ACTA(self, spline)
+                self._assign_card(self.acta, line_num)
+            elif word == 'DAMP':
+                # DAMP damp[0.7] limse[15]
+                self.damp = DAMP(self, spline)
+                self._assign_card(self.damp, line_num)
+            elif word == 'ABIN':
+                # ABIN n1 n2
+                self.abin = ABIN(self, spline)
+                self._assign_card(self.abin, line_num)
+            elif word == 'ANSC':
+                # ANSC six coefficients
+                if len(spline) == 7:
+                    self.ansc = [float(x) for x in spline[:1]]
+            elif word == 'ANSR':
+                # ANSR anres[0.001]
+                if len(spline) == 2:
+                    self.ansr = float(spline[1])
+            elif word == 'BIND':
+                # BIND atom1 atom2
+                if len(spline) == 3:
+                    self._append_card(self.bind, BIND(self, spline), line_num)
+            elif word == 'BLOC':
+                # BLOC n1 n2 atomnames
+                self._append_card(self.bloc, BLOC(self, spline), line_num)
+            elif word == 'BOND':
+                # BOND atomnames
+                self._append_card(self.bonds, BOND(self, spline), line_num)
+            elif word == 'BUMP':
+                # BUMP s [0.02]
+                self._append_card(self.restraints, BUMP(self, spline), line_num)
+            elif word == 'CHIV':
+                # CHIV V[0] s[0.1] atomnames
+                self._append_card(self.restraints, CHIV(self, spline), line_num)
+            elif word == 'CONF':
+                # CONF atomnames max_d[1.9] max_a[170]
+                self.conf = CONF(self, spline)
+                self._assign_card(self.conf, line_num)
+            elif word == 'CONN':
+                # CONN bmax[12] r[#] atomnames or CONN bmax[12]
+                # bonded are d < (r1 + r2 + 0.5) Å
+                self.conn = CONN(self, spline)
+                self._assign_card(self.conn, line_num)
+            elif word == 'DEFS':
+                # DEFS sd[0.02] sf[0.1] su[0.01] ss[0.04] maxsof[1]
+                self.defs = DEFS(self, spline)
+                self._assign_card(self.defs, line_num)
+            elif word == 'DISP':
+                # DISP E f' f"[#] mu[#]
+                if not lastcard == 'SFAC':
+                    raise ParseOrderError
+                self._append_card(self.disp, DISP(self, spline), line_num)
+            elif word == 'EQIV':
+                # EQIV $n symmetry operation
+                # TODO: implement EQUIV class
+                if len(spline) > 1 and spline[1].startswith('$'):
+                    self.eqiv.append(spline[1:])
+            elif word == 'EXTI':
+                # EXTI x[0]
+                self.exti = float(spline[1])
+            elif word == 'EXYZ':
+                # EXYZ atomnames
+                self._append_card(self.restraints, EXYZ(self, spline), line_num)
+            elif word == 'FRAG':
+                # FRAG code[17] a[1] b[1] c[1] α[90] β[90] γ[90]
+                if len(spline) == 8:
+                    self.frag = FRAG(self, spline)
+                    self._assign_card(self.frag, line_num)
+            elif word == 'FEND':
+                # FEND (must follow FRAG)
+                if not self.frag:
+                    raise ParseOrderError
+                self.frag = None  # Turns frag mode off.
+            elif word == 'FLAT':
+                # FLAT s[0.1] four or more atoms
+                self._append_card(self.restraints, FLAT(self, spline), line_num)
+            elif word == 'FREE':
+                # FREE atom1 atom2
+                self._append_card(self.free, FREE(self, spline), line_num)
+            elif word == 'GRID':
+                # GRID sl[#] sa[#] sd[#] dl[#] da[#] dd[#]
+                self.grid = GRID(self, spline)
+                self._assign_card(self.grid, line_num)
+            elif word == 'HKLF':
+                # HKLF N[0] S[1] r11...r33[1 0 0 0 1 0 0 0 1] sm[1] m[0]
+                self.hklf = HKLF(self, spline)
+                self._assign_card(self.hklf, line_num)
+            elif line.startswith('END'):
+                # END (after HKLF or ends an include file)
+                self.end = True
+            elif word == 'HTAB':
+                # HTAB dh[2.0]  or  HTAB donor-atom acceptor-atom
+                self.htab = HTAB(self, spline)
+                self._assign_card(self.htab, line_num)
+            elif word == 'ISOR':
+                # ISOR s[0.1] st[0.2] atomnames
+                self._append_card(self.restraints, ISOR(self, spline), line_num)
+            elif word == 'LAUE':
+                # LAUE E
+                # I completely do not understand the LAUE instruction description in the manual!
+                continue
+            elif word == 'MERG':
+                # MERG n[2]
+                self.merg = MERG(self, spline)
+                self._assign_card(self.merg, line_num)
+            elif word == 'MORE':
+                # MORE m[1]
+                self.more = MORE(self, spline)
+                self._assign_card(self.more, line_num)
+            elif word == 'FMAP':
+                # FMAP code[2] axis[#] nl[53]
+                self.fmap = FMAP(self, spline)
+                self._assign_card(self.fmap, line_num)
+            elif word == 'MOVE':
+                # MOVE dx[0] dy[0] dz[0] sign[1]
+                self.move = MOVE(self, spline)
+                self._assign_card(self.move, line_num)
+            elif word == 'MPLA':
+                # MPLA na atomnames
+                self.mpla = MPLA(self, spline)
+                self._assign_card(self.mpla, line_num)
+            elif word == 'NCSY':
+                # NCSY DN sd[0.1] su[0.05] atoms
+                self._append_card(self.restraints, NCSY(self, spline), line_num)
+            elif word == 'NEUT':
+                # NEUT
+                if not lastcard == 'SYMM':
+                    raise ParseOrderError
+            elif word == 'OMIT':
+                # OMIT atomnames  or  OMIT s[-2] 2θ(lim)[180]  or  OMIT h k l
+                # TODO: Implement OMIT class
+                self.omit.append(spline[1:])
+            elif word == 'PLAN':
+                # PLAN npeaks[20] d1[#] d2[#]
+                self.plan = PLAN(self, spline)
+                self._assign_card(self.plan, line_num)
+            elif word == 'PRIG':
+                # PRIG p[#]
+                self.prig = PRIG(self, spline)
+                self._assign_card(self.prig, line_num)
+            elif word == 'RTAB':
+                # RTAB codename atomnames  -->  codename: e.g. 'omeg' gets tabualted in the lst
+                self._append_card(self.rtab, RTAB(self, spline), line_num)
+            elif word == 'SAME':
+                # SAME s1[0.02] s2[0.04] atomnames
+                self._append_card(self.restraints, SAME(self, spline), line_num)
+            elif word == 'SHEL':
+                # SHEL lowres[infinite] highres[0]
+                self.shel = SHEL(self, spline)
+                self._assign_card(self.shel, line_num)
+            elif word == 'SIZE':
+                # SIZE dx dy dz
+                self.size = SIZE(self, spline)
+                self._assign_card(self.size, line_num)
+            elif word == 'SPEC':
+                # SPEC del[0.2]
+                if len(spline) > 1:
+                    self.spec = SPEC(self, spline)
+                    self._assign_card(self.spec, line_num)
+            elif word == 'STIR':
+                # STIR sres step[0.01]   -> stepwise improvement in the resolution sres
+                self.stir = STIR(self, spline)
+                self._assign_card(self.stir, line_num)
+            elif word == 'SUMP':
+                # SUMP c sigma c1 m1 c2 m2 ...
+                self._append_card(self.sump, SUMP(self, spline), line_num)
+            elif word == 'SWAT':
+                # SWAT g[0] U[2]
+                self.swat = spline[1:]
+            elif word == 'TEMP':
+                # TEMP T[20]  -> in Celsius
+                self.temp = float(spline[1].split('(')[0])
+                self.temp_in_kelvin = self.temp + 273.15
+            elif word == 'TWIN':
+                # TWIN 3x3 matrix [-1 0 0 0 -1 0 0 0 -1] N[2]
+                self.twin = TWIN(self, spline)
+                self._assign_card(self.twin, line_num)
+            elif word == 'TWST':
+                # TWST N[0] (N[1] after SHELXL-2018/3)
+                if len(spline) > 1:
+                    self.twst = TWST(self, spline)
+                    self._assign_card(self.twst, line_num)
+            elif word == 'WIGL':
+                # WIGL del[0.2] dU[0.2]
+                self.wigl = WIGL(self, spline)
+                self._assign_card(self.wigl, line_num)
+            elif word == 'WPDB':
+                # WPDB n[1]
+                self.wpdb = WPDB(self, spline)
+                self._assign_card(self.wpdb, line_num)
+            elif word == 'XNPD':
+                # XNPD Umin[-0.001]
+                self.xnpd = XNPD(self, spline)
+                self._assign_card(self.xnpd, line_num)
+            elif word == 'BEDE':
+                # Later...
+                continue
+            elif word == 'LONE':
+                # Later...
+                continue
+            elif word == 'MOLE':
+                # print('*** MOLE is deprecated! Do not use it! ***')
+                pass
+            elif word == 'HOPE':
+                # print('*** HOPE is deprecated! Do not use it! ***')
+                pass
+            elif line[:1] == '+':
+                pass
+            else:
+                if not line.strip():
+                    continue
+                if DEBUG:
+                    print("Error in line: {} -> {}".format(line_num, line))
+                    raise ParseUnknownParam
+
+    def add_atom(self, name: str = None, coordinates: list = None, element='C', uvals: list = None, part: int = 0,
+                 sof: float = 11.0):
+        """
+        Adds an atom to the ShelxFile.atoms list. If no element is given, carbon atoms are assumed.
+        """
+        if uvals is None:
+            uvals = [0.04]
+        part = PART(self, 'PART {}'.format(part).split())
+        afix = AFIX(self, 'AFIX 0'.split())
+        resi = RESI(self, 'RESI 0'.split())
+        a = Atom(self)
+        sfac_num = self.elem2sfac(element)
+        a.set_atom_parameters(name=name, sfac_num=sfac_num, coords=coordinates,
+                              part=part, afix=afix, resi=resi, site_occupation=sof, uvals=uvals)
+        self._append_card(self.atoms, a, 0)
+
+    def frac_to_cart(self, coordinates: list) -> Array:
+        """
+        fractional to cartesian coordinates by applying the orthogonal matrix.
+        """
+        return self.orthogonal_matrix * Array(coordinates)
+
+    def __repr__(self):
+        """
+        Represents the shelxl object.
+        """
+        resl = []
+        for num, line in enumerate(self._reslist):
+            if num in self.delete_on_write:
+                continue
+            try:
+                if line == '' and self._reslist[num + 1] == '':
+                    continue
+            except IndexError:
+                pass
+            # Prevent wrapping long lines with \n breaks by splitting first:
+            line = "".join([wrap_line(x) for x in str(line).split("\n")])
+            resl.append(line)
+        return "\n".join(resl)
+
+    def grow(self, with_qpeaks: bool = False):
+        """
+        Returns a list of atoms that represent the complete molecules of the structure.
+        """
+        sdm = SDM(self)
+        needsymm = sdm.calc_sdm()
+        packed_atoms = sdm.packer(sdm, needsymm, with_qpeaks=with_qpeaks)
+        return packed_atoms
+
+    def refine(self, cycles: Union[int, None] = None, backup_before: bool = True) -> bool:
+        filen = self.resfile.stem
+        # Go into path of resfile:
+        os.chdir(self.resfile.parent)
+        # so that shelxl can use the filename as parameter only (It does not like long names)
+        if cycles is not None:
+            self.cycles.number = cycles
+        # shutil.copyfile(filen+'.res', filen+'.ins')
+        ref = ShelxlRefine(self, self.resfile)
+        ref.remove_acta_card(self.acta)
+        self.write_shelx_file(filen + '.ins')
+        ref.run_shelxl(backup_before=backup_before)
+        self.reload()
+        ref.restore_acta_card()
+        # self.write_shelx_file(filen + '.res')
+        return True
+
+    def refine_weight_convergence(self, stop_after: int = 10):
+        """
+        Tries to refine weigting sheme from SHELXL until it converged (self.weight_difference() is zero) or
+        stopt_after cycles are reached. 
+        """
+        for _ in range(stop_after):
+            difference = self.wght.difference()
+            print("Weighting difference = {} {}".format(*difference))
+            if self._weight_converged(difference):
+                return True
+            else:
+                self.update_weight()
+                self.refine(9)
+        print("Maximum number of refinement cycles reached, but no WGHT convergence.")
+        return False
+
+    def _weight_converged(self, diff):
+        return diff == [0.0, 0.0]
+
+    def _append_card(self, obj, card, line_num):
+        """
+        Appends SHELX card to an object list, e.g. self.restraints and
+        assigns the line_num in reslist with the card instance.
+        """
+        obj.append(card)
+        self._reslist[line_num] = card
+        return card
+
+    def _assign_card(self, card, line_num):
+        self._reslist[line_num] = card
+        return card
+
+    @staticmethod
+    def is_atom(atomline: str) -> bool:
+        """
+        Returns True is line contains an atom.
+        """
+        # no empty line, not in cards and not space at start:
+        if atomline[:4].upper() not in SHX_CARDS:  # exclude all non-atom cards
+            spline = atomline.split()
+            # Too few parameter for an atom:
+            if len(spline) < 5:
+                return False
+            # means sfac number is missing:
+            if '.' in spline[1]:
+                return False
+            if Shelxfile._coordinates_are_unrealistic(spline):
+                return False
+            # Exclude lone pairs:
+            if len(spline) > 5 and spline[5] == '!':
+                return False
+            return True
+        else:
+            return False
+
+    @staticmethod
+    def _coordinates_are_unrealistic(spline):
+        return any(float(y) > 4.0 for y in spline[2:5])
+
+    def elem2sfac(self, atom_type: str) -> int:
+        """
+        returns an sfac-number for the element given in "atom_type"
+        """
+        for num, element in enumerate(self.sfac_table, 1):
+            if atom_type.upper() == element.upper():
+                return num  # return sfac number
+
+    def sfac2elem(self, sfacnum: int) -> str:
+        """
+        returns an element and needs an sfac-number
+        :param sfacnum: string like '2'
+        """
+        try:
+            elem = self.sfac_table[int(sfacnum)]
+        except IndexError:
+            return ''
+        return elem
+
+    def add_line(self, linenum: int, line: str):
+        """
+        Adds a new SHELX card to the reslist after linenum.
+        e.g. shx.add_line(shx.unit.position, 'ANIS')
+        """
+        self._reslist.insert(linenum + 1, line)
+
+    def replace_line(self, obj, new_line: str):
+        """
+        Replaces a single line in the res file with new_line.
+        """
+        self._reslist[self.index_of(obj)] = new_line
+
+    def index_of(self, obj):
+        return self._reslist.index(obj)
+
+    @property
+    def sum_formula(self) -> str:
+        """
+        The sum formula of the structure with regards of the UNIT instruction.
+        """
+        formstring = ''
+        try:
+            val = self.unit.values
+            eli = self.sfac_table.elements_list
+        except AttributeError:
+            return ''
+        if len(val) == len(eli):
+            for el, num in zip(self.sfac_table.elements_list, self.unit.values):
+                try:
+                    formstring += "{}{:,g} ".format(el, num / self.Z)
+                except ZeroDivisionError:
+                    return ''
+        return formstring.strip()
+
+    def update_weight(self):
+        try:
+            self.wght.a = self.wght_suggested.a
+            self.wght.b = self.wght_suggested.b
+            self.wght.c = self.wght_suggested.c
+            self.wght.d = self.wght_suggested.d
+            self.wght.e = self.wght_suggested.e
+            self.wght.f = self.wght_suggested.f
+        except AttributeError:
+            return
+
+    def insert_anis(self):
+        """
+        Inserts ANIS into a results file for refinement of anisotropic displacement parameters.
+        TODO: implement ANIS n and ANIS atoms
+        """
+        self.add_line(self.unit.position, 'ANIS')
+
+    @property
+    def sum_formula_exact(self) -> str:
+        """
+        The sum formula of the structure with all atom occupancies summed together as string.
+        """
+        formstring = ''
+        sumdict = self.sum_formula_ex_dict()
+        for el in sumdict:
+            formstring += "{}{:,g} ".format(el.capitalize(), round(sumdict[el], 2))
+        return formstring.strip()
+
+    def sum_formula_ex_dict(self) -> dict:
+        """
+        The sum formula of the structure with all atom occupancies summed together as dictionary.
+        """
+        sumdict = {}
+        for el in self.sfac_table.elements_list:
+            for atom in self.atoms:
+                if atom.element.upper() == el.upper() and not atom.qpeak:
+                    if el in sumdict:
+                        sumdict[el] += atom.occupancy
+                    else:
+                        sumdict[el] = atom.occupancy
+            if el not in sumdict:
+                sumdict[el] = 0.0
+        return sumdict
+
+    def insert_frag_fend_entry(self, dbatoms: list, cell: list):
+        """
+        Inserts the FRAG ... FEND entry in the res file.
+        :param dbatoms:   list of atoms in the database entry
+        :param cell:  string with "FRAG 17 cell" from the database entry
+        """
+        dblist = []
+        for line in dbatoms:
+            dblist.append("{:4} {:<4} {:>8}  {:>8}  {:>8}".format(*line))
+        dblines = ' The following is from DSR:\n'
+        dblines = dblines + 'FRAG 17 {} {} {} {} {} {}'.format(*cell) + '\n'
+        dblines = dblines + '\n'.join(dblist)
+        dblines = dblines + '\nFEND\n'
+        # insert the db entry right after FVAR
+        self.add_line(self.fvars.position, dblines)
+
+    def _get_residuals(self, spline, line):
+        if Shelxfile._r1_regex.match(line):
+            self._get_r1(spline)
+        if Shelxfile._wr2_regex.match(line):
+            self._get_wr2(spline)
+        if Shelxfile._parameters_regex.match(line):
+            self._get_params_and_restraints(spline)
+        if Shelxfile._diff_peak_regex.match(line):
+            self._get_peak_hole(spline)
+        if Shelxfile._goof_regex.match(line):
+            self._get_goof(spline)
+        if Shelxfile._spgrp_regex.match(line):
+            self._get_space_group(spline)
+
+    def _get_space_group(self, spline):
+        try:
+            self.space_group = spline[3]
+        except(IndexError, ValueError):
+            pass
+
+    def _get_goof(self, spline):
+        try:
+            self.goof = float(spline[8].split(',')[0])
+            self.rgoof = float(spline[12].split(',')[0])
+        except(IndexError, ValueError):
+            pass
+
+    def _get_peak_hole(self, spline):
+        # REM Highest difference peak  0.407,  deepest hole -0.691,  1-sigma level  0.073
+        try:
+            self.highest_peak = float(spline[4].split(",")[0])
+            self.deepest_hole = float(spline[7].split(",")[0])
+        except(IndexError, ValueError):
+            pass
+
+    def _get_params_and_restraints(self, spline):
+        try:
+            self.parameters = int(spline[1])
+            if self.data and self.parameters:
+                self.dat_to_param = float(self.data) / float(self.parameters)
+        except IndexError:
+            pass
+        try:
+            self.num_restraints = int(spline[-2])
+        except(IndexError, ValueError):
+            pass
+
+    def _get_wr2(self, spline):
+        try:
+            self.wr2 = float(spline[3].split(",")[0])
+        except(IndexError, ValueError):
+            pass
+
+    def _get_r1(self, spline):
+        try:
+            self.R1 = float(spline[3])
+        except(IndexError, ValueError):
+            pass
+        try:
+            self.data = int(spline[-2])
+        except(IndexError, ValueError):
+            pass
+
+
+if __name__ == "__main__":
+    print(Path('.').resolve())
+    # file = r'../shelxfile/tests/resources/p21c.res'
+    file = r'./shelxfile/tests/resources/p-31c.res'
+    shx = Shelxfile()
+    shx.read_file(file)
+    print(shx.atoms)
+    print(shx.sum_formula_exact)
+    print(shx.sum_formula)
+    print(shx.sum_formula_ex_dict())
+    print(shx.restraints)
+    sys.exit()
+
+    # noinspection PyUnreachableCode
+    """
+    #To get all available SHELX commands:
+    def get_shelx_commands():
+        url = "http://shelx.uni-goettingen.de/shelxl_html.php"
+        response = urlopen('{}/version.txt'.format(url))
+        html = response.read().decode('UTF-8')
+        #res = BeautifulSoup(html, "html5lib")
+        tags = res.findAll("p", {"class": 'instr'})
+        for l in tags:
+            if l:
+                print(str(l).split(">")[1].split("<")[0])
+    """
```

### Comparing `shelxfile-8/shelxfile.egg-info/PKG-INFO` & `shelxfile-9/shelxfile.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,232 +1,245 @@
-Metadata-Version: 2.1
-Name: shelxfile
-Version: 8
-Summary: A parser for SHELXL results files.
-Home-page: https://github.com/dkratzert/ShelXFile
-Author: Daniel Kratzert
-Author-email: dkratzert@gmx.de
-License: Beerware License
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: Environment :: Console
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# Shelxfile
-<a href="https://repology.org/project/python:shelxfile/versions">
-    <img src="https://repology.org/badge/vertical-allrepos/python:shelxfile.svg" alt="Packaging status" align="right">
-</a>
-
-[![Unit tests](https://github.com/dkratzert/ShelXFile/actions/workflows/python-package.yml/badge.svg)](https://github.com/dkratzert/ShelXFile/actions/workflows/python-package.yml)
-![Contributions](https://img.shields.io/badge/contributions-welcome-blue)
-
-This is a full implementation of the SHELXL[[1](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)] file syntax. Additionally it is able to edit SHELX properties using Python.
-The implementation is Python3-only and supports SHELXL after 2017 (You should not use old versions anyway).
-Shelxfile may eventually become a new heart of DSR[[2](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)] and is already used as file parser in StructureFinder[[3](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)].
-
-Shelxfile always keeps the file order intact. Every SHELX instruction like DFIX or an atom is stored as an class object in the list Shelxfile.\_reslist. When writing the Shelxfile content to disk, it wites the \_reslist content to disk.
-
-Shelxfile tries to detect all possible syntax errors that SHELXL would not like either. If Shelxfile.DEBUG is True, more output about syntax and other errors are printed out. Otherwise, the parser is quiet except for really severe errors like a missing unit cell.
-
-Not every part of Shelxfile is complete, for example it will not recognize if you add restraints with atom names that are not in the SHELX file. Please help me improving it!
-
-Examples:
-
-
-```python
-pip install shelxfile
-
->>> from shelxfile import Shelxfile
->>> shx = Shelxfile()
->>> shx.read_file('src/tests/resources/p21c.res')  # or .read_string() 
->>> shx.cell
-CELL 0.71073 10.5086 20.9035 20.5072 90 94.13 90
-
->>> list(shx.cell)
-[10.5086, 20.9035, 20.5072, 90.0, 94.13, 90.0]
-
->>> shx.cell.volume
-4493.047384590458
-
->>> shx.cell.a
-10.5086
-
-# You can overwrite any parameter in a shelx file:
->>> shx.plan
-20
-
->>> shx.plan = 30
->>> shx.plan
-30
-
->>> shx.atoms
-O1     3    0.074835    0.238436    0.402457   -31.00000    0.01579    0.03095      0.01852   -0.00468   -0.00210    0.01153
-C1     1    0.028576    0.234542    0.337234   -31.00000    0.02311    0.03617      0.01096   -0.01000    0.00201    0.00356
-C2     1    0.121540    0.194460    0.298291   -31.00000    0.02960    0.04586      0.01555   -0.00485   -0.00023    0.01102
-F
-...
-
->>> a = shx.atoms.get_atom_by_name('F1_2')  # Atom F1 in residue 2
->>> a
-Atom ID: 258  # <- The Atom ID is the index number in the Shelxfile._reslist list
-
->>> str(a)
-'F1    4    0.245205    0.192674    0.649231   -21.00000    0.05143    0.03826    0.03193   -0.00579   -0.01865   -0.00485'
-
->>> a.to_isotropic()
->>> str(a)
-'F1    4    0.245205    0.192674   0.649231  -21.00000    0.04000'
-
->>> a.position  # position in the SHELX .res file
-273
-
->>> str(shx._reslist[273])  # In regular code, do not access shx._reslist directly!
-'F1    4    0.245205    0.192674   0.649231  -21.00000    0.04000'
-
->>> a.name
-'F1'
-
->>> a.element
-'F'
-
->>> a.resinum
-2
-
->>> a.part
-2
-
->>> shx.sfac2elem(4)
-'F'
-
->>> shx.elem2sfac('F')
-4
-
->>> a.find_atoms_around(dist=2.0, only_part=1)
-[Atom ID: 254, Atom ID: 256, Atom ID: 260]  # Found some atoms 
-
->>> [str(x) for x in a.find_atoms_around(dist=2.2, only_part=2)]
-['C2     1    0.192984    0.140449    0.621265   -21.00000    0.04315    0.02747      0.02385    0.00686   -0.00757    0.00126', 
-'F2     4    0.264027    0.090306    0.642441   -21.00000    0.06073    0.04450      0.03972    0.01630   -0.01260    0.01460', 
-'F3     4    0.078582    0.131920    0.643529   -21.00000    0.05691    0.04955      0.03374    0.01040    0.01881    0.00375']
-
->>> a.cart_coords
-[1.617897551082389, 4.027560959000001, 13.279336538026433]
-
->>> a.frac_coords
-[0.245205, 0.192674, 0.649231]
-
->>> a.occupancy
-1.0
-
->>> a.sfac_num
-4
-
->>>[x for x in a.find_atoms_around(dist=2.5, only_part=2)]
-[Atom ID: 254, Atom ID: 256, Atom ID: 260, Atom ID: 262]
-
->>> for x in a.find_atoms_around(dist=2.5, only_part=2):
-...    x.delete()
-
->>> [x for x in a.find_atoms_around(dist=2.5, only_part=2)]
-[]  # Atoms are now deleted from shx._reslist.
-
->>> shx.restraints
-SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4
-SADI_CCF3 0.02 F1 C2 F2 C2 F3 C2 F4 C3 F5 C3 F6 C3 F7 C4 F8 C4 F9 C4
-SADI_CCF3 0.04 C2 C3 C3 C4 C2 C4
-SADI_CCF3 0.04 O1 C2 O1 C3 O1 C4
-SADI_CCF3 0.04 F1 F2 F2 F3 F3 F1 F4 F5 F5 F6 F6 F4 F7 F8 F8 F9 F9 F7
-...
-
->>> shx.restraints[1]
-SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4
-
-str(shx.restraints[1])
-'SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4'
-
-shx.restraints[1].residue_class
-'CCF3'
-
-shx.restraints[1].s
-0.02
-
-```
-
-Writes current shx object to test.ins
-All lines in Shelxfile._reslist get wrapped after 79 characters with " =\n " as
-specified by SHELXL during the file writing.
-
-```python
->>> shx.write_shelx_file('test.ins')
-```
-No matter if you loaded a .res or .ins file with refine(), SHELXL refines the structure of the Shelxfile() object:
-
-```python
->>> shx.insert_anis()
->>> shx.refine(2)
-
- Running SHELXL with "/usr/local/bin/shelxl -b3000 /Users/daniel/GitHub/Shelxfile/tests/p21c" and "L.S. 2"
- wR2 =  0.1143 before cycle   1 for   10786 data and    945 /    945 parameters
- wR2 =  0.1025 before cycle   2 for   10786 data and    945 /    945 parameters
- wR2 =  0.1006 before cycle   3 for   10786 data and      0 /    945 parameters
- SHELXL Version 2018/3
-```
-```python
-# Symmcards that are implied by lattice symmetry are generated on-the-fly:
->>> shx.symmcards
-| 1  0  0|   | 0.0|
-| 0  1  0| + | 0.0|
-| 0  0  1|   | 0.0|
-
-|-1  0  0|   | 0.0|
-| 0 -1  0| + | 0.0|
-| 0  0 -1|   | 0.0|
-
-|-1  0  0|   | 0.0|
-| 0  1  0| + | 0.5|
-| 0  0 -1|   | 0.5|
-
-| 1  0  0|   | 0.0|
-| 0 -1  0| + |-0.5|
-| 0  0  1|   |-0.5|
-
-# Complete or "grow" structures with higher symmetry: 
->>> shx = Shelxfile('./tests/p-31c.res')
-len(shx.atoms)
-88
-p = shx.grow()
-len(p)
-208
-
-# The (bond) angle between three atoms:
->>> at1 = shx.atoms.get_atom_by_name('O1_4')
->>> at2 = shx.atoms.get_atom_by_name('C1_4')
->>> at3 = shx.atoms.get_atom_by_name('C2_4')
->>> shx.atoms.angle(at1, at2, at3)
-109.688123
-
-# The torsion angle between four atoms:
->>> at1 = shx.atoms.get_atom_by_name('O1')
->>> at2 = shx.atoms.get_atom_by_name('C1')
->>> at3 = shx.atoms.get_atom_by_name('C2')
->>> at4 = shx.atoms.get_atom_by_name('F1')
->>> shx.atoms.torsion_angle(at1, at2, at3, at4)
-74.095731
-
-```
-
-and many more...
-
-## References
-[1] http://shelx.uni-goettingen.de/, G. M. Sheldrick, Acta Cryst. (2015). C71, 3-8.
-https://doi.org/10.1107/S2053229614024218
-
-[2] https://github.com/dkratzert/DSR
-
-[3] https://github.com/dkratzert/StructureFinder
-
+Metadata-Version: 2.1
+Name: shelxfile
+Version: 9
+Summary: A parser for SHELXL results files.
+Home-page: https://github.com/dkratzert/ShelXFile
+Author: Daniel Kratzert
+Author-email: dkratzert@gmx.de
+License: Beerware License
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Classifier: Environment :: Console
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# Shelxfile
+<a href="https://repology.org/project/python:shelxfile/versions">
+    <img src="https://repology.org/badge/vertical-allrepos/python:shelxfile.svg" alt="Packaging status" align="right">
+</a>
+
+[![Unit tests](https://github.com/dkratzert/ShelXFile/actions/workflows/python-package.yml/badge.svg)](https://github.com/dkratzert/ShelXFile/actions/workflows/python-package.yml)
+![Contributions](https://img.shields.io/badge/contributions-welcome-blue)
+
+This is a full implementation of the SHELXL[[1](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)] file syntax. Additionally it is able to edit SHELX properties using Python.
+The implementation is Python3-only and supports SHELXL after 2017 (You should not use old versions anyway).
+Shelxfile may eventually become a new heart of DSR[[2](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)] and is already used as file parser in StructureFinder[[3](https://github.com/dkratzert/Shelxfile/blob/master/README.md#references)].
+
+Shelxfile always keeps the file order intact. Every SHELX instruction like DFIX or an atom is stored as an class object in the list Shelxfile.\_reslist. When writing the Shelxfile content to disk, it wites the \_reslist content to disk.
+
+Shelxfile tries to detect all possible syntax errors that SHELXL would not like either. If Shelxfile.DEBUG is True, more output about syntax and other errors are printed out. Otherwise, the parser is quiet except for really severe errors like a missing unit cell.
+
+Not every part of Shelxfile is complete, for example it will not recognize if you add restraints with atom names that are not in the SHELX file. Please help me improving it!
+
+Examples:
+
+
+```python
+pip install shelxfile
+
+>>> from shelxfile import Shelxfile
+>>> shx = Shelxfile()
+>>> shx.read_file('src/tests/resources/p21c.res')  # or .read_string() 
+>>> shx.cell
+CELL 0.71073 10.5086 20.9035 20.5072 90 94.13 90
+
+>>> list(shx.cell)
+[10.5086, 20.9035, 20.5072, 90.0, 94.13, 90.0]
+
+>>> shx.cell.volume
+4493.047384590458
+
+>>> shx.cell.a
+10.5086
+
+# You can overwrite any parameter in a shelx file:
+>>> shx.plan
+PLAN 20
+
+>>> shx.plan.npeaks
+20
+
+>>> shx.plan.set('PLAN 30')
+>>> shx.plan
+PLAN 30
+
+>>> shx.atoms
+O1     3    0.074835    0.238436    0.402457   -31.00000    0.01579    0.03095      0.01852   -0.00468   -0.00210    0.01153
+C1     1    0.028576    0.234542    0.337234   -31.00000    0.02311    0.03617      0.01096   -0.01000    0.00201    0.00356
+C2     1    0.121540    0.194460    0.298291   -31.00000    0.02960    0.04586      0.01555   -0.00485   -0.00023    0.01102
+F
+...
+
+>>> shx.atoms.hydrogen_atoms
+[Atom ID: 81, Atom ID: 88, Atom ID: 95, ... ]
+
+>>> shx.atoms.n_hydrogen_atoms
+24
+
+# Atoms with a riding model e.g. hydrogen atom riding on a carbon atom:
+>>> shx.atoms.riding_atoms
+[Atom ID: 81, Atom ID: 88, Atom ID: 95, ... ]
+
+>>> a = shx.atoms.get_atom_by_name('F1_2')  # Atom F1 in residue 2
+>>> a
+Atom ID: 258  # <- The Atom ID is the index number in the Shelxfile._reslist list
+
+>>> str(a)
+'F1    4    0.245205    0.192674    0.649231   -21.00000    0.05143    0.03826    0.03193   -0.00579   -0.01865   -0.00485'
+
+>>> a.to_isotropic()
+>>> str(a)
+'F1    4    0.245205    0.192674   0.649231  -21.00000    0.04000'
+
+>>> a.position  # position in the SHELX .res file
+273
+
+>>> str(shx._reslist[273])  # In regular code, do not access shx._reslist directly!
+'F1    4    0.245205    0.192674   0.649231  -21.00000    0.04000'
+
+>>> a.name
+'F1'
+
+>>> a.element
+'F'
+
+>>> a.resinum
+2
+
+>>> a.part
+2
+
+>>> shx.sfac2elem(4)
+'F'
+
+>>> shx.elem2sfac('F')
+4
+
+>>> a.find_atoms_around(dist=2.0, only_part=1)
+[Atom ID: 254, Atom ID: 256, Atom ID: 260]  # Found some atoms 
+
+>>> [str(x) for x in a.find_atoms_around(dist=2.2, only_part=2)]
+['C2     1    0.192984    0.140449    0.621265   -21.00000    0.04315    0.02747      0.02385    0.00686   -0.00757    0.00126', 
+'F2     4    0.264027    0.090306    0.642441   -21.00000    0.06073    0.04450      0.03972    0.01630   -0.01260    0.01460', 
+'F3     4    0.078582    0.131920    0.643529   -21.00000    0.05691    0.04955      0.03374    0.01040    0.01881    0.00375']
+
+>>> a.cart_coords
+[1.617897551082389, 4.027560959000001, 13.279336538026433]
+
+>>> a.frac_coords
+[0.245205, 0.192674, 0.649231]
+
+>>> a.occupancy
+1.0
+
+>>> a.sfac_num
+4
+
+>>>[x for x in a.find_atoms_around(dist=2.5, only_part=2)]
+[Atom ID: 254, Atom ID: 256, Atom ID: 260, Atom ID: 262]
+
+>>> for x in a.find_atoms_around(dist=2.5, only_part=2):
+...    x.delete()
+
+>>> [x for x in a.find_atoms_around(dist=2.5, only_part=2)]
+[]  # Atoms are now deleted from shx._reslist.
+
+>>> shx.restraints
+SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4
+SADI_CCF3 0.02 F1 C2 F2 C2 F3 C2 F4 C3 F5 C3 F6 C3 F7 C4 F8 C4 F9 C4
+SADI_CCF3 0.04 C2 C3 C3 C4 C2 C4
+SADI_CCF3 0.04 O1 C2 O1 C3 O1 C4
+SADI_CCF3 0.04 F1 F2 F2 F3 F3 F1 F4 F5 F5 F6 F6 F4 F7 F8 F8 F9 F9 F7
+...
+
+>>> shx.restraints[1]
+SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4
+
+str(shx.restraints[1])
+'SADI_CCF3 0.02 C1 C2 C1 C3 C1 C4'
+
+shx.restraints[1].residue_class
+'CCF3'
+
+shx.restraints[1].s
+0.02
+
+```
+
+Writes current shx object to test.ins
+All lines in Shelxfile._reslist get wrapped after 79 characters with " =\n " as
+specified by SHELXL during the file writing.
+
+```python
+>>> shx.write_shelx_file('test.ins')
+```
+No matter if you loaded a .res or .ins file with refine(), SHELXL refines the structure of the Shelxfile() object:
+
+```python
+>>> shx.insert_anis()
+>>> shx.refine(2)
+
+ Running SHELXL with "/usr/local/bin/shelxl -b3000 /Users/daniel/GitHub/Shelxfile/tests/p21c" and "L.S. 2"
+ wR2 =  0.1143 before cycle   1 for   10786 data and    945 /    945 parameters
+ wR2 =  0.1025 before cycle   2 for   10786 data and    945 /    945 parameters
+ wR2 =  0.1006 before cycle   3 for   10786 data and      0 /    945 parameters
+ SHELXL Version 2018/3
+```
+```python
+# Symmcards that are implied by lattice symmetry are generated on-the-fly:
+>>> shx.symmcards
+| 1  0  0|   | 0.0|
+| 0  1  0| + | 0.0|
+| 0  0  1|   | 0.0|
+
+|-1  0  0|   | 0.0|
+| 0 -1  0| + | 0.0|
+| 0  0 -1|   | 0.0|
+
+|-1  0  0|   | 0.0|
+| 0  1  0| + | 0.5|
+| 0  0 -1|   | 0.5|
+
+| 1  0  0|   | 0.0|
+| 0 -1  0| + |-0.5|
+| 0  0  1|   |-0.5|
+
+# Complete or "grow" structures with higher symmetry: 
+>>> shx = Shelxfile('./tests/p-31c.res')
+len(shx.atoms)
+88
+p = shx.grow()
+len(p)
+208
+
+# The (bond) angle between three atoms:
+>>> at1 = shx.atoms.get_atom_by_name('O1_4')
+>>> at2 = shx.atoms.get_atom_by_name('C1_4')
+>>> at3 = shx.atoms.get_atom_by_name('C2_4')
+>>> shx.atoms.angle(at1, at2, at3)
+109.688123
+
+# The torsion angle between four atoms:
+>>> at1 = shx.atoms.get_atom_by_name('O1')
+>>> at2 = shx.atoms.get_atom_by_name('C1')
+>>> at3 = shx.atoms.get_atom_by_name('C2')
+>>> at4 = shx.atoms.get_atom_by_name('F1')
+>>> shx.atoms.torsion_angle(at1, at2, at3, at4)
+74.095731
+
+```
+
+and many more...
+
+## References
+[1] http://shelx.uni-goettingen.de/, G. M. Sheldrick, Acta Cryst. (2015). C71, 3-8.
+https://doi.org/10.1107/S2053229614024218
+
+[2] https://github.com/dkratzert/DSR
+
+[3] https://github.com/dkratzert/StructureFinder
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shelxfile Version: 8 Summary: A parser for SHELXL
+Metadata-Version: 2.1 Name: shelxfile Version: 9 Summary: A parser for SHELXL
 results files. Home-page: https://github.com/dkratzert/ShelXFile Author: Daniel
 Kratzert Author-email: dkratzert@gmx.de License: Beerware License Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
 Engineering :: Chemistry Classifier: Environment :: Console Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
@@ -28,25 +28,29 @@
 not recognize if you add restraints with atom names that are not in the SHELX
 file. Please help me improving it! Examples: ```python pip install shelxfile
 >>> from shelxfile import Shelxfile >>> shx = Shelxfile() >>> shx.read_file
 ('src/tests/resources/p21c.res') # or .read_string() >>> shx.cell CELL 0.71073
 10.5086 20.9035 20.5072 90 94.13 90 >>> list(shx.cell) [10.5086, 20.9035,
 20.5072, 90.0, 94.13, 90.0] >>> shx.cell.volume 4493.047384590458 >>>
 shx.cell.a 10.5086 # You can overwrite any parameter in a shelx file: >>>
-shx.plan 20 >>> shx.plan = 30 >>> shx.plan 30 >>> shx.atoms O1 3 0.074835
-0.238436 0.402457 -31.00000 0.01579 0.03095 0.01852 -0.00468 -0.00210 0.01153
-C1 1 0.028576 0.234542 0.337234 -31.00000 0.02311 0.03617 0.01096 -0.01000
-0.00201 0.00356 C2 1 0.121540 0.194460 0.298291 -31.00000 0.02960 0.04586
-0.01555 -0.00485 -0.00023 0.01102 F ... >>> a = shx.atoms.get_atom_by_name
-('F1_2') # Atom F1 in residue 2 >>> a Atom ID: 258 # <- The Atom ID is the
-index number in the Shelxfile._reslist list >>> str(a) 'F1 4 0.245205 0.192674
-0.649231 -21.00000 0.05143 0.03826 0.03193 -0.00579 -0.01865 -0.00485' >>>
-a.to_isotropic() >>> str(a) 'F1 4 0.245205 0.192674 0.649231 -21.00000 0.04000'
->>> a.position # position in the SHELX .res file 273 >>> str(shx._reslist[273])
-# In regular code, do not access shx._reslist directly! 'F1 4 0.245205 0.192674
+shx.plan PLAN 20 >>> shx.plan.npeaks 20 >>> shx.plan.set('PLAN 30') >>>
+shx.plan PLAN 30 >>> shx.atoms O1 3 0.074835 0.238436 0.402457 -31.00000
+0.01579 0.03095 0.01852 -0.00468 -0.00210 0.01153 C1 1 0.028576 0.234542
+0.337234 -31.00000 0.02311 0.03617 0.01096 -0.01000 0.00201 0.00356 C2 1
+0.121540 0.194460 0.298291 -31.00000 0.02960 0.04586 0.01555 -0.00485 -0.00023
+0.01102 F ... >>> shx.atoms.hydrogen_atoms [Atom ID: 81, Atom ID: 88, Atom ID:
+95, ... ] >>> shx.atoms.n_hydrogen_atoms 24 # Atoms with a riding model e.g.
+hydrogen atom riding on a carbon atom: >>> shx.atoms.riding_atoms [Atom ID: 81,
+Atom ID: 88, Atom ID: 95, ... ] >>> a = shx.atoms.get_atom_by_name('F1_2') #
+Atom F1 in residue 2 >>> a Atom ID: 258 # <- The Atom ID is the index number in
+the Shelxfile._reslist list >>> str(a) 'F1 4 0.245205 0.192674 0.649231 -
+21.00000 0.05143 0.03826 0.03193 -0.00579 -0.01865 -0.00485' >>> a.to_isotropic
+() >>> str(a) 'F1 4 0.245205 0.192674 0.649231 -21.00000 0.04000' >>>
+a.position # position in the SHELX .res file 273 >>> str(shx._reslist[273]) #
+In regular code, do not access shx._reslist directly! 'F1 4 0.245205 0.192674
 0.649231 -21.00000 0.04000' >>> a.name 'F1' >>> a.element 'F' >>> a.resinum 2
 >>> a.part 2 >>> shx.sfac2elem(4) 'F' >>> shx.elem2sfac('F') 4 >>>
 a.find_atoms_around(dist=2.0, only_part=1) [Atom ID: 254, Atom ID: 256, Atom
 ID: 260] # Found some atoms >>> [str(x) for x in a.find_atoms_around(dist=2.2,
 only_part=2)] ['C2 1 0.192984 0.140449 0.621265 -21.00000 0.04315 0.02747
 0.02385 0.00686 -0.00757 0.00126', 'F2 4 0.264027 0.090306 0.642441 -21.00000
 0.06073 0.04450 0.03972 0.01630 -0.01260 0.01460', 'F3 4 0.078582 0.131920
```

### Comparing `shelxfile-8/shelxfile.egg-info/SOURCES.txt` & `shelxfile-9/shelxfile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

