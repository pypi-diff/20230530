# Comparing `tmp/skulk-1.4.5-py2.py3-none-any.whl.zip` & `tmp/skulk-1.4.6rc7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 7288 bytes, number of entries: 8
--rw-r--r--  2.0 unx        5 b- defN 22-Jan-31 20:47 skulk/VERSION
--rw-r--r--  2.0 unx        0 b- defN 22-Jan-31 20:47 skulk/__init__.py
--rw-r--r--  2.0 unx    17422 b- defN 22-Jan-31 20:47 skulk/skulk.py
--rw-r--r--  2.0 unx      601 b- defN 22-Jan-31 20:47 skulk-1.4.5.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Jan-31 20:47 skulk-1.4.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 22-Jan-31 20:47 skulk-1.4.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 22-Jan-31 20:47 skulk-1.4.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      592 b- defN 22-Jan-31 20:47 skulk-1.4.5.dist-info/RECORD
-8 files, 18780 bytes uncompressed, 6254 bytes compressed:  66.7%
+Zip file size: 8696 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       10 b- defN 23-May-29 23:46 skulk/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 23-May-29 23:46 skulk/__init__.py
+-rw-r--r--  2.0 unx     9029 b- defN 23-May-29 23:46 skulk/bumper.py
+-rw-r--r--  2.0 unx     8697 b- defN 23-May-29 23:46 skulk/skulk.py
+-rw-r--r--  2.0 unx     2625 b- defN 23-May-29 23:46 skulk/util.py
+-rw-r--r--  2.0 unx      649 b- defN 23-May-29 23:46 skulk-1.4.6rc7.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-29 23:46 skulk-1.4.6rc7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 23-May-29 23:46 skulk-1.4.6rc7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-May-29 23:46 skulk-1.4.6rc7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      749 b- defN 23-May-29 23:46 skulk-1.4.6rc7.dist-info/RECORD
+10 files, 21919 bytes uncompressed, 7424 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -1,25 +1,31 @@
 Filename: skulk/VERSION
 Comment: 
 
 Filename: skulk/__init__.py
 Comment: 
 
+Filename: skulk/bumper.py
+Comment: 
+
 Filename: skulk/skulk.py
 Comment: 
 
-Filename: skulk-1.4.5.dist-info/METADATA
+Filename: skulk/util.py
+Comment: 
+
+Filename: skulk-1.4.6rc7.dist-info/METADATA
 Comment: 
 
-Filename: skulk-1.4.5.dist-info/WHEEL
+Filename: skulk-1.4.6rc7.dist-info/WHEEL
 Comment: 
 
-Filename: skulk-1.4.5.dist-info/entry_points.txt
+Filename: skulk-1.4.6rc7.dist-info/entry_points.txt
 Comment: 
 
-Filename: skulk-1.4.5.dist-info/top_level.txt
+Filename: skulk-1.4.6rc7.dist-info/top_level.txt
 Comment: 
 
-Filename: skulk-1.4.5.dist-info/RECORD
+Filename: skulk-1.4.6rc7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## skulk/VERSION

```diff
@@ -1 +1 @@
-1.4.5
+1.4.6-rc.7
```

## skulk/skulk.py

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 """
 Skulk.
 
 A tool to help get your repo in good shape before pushing.
 
 It works for packages intended for PyPi.
@@ -16,539 +16,238 @@
 
 2. run_pre_push_checks() : A function that is designed to be called from a git pre-push hook.
 
 Assumptions: 1. You have a file named VERSION at the top level of the repo. It should contain a
 simple semver such as 1.2.3 2. You have a CHANGELOG.md  at the top level of the repo.
 
 
+WIZARD MESSAGES:
+
+1. Nothing will happen until the end. You can exit at any time.
+2. Do you want to simply push your code(0), deploy a pre-release(1), or deploy a release(2)?
+3. If pre-release(1) or release(2):
+    a. You'll be shown the current version and the latest version on PyPi.
+    b. You'll be asked to choose a new version from the options.
+
 
 """
 
 from __future__ import print_function
 from builtins import input
 import datetime
 import os
-import re
-import json
-import subprocess
 import sys
