# Comparing `tmp/fastpdb-1.1.0.tar.gz` & `tmp/fastpdb-1.2.0.tar.gz`

## Comparing `fastpdb-1.1.0.tar` & `fastpdb-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 fastpdb-1.1.0/Cargo.toml
--rw-r--r--   0     1001      123     2517 2023-02-07 13:33:25.000000 fastpdb-1.1.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0     1001      123     1291 2023-02-07 13:33:25.000000 fastpdb-1.1.0/.gitignore
--rw-r--r--   0     1001      123     1524 2023-02-07 13:33:25.000000 fastpdb-1.1.0/LICENSE
--rw-r--r--   0     1001      123     1025 2023-02-07 13:33:25.000000 fastpdb-1.1.0/README.rst
--rw-r--r--   0     1001      123     2852 2023-02-07 13:33:25.000000 fastpdb-1.1.0/benchmark.py
--rw-r--r--   0     1001      123     1086 2023-02-07 13:33:25.000000 fastpdb-1.1.0/pyproject.toml
--rw-r--r--   0     1001      123    12992 2023-02-07 13:33:25.000000 fastpdb-1.1.0/python-src/fastpdb/__init__.py
--rw-r--r--   0     1001      123    28503 2023-02-07 13:33:25.000000 fastpdb-1.1.0/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-02-07 13:33:25.000000 fastpdb-1.1.0/tests/__init__.py
--rw-r--r--   0     1001      123   116316 2023-02-07 13:33:25.000000 fastpdb-1.1.0/tests/data/1aki.pdb
--rw-r--r--   0     1001      123  4394655 2023-02-07 13:33:26.000000 fastpdb-1.1.0/tests/data/1crr.pdb
--rw-r--r--   0     1001      123   172773 2023-02-07 13:33:26.000000 fastpdb-1.1.0/tests/data/1dix.pdb
--rw-r--r--   0     1001      123   464373 2023-02-07 13:33:26.000000 fastpdb-1.1.0/tests/data/1f2n.pdb
--rw-r--r--   0     1001      123  2933577 2023-02-07 13:33:26.000000 fastpdb-1.1.0/tests/data/1gya.pdb
--rw-r--r--   0     1001      123  1139022 2023-02-07 13:33:26.000000 fastpdb-1.1.0/tests/data/1igy.pdb
--rw-r--r--   0     1001      123   959040 2023-02-07 13:33:26.000000 fastpdb-1.1.0/tests/data/1l2y.pdb
--rw-r--r--   0     1001      123   228825 2023-02-07 13:33:26.000000 fastpdb-1.1.0/tests/data/1o1z.pdb
--rw-r--r--   0     1001      123  1278585 2023-02-07 13:33:26.000000 fastpdb-1.1.0/tests/data/2axd.pdb
--rw-r--r--   0     1001      123   270054 2023-02-07 13:33:26.000000 fastpdb-1.1.0/tests/data/3o5r.pdb
--rw-r--r--   0     1001      123   348948 2023-02-07 13:33:26.000000 fastpdb-1.1.0/tests/data/4gxy.pdb
--rw-r--r--   0     1001      123   221940 2023-02-07 13:33:26.000000 fastpdb-1.1.0/tests/data/4p5j.pdb
--rw-r--r--   0     1001      123   297351 2023-02-07 13:33:26.000000 fastpdb-1.1.0/tests/data/5h73.pdb
--rw-r--r--   0     1001      123   342630 2023-02-07 13:33:26.000000 fastpdb-1.1.0/tests/data/5ugo.pdb
--rw-r--r--   0     1001      123     4962 2023-02-07 13:33:26.000000 fastpdb-1.1.0/tests/test_fastpdb.py
--rw-r--r--   0     1001      123      777 2023-02-07 13:33:26.000000 fastpdb-1.1.0/tests/test_version.py
--rw-r--r--   0     1001      123     8794 2023-02-07 13:34:13.000000 fastpdb-1.1.0/Cargo.lock
--rw-r--r--   0        0        0     1923 1970-01-01 00:00:00.000000 fastpdb-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 fastpdb-1.2.0/Cargo.toml
+-rw-r--r--   0     1001      123     2517 2023-05-30 06:44:40.000000 fastpdb-1.2.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0     1001      123     1291 2023-05-30 06:44:40.000000 fastpdb-1.2.0/.gitignore
+-rw-r--r--   0     1001      123     1524 2023-05-30 06:44:40.000000 fastpdb-1.2.0/LICENSE
+-rw-r--r--   0     1001      123     1025 2023-05-30 06:44:40.000000 fastpdb-1.2.0/README.rst
+-rw-r--r--   0     1001      123     2852 2023-05-30 06:44:40.000000 fastpdb-1.2.0/benchmark.py
+-rw-r--r--   0     1001      123     1110 2023-05-30 06:44:40.000000 fastpdb-1.2.0/pyproject.toml
+-rw-r--r--   0     1001      123    12981 2023-05-30 06:44:40.000000 fastpdb-1.2.0/python-src/fastpdb/__init__.py
+-rw-r--r--   0     1001      123    29399 2023-05-30 06:44:40.000000 fastpdb-1.2.0/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-05-30 06:44:40.000000 fastpdb-1.2.0/tests/__init__.py
+-rw-r--r--   0     1001      123   116316 2023-05-30 06:44:40.000000 fastpdb-1.2.0/tests/data/1aki.pdb
+-rw-r--r--   0     1001      123  4394655 2023-05-30 06:44:40.000000 fastpdb-1.2.0/tests/data/1crr.pdb
+-rw-r--r--   0     1001      123   172773 2023-05-30 06:44:40.000000 fastpdb-1.2.0/tests/data/1dix.pdb
+-rw-r--r--   0     1001      123   464373 2023-05-30 06:44:40.000000 fastpdb-1.2.0/tests/data/1f2n.pdb
+-rw-r--r--   0     1001      123  2933577 2023-05-30 06:44:41.000000 fastpdb-1.2.0/tests/data/1gya.pdb
+-rw-r--r--   0     1001      123  1139022 2023-05-30 06:44:41.000000 fastpdb-1.2.0/tests/data/1igy.pdb
+-rw-r--r--   0     1001      123   959040 2023-05-30 06:44:41.000000 fastpdb-1.2.0/tests/data/1l2y.pdb
+-rw-r--r--   0     1001      123   228825 2023-05-30 06:44:41.000000 fastpdb-1.2.0/tests/data/1o1z.pdb
+-rw-r--r--   0     1001      123  1278585 2023-05-30 06:44:41.000000 fastpdb-1.2.0/tests/data/2axd.pdb
+-rw-r--r--   0     1001      123   270054 2023-05-30 06:44:41.000000 fastpdb-1.2.0/tests/data/3o5r.pdb
+-rw-r--r--   0     1001      123   348948 2023-05-30 06:44:41.000000 fastpdb-1.2.0/tests/data/4gxy.pdb
+-rw-r--r--   0     1001      123   221940 2023-05-30 06:44:41.000000 fastpdb-1.2.0/tests/data/4p5j.pdb
+-rw-r--r--   0     1001      123   297351 2023-05-30 06:44:41.000000 fastpdb-1.2.0/tests/data/5h73.pdb
+-rw-r--r--   0     1001      123   342630 2023-05-30 06:44:41.000000 fastpdb-1.2.0/tests/data/5ugo.pdb
+-rw-r--r--   0     1001      123     1377 2023-05-30 06:44:41.000000 fastpdb-1.2.0/tests/data/missing_CRYST1.pdb
+-rw-r--r--   0     1001      123     4966 2023-05-30 06:44:41.000000 fastpdb-1.2.0/tests/test_fastpdb.py
+-rw-r--r--   0     1001      123      777 2023-05-30 06:44:41.000000 fastpdb-1.2.0/tests/test_version.py
+-rw-r--r--   0     1001      123     8806 2023-05-30 06:46:16.000000 fastpdb-1.2.0/Cargo.lock
+-rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 fastpdb-1.2.0/PKG-INFO
```

### Comparing `fastpdb-1.1.0/.github/workflows/test_and_deploy.yml` & `fastpdb-1.2.0/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/.gitignore` & `fastpdb-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/LICENSE` & `fastpdb-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/README.rst` & `fastpdb-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/benchmark.py` & `fastpdb-1.2.0/benchmark.py`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/pyproject.toml` & `fastpdb-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [project]
 name = "fastpdb"
-version = "1.1.0"
+version = "1.2.0"
 description = "A high performance drop-in replacement for Biotite's PDBFile."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["pdb-files"]
 authors = [
   {name = "Patrick Kunzmann"},
+  {name = "Nick Coish"}
 ]
 maintainers = [
   {name = "Patrick Kunzmann"}
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
@@ -20,15 +21,15 @@
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
 ]
 dependencies = [
-  "biotite >= 0.29"
+  "biotite >= 0.37"
 ]
 
 [project.urls]
 homepage = "https://github.com/biotite-dev/fastpdb"
 repository = "https://github.com/biotite-dev/fastpdb"
 
 [tool.maturin]
```

