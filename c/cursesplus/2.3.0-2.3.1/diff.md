# Comparing `tmp/cursesplus-2.3.0.tar.gz` & `tmp/cursesplus-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.3.0.tar", last modified: Mon May 29 19:43:03 2023, max compression
+gzip compressed data, was "cursesplus-2.3.1.tar", last modified: Mon May 29 23:25:58 2023, max compression
```

## Comparing `cursesplus-2.3.0.tar` & `cursesplus-2.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-29 19:43:03.296406 cursesplus-2.3.0/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.3.0/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1413 2023-05-29 19:43:03.296406 cursesplus-2.3.0/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      810 2023-05-29 19:42:38.000000 cursesplus-2.3.0/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-05-29 19:40:43.000000 cursesplus-2.3.0/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-05-29 19:43:03.296406 cursesplus-2.3.0/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-29 19:43:03.286406 cursesplus-2.3.0/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      313 2023-05-29 19:28:28.000000 cursesplus-2.3.0/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-29 19:43:03.296406 cursesplus-2.3.0/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.3.0/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    15024 2023-05-29 19:39:12.000000 cursesplus-2.3.0/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.3.0/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.3.0/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-29 19:43:03.296406 cursesplus-2.3.0/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1413 2023-05-29 19:43:03.000000 cursesplus-2.3.0/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-05-29 19:43:03.000000 cursesplus-2.3.0/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-05-29 19:43:03.000000 cursesplus-2.3.0/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-05-29 19:43:03.000000 cursesplus-2.3.0/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-29 23:25:58.126382 cursesplus-2.3.1/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.3.1/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1491 2023-05-29 23:25:58.126382 cursesplus-2.3.1/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      888 2023-05-29 23:25:42.000000 cursesplus-2.3.1/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-05-29 23:25:17.000000 cursesplus-2.3.1/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-05-29 23:25:58.126382 cursesplus-2.3.1/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-29 23:25:58.116382 cursesplus-2.3.1/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      317 2023-05-29 23:14:15.000000 cursesplus-2.3.1/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-29 23:25:58.126382 cursesplus-2.3.1/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.3.1/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    15799 2023-05-29 23:22:30.000000 cursesplus-2.3.1/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.3.1/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.3.1/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-29 23:25:58.126382 cursesplus-2.3.1/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1491 2023-05-29 23:25:58.000000 cursesplus-2.3.1/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-05-29 23:25:58.000000 cursesplus-2.3.1/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-05-29 23:25:58.000000 cursesplus-2.3.1/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-05-29 23:25:58.000000 cursesplus-2.3.1/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.3.0/LICENSE` & `cursesplus-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.0/PKG-INFO` & `cursesplus-2.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.3.0
+Version: 2.3.1
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,20 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
+### Patch 2.3.1:
+
+-Add character limit to new input
+
+-Add more functionality
+
 ### Version 2.3: New Input
 
 -Rewrite cursesinput function
 
 -Remains backwards-compatible
 
 ### Version 2.0: Incompatible api changes
```

### Comparing `cursesplus-2.3.0/README.md` & `cursesplus-2.3.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
+### Patch 2.3.1:
+
+-Add character limit to new input
+
+-Add more functionality
+
 ### Version 2.3: New Input
 
 -Rewrite cursesinput function
 
 -Remains backwards-compatible
 
 ### Version 2.0: Incompatible api changes
```

### Comparing `cursesplus-2.3.0/pyproject.toml` & `cursesplus-2.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.3.0"
+version = "2.3.1"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.3.0/src/cursesplus/__init__.py` & `cursesplus-2.3.1/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.0/src/cursesplus/cp.py` & `cursesplus-2.3.1/src/cursesplus/cp.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,22 +104,25 @@
     
     for msgl in message:
         mi += 1
         stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl)
     stdscr.refresh()
 def __retr_nbl_lst(input:list)->list:
     return [l for l in input if str(l) != ""]  
-def __shft_lst(input:list)->list:
-    xl = [i for i in input if str(i) != ""]
-    return xl + ["" for _ in range(1000-len(xl))]
+def __calc_nbl_list(input:list)->int:
+    x = 0
+    for ls in input:
+        x += len(ls)
+    return x
 
 def cursesinput(stdscr,prompt: str,lines=1,maxlen=0) -> str:
     """
     Get input from the user. Set maxlen to 0 for no maximum
     """