-from distutils.version import LooseVersion
-from shutil import rmtree
-
-from git import InvalidGitRepositoryError, Repo
+from . import util
+from .bumper import Bumper
 
 
-PROD_PYPI_INDEX = "https://pypi.org/simple/"
-TEST_PYPI_INDEX = "https://test.pypi.org/simple/"
+class Skulk(object):
+    """A wizard to guide the user to a good version and changelog."""
 
-HOOK_CONTENT = """#!/usr/bin/env python
-
-import sys
-from skulk import skulk
-skulk.run_pre_push_checks()
-sys.exit(0)"""
-
-HOOK_DETECTION_LINE = "skulk.run_pre_push_checks()"
-
-
-def _green(rhs):
-    return "\033[92m{}\033[0m".format(rhs)
-
-
-def _red(rhs):
-    return "\033[91m{}\033[0m".format(rhs)
-
-
-def _get_commits_since_last_tag(repo):
-    """Return recent commits, or all commits if no tag."""
-    last_tag = _get_last_tag_version(repo)
-    if last_tag:
-        rev_spec = "{}..HEAD".format(last_tag)
-        commits = repo.iter_commits(rev_spec)
-    else:
-        commits = repo.iter_commits(repo.head)
-    return commits
-
-
-def _get_commit_messages_since_last_tag(repo):
-    """Return recent commit messages with truncated hashes."""
-    commits = _get_commits_since_last_tag(repo)
-    messages = []
-    for commit in commits:
-        msg = commit.message.strip()
-        messages.append("* {}. [{}]".format(msg.capitalize(), commit.hexsha[:7]))
-    return messages
-
-
-def _get_version_file(repo):
-    """Get the VERSION file from the top level of the repo."""
-    version_file = os.path.join(repo.working_dir, "VERSION")
-    if not os.path.isfile(version_file):
-        msg = "VERSION file does not exist at the top level of the repo.\n"
-        msg += "Add a file (VERSION) with a numeric only version such as 1.2.3\n"
-        sys.stderr.write(msg)
-        sys.exit(1)
-    return version_file
-
-
-def _get_changelog(repo):
-    """Get the CHANGELOG file from the top level of the repo."""
-    changelog = os.path.join(repo.working_dir, "CHANGELOG.md")
-    if not os.path.isfile(changelog):
-        sys.stderr.write(
-            "CHANGELOG does not exist. Please create it and try again. {}\n".format(changelog)
-        )
-        sys.exit(1)
-    return changelog
-
-
-def _get_version(version_file):
-    """Pull the version from the VERSION file."""
-    try:
-        return _first_nonblank_line(version_file)
-    except:
-        sys.stderr.write("Can't get version from the version file. {}\n".format(version_file))
-
-
-def _get_test_pypi_versions(pip_name):
-    return _get_pypi_versions(pip_name, TEST_PYPI_INDEX)
-
-
-def _get_prod_pypi_versions(pip_name):
-    return _get_pypi_versions(pip_name, PROD_PYPI_INDEX)
-
-
-def _get_pypi_versions(pip_name, index):
-    """
-    Return a list of all PyPi versions for the named package.
-
-    The package may not exist on PyPi, in which case we return an empty list. We
-    don't error out, because it's perfectly valid for no package to exist. We
-    can still deploy there.
-    """
-    result = []
-
-    # notice this command says: Install version== (i.e. it requests an invalid
-    # version). It fails as intended, and the result is a message to say can't
-    # find version in versions. It lists the existing versions which we split
-    # and return. Check for py3 and py 27 compatible by using both pips.
-    args = ["pip", "install", "--index-url", index, "{}==".format(pip_name)]
-    output = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE).communicate()
-    if len(output) < 2 or "none" in output[1].decode("utf-8"):
-        args = ["pip2.7", "install", "--index-url", index, "{}==".format(pip_name)]
-        output = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE).communicate()
-        if len(output) < 2 or "none" in output[1].decode("utf-8"):
-            return []
-
-    output = output[1]
-    regex = re.compile(r"^.*Could not find a version.*from versions:(.*)\).*", re.DOTALL)
-    match = regex.match(output.decode("utf-8"))
-    if match:
-        result = [v.strip() for v in match.group(1).split(r", ")]
-        result = _sorted_numeric_versions(result)
-    return result
-
-
-def _get_pip_name(repo):
-    """
-    Return the pip name, which may be different than the repo name.
-
-    If the pip name is different, it should be the first line of the MANIFEST
-    file as a comment.
-    """
-    manifest_file = os.path.join(repo.working_dir, "MANIFEST.in")
-    try:
-        first_line = _first_nonblank_line(manifest_file)
-        if first_line[0] == "#":
-            return first_line.split(" ")[1]
-    finally:
-        return os.path.basename(repo.working_dir)
-
-
-def _version_is_valid(last_versions, test_pypi_versions, version):
-    """
-    Return True if the version is the most recent and unique.
-
-    The version is tested against the tags, and the last PyPi versions. It is also tested against
-    all testPyPi versions for a direct clash. 
-    """
-
-    
-    if version in test_pypi_versions:
-        return False
-
-    print("Current version: ", version)
-    for key in ["prodpypi", "tag"]:
-        if last_versions.get(key) and version <= last_versions[key]:
-            return False
-    return True
+    def __init__(self):
+        self.repo = util.get_repo()
+        self.branch = self.repo.active_branch
+        self.branch_name = self.branch.name
+        self.working_dir = self.repo.working_dir
+        self.hook_filename = os.path.join(self.working_dir, ".git", "hooks", "pre-push")
+        self.changelog_filename = os.path.join(self.working_dir, "CHANGELOG.md")
+        self.version_filename = os.path.join(self.working_dir, "VERSION")
+        self.pip_name = util.get_pip_name(self.repo)
+        self.bumper = None
+        self.edit_changelog = False
+        self.changelog_addition = None
+
+    def run(self):
+        """
+        Guide the user to ensure version and changelog are valid.
+        """
+
+        # wizard.check_pre_push_hook()
+        self.check_clean()
+        self.bumper = Bumper(self.repo, self.pip_name)
+        if self.ask_do_tag_release():
+            self.bumper.run()
+
+        self.ask_changelog_additions()
+
+        # Now we do the actual work.
+        # CHANGELOG
+        if self.edit_changelog:
+            self.resolve_changelog()
  