### Comparing `fastpdb-1.1.0/python-src/fastpdb/__init__.py` & `fastpdb-1.2.0/python-src/fastpdb/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "fastpdb"
 __author__ = "Patrick Kunzmann"
 __all__ = ["PDBFile"]
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 
 import os
 import numpy as np
 from biotite.file import is_text
 import biotite.structure as struc
 from biotite.structure.io.pdb import PDBFile as BiotitePDBFile
 from .fastpdb import PDBFile as RustPDBFile
@@ -29,14 +29,15 @@
         else:
             if not is_text(file):
                 raise TypeError("A file opened in 'text' mode is required")
             pdb_file._pdb_file = RustPDBFile(file.read().splitlines())
     
         # Synchronize with PDB file representation in Rust            
         pdb_file.lines = pdb_file._pdb_file.lines
+        pdb_file._index_models_and_atoms()
         return pdb_file
     
     def get_model_count(self):
         return self._pdb_file.get_model_count()
     
     def get_remark(self, number):
         return self._pdb_file.parse_remark(int(number))
@@ -170,20 +171,20 @@
             atoms.box = None
         else:
             len_a, len_b, len_c, alpha, beta, gamma = box
             box = struc.vectors_from_unitcell(
                 len_a, len_b, len_c,
                 np.deg2rad(alpha), np.deg2rad(beta), np.deg2rad(gamma)
             )
