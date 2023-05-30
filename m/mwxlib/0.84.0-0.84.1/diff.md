# Comparing `tmp/mwxlib-0.84.0-py3-none-any.whl.zip` & `tmp/mwxlib-0.84.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 162268 bytes, number of entries: 22
+Zip file size: 162377 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat     2520 b- defN 23-May-02 16:40 mwx/__init__.py
 -rw-rw-rw-  2.0 fat    43445 b- defN 23-May-02 17:15 mwx/controls.py
--rw-rw-rw-  2.0 fat    73540 b- defN 23-May-27 03:59 mwx/framework.py
+-rw-rw-rw-  2.0 fat    73753 b- defN 23-May-30 08:08 mwx/framework.py
 -rw-rw-rw-  2.0 fat    69520 b- defN 23-May-25 03:20 mwx/graphman.py
 -rw-rw-rw-  2.0 fat    46248 b- defN 23-Feb-21 08:49 mwx/images.py
 -rw-rw-rw-  2.0 fat    36017 b- defN 23-May-17 04:56 mwx/matplot2.py
 -rw-rw-rw-  2.0 fat    68253 b- defN 23-May-17 11:19 mwx/matplot2g.py
 -rw-rw-rw-  2.0 fat    27606 b- defN 23-Apr-27 09:45 mwx/matplot2lg.py
 -rw-rw-rw-  2.0 fat     6878 b- defN 23-Feb-21 08:50 mwx/mgplt.py
--rw-rw-rw-  2.0 fat   138667 b- defN 23-May-27 04:10 mwx/nutshell.py
--rw-rw-rw-  2.0 fat    37403 b- defN 23-May-25 03:20 mwx/utilus.py
+-rw-rw-rw-  2.0 fat   138760 b- defN 23-May-30 08:08 mwx/nutshell.py
+-rw-rw-rw-  2.0 fat    37431 b- defN 23-May-30 08:08 mwx/utilus.py
 -rw-rw-rw-  2.0 fat    11343 b- defN 23-May-16 07:42 mwx/wxmon.py
 -rw-rw-rw-  2.0 fat    19367 b- defN 23-May-16 07:42 mwx/wxpdb.py
 -rw-rw-rw-  2.0 fat     5254 b- defN 23-May-16 07:42 mwx/wxwil.py
 -rw-rw-rw-  2.0 fat     7424 b- defN 23-May-16 07:42 mwx/wxwit.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-23 14:06 mwx/py/__init__.py
 -rw-rw-rw-  2.0 fat    16794 b- defN 23-Apr-27 09:45 mwx/py/filling.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-27 16:26 mwxlib-0.84.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1893 b- defN 23-May-27 16:26 mwxlib-0.84.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-27 16:26 mwxlib-0.84.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-May-27 16:26 mwxlib-0.84.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1609 b- defN 23-May-27 16:26 mwxlib-0.84.0.dist-info/RECORD
-22 files, 614968 bytes uncompressed, 159766 bytes compressed:  74.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-30 08:37 mwxlib-0.84.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1893 b- defN 23-May-30 08:37 mwxlib-0.84.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 08:37 mwxlib-0.84.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-May-30 08:37 mwxlib-0.84.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1609 b- defN 23-May-30 08:37 mwxlib-0.84.1.dist-info/RECORD
+22 files, 615302 bytes uncompressed, 159875 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: mwx/py/__init__.py
 Comment: 
 
 Filename: mwx/py/filling.py
 Comment: 
 
-Filename: mwxlib-0.84.0.dist-info/LICENSE
+Filename: mwxlib-0.84.1.dist-info/LICENSE
 Comment: 
 
-Filename: mwxlib-0.84.0.dist-info/METADATA
+Filename: mwxlib-0.84.1.dist-info/METADATA
 Comment: 
 
-Filename: mwxlib-0.84.0.dist-info/WHEEL
+Filename: mwxlib-0.84.1.dist-info/WHEEL
 Comment: 
 