+    ERROR = ""
     mx,my = os.get_terminal_size()
     extoffscr = lines > my-3
     if extoffscr:
         lnrectmaxy = my-2
     else:
         lnrectmaxy = lines+2
     text: list[list[str]] = [[] for _ in range(lines)]
@@ -132,77 +135,92 @@
         rectangle(stdscr,1,0,lnrectmaxy,mx-1)
         chi = 1
         for chln in text:
             chi+= 1
             stdscr.addstr(chi,1,"".join(chln)[xoffset:xoffset+mx-3])
             if xoffset > 0:
                 stdscr.addstr(chi,0,"<",set_colour(BLUE,WHITE))
+            if len(text[chi-2]) > xoffset + mx - 3:
+                stdscr.addstr(chi,mx-1,">",set_colour(GREEN,WHITE))
         stdscr.addstr(0,mx-10,f"{ln},{col}",set_colour(WHITE,BLACK))
+        stdscr.addstr(0,30,ERROR,set_colour(WHITE,RED))
         stdscr.move(ln+2,col-xoffset+1)
         
+        if ERROR != "":
+            ERROR = ""
         stdscr.refresh()
         ch = stdscr.getch()
         chn = curses.keyname(ch)
         if ch == 10 or ch == 13 or ch == curses.KEY_ENTER or ch == curses.KEY_DOWN:
             if ln == lines - 1:
+                ERROR = " You have reached the bottom of the page. "
                 curses.beep()
             else:
                 ln += 1
                 col = 0
         elif ch == curses.KEY_LEFT:
             if col > 0:
                 col -= 1
                 if xoffset > 0:
                     xoffset -= 1
                     stdscr.clear()
             else:
+                ERROR = " You have reached the end of the text "
+
                 curses.beep()
         elif ch == curses.KEY_RIGHT:
             if col < len(__retr_nbl_lst(text[ln])):
                 col += 1
                 if col-xoffset > mx-2:
                     xoffset += 1
                     stdscr.clear()
             else:
+                ERROR = " You have reached the end of the text "
                 curses.beep()
         elif ch == curses.KEY_BACKSPACE:
             if col > 0:
                 del text[ln][col-1]
                 col -= 1
                 if xoffset > 0:
                     xoffset -= 1
                 stdscr.clear()#Fix render errors
               
             else:
+                ERROR = " You may not backspace further "
                 curses.beep()
         elif ch == curses.KEY_UP:
             if ln > 0:
                 ln -= 1
                 col = 0
+            else:
+                ERROR = " You have reached the top of the text "
+                curses.beep()
         else:
             if len(chn) > 1:
                 #Special char
                 if chn == b"^D":
                     stdscr.erase()
                     return "\n".join(["".join(t) for t in text])
                 elif chn == b"^K":
                     text = [[] for _ in range(lines)]#Delete
                     ln = 0
                     col = 0
                     stdscr.erase()
-                else:
-                    curses.beep()
             else:
                 #append
-                col += 1
-                text[ln].insert(col-1,chn.decode())
-                
-                if col > mx-2:
-                    xoffset += 1
-                    stdscr.clear()
+                if __calc_nbl_list(text) == maxlen and maxlen != 0:
+                    curses.beep()
+                    ERROR = f" You have reached the character limit ({maxlen}) "
+                else:
+                    col += 1
+                    text[ln].insert(col-1,chn.decode())
+                    
+                    if col > mx-2:
+                        xoffset += 1
+                        stdscr.clear()
     
 
 def displayops(stdscr,options: list,title="Please choose an option") -> int:
     """Display an options menu provided by options list. ALso displays title. Returns integer value of selected item."""
     mx, my = os.get_terminal_size()
     selected = 0
```

### Comparing `cursesplus-2.3.0/src/cursesplus/filedialog.py` & `cursesplus-2.3.1/src/cursesplus/filedialog.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.0/src/cursesplus/messagebox.py` & `cursesplus-2.3.1/src/cursesplus/messagebox.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.0/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.3.1/src/cursesplus.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.3.0
+Version: 2.3.1
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,20 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
+### Patch 2.3.1:
+
+-Add character limit to new input
+
+-Add more functionality
+
 ### Version 2.3: New Input
 
 -Rewrite cursesinput function
 
 -Remains backwards-compatible
 
 ### Version 2.0: Incompatible api changes
```