+        next_version = self.bumper.next_version
+        if next_version:
+            # VERSION FILE
+            with open(self.version_filename, "w", encoding="utf-8") as vf:
+                vf.write(next_version)
+
+            # COMMIT CHANGES
+            if self.repo.is_dirty():
+                self.repo.index.add([self.changelog_filename, self.version_filename])
+                self.repo.index.commit(
+                    f"Update changelog and sets version to {next_version}"
+                )
+                print("Committed Version and Changelog\n")
+
+        elif self.edit_changelog:
+            # COMMIT CHANGES
+            if self.repo.is_dirty():
+                self.repo.index.add([self.changelog_filename])
+                self.repo.index.commit("Update changelog")
+                print("Committed Changelog\n")
+
+        # GIT TAG
+
+        origin = self.repo.remote("origin")
+        if next_version:
+            label = "Pre-release" if self.bumper.is_prerelease() else "Release"
+            tag = self.repo.create_tag(next_version, message=f"{label}: {next_version}")
+
+            # PUSH
+            do_push = util.yes_no(
+                f"Do you want me to push the branch and tag: {self.branch_name} + {tag.name}` for you?"
+            )
 
-def _get_last_versions(repo):
-    """Get the most recent of each version: testpypi, prodpypi, git-tag."""
-    pip_name = _get_pip_name(repo)
-    print(
-        "Getting PyPi versions for",
-    )
-    # test_pypi_versions = _get_test_pypi_versions(pip_name)
-    prod_pypi_versions = _get_prod_pypi_versions(pip_name)
-    last_tag_version = _get_last_tag_version(repo)
-    return {
-        # "testpypi": test_pypi_versions[-1] if test_pypi_versions else "0.0.0",
-        "prodpypi": prod_pypi_versions[-1] if prod_pypi_versions else "0.0.0",
-        "tag": last_tag_version or "0.0.0",
-    }
-
-
-def _get_last_tag_version(repo):
-    """Get the most recent git tag version"""
-    tags = _sorted_numeric_versions(repo.tags)
-    if tags:
-        return str(tags[-1])
-
-
-def _get_last_changelog_version(changelog):
-    """
-    Extract the version from first line of the changelog.
-    """
-    try:
-        return _first_nonblank_line(changelog).split(":")[1].split(" ")[0].strip()
-    except:
-        sys.stderr.write("Can't get the last version used in the changelog. {}\n".format(changelog))
-
-
-def _nonblank_lines(fileobject):
-    """Generator to help search a file."""
-    for line in fileobject:
-        line = line.rstrip()
-        if line:
-            yield line
-
-
-def _first_nonblank_line(filename):
-    """Use a generator to return the first non blank line, or None."""
-    try:
-        with open(filename) as f:
-            gen = _nonblank_lines(f)
-            return next(gen, None)
-    except:
-        pass
-
-
-def _get_repo():
-    """Return the Repository object.
-
-    Exit if not in a workable state.
-    """
-    try:
-        repo = Repo(".")
-    except InvalidGitRepositoryError:
-        sys.stderr.write("Not a git repo. Can't continue.\n")
-        sys.exit(1)
-    if repo.untracked_files:
-        sys.stderr.write("Untracked files. Can't continue.\n")
-        sys.exit(1)
-    if repo.is_dirty():
-        sys.stderr.write("Dirty repo. Can't continue.\n")
-        sys.exit(1)
-    return repo
-
-
-def _resolve_version(repo, version, version_file):
-    """
-    Resolve and return the version we want to use.
-
-    If currentr version is valid, user has the option to bump it.
-    Otherwise he must bump it.
-    """
-    last_versions = _get_last_versions(repo)
-
-    print("Latest Versions:")
-    print(json.dumps(last_versions, indent=3))
-
-    versions = _sorted_numeric_versions([last_versions["prodpypi"], last_versions["tag"], version])
-    test_pypi_versions = _get_test_pypi_versions(_get_pip_name(repo))
-    print("TestPyPi Versions:")
-    print(json.dumps(test_pypi_versions, indent=3))
-
-    valid = _version_is_valid(last_versions, test_pypi_versions, version)
-    do_bump = True
-    if not valid:
-        print("Version invalid: ({}) must be greater than prod and tag versions  and must not clash with testPyPi versions.".format(version))
-    else:
-        print("Version is valid ({}). However, you may bump it if you wish.".format(version))
-        do_bump = _yes_no("Do you wish to bump the version anyway?")
-
-    if not do_bump:
-        return version
-
-    print("To bump the version, please enter the type of change this push represents...")
-
-    options = ["Fix.", "Feature.", "Breaking change.", "Abort!"]
-    for i, opt in enumerate(options):
-        print("{}:{}".format(i + 1, opt))
-    inp = int(input(_green("Enter a number: ")))
-
-    if inp not in [1, 2, 3]:
-        sys.stderr.write("Aborted:\n")
-        sys.exit(1)
-
-    version = _bump(versions[-1],test_pypi_versions, inp)
-
-    print("You bumped the version to: ({})".format(version))
-
-    print("Overwriting version file...")
-    with open(version_file, "w") as f:
-        f.write(version)
-
-    return version
-
-
-def _bump(version, test_pypi_versions, which):
-    """
-    Return a bumped sem-ver version according to which.
-
-    which = 1:patch, 2:minor, 3:major
-
-    If there's a clash with a testpypi version, then bump the patch until there isn't.
-    """
-    parts = [int(c) for c in version.split(".")]
-
-    if which == 2:
-        parts[1] += 1
-        parts[2] = 0
-    elif which == 3:
-        parts[0] += 1
-        parts[1] = 0
-        parts[2] = 0
-    else:
-        parts[2] += 1
-
-    while True:
-        result = ".".join([str(p) for p in parts])
-        if result not in test_pypi_versions:
-            break
-        parts[2] += 1
-
-    return result
-
-def _resolve_changelog(repo, version, changelog):
-    """
-    Help the user to get the changelog up-to-date.
-
-    We print recent commit messages in the shell, and insert them under a
-    heading in the CHANGELOG. The user only needs to edit for human clarity then
-    save the file and hit continue.
-    """
-    print("resolve changelog here:")
-
-    print("Edit and save the changelog now. Here are some recent commits...")
-
-    most_recent_messages = _get_commit_messages_since_last_tag(repo)
-    print("=" * 30)
-    for msg in most_recent_messages:
-        print(msg)
-    print("=" * 30)
-
-    today = datetime.date.today().strftime("%d %b %Y")
-    recent_block = "### Version:{} -- {}\n\n".format(version, today)
-    recent_block += "\n".join(most_recent_messages) or ""
-
-    with open(changelog, "r") as clog:
-        data = clog.read() or "--"
-
-    new_content = recent_block + "\n\n" + data
-
-    with open(changelog, "w") as clog:
-        clog.write(new_content)
-
-    print("A new section has been prepended to your changelog.")
-
-    input(
-        _green(
-            "Please edit and save your CHANGELOG (There's no need to commit), then press enter to continue."
-        )
-    )
-
-
-def _yes_no(question, *args):
-    options = args or ["No", "Yes"]
+            if do_push:
+                origin.push(self.branch)
+                origin.push(tag)
+                print("Pushed branch and tag.\n")
+            else:
+                print(
+                    "No worries. Use the following command to push the branch and tag later. Bye\n"
+                )
+                print(f"git push --atomic origin {self.branch_name} {tag.name}")
 