-Filename: mwxlib-0.84.0.dist-info/top_level.txt
+Filename: mwxlib-0.84.1.dist-info/top_level.txt
 Comment: 
 
-Filename: mwxlib-0.84.0.dist-info/RECORD
+Filename: mwxlib-0.84.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mwx/framework.py

```diff
@@ -1,14 +1,14 @@
 #! python3
 # -*- coding: utf-8 -*-
 """mwxlib framework
 
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 """
-__version__ = "0.84.0"
+__version__ = "0.84.1"
 __author__ = "Kazuya O'moto <komoto@jeol.co.jp>"
 
 from functools import wraps, partial
 from importlib import reload
 import traceback
 import builtins
 import datetime
@@ -371,21 +371,22 @@
     assert not wx.ID_LOWEST <= id <= wx.ID_HIGHEST
     return id
 
 
 def pack(self, items, orient=wx.HORIZONTAL, style=None, label=None):
     """Do layout
     
-    Examples:
-        >>> self.SetSizer(
+    Examples::
+    
+        self.SetSizer(
             pack(self, (
                 (label, 0, wx.ALIGN_CENTER | wx.LEFT, 4),
                 ( ctrl, 1, wx.ALIGN_CENTER | wx.LEFT, 4),
-                ))
-            )
+            ))
+        )
     
     Args:
         items   : wx objects (with some packing parameters)
         
                 - (obj, 1) -> sized with ratio 1 (parallel to `orient`)
                 - (obj, 1, wx.EXPAND) -> expanded with ratio 1 (perpendicular to `orient`)
                 - (obj, 0, wx.ALIGN_CENTER | wx.LEFT, 4) -> center with 4 pixel at wx.LEFT
@@ -485,23 +486,22 @@
         parent.PopupMenu(menu, *args, **kwargs)
         menu.Destroy()
 
 
 class MenuBar(wx.MenuBar, TreeList):
     """MenuBar control
     
-    Construct menubar in the order of menu:list
-    -> root
-        ├ [key, [item,
-        │        item,...]],
-        │
-        ├ [key, [item,
-        │        item,
-        │        submenu => [key, [item,
-        ：        ...               item,...]],
+    Construct menubar in the order of menu<TreeList>::
+    
+        root
+         ├ [key, [item,
+         │        item,...]],
+         ├ [key, [item,
+         │        submenu => [key, [item,
+         ：        ...               item,...]],
     """
     def __init__(self, *args, **kwargs):
         wx.MenuBar.__init__(self, *args, **kwargs)
         TreeList.__init__(self)
     
     def getmenu(self, key, root=None):
         if '/' in key:
@@ -1053,15 +1053,15 @@
             evt.Skip()
             if not evt.Active:
                 ## Reset autoload when active focus going outside.
                 self.__autoload = True
             elif evt.GetActivationReason() == evt.Reason_Mouse\
               and self.__autoload:
                 ## Check all buffers that need to be loaded.
-                for book in self.get_all_pages(type(self.Log)):
+                for book in self.all_books:
                     for buf in book.all_buffers:
                         if buf.need_buffer_load:
                             if wx.MessageBox( # Confirm load.
                                     "The file has been modified externally.\n\n"
                                     "The contents of the buffer will be overwritten.\n"
                                     "Continue loading?",
                                     "Load {!r}".format(buf.name),
@@ -1181,15 +1181,15 @@
                     wildcard="Session file (*.debrc)|*.debrc",
                     style=wx.FD_OPEN|wx.FD_FILE_MUST_EXIST|wx.FD_CHANGE_DIR) as dlg:
                 if dlg.ShowModal() != wx.ID_OK:
                     return
                 rc = dlg.Path
         
         if flush:
-            for book in self.get_all_pages(type(self.Log)):
+            for book in self.all_books:
                 book.delete_all_buffers()
         
         self.SESSION_FILE = os.path.abspath(rc)
         try:
             scratch = self.Scratch.default_buffer
             if not scratch or scratch.mtdelta is not None:
                 scratch = self.Scratch.new_buffer()
@@ -1217,42 +1217,32 @@
         scratch = self.Scratch.default_buffer
         if scratch and scratch.mtdelta is None:
             scratch.SaveFile(self.SCRATCH_FILE)
         
         with open(self.SESSION_FILE, 'w', encoding='utf-8', newline='') as o:
             o.write("#! Session file (This file is generated automatically)\n")
             
-            for book in self.get_all_pages(type(self.Log)):
+            for book in self.all_books:
                 for buf in book.all_buffers:
                     if buf.mtdelta is not None:
-                        o.write("self._load_file({!r}, {!r}, {})\n"
-                                .format(book.Name, buf.filename, buf.markline+1))
+                        o.write("self.load({!r}, {!r}, {!r})\n"
+                                .format(buf.filename, buf.markline+1, book.Name))
             o.write('\n'.join((
                 "self.SetSize({})".format(self.Size),
                 "self.SetPosition({})".format(self.Position),
                 "self.ghost.SetSelection({})".format(self.ghost.Selection),
                 "self.watcher.SetSelection({})".format(self.watcher.Selection),
                 "self._mgr.LoadPerspective({!r})".format(self._mgr.SavePerspective()),
                 "self.ghost.loadPerspective({!r})".format(self.ghost.savePerspective()),
                 "self.watcher.loadPerspective({!r})".format(self.watcher.savePerspective()),
                 ## "self._mgr.GetPane('ghost').FloatingPosition(self.Position)",
                 ## "self._mgr.GetPane('watcher').FloatingPosition(self.Position)",
                 "self._mgr.Update()\n",
             )))
     
-    def _load_file(self, bookname, filename, lineno):
-        try:
-            book = getattr(self, bookname)
-            if re.match(r"https?://[\w/:%#\$&\?()~.=+-]+", filename): # url_re
-                book.load_url(filename, lineno)
-            else:
-                book.load_file(filename, lineno)
-        except Exception:
-            pass
-    
     def Init(self):
         msg = "#! Opened: <{}>\r\n".format(datetime.datetime.now())
         self.add_history(msg)
         self.add_log(msg)
         self.load_session(self.SESSION_FILE)
     
     def Destroy(self):
@@ -1281,15 +1271,15 @@
             self.Quit()
         
         if self.debugger.tracing:
             wx.MessageBox("The debugger ends tracing.\n\n"
                           "The trace pointer will be cleared.")
             self.debugger.unwatch() # cf. [pointer_unset] stop_trace
         
-        for book in self.get_all_pages(type(self.Log)):
+        for book in self.all_books:
             for buf in book.all_buffers:
                 if buf.need_buffer_save:
                     self.popup_window(book)
                     buf.SetFocus()
                     if wx.MessageBox( # Confirm close.
                             "You are closing unsaved content.\n\n"
                             "Changes to the content will be discarded.\n"
@@ -1387,15 +1377,15 @@
                 "#{!r}".format(wx),
                 "To show the credit, press C-M-Mbutton.\n",
                 ))
             )
         self.popup_window(self.Help, focus=0)
     
     def toggle_window(self, win, focus=False):
-        self.popup_window(win, None, focus)
+        self.popup_window(win, show=None, focus=focus)
     
     def popup_window(self, win, show=True, focus=True):
         """Show the notebook page and move the focus.
         
         Args:
             win  : window to popup
             show : True, False, otherwise None:toggle
@@ -1442,35 +1432,49 @@
         self.debugger.send_input('\n') # terminates the reader
         shell = self.debugger.interactive_shell # reset interp locals
         del shell.locals
         del shell.globals
         self.indicator.Value = 1
         self.message("Quit")
     
-    def load(self, filename, lineno=0, show=True, focus=False):
+    def load(self, filename, lineno=0, book=None, show=True, focus=False):
         """Load file @where the object is defined.
         
         Args:
-            filename : target filename or object.
+            filename : target filename:str or object.
+                       It also supports <'filename:lineno'> format.
+            lineno   : Set mark to lineno on load.
+            book     : book of the buffer to load.
+            show     : Show the book.
             focus    : Set the focus if the window is displayed.
         """
         if not isinstance(filename, str):
             filename = where(filename)
             if filename is None:
                 return False
-        ## Support <'filename:lineno'>
         if not lineno:
             m = re.match("(.*?):([0-9]+)", filename)
             if m:
                 filename, ln = m.groups()
                 lineno = int(ln)
-        book = next((x for x in self.get_all_pages(type(self.Log))
-                             if x.find_buffer(filename)), self.Log)
-        self.popup_window(book, show, focus)
-        return book.load_file(filename, lineno)
+        if isinstance(book, str):
+            try:
+                book = getattr(self, book)
+            except Exception:
+                pass
+        if not book:
+            book = next((x for x in self.all_books
+                            if x.find_buffer(filename)), self.Log)
+        if show:
+            self.popup_window(book, focus=focus)
+        
+        if re.match(r"https?://[\w/:%#\$&\?()~.=+-]+", filename): # url_re
+            return book.load_url(filename, lineno)
+        else:
+            return book.load_file(filename, lineno)
     
     def info(self, obj):
         self.rootshell.info(obj)
     
     def help(self, obj):
         self.rootshell.help(obj)
     
@@ -1703,14 +1707,19 @@
         """Yields all pages of the specified type in the notebooks."""
         yield from self.console.get_pages(type)
         yield from self.ghost.get_pages(type)
     
     get_pages = get_all_pages # for backward compatibility
     
     @property
+    def all_books(self):
+        """Yields all books in the notebooks."""
+        yield from self.get_all_pages(type(self.Log))
+    
+    @property
     def current_shell(self):
         """Currently selected shell or rootshell."""
         return self.console.CurrentPage
     
     ## --------------------------------
     ## Find text dialog
     ## --------------------------------
```