-        if isinstance(atoms, struc.AtomArray):
-            atoms.box = box
-        else:
-            atoms.box = np.repeat(
-                box[np.newaxis, ...], atoms.stack_depth(), axis=0
-            )
+            if isinstance(atoms, struc.AtomArray):
+                atoms.box = box
+            else:
+                atoms.box = np.repeat(
+                    box[np.newaxis, ...], atoms.stack_depth(), axis=0
+                )
         
 
         # Filter altloc IDs
         if altloc == "occupancy":
             filter = struc.filter_highest_occupancy_altloc(
                 atoms, altloc_id, occupancy
             )
@@ -199,22 +200,15 @@
             raise ValueError(f"'{altloc}' is not a valid 'altloc' option")
         
 
         if include_bonds:
             bond_list = struc.BondList(
                 atoms.array_length(), self._pdb_file.parse_bonds(atom_id)
             )
-            bond_list = bond_list.merge(struc.connect_via_residue_names(
-                atoms,
-                # The information for non-hetero residues and water
-                # are not part of CONECT records
-                (~atoms.hetero) | struc.filter_solvent(atoms)
-            ))
-            # Remove bond order from inter residue bonds for consistency
-            bond_list.remove_bond_order()
+            bond_list = bond_list.merge(struc.connect_via_residue_names(atoms))
             atoms.bonds = bond_list
 
 
         return atoms
     
 
     def set_structure(self, atoms):
