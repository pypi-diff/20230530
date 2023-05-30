# Comparing `tmp/skulk-1.4.6rc7-py2.py3-none-any.whl.zip` & `tmp/skulk-1.4.6rc8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8696 bytes, number of entries: 10
--rw-r--r--  2.0 unx       10 b- defN 23-May-29 23:46 skulk/VERSION
--rw-r--r--  2.0 unx        0 b- defN 23-May-29 23:46 skulk/__init__.py
--rw-r--r--  2.0 unx     9029 b- defN 23-May-29 23:46 skulk/bumper.py
--rw-r--r--  2.0 unx     8697 b- defN 23-May-29 23:46 skulk/skulk.py
--rw-r--r--  2.0 unx     2625 b- defN 23-May-29 23:46 skulk/util.py
--rw-r--r--  2.0 unx      649 b- defN 23-May-29 23:46 skulk-1.4.6rc7.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-29 23:46 skulk-1.4.6rc7.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 23-May-29 23:46 skulk-1.4.6rc7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-May-29 23:46 skulk-1.4.6rc7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      749 b- defN 23-May-29 23:46 skulk-1.4.6rc7.dist-info/RECORD
-10 files, 21919 bytes uncompressed, 7424 bytes compressed:  66.1%
+Zip file size: 8922 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       10 b- defN 23-May-30 05:44 skulk/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 23-May-30 05:44 skulk/__init__.py
+-rw-r--r--  2.0 unx     9348 b- defN 23-May-30 05:44 skulk/bumper.py
+-rw-r--r--  2.0 unx     9105 b- defN 23-May-30 05:44 skulk/skulk.py
+-rw-r--r--  2.0 unx     2625 b- defN 23-May-30 05:44 skulk/util.py
+-rw-r--r--  2.0 unx      649 b- defN 23-May-30 05:44 skulk-1.4.6rc8.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-30 05:44 skulk-1.4.6rc8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 23-May-30 05:44 skulk-1.4.6rc8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-May-30 05:44 skulk-1.4.6rc8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      749 b- defN 23-May-30 05:44 skulk-1.4.6rc8.dist-info/RECORD
+10 files, 22646 bytes uncompressed, 7650 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: skulk/skulk.py
 Comment: 
 
 Filename: skulk/util.py
 Comment: 
 
-Filename: skulk-1.4.6rc7.dist-info/METADATA
+Filename: skulk-1.4.6rc8.dist-info/METADATA
 Comment: 
 
-Filename: skulk-1.4.6rc7.dist-info/WHEEL
+Filename: skulk-1.4.6rc8.dist-info/WHEEL
 Comment: 
 
-Filename: skulk-1.4.6rc7.dist-info/entry_points.txt
+Filename: skulk-1.4.6rc8.dist-info/entry_points.txt
 Comment: 
 
-Filename: skulk-1.4.6rc7.dist-info/top_level.txt
+Filename: skulk-1.4.6rc8.dist-info/top_level.txt
 Comment: 
 
-Filename: skulk-1.4.6rc7.dist-info/RECORD
+Filename: skulk-1.4.6rc8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## skulk/VERSION

```diff
@@ -1 +1 @@
-1.4.6-rc.7
+1.4.6-rc.8
```

## skulk/bumper.py