-    print(question)
-    for i, opt in enumerate(options):
-        print("{}:{}".format(i, opt))
-    while True:
-        inp = int(input(_green("Enter a number: ")))
-        if inp in [0, 1]:
-            return [False, True][inp]
         else:
-            print("You must choose 0 for {}, or 1 for {}..".format(*options))
-
-
-def _check_clean(repo):
-    options = ["Continue", "Abort"]
-    while repo.is_dirty():
-        print("Repo is dirty. Maybe you changed something else along the way?.\n")
-        print("Please check, and then either commit changes or add files to .gitignore so that the repo is clean..\n")
-        print("When you are done, choose one of the options below.")
-        for i, opt in enumerate(options):
-            print("{}:{}".format(i, opt))
-
-        inp = int(input(_green("Enter a number: ")))
-
-        if inp == 1:
-            sys.stderr.write("Aborted:\n")
-            sys.stderr.write(
-                "NOTE: Although this stage was stopped. Changes may have been made to the version and changelog already.\n"
+            do_push = util.yes_no(
+                f"Do you want me to push the branch: {self.branch_name} for you?"
             )
-            sys.exit(1)
-
-
-def _sorted_numeric_versions(versions):
-    versions = list(set([str(v) for v in versions or [] if v and str(v)[0].isdigit()]))
-    return sorted(versions, key=LooseVersion)
-
-
+            if do_push:
+                origin.push(self.branch)
+                print("Pushed branch.\n")
+            else:
+                print(
+                    "No worries. Use the following command to push the branch later. Bye\n"
+                )
+                print(f"git push origin {self.branch_name}")
 
-def run_pre_push_checks():
-    """
-    Non interactive check for version issues.
-
-    This function is intended to be called from a pre_push git hook.
-
-    The content of the hook file should be as follows:
-
-    #!/usr/bin/env python
+        sys.exit(0)
 
-    import sys
-    from skulk import skulk
-    skulk.run_pre_push_checks()
-    sys.exit(0)
+    def check_clean(self):
+        """Check that the repo is clean.
 
-    """
-    repo = _get_repo()
-    version_file = _get_version_file(repo)
-    version = _get_version(version_file)
+        User can continue with a dirty repo, but we at least want to warn them.
+        """
+        if not self.repo.is_dirty():
+            print("Repo clean. Good to go.")
+            return
 
-    last_versions = _get_last_versions(repo)
-    test_pypi_versions = _get_test_pypi_versions(_get_pip_name(repo))
+        mods = [item.a_path for item in self.repo.index.diff(None)]
+        untracked = self.repo.untracked_files
+        if mods:
+            print(util.magenta("Modified files:\n{}".format("\n".join(mods))))
+        if untracked:
+            print(util.magenta("Untracked files:\n{}".format("\n".join(untracked))))
 
-    if not _version_is_valid(last_versions, test_pypi_versions, version):
-        sys.stderr.write(
-            "Version {} is not valid.\nCan't continue. Please run skulk to rectify this.\n".format(
-                version
+        print(
+            "----------\nAttention: Repo is dirty. Uncommitted changes won't be included. Is this ok?"
+        )
+        print("If you want to include them, please commit them now.")
+        cont = input(
+            util.green(
+                "When you are happy, press enter to continue or type 'exit' to exit."
             )
         )
-        sys.exit(1)
-
-    changelog = _get_changelog(repo)
-    last_changelog_version = _get_last_changelog_version(changelog)
-    if last_changelog_version != version:
-        msg = "The last CHANGELOG entry ({}) is not up to date with the current version ({}).\n"
-        msg += "Can't continue. Please run skulk to rectify this.\n"
-        sys.stderr.write(msg.format(last_changelog_version, version))
-        sys.exit(1)
-
-
-def _check_pre_push_hook(repo):
-    """ """
-    hook_file = os.path.join(repo.working_dir, ".git", "hooks", "pre-push")
-    if os.path.exists(hook_file):
-        with open(hook_file) as f:
-            for line in f:
-                if line.strip() == HOOK_DETECTION_LINE:
-                    return
-        _show_manual_hook_instructions(hook_file, HOOK_CONTENT)
-        do_continue = _yes_no(
-            "Do you want to continue without the hook, or exit skulk while you add the hook code? Continue?"
+        if cont == "exit":
+            sys.stderr.write("Exited.\n")
+            sys.exit(0)
+
+    def ask_do_tag_release(self):
+        """Ask the user if he wants to make a pre-release from this branch."""
+        return util.yes_no(
+            "Do you want to tag and deploy from this branch?",
+            "No, push only",
+            "Yes, push and deploy a taged release.",
         )
-        if do_continue:
-            return
-        sys.exit(1)
-
-    # We got here, so the file does not exist.
-    _show_auto_hook_preamble()
 
-    do_create = _yes_no("Do you want me to create the pre-push hook for you?")
+    def ask_changelog_additions(self):
+        """Generate the reference additions to the changelog.
 
-    if do_create:
-        print("Creating '{}' ...".format(hook_file))
-        with open(hook_file, "w") as f:
-            f.write(HOOK_CONTENT)
-            f.write("\n")
-        os.chmod(hook_file, 0o755)
-    else:
-        print("No worries. Just be sure to always use the skulk command, and not git push\n")
-
-
-def _show_auto_hook_preamble():
-    sys.stderr.write("There's no pre-push git hook active in this repository.\n")
-    sys.stderr.write(
-        "It is recommeded to have a hook for skulk so you don't accidentally push without a \n"
-    )
-    sys.stderr.write("version bump or an up to date changelog.\n")
-
-
-def _show_manual_hook_instructions(hook_file, HOOK_CONTENT):
-    sys.stderr.write("A pre-push git hook exists, but it doesn't contain the skulk check.\n")
-    sys.stderr.write("It is recommeded to create the hook so you don't push without a \n")
-    sys.stderr.write("version bump or an up to date changelog.\n")
-    sys.stderr.write("Please integrate the following code and make sure the hook is executable:\n")
-    sys.stderr.write("Filename: '{}'\n".format(hook_file))
-    sys.stderr.write("Code:\n")
-    sys.stderr.write("###############\n")
-    sys.stderr.write(HOOK_CONTENT)
-    sys.stderr.write("\n###############\n")
+        Do not write anything to the changelog file yet."""
+        block = ""
+        write_block = self.bumper.next_version or self.changelog_needs_unreleased_stub()
+        if self.bumper.next_version:
+            self.edit_changelog = True
+            date_string = datetime.date.today().strftime("%d %b %Y")
+            block = f"## Version:{self.bumper.next_version} -- {date_string}\n\n"
+        else:
+            self.edit_changelog = util.yes_no(
+                "No version bump. Do you want to add entries in the changelog anyway?"
+            )
+            block = "## Unreleased\n\n"
+        sections = ["Added", "Changed", "Deprecated", "Removed", "Fixed", "Security"]
+        block += "\n".join([f"### {s}\n" for s in sections])
+
+        if self.edit_changelog:
+            commits = self.get_commits()
+            commit_messages = ["\n# Raw commit messages for reference.\n"]
+            commit_messages.extend([f"* {c.summary} [{c.hexsha[:7]}]" for c in commits])
+            commit_block = "\n".join(commit_messages) or ""
+
+            print(commit_block)
+
+            self.changelog_addition = commit_block
+            if write_block:
+                self.changelog_addition = commit_block + "\n\n" + block
+
+    def resolve_changelog(self):
+        """Help the user to get the changelog file up-to-date."""
+        with open(self.changelog_filename, "r", encoding="utf-8") as clog:
+            content = clog.read() or "--"
+
+        content = self.changelog_addition + "\n\n" + content
+
+        with open(self.changelog_filename, "w", encoding="utf-8") as clog:
+            clog.write(content)
+
+        print("Resolve CHANGELOG:")
+        print("Edit and save the changelog now.")
+
+        input(
+            util.green(
+                "Please EDIT and SAVE your CHANGELOG (There's no need to commit), then press enter to continue."
+            )
+        )
 
+    def changelog_needs_unreleased_stub(self):
+        with open(self.changelog_filename, "r", encoding="utf-8") as f:
+            datafile = f.readlines()
+
+        for line in datafile:
+            if line.startswith("## Unreleased"):
+                return False
+            elif line.startswith("## Version"):
+                return True
+        return True
+
+    # PRIVATE
+
+    def get_commits(self):
+        """Get commits that are on the active branch but not on the master branch."""
+        result = []
+        master_shas = set(
+            [c.hexsha for c in self.repo.iter_commits(rev=self.repo.branches.master)]
+        )
+        for commit in self.repo.iter_commits(rev=self.branch):
+            if commit.hexsha in master_shas:
+                continue
+            result.append(commit)
+        return result
 
 def main():
-    """
-    Wizard to guide the user to ensure version and changelog are valid.
-    """
-    repo = _get_repo()
-
-    _check_pre_push_hook(repo)
-
-    do_cicd = _yes_no(
-        "Do you want to simply push your code(0), or bump the version and run CICD(1)",
-        "Push",
-        "Bump/Push/CICD",
-    )
-    if not do_cicd:
-        repo.index.commit("[ci skip] This commit has not been bumped and skips CICD.")
-        os.system("git push origin {} --no-verify".format(repo.active_branch.name))
-        print("Pushed without bump or CICD...\n")
-        sys.exit(0)
-
-    version_file = _get_version_file(repo)
-    version = _get_version(version_file)
-    changelog = _get_changelog(repo)
-
-    version = _resolve_version(repo, version, version_file)
-    _resolve_changelog(repo, version, changelog)
-
-    if repo.is_dirty():
-        repo.index.add([changelog, version_file])
-        repo.index.commit("Updates Changelog and sets version to {}".format(version))
-        print("Committed Version and Changelog\n")
-
-    _check_clean(repo)
-
-    sys.stderr.write("Done! The repo is now in good shape and ready to push.\n")
-
-    do_push = _yes_no(
-        "Do you want me to run `git push origin {}` for you?".format(repo.active_branch.name)
-    )
-
-    if do_push:
-        # We've already verified, so the git hook is not needed, and in fact confuses things during
-        # development.
-        os.system("git push origin {} --no-verify".format(repo.active_branch.name))
-        print("Pushed...\n")
-    else:
-        print("No worries. Use the above command to push the branch later. Bye\n")
-
-    sys.exit(0)
+    """Run the wizard."""
+    wizard = Skulk()
+    wizard.run()
 
 
 if __name__ == "__main__":
     main()
```

## Comparing `skulk-1.4.5.dist-info/METADATA` & `skulk-1.4.6rc7.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: skulk
-Version: 1.4.5
+Version: 1.4.6rc7
 Summary: Streamline release for Conductor client tools and others
 Home-page: https://github.com/ConductorTechnologies/skulk
 Author: Julian Mann
 Author-email: julian@conductortech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
-Requires-Dist: GitPython (>=2.1.15)
-Requires-Dist: twine (>=1.15.0)
-Requires-Dist: future (>=0.18.2)
+Requires-Dist: GitPython (<4.0.0,>=3.1.31)
+Requires-Dist: semver (<4.0.0,>=3.0.0)
+Requires-Dist: twine (>=4.0.2)
+Requires-Dist: future (>=0.18.3)
 
 Streamline release for Conductor client tools and others
```