@@ -314,8 +308,15 @@
             atom_id = np.arange(1, atoms.array_length()+1, dtype=np.int64) \
                       if atom_id is None else atom_id
             self._pdb_file.write_bonds(
                 bonds.astype(np.int32, copy=False), atom_id
             )
 
         # Synchronize with PDB file representation in Rust            
-        self.lines = self._pdb_file.lines
+        self.lines = self._pdb_file.lines
+        self._index_models_and_atoms()
+    
+
+    def _index_models_and_atoms(self):
+        self._pdb_file.index_models_and_atoms()
+        self._model_start_i = self._pdb_file.model_start_i
+        self._atom_line_i = self._pdb_file.atom_line_i
```

### Comparing `fastpdb-1.1.0/src/lib.rs` & `fastpdb-1.2.0/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -20,57 +20,93 @@
 
 
 /// Used to allow a function to process both, `AtomArray` and `AtomArrayStack` objects,
 /// since they differ only in the shape of the objects.
 #[derive(Debug)]
 enum CoordArray {
     Single(Array<f32, Ix2>),
-    Multi(Array<f32, Ix3>),
+    Multi(Array<f32, Ix3>)
 }
 
 
 /// This is a low-level abstraction of a PDB file.
 /// While the actual file input and output is managed in Python, this struct is able to parse
 /// coordinates, models, bonds etc. from lines of text and vice versa.
 #[pyclass]
 struct PDBFile {
     /// Lines of text from the PDB file.
     #[pyo3(get)]
-    lines: Vec<String>
+    lines: Vec<String>,
+    model_start_i: Vec<usize>,
+    atom_line_i: Vec<usize>
 }
 
 
 #[pymethods]
 impl PDBFile {
     
     /// Create an new [`PDBFile`].
     /// The lines of text are given to `lines`.
     /// An empty `Vec` represents and empty PDB file.
     #[new]
     fn new(lines: Vec<String>) -> Self {
         //let ljust_lines = lines.iter().map(|line| format!("{:<80}", line)).collect();
-        PDBFile { lines: lines }
+        let mut pdb_file = PDBFile {
+            lines: lines,
+            model_start_i: Vec::new(),
+            atom_line_i: Vec::new()
+        };
+        pdb_file.index_models_and_atoms();
+        pdb_file
     }
 
 
     /// Read a [`PDBFile`] from a file.
     /// The file is indicated by its file path as `String`.
     #[staticmethod]
     fn read(file_path: &str) -> PyResult<Self> {
         let contents = fs::read_to_string(file_path).map_err(
             |_| exceptions::PyOSError::new_err(format!("'{}' cannot be read", file_path))
         )?;
-        let lines = contents.lines().map(|line| format!("{:<80}", line)).collect();
-        Ok(PDBFile { lines: lines })
+        let lines = contents.lines().map(
+            |line| format!("{:<80}", line)
+        ).collect();
+        let mut pdb_file = PDBFile {
+            lines: lines,
+            model_start_i: Vec::new(),
+            atom_line_i: Vec::new()
+        };
+        pdb_file.index_models_and_atoms();
+        Ok(pdb_file)
+    }
+
+
+    #[getter]
+    fn model_start_i(&self) -> PyResult<Py<PyArray<i64, Ix1>>> {
+        Python::with_gil(|py| {
+            Ok(PyArray::from_iter(
+                py, self.model_start_i.iter().map(|x| *x as i64)
+            ).to_owned())
+        })
+    }
+
+
+    #[getter]
+    fn atom_line_i(&self) -> PyResult<Py<PyArray<i64, Ix1>>> {
+        Python::with_gil(|py| {
+            Ok(PyArray::from_iter(
+                py, self.atom_line_i.iter().map(|x| *x as i64)
+            ).to_owned())
+        })
     }
 
     
     /// Get the number of models contained in the file.
     fn get_model_count(&self) -> usize {
-        self.get_model_start_indices().len()
+        self.model_start_i.len()
     }
 
 
     /// Parse the given `REMARK` record of the PDB file to obtain its content as strings
     fn parse_remark(&self, number: i64) -> PyResult<Option<Vec<String>>> {
         const CONTENT_START_COLUMN: usize = 11;
 
@@ -170,18 +206,15 @@
                                                            Py<PyArray<u32,  Ix2>>,
                                                            Py<PyArray<u32,  Ix2>>,
                                                            Py<PyArray<u32,  Ix2>>,
                                                            Option<Py<PyArray<i64,  Ix1>>>,
                                                            Option<Py<PyArray<f64,  Ix1>>>,
                                                            Option<Py<PyArray<f64,  Ix1>>>,
                                                            Option<Py<PyArray<i64,  Ix1>>>)> {
-        let model_start_i = self.get_model_start_indices();
-        let (model_start, model_stop) = self.get_model_boundaries(model, &model_start_i)?;
-
-        let atom_line_i: Vec<usize> = self.get_atom_indices(model_start, model_stop);
+        let atom_line_i: Vec<usize> = self.get_atom_indices(model)?;
         
         let mut chain_id:  Array<u32,  Ix2> = Array::zeros((atom_line_i.len(), 4));
         let mut res_id:    Array<i64,  Ix1> = Array::zeros(atom_line_i.len());
         let mut ins_code:  Array<u32,  Ix2> = Array::zeros((atom_line_i.len(), 1));
         let mut res_name:  Array<u32,  Ix2> = Array::zeros((atom_line_i.len(), 3));
         let mut hetero:    Array<bool, Ix1> = Array::default(atom_line_i.len());
         let mut atom_name: Array<u32,  Ix2> = Array::zeros((atom_line_i.len(), 6));
@@ -471,141 +504,132 @@
                 if n_added > 0 {
                     self.lines.push(line);
                 }
             }
             Ok(())
         })
     }