```diff
@@ -8,100 +8,101 @@
 
 from . import util
 
 
 MOCKED = False
 MOCK_VERSIONS = {
     "pypi": ["0.1.7", "1.4.3", "1.4.4", "1.4.5"],
-    "tags": ["0.1.2", "0.1.3", "1.4.4", "1.4.6-rc.1"],
+    "tags": ["0.1.2", "0.1.3", "1.4.4", "1.4.5"],
 }
 
 
 class Bumper(object):
     """A class to help the user bump the version."""
+
     def __init__(self, repo, pip_name):
         self.repo = repo
         self.pip_name = pip_name
         self.version_filename = os.path.join(self.repo.working_dir, "VERSION")
         self.current_version = _read_version_file(self.version_filename)
         self.versions = None
         self.next_version = None
 
         self.latest_pypi_version = None
         self.latest_tag_version = None
-        self.latest_version =  None
+        self.latest_version = None
 
     def is_prerelease(self):
         """Return True if the current version is a prerelease."""
         return semver.Version.parse(self.current_version).prerelease is not None
 
     def run(self):
         """Wizard to choose a version."""
-        
+
         self._set_versions()
-        
+
         print("Versions:")
         print(json.dumps(self.versions, indent=3))
         print(f"The latest version on PyPi is: {self.latest_pypi_version}")
         print(f"The latest tag in the repo is: {self.latest_tag_version}")
         print(
             "When you push this branch, we'll deploy to PyPi and we'll tag the repo with the version you choose."
         )
 
-        if (self.current_version not in self.versions["pypi"] + self.versions["tags"]
-        ):
-            
+        if self.current_version not in self.versions["pypi"] + self.versions["tags"]:
             print(
                 f"The local VERSION file contains a valid version: {self.current_version}."
             )
-            
+
             print("You can use this version or you can bump to a new version.")
             do_bump = util.yes_no("Do you wish to bump the version?")
             if not do_bump:
                 return
-            
+
         else:
             do_bump = True
             print(
                 f"The local VERSION file contains an invalid version: {self.current_version}. It has been used already."
             )
             print("You'll need to bump the version.")
 
         latest = semver.Version.parse(self.latest_version)
 
         version_options = [
-            (latest.next_version(part="prerelease"), "(Pre-release bump only)"),
+            (str(latest.next_version(part="prerelease")), "The next pre-release"),
+            (str(latest.next_version(part="patch")), "The next patch release"),
             (
-                latest.next_version(part="patch").next_version(part="prerelease"),
-                "(Pre-release a new patch)",
+                str(latest.next_version(part="minor").bump_prerelease()),
+                "Pre-release for a new feature",
             ),
+            (str(latest.next_version(part="minor")), "Release a new feature"),
             (
-                latest.next_version(part="minor").next_version(part="prerelease"),
-                "(Pre-release a new feature)",
+                str(latest.next_version(part="major").bump_prerelease()),
+                "Pre-release for a breaking change",
             ),
+            (str(latest.next_version(part="major")), "Release a breaking change"),
+        ]
+
+        version_options += [
+            ("Explicit", "Specify a version manually. This is not recommended."),
             (
-                latest.next_version(part="major").next_version(part="prerelease"),
-                "(Pre-release a breaking change)",
+                "Cancel",
+                "I changed my mind. I don't want to tag or release. I just want to push.",
             ),
-            (latest.next_version(part="patch"), "(Release a new patch)"),
-            (latest.next_version(part="minor"), "(Release a new feature)"),
-            (latest.next_version(part="major"), "(Release a breaking change)"),
-            ("Specify a version", "(Not recommended)"),
-            ("Changed my mind", "(I just want to push with no tag or release)"),
             ("Exit!", ""),
         ]
 
-        options = [f"{v[0]} {v[1]}" for v in version_options]
+        options = [f"{v[0]: <16} {v[1]}" for v in version_options]
         num_options = len(options)
         exit_option = num_options
         no_tags_option = num_options - 1
         custom_option = num_options - 2
 
         bump_type = 0
-        msg = "Choose a new prerelease version"
+        msg = "Choose a new version"
         while bump_type not in range(1, len(options) + 1):
             print(msg)
             for i, opt in enumerate(options):
                 n = i + 1
                 print(f"{n}: {opt}")
             bump_type = input(util.green("Enter a number: "))
             if not bump_type.isdigit():
@@ -168,15 +169,21 @@
         can still deploy there.
         """
 
         # notice this command says: Install version== (i.e. it requests an invalid
         # version). It fails as intended, and the result is a message to say can't
         # find version in versions. It lists the existing versions which we split
         # and return. Check for py3 and py 27 compatible by using both pips.
-        args = ["pip3", "install", "--index-url", util.PROD_PYPI_INDEX, f"{self.pip_name}=="]
+        args = [
+            "pip3",
+            "install",
+            "--index-url",
+            util.PROD_PYPI_INDEX,
+            f"{self.pip_name}==",
+        ]
         output = subprocess.Popen(
             args, stdout=subprocess.PIPE, stderr=subprocess.PIPE
         ).communicate()
         if len(output) < 2 or "none" in output[1].decode("utf-8"):
             args = [
                 "pip2.7",
                 "install",
@@ -212,14 +219,24 @@
             semver.Version.parse(version).replace(prerelease=None, build=None)
         )
         if release_version in self.versions["pypi"] + self.versions["tags"]:
             return release_version
         return None
 
 
+# def version_compare(version1, version2):
+#     """Compare two versions.
+
+#     Versions may be semvers or tuples with semver at element[0].
+#     """
+#     if isinstance(version1, tuple) and isinstance(version2, tuple):
+#        return semver.compare(str(version1[0]), str(version2[0]))
+#     return semver.compare(str(version1), str(version2))
+
+
 def _sorted_versions(versions):
     """Sort a list of versions."""
     return sorted(versions, key=functools.cmp_to_key(semver.compare))
 
 
 def _read_version_file(filename):
     """Pull the version from the VERSION file."""
```