## mwx/nutshell.py

```diff
@@ -1883,14 +1883,17 @@
     
     ## --------------------------------
     ## Buffer list controls
     ## --------------------------------
     
     @property
     def all_buffers(self):
+        """Returns all buffer pages.
+        cf. equiv. AuiNotebook.all_pages
+        """
         return [self.GetPage(j) for j in range(self.PageCount)]
     
     @property
     def menu(self):
         """Yields context menu."""
         def _menu(j, buf):
             caption = "{}:{}".format(buf.filename, buf.markline+1)
```

## mwx/utilus.py

```diff
@@ -877,23 +877,24 @@
             except AttributeError:
                 warn("- FSM:warning: removing action from context ({!r} : {!r})\n"
                      "  The transaction must be a list, not a tuple".format(state, event))
         return False
 
 
 class TreeList(object):
-    """Tree access wrapper of list<item : (key, value)>
-    [
-        [key, [item,
-               item, ...]],
-        [key, [item,
-               [branch], => [key, [item,
-                                   item, ...]],
-               ...]],
-    ]
+    """Interface class for tree list control.
+    
+    >>> list<item : (key, value)>
+        [[key, [item,
+                item, ...]],
+         [key, [item,
+                branch => [key, [item,
+                                 item, ...]],
+                ...]],
+        ]
     """
     ## A dummy list to avoid RecursionError occurs when
     ## __getattr__ may be called before __init__.
     __items = None
     
     def __init__(self, ls=None):
         self.__items = ls or []
```

## Comparing `mwxlib-0.84.0.dist-info/LICENSE` & `mwxlib-0.84.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mwxlib-0.84.0.dist-info/METADATA` & `mwxlib-0.84.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwxlib
-Version: 0.84.0
+Version: 0.84.1
 Summary: A wrapper of matplotlib and wxPython (phoenix)
 Home-page: https://github.com/komoto48g/mwxlib
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 Author-email: komoto@jeol.co.jp
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

