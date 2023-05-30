# Comparing `tmp/nb_helpers-0.5.2.tar.gz` & `tmp/nb_helpers-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_helpers-0.5.2.tar", last modified: Mon May 22 16:44:20 2023, max compression
+gzip compressed data, was "nb_helpers-0.5.3.tar", last modified: Tue May 30 20:43:29 2023, max compression
```

## Comparing `nb_helpers-0.5.2.tar` & `nb_helpers-0.5.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:44:20.022426 nb_helpers-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-22 16:44:20.022426 nb_helpers-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:44:20.022426 nb_helpers-0.5.2/nb_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/colab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:44:20.022426 nb_helpers-0.5.2/nb_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-22 16:44:19.000000 nb_helpers-0.5.2/nb_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-22 16:44:19.000000 nb_helpers-0.5.2/nb_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:44:19.000000 nb_helpers-0.5.2/nb_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-22 16:44:19.000000 nb_helpers-0.5.2/nb_helpers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:44:19.000000 nb_helpers-0.5.2/nb_helpers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 16:44:19.000000 nb_helpers-0.5.2/nb_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 16:44:19.000000 nb_helpers-0.5.2/nb_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:44:20.022426 nb_helpers-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:43:29.277111 nb_helpers-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-30 20:43:29.277111 nb_helpers-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:43:29.277111 nb_helpers-0.5.3/nb_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/colab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:43:29.277111 nb_helpers-0.5.3/nb_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-30 20:43:29.000000 nb_helpers-0.5.3/nb_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-30 20:43:29.000000 nb_helpers-0.5.3/nb_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:43:29.000000 nb_helpers-0.5.3/nb_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-30 20:43:29.000000 nb_helpers-0.5.3/nb_helpers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:43:29.000000 nb_helpers-0.5.3/nb_helpers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-30 20:43:29.000000 nb_helpers-0.5.3/nb_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 20:43:29.000000 nb_helpers-0.5.3/nb_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:43:29.277111 nb_helpers-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/setup.py
```

### Comparing `nb_helpers-0.5.2/LICENSE` & `nb_helpers-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.2/PKG-INFO` & `nb_helpers-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_helpers
-Version: 0.5.2
+Version: 0.5.3
 Summary: A set of tools for nb handling
 Home-page: https://github.com/wandb/nb_helpers/tree/main/
 Author: Thomas Capelle
 Author-email: tcapelle@wandb.com
 License: MIT License
 Keywords: jupyter notebook
 Platform: UNKNOWN