## skulk/skulk.py

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 """
 Skulk.
 
-A tool to help get your repo in good shape before pushing.
+A tool to help get your repo in good shape for a release.
 
 It works for packages intended for PyPi.
 
 It has 2 public functions:
 
 1. main() : A wizard that guides you to choosing a version that does not conflict with any git tags
    or PyPi versions.
@@ -69,75 +69,81 @@
 
         self.ask_changelog_additions()
 
         # Now we do the actual work.
         # CHANGELOG
         if self.edit_changelog:
             self.resolve_changelog()
- 
-        next_version = self.bumper.next_version
-        if next_version:
-            # VERSION FILE
-            with open(self.version_filename, "w", encoding="utf-8") as vf:
-                vf.write(next_version)
 
-            # COMMIT CHANGES
+        if self.bumper.next_version:
+            with open(self.version_filename, "w", encoding="utf-8") as vfn:
+                vfn.write(self.bumper.next_version)
+
+        self.commit_version_changelog()
+        tag = self.add_tag()
+        do_push = self.ask_push(tag)
+        if do_push:
+            self.push(tag)
+        else:
+            print("No worries. Use the following command to push later. Bye\n")
+            if tag:
+                print(f"git push --atomic origin {self.branch_name} {tag.name}")
+            else:
+                print(f"git push origin {self.branch_name}")
+        sys.exit(0)
+
+    # PRIVATE
+    def ask_push(self, tag=None):
+        """Ask the user if he wants to push the branch and tag."""
+        if tag:
+            question = f"Do you want me to push the branch and tag: {self.branch_name} + {tag.name}` for you?"
+        else:
+            question = f"Do you want me to push the branch: {self.branch_name} for you?"
+        return util.yes_no(question)
+
+    def push(self, tag=None):
+        """Push the branch and tag."""
+        origin = self.repo.remote("origin")
+        if tag:
+            origin.push(self.branch)
+            origin.push(tag)
+            print("Pushed branch and tag.\n")
+        else:
+            origin.push(self.branch)
+            print("Pushed branch.\n")
+
+    def add_tag(self):
+        """Add a tag to the repo."""
+        if self.bumper.next_version:
+            label = "Pre-release" if self.bumper.is_prerelease() else "Release"
+            tag = self.repo.create_tag(
+                self.bumper.next_version, message=f"{label}: {self.bumper.next_version}"
+            )
+            print(f"Created tag: {tag.name}")
+            return tag
+        return None
+
+    def commit_version_changelog(self):
+        """Commit the version and changelog files."""
+        if self.bumper.next_version:
             if self.repo.is_dirty():
                 self.repo.index.add([self.changelog_filename, self.version_filename])
                 self.repo.index.commit(
-                    f"Update changelog and sets version to {next_version}"
+                    f"Update changelog and sets version to {self.bumper.next_version}"
                 )
                 print("Committed Version and Changelog\n")
 
         elif self.edit_changelog:
-            # COMMIT CHANGES
             if self.repo.is_dirty():
                 self.repo.index.add([self.changelog_filename])
                 self.repo.index.commit("Update changelog")
                 print("Committed Changelog\n")
 
-        # GIT TAG
-
-        origin = self.repo.remote("origin")
-        if next_version:
-            label = "Pre-release" if self.bumper.is_prerelease() else "Release"
-            tag = self.repo.create_tag(next_version, message=f"{label}: {next_version}")
-
-            # PUSH
-            do_push = util.yes_no(
-                f"Do you want me to push the branch and tag: {self.branch_name} + {tag.name}` for you?"
-            )
-
-            if do_push:
-                origin.push(self.branch)
-                origin.push(tag)
-                print("Pushed branch and tag.\n")
-            else:
-                print(
-                    "No worries. Use the following command to push the branch and tag later. Bye\n"
-                )
-                print(f"git push --atomic origin {self.branch_name} {tag.name}")
-
-        else:
-            do_push = util.yes_no(
-                f"Do you want me to push the branch: {self.branch_name} for you?"
-            )
-            if do_push:
-                origin.push(self.branch)
-                print("Pushed branch.\n")
-            else:
-                print(
-                    "No worries. Use the following command to push the branch later. Bye\n"
-                )
-                print(f"git push origin {self.branch_name}")
-
-        sys.exit(0)
-
     def check_clean(self):
-        """Check that the repo is clean.
+        """Check that the repo is clean and give user a chance to clean it up.
 
         User can continue with a dirty repo, but we at least want to warn them.
         """
         if not self.repo.is_dirty():
             print("Repo clean. Good to go.")
             return
 
@@ -215,14 +221,15 @@
         input(
             util.green(
                 "Please EDIT and SAVE your CHANGELOG (There's no need to commit), then press enter to continue."
             )
         )
 
     def changelog_needs_unreleased_stub(self):
+        """Return True if the changelog needs an unreleased stub."""
         with open(self.changelog_filename, "r", encoding="utf-8") as f:
             datafile = f.readlines()
 
         for line in datafile:
             if line.startswith("## Unreleased"):
                 return False
             elif line.startswith("## Version"):
@@ -239,14 +246,15 @@
         )
         for commit in self.repo.iter_commits(rev=self.branch):
             if commit.hexsha in master_shas:
                 continue
             result.append(commit)
         return result
 
+
 def main():
     """Run the wizard."""
     wizard = Skulk()
     wizard.run()
 
 
 if __name__ == "__main__":
```

## Comparing `skulk-1.4.6rc7.dist-info/METADATA` & `skulk-1.4.6rc8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skulk
-Version: 1.4.6rc7
+Version: 1.4.6rc8
 Summary: Streamline release for Conductor client tools and others
 Home-page: https://github.com/ConductorTechnologies/skulk
 Author: Julian Mann
 Author-email: julian@conductortech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