+
+    /// Index lines in the file that correspond to starts of new models and to
+    /// `ATOM` or `HETATM` records.
+    /// Must be called after the content of the file has been changed.
+    fn index_models_and_atoms(&mut self) {
+        self.atom_line_i = self.lines.iter().enumerate()
+            .filter(|(_i, line)| line.starts_with("ATOM") || line.starts_with("HETATM"))
+            .map(|(i, _line)| i)
+            .collect();
+        self.model_start_i= self.lines.iter().enumerate()
+            .filter(|(_i, line)| line.starts_with("MODEL"))
+            .map(|(i, _line)| i)
+            .collect();
+        // It could be an empty file or a file with a single model,
+        // where the 'MODEL' line is missing
+        if self.model_start_i.is_empty() && !self.atom_line_i.is_empty(){
+            self.model_start_i = vec![0]
+        }
+    }
 }
 
 
 impl PDBFile {
 
     /// Get a *NumPy* array containing coordinates for a single model (2D) or
     /// multiple models (3D) in the file.
     /// The number of returned dimensions is based on whether a `model` is
     /// given.
     fn parse_coord(&self, model: Option<isize>) -> PyResult<CoordArray> {
-        let model_start_i = self.get_model_start_indices();
-        
-        let (model_start, model_stop) = match model {
-            Some(model_number) => self.get_model_boundaries(model_number, &model_start_i)?,
-            None => (0, self.lines.len())
-        };
-    
-        let atom_line_i: Vec<usize> = self.get_atom_indices(model_start, model_stop);
-        
-        let mut coord = Array::zeros((atom_line_i.len(), 3));
-        for (atom_i, line_i) in atom_line_i.iter().enumerate() {
-            let line = &self.lines[*line_i];
-            if line.len() < 80 {
-                return Err(biotite::InvalidFileError::new_err("Line is too short"))
-            }
-            coord[[atom_i, 0]] = line[30..38].trim().parse().map_err(|_|
-                biotite::InvalidFileError::new_err(format!(
-                    "'{}' cannot be parsed into a float", line[30..38].trim()
-                ))
-            )?;
-            coord[[atom_i, 1]] = line[38..46].trim().parse().map_err(|_|
-                biotite::InvalidFileError::new_err(format!(
-                    "'{}' cannot be parsed into a float", line[38..46].trim()
-                ))
-            )?;
-            coord[[atom_i, 2]] = line[46..54].trim().parse().map_err(|_|
-                biotite::InvalidFileError::new_err(format!(
-                    "'{}' cannot be parsed into a float", line[46..54].trim()
-                ))
-            )?;
-        }
-        
         match model {
-            Some(_) => Ok(CoordArray::Single(coord)),
+            Some(model_number) => {
+                let atom_line_i = self.get_atom_indices(model_number)?;
+                let mut coord = Array::zeros((atom_line_i.len(), 3));
+                for (atom_i, line_i) in atom_line_i.iter().enumerate() {
+                    let line = &self.lines[*line_i];
+                    if line.len() < 80 {
+                        return Err(biotite::InvalidFileError::new_err("Line is too short"))
+                    }
+                    coord[[atom_i, 0]] = parse_float_from_string(line, 30, 38)?;
+                    coord[[atom_i, 1]] = parse_float_from_string(line, 38, 46)?;
+                    coord[[atom_i, 2]] = parse_float_from_string(line, 46, 54)?;
+                }
+                Ok(CoordArray::Single(coord))
+            },
+            
             None => {
-                // Check whether all models have the same length
-                let length = self.get_model_length(&model_start_i, &atom_line_i)?;
+                let length = self.get_model_length()?;
+                let mut coord = Array::zeros((self.atom_line_i.len(), 3));
+                for (atom_i, line_i) in self.atom_line_i.iter().enumerate() {
+                    let line = &self.lines[*line_i];
+                    if line.len() < 80 {
+                        return Err(biotite::InvalidFileError::new_err("Line is too short"))
+                    }
+                    coord[[atom_i, 0]] = parse_float_from_string(line, 30, 38)?;
+                    coord[[atom_i, 1]] = parse_float_from_string(line, 38, 46)?;
+                    coord[[atom_i, 2]] = parse_float_from_string(line, 46, 54)?;
+                }
                 Ok(
-                    CoordArray::Multi(coord.into_shape((model_start_i.len(), length, 3))
+                    CoordArray::Multi(coord.into_shape((self.model_start_i.len(), length, 3))
                     .expect("Model length is invalid"))
                 )
             }
         }
     }
 
 
-    /// Get indices to lines of text containing `ATOM` and `HETATM` records.
-    /// The indices are limited to the range of a model given by the `model_start`
-    /// and the exclusive `model_stop`.
-    fn get_atom_indices(&self, model_start: usize, model_stop: usize) -> Vec<usize> {
-        self.lines[model_start..model_stop].iter().enumerate()
-            .filter(|(_i, line)| line.starts_with("ATOM") || line.starts_with("HETATM"))
-            .map(|(i, _line)| i + model_start)
-            .collect()
-    }
-
-    
-    /// Get indices to lines of text containing `MODEL` records.
-    /// If no `MODEL` records is found, which occurs frequently in PDB files containing only one
-    /// model, a single start at the beginning of the file is returned.
-    fn get_model_start_indices(&self) -> Vec<usize> {
-        let mut model_start_i: Vec<usize> = self.lines.iter().enumerate()
-            .filter(|(_i, line)| line.starts_with("MODEL"))
-            .map(|(i, _line)| i)
-            .collect();
-        // Structures containing only one model may omit MODEL record
-        // In these cases model starting index is set to 0
-        if model_start_i.is_empty() {
-            model_start_i = vec![0]
-        }
-        model_start_i
-    }
-    
-
-    /// Find the model start and stop index for the given `model` number (1-based).
-    /// `model_start_i` is the return value of [`get_model_start_indices()`].
-    fn get_model_boundaries(&self,
-                            model: isize,
-                            model_start_i: &[usize]) -> PyResult<(usize, usize)> {
+    /// Get indices to `ATOM` and `HETATM` records within the given model number.
+    fn get_atom_indices(&self, model: isize) -> PyResult<Vec<usize>> {
+        // Find the model index corresponding to the given model number
         let model_i: isize;
         match model.cmp(&0) {
             Ordering::Greater => model_i = model - 1,
-            Ordering::Less => model_i = model_start_i.len() as isize + model,
+            Ordering::Less => model_i = self.model_start_i.len() as isize + model,
             Ordering::Equal => return Err(exceptions::PyValueError::new_err(
                 "Model index must not be 0"
             )),
         };
-    
-        if model_i >= model_start_i.len() as isize || model_i < 0 {
+        if model_i >= self.model_start_i.len() as isize || model_i < 0 {
             return Err(exceptions::PyValueError::new_err(format!(
                 "The file has {} models, the given model {} does not exist",
-                model_start_i.len(), model
+                self.model_start_i.len(), model
             )));
         }
-    
-        if model_i == model_start_i.len() as isize - 1 {
+        
+        // Get the start and stop line index for this model index
+        let (model_start, model_stop) = match model_i.cmp(&(self.model_start_i.len() as isize - 1)){
+            Ordering::Less => (
+                self.model_start_i[model_i as usize],
+                self.model_start_i[(model_i+1) as usize]
+            ),
             // Last model -> Model reaches to end of file
-            Ok((model_start_i[model_i as usize], self.lines.len()))
-        }
-        else {
-            Ok((model_start_i[model_i as usize], model_start_i[(model_i+1) as usize]))
-        }
+            Ordering::Equal => (
+                self.model_start_i[model_i as usize], 
+                self.lines.len()
+            ),
+            // This case was excluded above
+            _ => panic!("This branch should not be reached")
+        };
+        
+        // Get the atom records within these line boundaries
+        Ok(
+            self.atom_line_i.iter().copied()
+                .filter(|i| *i >= model_start && *i < model_stop)
+                .collect()
+        )
     }
     
 
     /// Get the number of atoms in each model of the PDB file.
     /// A `PyErr` is returned if the number of atoms per model differ from each other.
-    fn get_model_length(&self,
-                        model_start_i: &[usize],
-                        atom_line_i: &[usize]) -> PyResult<usize> {
-        let n_models = model_start_i.len();
+    fn get_model_length(&self) -> PyResult<usize> {
+        let n_models = self.model_start_i.len();
         let mut length: Option<usize> = None;
         for model_i in 0..n_models {
-            let model_start: usize = model_start_i[model_i];
-            let model_stop: usize = if model_i+1 < n_models { model_start_i[model_i+1] }
+            let model_start: usize = self.model_start_i[model_i];
+            let model_stop: usize = if model_i+1 < n_models { self.model_start_i[model_i+1] }
                                     else { self.lines.len() };
-            let model_length = atom_line_i.iter()
+            let model_length = self.atom_line_i.iter()
                 .filter(|&line_i| *line_i >= model_start && *line_i < model_stop)
                 .count();
             match length {
                 None => length = Some(model_length),
                 Some(l) => if model_length != l { return Err(biotite::InvalidFileError::new_err(
                     "Inconsistent number of models"
                 )); }
@@ -668,14 +692,23 @@
         || Err(biotite::InvalidFileError::new_err(format!(
             "'{}' cannot be parsed into a number", digit)
         )),
         |v| Ok(v as i64)
     )
 }
 
+//
+fn parse_float_from_string(line: &str, start: usize, stop: usize) -> PyResult<f32>{
+    line[start..stop].trim().parse().map_err(|_|
+        biotite::InvalidFileError::new_err(format!(
+            "'{}' cannot be parsed into a float", line[start..stop].trim()
+        ))
+    )
+}
+
 
 /// If a given `id` exceeds `max_id` the returned ID restarts counting at 1.
 /// Otherwise, `id` is returned.
 /// This function is necessary, because there is a maximum number for atom and residue IDs in
 /// PDB files.
 #[inline(always)]
 fn truncate_id(id: i64, max_id: i64) -> i64 {
```

### Comparing `fastpdb-1.1.0/tests/data/1aki.pdb` & `fastpdb-1.2.0/tests/data/1aki.pdb`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/tests/data/1crr.pdb` & `fastpdb-1.2.0/tests/data/1crr.pdb`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/tests/data/1dix.pdb` & `fastpdb-1.2.0/tests/data/1dix.pdb`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/tests/data/1f2n.pdb` & `fastpdb-1.2.0/tests/data/1f2n.pdb`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/tests/data/1gya.pdb` & `fastpdb-1.2.0/tests/data/1gya.pdb`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/tests/data/1igy.pdb` & `fastpdb-1.2.0/tests/data/1igy.pdb`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/tests/data/1l2y.pdb` & `fastpdb-1.2.0/tests/data/1l2y.pdb`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/tests/data/1o1z.pdb` & `fastpdb-1.2.0/tests/data/1o1z.pdb`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/tests/data/2axd.pdb` & `fastpdb-1.2.0/tests/data/2axd.pdb`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/tests/data/3o5r.pdb` & `fastpdb-1.2.0/tests/data/3o5r.pdb`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/tests/data/4gxy.pdb` & `fastpdb-1.2.0/tests/data/4gxy.pdb`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/tests/data/4p5j.pdb` & `fastpdb-1.2.0/tests/data/4p5j.pdb`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/tests/data/5h73.pdb` & `fastpdb-1.2.0/tests/data/5h73.pdb`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/tests/data/5ugo.pdb` & `fastpdb-1.2.0/tests/data/5ugo.pdb`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/tests/test_fastpdb.py` & `fastpdb-1.2.0/tests/test_fastpdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         model, altloc, extra_fields, include_bonds
     )
 
     
     if ref_atoms.box is not None:
         assert np.allclose(test_atoms.box, ref_atoms.box)
     else:
-        assert test_atoms == None
+        assert test_atoms.box is None
     
     assert test_atoms.bonds == ref_atoms.bonds
     
     for category in ref_atoms.get_annotation_categories():
         if np.issubdtype(ref_atoms.get_annotation(category).dtype, float):
             assert test_atoms.get_annotation(category).tolist() \
                 == pytest.approx(ref_atoms.get_annotation(category).tolist())
```

### Comparing `fastpdb-1.1.0/tests/test_version.py` & `fastpdb-1.2.0/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `fastpdb-1.1.0/Cargo.lock` & `fastpdb-1.2.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "fastpdb"
-version = "1.1.0"
+version = "1.2.0"
 dependencies = [
  "ndarray",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
@@ -65,34 +65,35 @@
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if 1.0.0",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "matrixmultiply"
-version = "0.3.2"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
+checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
+ "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "ndarray"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -145,17 +146,17 @@
  "num-complex",
  "num-traits",
  "pyo3",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
 
 [[package]]
 name = "parking_lot"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
 dependencies = [
@@ -201,17 +202,17 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.14.5"
@@ -258,17 +259,17 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rawpointer"
 version = "0.2.1"
@@ -294,28 +295,28 @@
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
```

### Comparing `fastpdb-1.1.0/PKG-INFO` & `fastpdb-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: fastpdb
-Version: 1.1.0
+Version: 1.2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Dist: biotite >= 0.29
+Requires-Dist: biotite >= 0.37
 License-File: LICENSE
 Summary: A high performance drop-in replacement for Biotite's PDBFile.
 Keywords: pdb-files
-Author: Patrick Kunzmann
+Author: Patrick Kunzmann, Nick Coish
 Maintainer: Patrick Kunzmann
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 Project-URL: homepage, https://github.com/biotite-dev/fastpdb
 Project-URL: repository, https://github.com/biotite-dev/fastpdb
 
 .. image:: https://raw.githubusercontent.com/biotite-dev/fastpdb/main/logo.svg
```