```

### Comparing `nb_helpers-0.5.2/README.md` & `nb_helpers-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.2/nb_helpers/_modidx.py` & `nb_helpers-0.5.3/nb_helpers/_modidx.py`

 * *Files 10% similar despite different names*

```diff
@@ -77,14 +77,17 @@
                                   'nb_helpers.utils.git_branches': ('utils.html#git_branches', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.git_current_branch': ('utils.html#git_current_branch', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.git_last_commit': ('utils.html#git_last_commit', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.git_local_repo': ('utils.html#git_local_repo', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.git_main_name': ('utils.html#git_main_name', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.git_origin_repo': ('utils.html#git_origin_repo', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.is_nb': ('utils.html#is_nb', 'nb_helpers/utils.py'),
+                                  'nb_helpers.utils.load_list_from_file': ('utils.html#load_list_from_file', 'nb_helpers/utils.py'),
+                                  'nb_helpers.utils.load_notebooks_from_file': ( 'utils.html#load_notebooks_from_file',
+                                                                                 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.print_output': ('utils.html#print_output', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.remove_rich_format': ('utils.html#remove_rich_format', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.search_cell': ('utils.html#search_cell', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.search_cells': ('utils.html#search_cells', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.search_string_in_nb': ('utils.html#search_string_in_nb', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.today': ('utils.html#today', 'nb_helpers/utils.py')},
             'nb_helpers.wandb': { 'nb_helpers.wandb.filter_nbs': ('wandb.html#filter_nbs', 'nb_helpers/wandb.py'),
```

### Comparing `nb_helpers-0.5.2/nb_helpers/actions.py` & `nb_helpers-0.5.3/nb_helpers/actions.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.2/nb_helpers/clean.py` & `nb_helpers-0.5.3/nb_helpers/clean.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.2/nb_helpers/colab.py` & `nb_helpers-0.5.3/nb_helpers/colab.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.2/nb_helpers/docker.py` & `nb_helpers-0.5.3/nb_helpers/docker.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.2/nb_helpers/export.py` & `nb_helpers-0.5.3/nb_helpers/export.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.2/nb_helpers/run.py` & `nb_helpers-0.5.3/nb_helpers/run.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.2/nb_helpers/utils.py` & `nb_helpers-0.5.3/nb_helpers/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_utils.ipynb.
 
 # %% auto 0
 __all__ = ['LOGFORMAT', 'LOGFORMAT_RICH', 'STATUS', 'CellType', 'create_table', 'remove_rich_format', 'csv_to_md', 'RichLogger',
-           'is_nb', 'find_nbs', 'print_output', 'search_cell', 'search_cells', 'search_string_in_nb', 'extract_libs',
-           'detect_imported_libs', 'get_repo', 'git_current_branch', 'git_branches', 'git_main_name', 'git_origin_repo',
-           'git_local_repo', 'git_last_commit', 'today']
+           'is_nb', 'load_list_from_file', 'load_notebooks_from_file', 'find_nbs', 'print_output', 'search_cell',
+           'search_cells', 'search_string_in_nb', 'extract_libs', 'detect_imported_libs', 'get_repo',
+           'git_current_branch', 'git_branches', 'git_main_name', 'git_origin_repo', 'git_local_repo',
+           'git_last_commit', 'today']
 
 # %% ../nbs/02_utils.ipynb 3
 import io, json, sys, re, csv, logging
 import git
 from types import SimpleNamespace
 from logging import Formatter
 from logging.handlers import RotatingFileHandler
@@ -183,59 +184,71 @@
 
 # %% ../nbs/02_utils.ipynb 22
 def is_nb(fname: Path):
     "filter files that are jupyter notebooks"
     return (fname.suffix == ".ipynb") and (not fname.name.startswith("_")) and (not "checkpoint" in str(fname))  and (not fname.is_symlink())
 
 # %% ../nbs/02_utils.ipynb 24
+def load_list_from_file(path: Path):
+    "Load a list from a file"
+    return path.read_text().split("\n")
+
+def load_notebooks_from_file(path: Path):
+    "Load a list of notebooks from a file"
+    files = [Path(f) for f in load_list_from_file(path)]
+    return [f.resolve() for f in files if is_nb(f)]
+
+# %% ../nbs/02_utils.ipynb 26
 def find_nbs(path: Path):
     "Get all nbs on path recursively"
     path = Path(path).resolve()
     if is_nb(path):
         return [path]
+    if path.suffix == ".txt":
+        return load_notebooks_from_file(path)
     return L([nb.resolve() for nb in path.rglob("*.ipynb") if is_nb(nb)]).sorted()
 
-# %% ../nbs/02_utils.ipynb 28
+# %% ../nbs/02_utils.ipynb 31
 def print_output(notebook):  # pragma: no cover
     "Print `notebook` in stdout for git things"
     output_stream = io.TextIOWrapper(sys.stdout.buffer, encoding="utf-8")
     x = json.dumps(notebook, sort_keys=True, indent=1, ensure_ascii=False)
     output_stream.write(x)
     output_stream.write("\n")
     output_stream.flush()
 
-# %% ../nbs/02_utils.ipynb 30
+# %% ../nbs/02_utils.ipynb 33
 CellType = SimpleNamespace(code="code", md="markdown")
 
-# %% ../nbs/02_utils.ipynb 31
+# %% ../nbs/02_utils.ipynb 34
 def search_cell(cell, string) -> bool:
     "Search string in cell source, can be a list"
     source = listify(cell["source"])
     source = "".join(source)
     if string in source:
         return True
     return False
 
-# %% ../nbs/02_utils.ipynb 34
+# %% ../nbs/02_utils.ipynb 37
 def search_cells(nb, string: str = None, cell_type=CellType.code):
     "Get cells containing string, you can pass comma separated strings"
     strings = ifnone(string, "").replace(" ", "").split(",")
     cells = []
     for cell in nb["cells"]:
         if cell["cell_type"] == cell_type:
             if any([search_cell(cell, string) for string in strings]):
                 cells.append(cell["source"])
     return cells
 
-# %% ../nbs/02_utils.ipynb 38
+# %% ../nbs/02_utils.ipynb 41
 def search_string_in_nb(nb, string: str = None, cell_type=CellType.code):
     "Check if string is present in notebook cells, you can pass comma separated strings"
     return len(search_cells(nb, string, cell_type)) > 0
 
-# %% ../nbs/02_utils.ipynb 41
+# %% ../nbs/02_utils.ipynb 44
 def extract_libs(strings):
     "Automatically detect libraries imported in `strings`"
 
     after_import_regex = re.compile(r"^import\s([^\.]*)", re.VERBOSE)
     before_as_regex = re.compile(r"([^\s]*?)\sas\s", re.VERBOSE)
     between_from_import_regex = re.compile(r"^from\s(.*?)\simport", re.VERBOSE)
 
@@ -254,89 +267,89 @@
             string = _search_with_regex(after_import_regex, string)
             if "as" in string:
                 string = _search_with_regex(before_as_regex, string)
         if string:
             libs.append(string.replace(" ", "").split(","))
     return L(libs).concat().unique()
 
-# %% ../nbs/02_utils.ipynb 45
+# %% ../nbs/02_utils.ipynb 48
 def detect_imported_libs(notebook):
     "Guess imported libs from notebook"
     text_list = L(search_cells(notebook, "import,from")).concat()
 
     # format lines
     text_list = L([x.split("\n") for x in text_list]).concat()
     text_list = [line for line in text_list if (("from" in line) or ("import" in line))]
 
     return extract_libs(text_list)
 
-# %% ../nbs/02_utils.ipynb 49
+# %% ../nbs/02_utils.ipynb 52
 def get_repo(fname) -> git.Repo:
     try:
         repo = git.Repo(fname, search_parent_directories=True)
         return repo
     except Exception as e:
         raise Exception(f"Probably not in a git repo: {e}")
 
-# %% ../nbs/02_utils.ipynb 51
+# %% ../nbs/02_utils.ipynb 54
 def git_current_branch(fname) -> str:
     "Get current git branch"
     repo = get_repo(fname)
     try:
         return repo.active_branch.name
     except Exception as e:
         return "master"
 
-# %% ../nbs/02_utils.ipynb 53
+# %% ../nbs/02_utils.ipynb 56
 def git_branches(repo: git.Repo, remote=True):
     "Get all remote or local banches"
     branches = set([b.name for b in repo.branches])
     remote_branches =  set([r.name.split("/")[-1] for r in repo.remote().refs])
     return branches.union(remote_branches) if remote else branches
 
-# %% ../nbs/02_utils.ipynb 55
+# %% ../nbs/02_utils.ipynb 58
 def git_main_name(fname) -> str:
     "Get the name of master/main branch"
     repo = get_repo(fname)
     branches = git_branches(repo)
     return "main" if "main" in branches else "master"
 
-# %% ../nbs/02_utils.ipynb 57
+# %% ../nbs/02_utils.ipynb 60
 def _get_github_repo_remote(repo_url):
     if "git@" in repo_url:
         github_repo = re.search(r".com:(.*).git", repo_url).group(1)
     else:
         github_repo = re.search(r".com/(.*)", repo_url).group(1)
     return github_repo
 
-# %% ../nbs/02_utils.ipynb 59
+# %% ../nbs/02_utils.ipynb 62
 def git_origin_repo(fname):
     "Get github repo name from `fname`"
     repo = get_repo(fname)
     repo_url = repo.remote().url
 
     # check if ssh or html
     if repo_url != "":
         return _get_github_repo_remote(repo_url)
     else:
         raise Exception(f"Not in a valid github repo: {fname=}")
 
-# %% ../nbs/02_utils.ipynb 61
+# %% ../nbs/02_utils.ipynb 64
 def git_local_repo(fname):
     "Get local github repo path"
     repo = get_repo(fname)
     return Path(repo.git_dir).parent.resolve()
 
-# %% ../nbs/02_utils.ipynb 63
+# %% ../nbs/02_utils.ipynb 66
 def git_last_commit(fname):
     "Gets the last commit on fname"
     repo = get_repo(fname)
     return repo.commit().hexsha
 
-# %% ../nbs/02_utils.ipynb 66
+# %% ../nbs/02_utils.ipynb 69
 def today():
     "datetime object containing current date and time"
     now = datetime.now()
 
     # dd/mm/YY H:M:S
     dt_string = now.strftime("%d/%m/%Y %H:%M:%S")
     return dt_string
```

### Comparing `nb_helpers-0.5.2/nb_helpers/wandb.py` & `nb_helpers-0.5.3/nb_helpers/wandb.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.2/nb_helpers.egg-info/PKG-INFO` & `nb_helpers-0.5.3/nb_helpers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-helpers
-Version: 0.5.2
+Version: 0.5.3
 Summary: A set of tools for nb handling
 Home-page: https://github.com/wandb/nb_helpers/tree/main/
 Author: Thomas Capelle
 Author-email: tcapelle@wandb.com
 License: MIT License
 Keywords: jupyter notebook
 Platform: UNKNOWN
```

### Comparing `nb_helpers-0.5.2/setup.py` & `nb_helpers-0.5.3/setup.py`

 * *Files identical despite different names*

