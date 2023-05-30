# Comparing `tmp/aqimon-0.5.1.tar.gz` & `tmp/aqimon-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqimon-0.5.1.tar", max compression
+gzip compressed data, was "aqimon-0.6.0.tar", max compression
```

## Comparing `aqimon-0.5.1.tar` & `aqimon-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1065 2023-05-16 05:30:11.370659 aqimon-0.5.1/LICENSE
--rw-r--r--   0        0        0     5905 2023-05-16 05:30:11.370659 aqimon-0.5.1/README.md
--rw-r--r--   0        0        0       45 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/__init__.py
--rw-r--r--   0        0        0     2633 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/aqi_common.py
--rw-r--r--   0        0        0     2372 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/config.py
--rw-r--r--   0        0        0     7030 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/database.py
--rw-r--r--   0        0        0      881 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/read/__init__.py
--rw-r--r--   0        0        0     1712 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/read/mock.py
--rw-r--r--   0        0        0     2139 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/read/novapm.py
--rw-r--r--   0        0        0     8437 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/server.py
--rw-r--r--   0        0        0     6835 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/static/android-chrome-192x192.png
--rw-r--r--   0        0        0    20365 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/static/android-chrome-512x512.png
--rw-r--r--   0        0        0     6288 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/static/apple-touch-icon.png
--rw-r--r--   0        0        0   452012 2023-05-16 05:30:37.362727 aqimon-0.5.1/aqimon/static/elm.js
--rw-r--r--   0        0        0      351 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/static/favicon-16x16.png
--rw-r--r--   0        0        0      754 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/static/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/static/favicon.ico
--rw-r--r--   0        0        0     1799 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/static/images/failing.png
--rw-r--r--   0        0        0     2418 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/static/images/idle.png
--rw-r--r--   0        0        0     6349 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/static/images/loading.gif
--rw-r--r--   0        0        0    44088 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/static/images/warmingup.gif
--rw-r--r--   0        0        0      696 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/static/index.html
--rw-r--r--   0        0        0     5587 2023-05-16 05:30:11.370659 aqimon-0.5.1/aqimon/templates/index.html
--rw-r--r--   0        0        0      989 2023-05-16 05:30:11.370659 aqimon-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     6539 1970-01-01 00:00:00.000000 aqimon-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-30 02:26:35.980069 aqimon-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5921 2023-05-30 02:26:35.980069 aqimon-0.6.0/README.md
+-rw-r--r--   0        0        0       45 2023-05-30 02:26:35.980069 aqimon-0.6.0/aqimon/__init__.py
+-rw-r--r--   0        0        0     2633 2023-05-30 02:26:35.980069 aqimon-0.6.0/aqimon/aqi_common.py
+-rw-r--r--   0        0        0     2372 2023-05-30 02:26:35.980069 aqimon-0.6.0/aqimon/config.py
+-rw-r--r--   0        0        0     7030 2023-05-30 02:26:35.980069 aqimon-0.6.0/aqimon/database.py
+-rw-r--r--   0        0        0      881 2023-05-30 02:26:35.980069 aqimon-0.6.0/aqimon/read/__init__.py
+-rw-r--r--   0        0        0     1712 2023-05-30 02:26:35.980069 aqimon-0.6.0/aqimon/read/mock.py
+-rw-r--r--   0        0        0     2139 2023-05-30 02:26:35.980069 aqimon-0.6.0/aqimon/read/novapm.py
+-rw-r--r--   0        0        0     8437 2023-05-30 02:26:35.980069 aqimon-0.6.0/aqimon/server.py
+-rw-r--r--   0        0        0     6835 2023-05-30 02:26:35.980069 aqimon-0.6.0/aqimon/static/android-chrome-192x192.png
+-rw-r--r--   0        0        0    20365 2023-05-30 02:26:35.984068 aqimon-0.6.0/aqimon/static/android-chrome-512x512.png
+-rw-r--r--   0        0        0     6288 2023-05-30 02:26:35.984068 aqimon-0.6.0/aqimon/static/apple-touch-icon.png
+-rw-r--r--   0        0        0   457813 2023-05-30 02:27:01.472333 aqimon-0.6.0/aqimon/static/elm.js
+-rw-r--r--   0        0        0      351 2023-05-30 02:26:35.984068 aqimon-0.6.0/aqimon/static/favicon-16x16.png
+-rw-r--r--   0        0        0      754 2023-05-30 02:26:35.984068 aqimon-0.6.0/aqimon/static/favicon-32x32.png
+-rw-r--r--   0        0        0     1001 2023-05-30 02:26:35.984068 aqimon-0.6.0/aqimon/static/favicon.ico
+-rw-r--r--   0        0        0     8099 2023-05-30 02:26:35.984068 aqimon-0.6.0/aqimon/static/images/aqimon.png
+-rw-r--r--   0        0        0     1799 2023-05-30 02:26:35.984068 aqimon-0.6.0/aqimon/static/images/failing.png
+-rw-r--r--   0        0        0     2418 2023-05-30 02:26:35.984068 aqimon-0.6.0/aqimon/static/images/idle.png
+-rw-r--r--   0        0        0     6349 2023-05-30 02:26:35.984068 aqimon-0.6.0/aqimon/static/images/loading.gif
+-rw-r--r--   0        0        0    44088 2023-05-30 02:26:35.984068 aqimon-0.6.0/aqimon/static/images/warmingup.gif
+-rw-r--r--   0        0        0      759 2023-05-30 02:26:35.984068 aqimon-0.6.0/aqimon/static/index.html
+-rw-r--r--   0        0        0      989 2023-05-30 02:26:35.984068 aqimon-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6555 1970-01-01 00:00:00.000000 aqimon-0.6.0/PKG-INFO
```

### Comparing `aqimon-0.5.1/LICENSE` & `aqimon-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aqimon-0.5.1/README.md` & `aqimon-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AQIMON
+# ![AQIMON](header.png) 
 
 A simple Air Quality Index monitor, designed to work on the Raspberry Pi with the SDS011 Nova PM Sensor.
 
 - [AQIMON](#aqimon)
   - [Screenshot](#screenshot) 
   - [Installation](#installation)
     - [Pre-Requisites](#pre-requisites)
```

### Comparing `aqimon-0.5.1/aqimon/aqi_common.py` & `aqimon-0.6.0/aqimon/aqi_common.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.5.1/aqimon/config.py` & `aqimon-0.6.0/aqimon/config.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.5.1/aqimon/database.py` & `aqimon-0.6.0/aqimon/database.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.5.1/aqimon/read/__init__.py` & `aqimon-0.6.0/aqimon/read/__init__.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.5.1/aqimon/read/mock.py` & `aqimon-0.6.0/aqimon/read/mock.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.5.1/aqimon/read/novapm.py` & `aqimon-0.6.0/aqimon/read/novapm.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.5.1/aqimon/server.py` & `aqimon-0.6.0/aqimon/server.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.5.1/aqimon/static/android-chrome-192x192.png` & `aqimon-0.6.0/aqimon/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.5.1/aqimon/static/android-chrome-512x512.png` & `aqimon-0.6.0/aqimon/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.5.1/aqimon/static/apple-touch-icon.png` & `aqimon-0.6.0/aqimon/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.5.1/aqimon/static/elm.js` & `aqimon-0.6.0/aqimon/static/elm.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -828,18 +828,18 @@
 
             case 11:
                 throw new Error('Cannot perform mod 0. Division by zero error.');
         }
     }
 
     function _Debug_regionToString(region) {
-        if (region.dz.aY === region.d_.aY) {
-            return 'on line ' + region.dz.aY;
+        if (region.dB.a_ === region.d0.a_) {
+            return 'on line ' + region.dB.a_;
         }
-        return 'on lines ' + region.dz.aY + ' through ' + region.d_.aY;
+        return 'on lines ' + region.dB.a_ + ' through ' + region.d0.a_;
     }
 
 
 
     // MATH
 
     var _Basics_add = F2(function(a, b) {
@@ -1822,17 +1822,17 @@
     // PROGRAMS
 
 
     var _Platform_worker = F4(function(impl, flagDecoder, debugMetadata, args) {
         return _Platform_initialize(
             flagDecoder,
             args,
-            impl.fQ,
-            impl.gu,
-            impl.gd,
+            impl.fR,
+            impl.gv,
+            impl.ge,
             function() {
                 return function() {}
             }
         );
     });
 
 
@@ -2623,16 +2623,16 @@
     var _VirtualDom_mapEventTuple = F2(function(func, tuple) {
         return _Utils_Tuple2(func(tuple.a), tuple.b);
     });
 
     var _VirtualDom_mapEventRecord = F2(function(func, record) {
         return {
             ae: func(record.ae),
-            dB: record.dB,
-            dm: record.dm
+            dD: record.dD,
+            $7: record.$7
         }
     });
 
 
 
     // ORGANIZE FACTS
 
@@ -2865,18 +2865,18 @@
             // 0 = Normal
             // 1 = MayStopPropagation
             // 2 = MayPreventDefault
             // 3 = Custom
 
             var value = result.a;
             var message = !tag ? value : tag < 3 ? value.a : value.ae;
-            var stopPropagation = tag == 1 ? value.b : tag == 3 && value.dB;
+            var stopPropagation = tag == 1 ? value.b : tag == 3 && value.dD;
             var currentEventNode = (
                 stopPropagation && event.stopPropagation(),
-                (tag == 2 ? value.b : tag == 3 && value.dm) && event.preventDefault(),
+                (tag == 2 ? value.b : tag == 3 && value.$7) && event.preventDefault(),
                 eventNode
             );
             var tagger;
             var i;
             while (tagger = currentEventNode.j) {
                 if (typeof tagger == 'function') {
                     message = tagger(message);
@@ -3717,19 +3717,19 @@
 
     var _Debugger_element;
 
     var _Browser_element = _Debugger_element || F4(function(impl, flagDecoder, debugMetadata, args) {
         return _Platform_initialize(
             flagDecoder,
             args,
-            impl.fQ,
-            impl.gu,
-            impl.gd,
+            impl.fR,
+            impl.gv,
+            impl.ge,
             function(sendToApp, initialModel) {
-                var view = impl.gw;
+                var view = impl.gx;
                 /**/
                 var domNode = args['node'];
                 //*/
                 /**_UNUSED/
                 var domNode = args && args['node'] ? args['node'] : _Debug_crash(0);
                 //*/
                 var currNode = _VirtualDom_virtualize(domNode);
@@ -3751,32 +3751,32 @@
 
     var _Debugger_document;
 
     var _Browser_document = _Debugger_document || F4(function(impl, flagDecoder, debugMetadata, args) {
         return _Platform_initialize(
             flagDecoder,
             args,
-            impl.fQ,
-            impl.gu,
-            impl.gd,
+            impl.fR,
+            impl.gv,
+            impl.ge,
             function(sendToApp, initialModel) {
-                var divertHrefToApp = impl.ds && impl.ds(sendToApp)
-                var view = impl.gw;
+                var divertHrefToApp = impl.du && impl.du(sendToApp)
+                var view = impl.gx;
                 var title = _VirtualDom_doc.title;
                 var bodyNode = _VirtualDom_doc.body;
                 var currNode = _VirtualDom_virtualize(bodyNode);
                 return _Browser_makeAnimator(initialModel, function(model) {
                     _VirtualDom_divertHrefToApp = divertHrefToApp;
                     var doc = view(model);
-                    var nextNode = _VirtualDom_node('body')(_List_Nil)(doc.fs);
+                    var nextNode = _VirtualDom_node('body')(_List_Nil)(doc.ft);
                     var patches = _VirtualDom_diff(currNode, nextNode);
                     bodyNode = _VirtualDom_applyPatches(bodyNode, currNode, patches, sendToApp);
                     currNode = nextNode;
                     _VirtualDom_divertHrefToApp = 0;
-                    (title !== doc.gi) && (_VirtualDom_doc.title = title = doc.gi);
+                    (title !== doc.gj) && (_VirtualDom_doc.title = title = doc.gj);
                 });
             }
         );
     });
 
 
 
@@ -3825,50 +3825,50 @@
 
 
 
     // APPLICATION
 
 
     function _Browser_application(impl) {
-        var onUrlChange = impl.f_;
-        var onUrlRequest = impl.f$;
+        var onUrlChange = impl.f$;
+        var onUrlRequest = impl.f0;
         var key = function() {
             key.a(onUrlChange(_Browser_getUrl()));
         };
 
         return _Browser_document({
-            ds: function(sendToApp) {
+            du: function(sendToApp) {
                 key.a = sendToApp;
                 _Browser_window.addEventListener('popstate', key);
                 _Browser_window.navigator.userAgent.indexOf('Trident') < 0 || _Browser_window.addEventListener('hashchange', key);
 
                 return F2(function(domNode, event) {
                     if (!event.ctrlKey && !event.metaKey && !event.shiftKey && event.button < 1 && !domNode.target && !domNode.hasAttribute('download')) {
                         event.preventDefault();
                         var href = domNode.href;
                         var curr = _Browser_getUrl();
                         var next = $elm$url$Url$fromString(href).a;
                         sendToApp(onUrlRequest(
                             (next &&
-                                curr.eM === next.eM &&
-                                curr.eb === next.eb &&
-                                curr.eH.a === next.eH.a
+                                curr.eN === next.eN &&
+                                curr.ec === next.ec &&
+                                curr.eI.a === next.eI.a
                             ) ?
                             $elm$browser$Browser$Internal(next) :
                             $elm$browser$Browser$External(href)
                         ));
                     }
                 });
             },
-            fQ: function(flags) {
-                return A3(impl.fQ, flags, _Browser_getUrl(), key);
+            fR: function(flags) {
+                return A3(impl.fR, flags, _Browser_getUrl(), key);
             },
-            gw: impl.gw,
-            gu: impl.gu,
-            gd: impl.gd
+            gx: impl.gx,
+            gv: impl.gv,
+            ge: impl.ge
         });
     }
 
     function _Browser_getUrl() {
         return $elm$url$Url$fromString(_VirtualDom_doc.location.href).a || _Debug_crash(1);
     }
 
@@ -3928,35 +3928,35 @@
 
     // PAGE VISIBILITY
 
 
     function _Browser_visibilityInfo() {
         return (typeof _VirtualDom_doc.hidden !== 'undefined') ?
             {
-                fJ: 'hidden',
-                fu: 'visibilitychange'
+                fK: 'hidden',
+                fv: 'visibilitychange'
             } :
             (typeof _VirtualDom_doc.mozHidden !== 'undefined') ?
             {
-                fJ: 'mozHidden',
-                fu: 'mozvisibilitychange'
+                fK: 'mozHidden',
+                fv: 'mozvisibilitychange'
             } :
             (typeof _VirtualDom_doc.msHidden !== 'undefined') ?
             {
-                fJ: 'msHidden',
-                fu: 'msvisibilitychange'
+                fK: 'msHidden',
+                fv: 'msvisibilitychange'
             } :
             (typeof _VirtualDom_doc.webkitHidden !== 'undefined') ?
             {
-                fJ: 'webkitHidden',
-                fu: 'webkitvisibilitychange'
+                fK: 'webkitHidden',
+                fv: 'webkitvisibilitychange'
             } :
             {
-                fJ: 'hidden',
-                fu: 'visibilitychange'
+                fK: 'hidden',
+                fv: 'visibilitychange'
             };
     }
 
 
 
     // ANIMATION FRAMES
 
@@ -4020,30 +4020,30 @@
 
 
     // WINDOW VIEWPORT
 
 
     function _Browser_getViewport() {
         return {
-            eZ: _Browser_getScene(),
-            ff: {
-                fj: _Browser_window.pageXOffset,
-                fk: _Browser_window.pageYOffset,
-                fi: _Browser_doc.documentElement.clientWidth,
-                ea: _Browser_doc.documentElement.clientHeight
+            e_: _Browser_getScene(),
+            fg: {
+                fk: _Browser_window.pageXOffset,
+                fl: _Browser_window.pageYOffset,
+                fj: _Browser_doc.documentElement.clientWidth,
+                eb: _Browser_doc.documentElement.clientHeight
             }
         };
     }
 
     function _Browser_getScene() {
         var body = _Browser_doc.body;
         var elem = _Browser_doc.documentElement;
         return {
-            fi: Math.max(body.scrollWidth, body.offsetWidth, elem.scrollWidth, elem.offsetWidth, elem.clientWidth),
-            ea: Math.max(body.scrollHeight, body.offsetHeight, elem.scrollHeight, elem.offsetHeight, elem.clientHeight)
+            fj: Math.max(body.scrollWidth, body.offsetWidth, elem.scrollWidth, elem.offsetWidth, elem.clientWidth),
+            eb: Math.max(body.scrollHeight, body.offsetHeight, elem.scrollHeight, elem.offsetHeight, elem.clientHeight)
         };
     }
 
     var _Browser_setViewport = F2(function(x, y) {
         return _Browser_withWindow(function() {
             _Browser_window.scroll(x, y);
             return _Utils_Tuple0;
@@ -4054,23 +4054,23 @@
 
     // ELEMENT VIEWPORT
 
 
     function _Browser_getViewportOf(id) {
         return _Browser_withNode(id, function(node) {
             return {
-                eZ: {
-                    fi: node.scrollWidth,
-                    ea: node.scrollHeight
+                e_: {
+                    fj: node.scrollWidth,
+                    eb: node.scrollHeight
                 },
-                ff: {
-                    fj: node.scrollLeft,
-                    fk: node.scrollTop,
-                    fi: node.clientWidth,
-                    ea: node.clientHeight
+                fg: {
+                    fk: node.scrollLeft,
+                    fl: node.scrollTop,
+                    fj: node.clientWidth,
+                    eb: node.clientHeight
                 }
             };
         });
     }
 
 
     var _Browser_setViewportOf = F3(function(id, x, y) {
@@ -4088,26 +4088,26 @@
 
     function _Browser_getElement(id) {
         return _Browser_withNode(id, function(node) {
             var rect = node.getBoundingClientRect();
             var x = _Browser_window.pageXOffset;
             var y = _Browser_window.pageYOffset;
             return {
-                eZ: _Browser_getScene(),
-                ff: {
-                    fj: x,
-                    fk: y,
-                    fi: _Browser_doc.documentElement.clientWidth,
-                    ea: _Browser_doc.documentElement.clientHeight
+                e_: _Browser_getScene(),
+                fg: {
+                    fk: x,
+                    fl: y,
+                    fj: _Browser_doc.documentElement.clientWidth,
+                    eb: _Browser_doc.documentElement.clientHeight
                 },
-                fE: {
-                    fj: x + rect.left,
-                    fk: y + rect.top,
-                    fi: rect.width,
-                    ea: rect.height
+                fF: {
+                    fk: x + rect.left,
+                    fl: y + rect.top,
+                    fj: rect.width,
+                    eb: rect.height
                 }
             };
         });
     }
 
 
 
@@ -4174,58 +4174,58 @@
 
 
     // SEND REQUEST
 
     var _Http_toTask = F3(function(router, toTask, request) {
         return _Scheduler_binding(function(callback) {
             function done(response) {
-                callback(toTask(request.cZ.a(response)));
+                callback(toTask(request.c$.a(response)));
             }
 
             var xhr = new XMLHttpRequest();
             xhr.addEventListener('error', function() {
                 done($elm$http$Http$NetworkError_);
             });
             xhr.addEventListener('timeout', function() {
                 done($elm$http$Http$Timeout_);
             });
             xhr.addEventListener('load', function() {
-                done(_Http_toResponse(request.cZ.b, xhr));
+                done(_Http_toResponse(request.c$.b, xhr));
             });
-            $elm$core$Maybe$isJust(request.fc) && _Http_track(router, xhr, request.fc.a);
+            $elm$core$Maybe$isJust(request.fd) && _Http_track(router, xhr, request.fd.a);
 
             try {
-                xhr.open(request.fX, request.dF, true);
+                xhr.open(request.fY, request.dH, true);
             } catch (e) {
-                return done($elm$http$Http$BadUrl_(request.dF));
+                return done($elm$http$Http$BadUrl_(request.dH));
             }
 
             _Http_configureRequest(xhr, request);
 
-            request.fs.a && xhr.setRequestHeader('Content-Type', request.fs.a);
-            xhr.send(request.fs.b);
+            request.ft.a && xhr.setRequestHeader('Content-Type', request.ft.a);
+            xhr.send(request.ft.b);
 
             return function() {
                 xhr.c = true;
                 xhr.abort();
             };
         });
     });
 
 
     // CONFIGURE
 
     function _Http_configureRequest(xhr, request) {
-        for (var headers = request.d9; headers.b; headers = headers.b) // WHILE_CONS
+        for (var headers = request.ea; headers.b; headers = headers.b) // WHILE_CONS
         {
             xhr.setRequestHeader(headers.a.a, headers.a.b);
         }
-        xhr.timeout = request.gg.a || 0;
-        xhr.responseType = request.cZ.d;
-        xhr.withCredentials = request.fn;
+        xhr.timeout = request.gh.a || 0;
+        xhr.responseType = request.c$.d;
+        xhr.withCredentials = request.fo;
     }
 
 
     // RESPONSES
 
     function _Http_toResponse(toBody, xhr) {
         return A2(
@@ -4236,18 +4236,18 @@
     }
 
 
     // METADATA
 
     function _Http_toMetadata(xhr) {
         return {
-            dF: xhr.responseURL,
-            gb: xhr.status,
-            gc: xhr.statusText,
-            d9: _Http_parseHeaders(xhr.getAllResponseHeaders())
+            dH: xhr.responseURL,
+            gc: xhr.status,
+            gd: xhr.statusText,
+            ea: _Http_parseHeaders(xhr.getAllResponseHeaders())
         };
     }
 
 
     // HEADERS
 
     function _Http_parseHeaders(rawHeaders) {
@@ -4338,25 +4338,25 @@
         // TODO check out lengthComputable on loadstart event
 
         xhr.upload.addEventListener('progress', function(event) {
             if (xhr.c) {
                 return;
             }
             _Scheduler_rawSpawn(A2($elm$core$Platform$sendToSelf, router, _Utils_Tuple2(tracker, $elm$http$Http$Sending({
-                f8: event.loaded,
-                e1: event.total
+                f9: event.loaded,
+                e2: event.total
             }))));
         });
         xhr.addEventListener('progress', function(event) {
             if (xhr.c) {
                 return;
             }
             _Scheduler_rawSpawn(A2($elm$core$Platform$sendToSelf, router, _Utils_Tuple2(tracker, $elm$http$Http$Receiving({
-                f3: event.loaded,
-                e1: event.lengthComputable ? $elm$core$Maybe$Just(event.total) : $elm$core$Maybe$Nothing
+                f4: event.loaded,
+                e2: event.lengthComputable ? $elm$core$Maybe$Just(event.total) : $elm$core$Maybe$Nothing
             }))));
         });
     }
 
 
     var _Bitwise_and = F2(function(a, b) {
         return a & b;
@@ -4926,20 +4926,20 @@
     };
     var $elm$browser$Browser$Dom$NotFound = $elm$core$Basics$identity;
     var $elm$url$Url$Http = 0;
     var $elm$url$Url$Https = 1;
     var $elm$url$Url$Url = F6(
         function(protocol, host, port_, path, query, fragment) {
             return {
-                d7: fragment,
-                eb: host,
-                eD: path,
-                eH: port_,
-                eM: protocol,
-                eN: query
+                d8: fragment,
+                ec: host,
+                eE: path,
+                eI: port_,
+                eN: protocol,
+                eO: query
             };
         });
     var $elm$core$String$contains = _String_contains;
     var $elm$core$String$length = _String_length;
     var $elm$core$String$slice = _String_slice;
     var $elm$core$String$dropLeft = F2(
         function(n, string) {
@@ -5223,14 +5223,20 @@
     };
     var $author$project$Main$FetchLatest = function(a) {
         return {
             $: 1,
             a: a
         };
     };
+    var $author$project$Main$GetTimeZone = function(a) {
+        return {
+            $: 3,
+            a: a
+        };
+    };
     var $author$project$Main$Hour = 1;
     var $author$project$DeviceStatus$Idle = 2;
     var $elm$core$Platform$Cmd$batch = _Platform_batch;
     var $elm$time$Time$Name = function(a) {
         return {
             $: 0,
             a: a
@@ -5247,56 +5253,60 @@
             return {
                 $: 0,
                 a: a,
                 b: b
             };
         });
     var $elm$time$Time$customZone = $elm$time$Time$Zone;
+    var $elm$time$Time$here = _Time_here(0);
     var $elm$time$Time$Posix = $elm$core$Basics$identity;
     var $elm$time$Time$millisToPosix = $elm$core$Basics$identity;
     var $elm$time$Time$now = _Time_now($elm$time$Time$millisToPosix);
+    var $elm$time$Time$utc = A2($elm$time$Time$Zone, 0, _List_Nil);
     var $author$project$Main$init = function(_v0) {
         return _Utils_Tuple2({
-                bp: _List_Nil,
-                bq: _List_Nil,
-                aO: 0,
-                dU: $elm$core$Maybe$Nothing,
-                dV: true,
+                br: _List_Nil,
+                bs: _List_Nil,
+                aQ: 0,
+                dW: $elm$core$Maybe$Nothing,
+                dX: true,
                 G: {
                     U: '',
                     V: '',
                     W: false
                 },
-                bV: _List_Nil,
-                bW: _List_Nil,
+                bX: _List_Nil,
+                bY: _List_Nil,
                 ad: {
-                    d$: $elm$core$Maybe$Nothing,
-                    d0: $elm$core$Maybe$Nothing,
-                    eF: $elm$core$Maybe$Nothing,
-                    eG: $elm$core$Maybe$Nothing
+                    c_: $elm$core$Maybe$Nothing,
+                    d1: $elm$core$Maybe$Nothing,
+                    eG: $elm$core$Maybe$Nothing,
+                    eH: $elm$core$Maybe$Nothing
                 },
-                b_: $elm$core$Maybe$Nothing,
+                b0: $elm$core$Maybe$Nothing,
                 Y: {
-                    dU: $elm$core$Maybe$Nothing,
-                    eo: $elm$core$Maybe$Nothing,
-                    eA: $elm$core$Maybe$Nothing,
-                    a1: 2
+                    dW: $elm$core$Maybe$Nothing,
+                    ep: $elm$core$Maybe$Nothing,
+                    eB: $elm$core$Maybe$Nothing,
+                    a3: 2
                 },
+                aJ: $elm$time$Time$utc,
                 ai: 1
             },
             $elm$core$Platform$Cmd$batch(
                 _List_fromArray(
                     [
                         A2($elm$core$Task$perform, $author$project$Main$FetchData, $elm$time$Time$now),
-                        A2($elm$core$Task$perform, $author$project$Main$FetchLatest, $elm$time$Time$now)
+                        A2($elm$core$Task$perform, $author$project$Main$FetchLatest, $elm$time$Time$now),
+                        A2($elm$core$Task$perform, $author$project$Main$GetTimeZone, $elm$time$Time$here)
                     ])));
     };
     var $author$project$Main$Tick = function(a) {
         return {
-            $: 9,
+            $: 10,
             a: a
         };
     };
     var $elm$core$Platform$Sub$batch = _Platform_batch;
     var $elm$time$Time$Every = F2(
         function(a, b) {
             return {
@@ -5304,16 +5314,16 @@
                 a: a,
                 b: b
             };
         });
     var $elm$time$Time$State = F2(
         function(taggers, processes) {
             return {
-                eL: processes,
-                e4: taggers
+                eM: processes,
+                e5: taggers
             };
         });
     var $elm$core$Dict$RBEmpty_elm_builtin = {
         $: -2
     };
     var $elm$core$Dict$empty = $elm$core$Dict$RBEmpty_elm_builtin;
     var $elm$time$Time$init = $elm$core$Task$succeed(
@@ -5593,15 +5603,15 @@
                         A3($elm$core$Dict$insert, interval, id, processes));
                 };
                 return A2($elm$core$Task$andThen, spawnRest, spawnTimer);
             }
         });
     var $elm$time$Time$onEffects = F3(
         function(router, subs, _v0) {
-            var processes = _v0.eL;
+            var processes = _v0.eM;
             var rightStep = F3(
                 function(_v6, id, _v7) {
                     var spawns = _v7.a;
                     var existing = _v7.b;
                     var kills = _v7.c;
                     return _Utils_Tuple3(
                         spawns,
@@ -5659,15 +5669,15 @@
                     function(_v2) {
                         return A3($elm$time$Time$spawnHelp, router, spawnList, existingDict);
                     },
                     killTask));
         });
     var $elm$time$Time$onSelfMsg = F3(
         function(router, interval, state) {
-            var _v0 = A2($elm$core$Dict$get, interval, state.e4);
+            var _v0 = A2($elm$core$Dict$get, interval, state.e5);
             if (_v0.$ === 1) {
                 return $elm$core$Task$succeed(state);
             } else {
                 var taggers = _v0.a;
                 var tellTaggers = function(time) {
                     return $elm$core$Task$sequence(
                         A2(
@@ -5746,47 +5756,47 @@
             default:
                 var errorMessage = error.a;
                 return errorMessage;
         }
     };
     var $author$project$Main$GotData = function(a) {
         return {
-            $: 3,
+            $: 4,
             a: a
         };
     };
     var $author$project$Main$AllData = F2(
         function(reads, epas) {
             return {
-                d1: epas,
-                eQ: reads
+                d2: epas,
+                eR: reads
             };
         });
     var $author$project$Main$EpaData = F2(
         function(time, epa) {
             return {
-                d$: epa,
-                cF: time
+                c_: epa,
+                aI: time
             };
         });
     var $elm$json$Json$Decode$field = _Json_decodeField;
     var $elm$json$Json$Decode$float = _Json_decodeFloat;
     var $elm$json$Json$Decode$list = _Json_decodeList;
     var $author$project$Main$epaDataDecoder = $elm$json$Json$Decode$list(
         A3(
             $elm$json$Json$Decode$map2,
             $author$project$Main$EpaData,
             A2($elm$json$Json$Decode$field, 't', $elm$json$Json$Decode$float),
             A2($elm$json$Json$Decode$field, 'epa', $elm$json$Json$Decode$float)));
     var $author$project$Main$ReadData = F3(
         function(time, pm25, pm10) {
             return {
-                eF: pm10,
-                eG: pm25,
-                cF: time
+                eG: pm10,
+                eH: pm25,
+                aI: time
             };
         });
     var $elm$json$Json$Decode$map3 = _Json_map3;
     var $author$project$Main$readDataDecoder = $elm$json$Json$Decode$list(
         A4(
             $elm$json$Json$Decode$map3,
             $author$project$Main$ReadData,
@@ -6275,15 +6285,15 @@
                 case 1:
                     return $elm$core$Result$Err($elm$http$Http$Timeout);
                 case 2:
                     return $elm$core$Result$Err($elm$http$Http$NetworkError);
                 case 3:
                     var metadata = response.a;
                     return $elm$core$Result$Err(
-                        $elm$http$Http$BadStatus(metadata.gb));
+                        $elm$http$Http$BadStatus(metadata.gc));
                 default:
                     var body = response.b;
                     return A2(
                         $elm$core$Result$mapError,
                         $elm$http$Http$BadBody,
                         toResult(body));
             }
@@ -6307,16 +6317,16 @@
             $: 1,
             a: a
         };
     };
     var $elm$http$Http$State = F2(
         function(reqs, subs) {
             return {
-                eS: reqs,
-                e3: subs
+                eT: reqs,
+                e4: subs
             };
         });
     var $elm$http$Http$init = $elm$core$Task$succeed(
         A2($elm$http$Http$State, $elm$core$Dict$empty, _List_Nil));
     var $elm$http$Http$updateReqs = F3(
         function(router, cmds, reqs) {
             updateReqs: while (true) {
@@ -6350,15 +6360,15 @@
                                 $elm$core$Process$kill(pid));
                         }
                     } else {
                         var req = cmd.a;
                         return A2(
                             $elm$core$Task$andThen,
                             function(pid) {
-                                var _v4 = req.fc;
+                                var _v4 = req.fd;
                                 if (_v4.$ === 1) {
                                     return A3($elm$http$Http$updateReqs, router, otherCmds, reqs);
                                 } else {
                                     var tracker = _v4.a;
                                     return A3(
                                         $elm$http$Http$updateReqs,
                                         router,
@@ -6380,15 +6390,15 @@
         function(router, cmds, subs, state) {
             return A2(
                 $elm$core$Task$andThen,
                 function(reqs) {
                     return $elm$core$Task$succeed(
                         A2($elm$http$Http$State, reqs, subs));
                 },
-                A3($elm$http$Http$updateReqs, router, cmds, state.eS));
+                A3($elm$http$Http$updateReqs, router, cmds, state.eT));
         });
     var $elm$core$List$maybeCons = F3(
         function(f, mx, xs) {
             var _v0 = f(mx);
             if (!_v0.$) {
                 var x = _v0.a;
                 return A2($elm$core$List$cons, x, xs);
@@ -6423,15 +6433,15 @@
                 function(_v1) {
                     return $elm$core$Task$succeed(state);
                 },
                 $elm$core$Task$sequence(
                     A2(
                         $elm$core$List$filterMap,
                         A3($elm$http$Http$maybeSend, router, tracker, progress),
-                        state.e3)));
+                        state.e4)));
         });
     var $elm$http$Http$Cancel = function(a) {
         return {
             $: 0,
             a: a
         };
     };
@@ -6439,22 +6449,22 @@
         function(func, cmd) {
             if (!cmd.$) {
                 var tracker = cmd.a;
                 return $elm$http$Http$Cancel(tracker);
             } else {
                 var r = cmd.a;
                 return $elm$http$Http$Request({
-                    fn: r.fn,
-                    fs: r.fs,
-                    cZ: A2(_Http_mapExpect, func, r.cZ),
-                    d9: r.d9,
-                    fX: r.fX,
-                    gg: r.gg,
-                    fc: r.fc,
-                    dF: r.dF
+                    fo: r.fo,
+                    ft: r.ft,
+                    c$: A2(_Http_mapExpect, func, r.c$),
+                    ea: r.ea,
+                    fY: r.fY,
+                    gh: r.gh,
+                    fd: r.fd,
+                    dH: r.dH
                 });
             }
         });
     var $elm$http$Http$MySub = F2(
         function(a, b) {
             return {
                 $: 0,
@@ -6473,33 +6483,33 @@
         });
     _Platform_effectManagers['Http'] = _Platform_createManager($elm$http$Http$init, $elm$http$Http$onEffects, $elm$http$Http$onSelfMsg, $elm$http$Http$cmdMap, $elm$http$Http$subMap);
     var $elm$http$Http$command = _Platform_leaf('Http');
     var $elm$http$Http$subscription = _Platform_leaf('Http');
     var $elm$http$Http$request = function(r) {
         return $elm$http$Http$command(
             $elm$http$Http$Request({
-                fn: false,
-                fs: r.fs,
-                cZ: r.cZ,
-                d9: r.d9,
-                fX: r.fX,
-                gg: r.gg,
-                fc: r.fc,
-                dF: r.dF
+                fo: false,
+                ft: r.ft,
+                c$: r.c$,
+                ea: r.ea,
+                fY: r.fY,
+                gh: r.gh,
+                fd: r.fd,
+                dH: r.dH
             }));
     };
     var $elm$http$Http$get = function(r) {
         return $elm$http$Http$request({
-            fs: $elm$http$Http$emptyBody,
-            cZ: r.cZ,
-            d9: _List_Nil,
-            fX: 'GET',
-            gg: $elm$core$Maybe$Nothing,
-            fc: $elm$core$Maybe$Nothing,
-            dF: r.dF
+            ft: $elm$http$Http$emptyBody,
+            c$: r.c$,
+            ea: _List_Nil,
+            fY: 'GET',
+            gh: $elm$core$Maybe$Nothing,
+            fd: $elm$core$Maybe$Nothing,
+            dH: r.dH
         });
     };
     var $author$project$Main$getData = function(windowDuration) {
         var stringDuration = function() {
             switch (windowDuration) {
                 case 0:
                     return 'all';
@@ -6508,31 +6518,31 @@
                 case 2:
                     return 'day';
                 default:
                     return 'week';
             }
         }();
         return $elm$http$Http$get({
-            cZ: A2($elm$http$Http$expectJson, $author$project$Main$GotData, $author$project$Main$allDataDecoder),
-            dF: '/api/sensor_data?window=' + stringDuration
+            c$: A2($elm$http$Http$expectJson, $author$project$Main$GotData, $author$project$Main$allDataDecoder),
+            dH: '/api/sensor_data?window=' + stringDuration
         });
     };
     var $author$project$Main$GotLatest = function(a) {
         return {
-            $: 4,
+            $: 5,
             a: a
         };
     };
     var $author$project$Main$LatestData = F4(
         function(pm25, pm10, epa, epaLevel) {
             return {
-                d$: epa,
-                d0: epaLevel,
-                eF: pm10,
-                eG: pm25
+                c_: epa,
+                d1: epaLevel,
+                eG: pm10,
+                eH: pm25
             };
         });
     var $author$project$EpaCommon$Good = 5;
     var $author$project$EpaCommon$Hazardous = 0;
     var $author$project$EpaCommon$Moderate = 4;
     var $author$project$EpaCommon$Unhealthy = 2;
     var $author$project$EpaCommon$UnhealthyForSensitive = 3;
@@ -6579,29 +6589,29 @@
         $elm$json$Json$Decode$maybe(
             A2($elm$json$Json$Decode$field, 'pm10', $elm$json$Json$Decode$float)),
         $elm$json$Json$Decode$maybe(
             A2($elm$json$Json$Decode$field, 'epa', $elm$json$Json$Decode$float)),
         $elm$json$Json$Decode$maybe(
             A2($elm$json$Json$Decode$field, 'level', $author$project$Main$epaLevelDecoder)));
     var $author$project$Main$getLatest = $elm$http$Http$get({
-        cZ: A2($elm$http$Http$expectJson, $author$project$Main$GotLatest, $author$project$Main$latestDataDecoder),
-        dF: '/api/latest_data'
+        c$: A2($elm$http$Http$expectJson, $author$project$Main$GotLatest, $author$project$Main$latestDataDecoder),
+        dH: '/api/latest_data'
     });
     var $author$project$Main$GotStatus = function(a) {
         return {
-            $: 5,
+            $: 6,
             a: a
         };
     };
     var $author$project$Main$DeviceInfoResponse = F3(
         function(readerStatus, readerException, nextSchedule) {
             return {
-                eA: nextSchedule,
-                eO: readerException,
-                eP: readerStatus
+                eB: nextSchedule,
+                eP: readerException,
+                eQ: readerStatus
             };
         });
     var $elm$json$Json$Decode$int = _Json_decodeInt;
     var $author$project$DeviceStatus$Failing = 3;
     var $author$project$DeviceStatus$Reading = 0;
     var $author$project$DeviceStatus$WarmingUp = 1;
     var $author$project$Main$stateDecoder = A2(
@@ -6626,16 +6636,16 @@
         $author$project$Main$DeviceInfoResponse,
         A2($elm$json$Json$Decode$field, 'reader_status', $author$project$Main$stateDecoder),
         $elm$json$Json$Decode$maybe(
             A2($elm$json$Json$Decode$field, 'reader_exception', $elm$json$Json$Decode$string)),
         $elm$json$Json$Decode$maybe(
             A2($elm$json$Json$Decode$field, 'next_schedule', $elm$json$Json$Decode$int)));
     var $author$project$Main$getStatus = $elm$http$Http$get({
-        cZ: A2($elm$http$Http$expectJson, $author$project$Main$GotStatus, $author$project$Main$statusDecoder),
-        dF: '/api/status'
+        c$: A2($elm$http$Http$expectJson, $author$project$Main$GotStatus, $author$project$Main$statusDecoder),
+        dH: '/api/status'
     });
     var $elm$core$Maybe$map = F2(
         function(f, maybe) {
             if (!maybe.$) {
                 var value = maybe.a;
                 return $elm$core$Maybe$Just(
                     f(value));
@@ -6684,39 +6694,39 @@
         function(model, currentTime) {
             var timeToNextRead = A2(
                 $elm$core$Maybe$withDefault,
                 1,
                 A3(
                     $elm$core$Maybe$map2,
                     $author$project$Main$getDuration,
-                    model.Y.eA,
+                    model.Y.eB,
                     $elm$core$Maybe$Just(currentTime)));
             var maxTimeBetweenPolls = 15000;
             var timeSinceLastPoll = A2(
                 $elm$core$Maybe$withDefault,
                 maxTimeBetweenPolls + 1,
                 A3(
                     $elm$core$Maybe$map2,
                     $author$project$Main$getDuration,
-                    model.b_,
+                    model.b0,
                     $elm$core$Maybe$Just(currentTime)));
-            return ((!model.Y.a1) || (model.Y.a1 === 1)) || ((_Utils_cmp(timeSinceLastPoll, maxTimeBetweenPolls) > 0) || (_Utils_cmp(timeToNextRead, -1) > 0));
+            return ((!model.Y.a3) || (model.Y.a3 === 1)) || ((_Utils_cmp(timeSinceLastPoll, maxTimeBetweenPolls) > 0) || (_Utils_cmp(timeToNextRead, -1) > 0));
         });
     var $author$project$Main$update = F2(
         function(msg, model) {
             switch (msg.$) {
-                case 3:
+                case 4:
                     var result = msg.a;
                     if (!result.$) {
                         var data = result.a;
                         return _Utils_Tuple2(
                             _Utils_update(
                                 model, {
-                                    bp: data.d1,
-                                    bq: data.eQ,
+                                    br: data.d2,
+                                    bs: data.eR,
                                     G: {
                                         U: '',
                                         V: '',
                                         W: false
                                     }
                                 }),
                             $elm$core$Platform$Cmd$none);
@@ -6734,18 +6744,26 @@
                             $elm$core$Platform$Cmd$none);
                     }
                 case 0:
                     var newTime = msg.a;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                dU: $elm$core$Maybe$Just(newTime)
+                                dW: $elm$core$Maybe$Just(newTime)
                             }),
                         $author$project$Main$getData(model.ai));
-                case 4:
+                case 3:
+                    var timeZone = msg.a;
+                    return _Utils_Tuple2(
+                        _Utils_update(
+                            model, {
+                                aJ: timeZone
+                            }),
+                        $elm$core$Platform$Cmd$none);
+                case 5:
                     var result = msg.a;
                     if (!result.$) {
                         var data = result.a;
                         return _Utils_Tuple2(
                             _Utils_update(
                                 model, {
                                     G: {
@@ -6770,26 +6788,26 @@
                             $elm$core$Platform$Cmd$none);
                     }
                 case 1:
                     var newTime = msg.a;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                dU: $elm$core$Maybe$Just(newTime)
+                                dW: $elm$core$Maybe$Just(newTime)
                             }),
                         $author$project$Main$getLatest);
-                case 5:
+                case 6:
                     var result = msg.a;
                     if (!result.$) {
                         var data = result.a;
                         var deviceInfo = {
-                            dU: model.dU,
-                            eo: data.eO,
-                            eA: A2($elm$core$Maybe$map, $elm$time$Time$millisToPosix, data.eA),
-                            a1: data.eP
+                            dW: model.dW,
+                            ep: data.eP,
+                            eB: A2($elm$core$Maybe$map, $elm$time$Time$millisToPosix, data.eB),
+                            a3: data.eQ
                         };
                         return _Utils_Tuple2(
                             _Utils_update(
                                 model, {
                                     G: {
                                         U: '',
                                         V: '',
@@ -6812,85 +6830,85 @@
                             $elm$core$Platform$Cmd$none);
                     }
                 case 2:
                     var newTime = msg.a;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                dU: $elm$core$Maybe$Just(newTime),
-                                b_: $elm$core$Maybe$Just(newTime)
+                                dW: $elm$core$Maybe$Just(newTime),
+                                b0: $elm$core$Maybe$Just(newTime)
                             }),
                         $author$project$Main$getStatus);
-                case 6:
+                case 7:
                     var window = msg.a;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
                                 ai: window
                             }),
                         A2($elm$core$Task$perform, $author$project$Main$FetchData, $elm$time$Time$now));
-                case 7:
+                case 8:
                     var hovering = msg.a;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                bW: hovering
+                                bY: hovering
                             }),
                         $elm$core$Platform$Cmd$none);
-                case 8:
+                case 9:
                     var hovering = msg.a;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                bV: hovering
+                                bX: hovering
                             }),
                         $elm$core$Platform$Cmd$none);
-                case 9:
+                case 10:
                     var newTime = msg.a;
                     var readerState = model.Y;
                     var updatedReaderState = _Utils_update(
                         readerState, {
-                            dU: $elm$core$Maybe$Just(newTime)
+                            dW: $elm$core$Maybe$Just(newTime)
                         });
                     var cmd = A2($author$project$Main$shouldFetchStatus, model, newTime) ? A2($elm$core$Task$perform, $author$project$Main$FetchStatus, $elm$time$Time$now) : $elm$core$Platform$Cmd$none;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                dU: $elm$core$Maybe$Just(newTime),
+                                dW: $elm$core$Maybe$Just(newTime),
                                 Y: updatedReaderState
                             }),
                         cmd);
                 default:
                     var newView = msg.a;
                     var newGraph = (newView === 'pm') ? 1 : 0;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                aO: newGraph
+                                aQ: newGraph
                             }),
                         $elm$core$Platform$Cmd$none);
             }
         });
     var $author$project$Main$All = 0;
     var $author$project$Main$ChangeGraphView = function(a) {
         return {
-            $: 10,
+            $: 11,
             a: a
         };
     };
     var $author$project$Main$Day = 2;
     var $author$project$Main$OnEpaHover = function(a) {
         return {
-            $: 8,
+            $: 9,
             a: a
         };
     };
     var $author$project$Main$OnReadHover = function(a) {
         return {
-            $: 7,
+            $: 8,
             a: a
         };
     };
     var $author$project$Main$Week = 3;
     var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$Attrs = function(a) {
         return {
             $: 2,
@@ -6919,16 +6937,16 @@
         return $rundis$elm_bootstrap$Bootstrap$Grid$Internal$RowAttrs(attrs_);
     };
     var $rundis$elm_bootstrap$Bootstrap$General$Internal$Center = 1;
     var $rundis$elm_bootstrap$Bootstrap$General$Internal$MD = 2;
     var $rundis$elm_bootstrap$Bootstrap$General$Internal$HAlign = F2(
         function(screenSize, align) {
             return {
-                dL: align,
-                e_: screenSize
+                dN: align,
+                e$: screenSize
             };
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$RowHAlign = function(a) {
         return {
             $: 1,
             a: a
         };
@@ -6953,16 +6971,16 @@
             $: 0,
             a: a
         };
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$col = F2(
         function(options, children) {
             return $rundis$elm_bootstrap$Bootstrap$Grid$Column({
-                dR: children,
-                dh: options
+                dT: children,
+                dj: options
             });
         });
     var $elm$html$Html$div = _VirtualDom_node('div');
     var $rundis$elm_bootstrap$Bootstrap$Grid$container = F2(
         function(attributes, children) {
             return A2(
                 $elm$html$Html$div,
@@ -6999,213 +7017,213 @@
             'href',
             _VirtualDom_noJavaScriptUri(url));
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$Col = 0;
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$Width = F2(
         function(screenSize, columnCount) {
             return {
-                dT: columnCount,
-                e_: screenSize
+                dV: columnCount,
+                e$: screenSize
             };
         });
     var $rundis$elm_bootstrap$Bootstrap$General$Internal$XS = 0;
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColAlign = F2(
         function(align_, options) {
-            var _v0 = align_.e_;
+            var _v0 = align_.e$;
             switch (_v0) {
                 case 0:
                     return _Utils_update(
                         options, {
-                            bo: $elm$core$Maybe$Just(align_)
+                            bq: $elm$core$Maybe$Just(align_)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            bm: $elm$core$Maybe$Just(align_)
+                            bo: $elm$core$Maybe$Just(align_)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            bl: $elm$core$Maybe$Just(align_)
+                            bn: $elm$core$Maybe$Just(align_)
                         });
                 case 3:
                     return _Utils_update(
                         options, {
-                            bk: $elm$core$Maybe$Just(align_)
+                            bm: $elm$core$Maybe$Just(align_)
                         });
                 default:
                     return _Utils_update(
                         options, {
-                            bn: $elm$core$Maybe$Just(align_)
+                            bp: $elm$core$Maybe$Just(align_)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOffset = F2(
         function(offset_, options) {
-            var _v0 = offset_.e_;
+            var _v0 = offset_.e$;
             switch (_v0) {
                 case 0:
                     return _Utils_update(
                         options, {
-                            b9: $elm$core$Maybe$Just(offset_)
+                            cb: $elm$core$Maybe$Just(offset_)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            b6: $elm$core$Maybe$Just(offset_)
+                            b8: $elm$core$Maybe$Just(offset_)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            b5: $elm$core$Maybe$Just(offset_)
+                            b7: $elm$core$Maybe$Just(offset_)
                         });
                 case 3:
                     return _Utils_update(
                         options, {
-                            b4: $elm$core$Maybe$Just(offset_)
+                            b6: $elm$core$Maybe$Just(offset_)
                         });
                 default:
                     return _Utils_update(
                         options, {
-                            b8: $elm$core$Maybe$Just(offset_)
+                            ca: $elm$core$Maybe$Just(offset_)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOrder = F2(
         function(order_, options) {
-            var _v0 = order_.e_;
+            var _v0 = order_.e$;
             switch (_v0) {
                 case 0:
                     return _Utils_update(
                         options, {
-                            cj: $elm$core$Maybe$Just(order_)
+                            cl: $elm$core$Maybe$Just(order_)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            ch: $elm$core$Maybe$Just(order_)
+                            cj: $elm$core$Maybe$Just(order_)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            cg: $elm$core$Maybe$Just(order_)
+                            ci: $elm$core$Maybe$Just(order_)
                         });
                 case 3:
                     return _Utils_update(
                         options, {
-                            cf: $elm$core$Maybe$Just(order_)
+                            ch: $elm$core$Maybe$Just(order_)
                         });
                 default:
                     return _Utils_update(
                         options, {
-                            ci: $elm$core$Maybe$Just(order_)
+                            ck: $elm$core$Maybe$Just(order_)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColPull = F2(
         function(pull_, options) {
-            var _v0 = pull_.e_;
+            var _v0 = pull_.e$;
             switch (_v0) {
                 case 0:
                     return _Utils_update(
                         options, {
-                            cp: $elm$core$Maybe$Just(pull_)
+                            cr: $elm$core$Maybe$Just(pull_)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            cn: $elm$core$Maybe$Just(pull_)
+                            cp: $elm$core$Maybe$Just(pull_)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            cm: $elm$core$Maybe$Just(pull_)
+                            co: $elm$core$Maybe$Just(pull_)
                         });
                 case 3:
                     return _Utils_update(
                         options, {
-                            cl: $elm$core$Maybe$Just(pull_)
+                            cn: $elm$core$Maybe$Just(pull_)
                         });
                 default:
                     return _Utils_update(
                         options, {
-                            co: $elm$core$Maybe$Just(pull_)
+                            cq: $elm$core$Maybe$Just(pull_)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColPush = F2(
         function(push_, options) {
-            var _v0 = push_.e_;
+            var _v0 = push_.e$;
             switch (_v0) {
                 case 0:
                     return _Utils_update(
                         options, {
-                            cu: $elm$core$Maybe$Just(push_)
+                            cw: $elm$core$Maybe$Just(push_)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            cs: $elm$core$Maybe$Just(push_)
+                            cu: $elm$core$Maybe$Just(push_)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            cr: $elm$core$Maybe$Just(push_)
+                            ct: $elm$core$Maybe$Just(push_)
                         });
                 case 3:
                     return _Utils_update(
                         options, {
-                            cq: $elm$core$Maybe$Just(push_)
+                            cs: $elm$core$Maybe$Just(push_)
                         });
                 default:
                     return _Utils_update(
                         options, {
-                            ct: $elm$core$Maybe$Just(push_)
+                            cv: $elm$core$Maybe$Just(push_)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColWidth = F2(
         function(width_, options) {
-            var _v0 = width_.e_;
+            var _v0 = width_.e$;
             switch (_v0) {
                 case 0:
                     return _Utils_update(
                         options, {
-                            bc: $elm$core$Maybe$Just(width_)
+                            be: $elm$core$Maybe$Just(width_)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            ba: $elm$core$Maybe$Just(width_)
+                            bc: $elm$core$Maybe$Just(width_)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            a9: $elm$core$Maybe$Just(width_)
+                            bb: $elm$core$Maybe$Just(width_)
                         });
                 case 3:
                     return _Utils_update(
                         options, {
-                            a8: $elm$core$Maybe$Just(width_)
+                            ba: $elm$core$Maybe$Just(width_)
                         });
                 default:
                     return _Utils_update(
                         options, {
-                            bb: $elm$core$Maybe$Just(width_)
+                            bd: $elm$core$Maybe$Just(width_)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOption = F2(
         function(modifier, options) {
             switch (modifier.$) {
                 case 6:
                     var attrs = modifier.a;
                     return _Utils_update(
                         options, {
-                            bt: _Utils_ap(options.bt, attrs)
+                            bv: _Utils_ap(options.bv, attrs)
                         });
                 case 0:
                     var width_ = modifier.a;
                     return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColWidth, width_, options);
                 case 1:
                     var offset_ = modifier.a;
                     return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOffset, offset_, options);
@@ -7221,15 +7239,15 @@
                 case 5:
                     var align = modifier.a;
                     return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColAlign, align, options);
                 default:
                     var align = modifier.a;
                     return _Utils_update(
                         options, {
-                            cE: $elm$core$Maybe$Just(align)
+                            cG: $elm$core$Maybe$Just(align)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$columnCountOption = function(size) {
         switch (size) {
             case 0:
                 return $elm$core$Maybe$Nothing;
@@ -7272,16 +7290,16 @@
             case 3:
                 return $elm$core$Maybe$Just('lg');
             default:
                 return $elm$core$Maybe$Just('xl');
         }
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colWidthClass = function(_v0) {
-        var screenSize = _v0.e_;
-        var columnCount = _v0.dT;
+        var screenSize = _v0.e$;
+        var columnCount = _v0.dV;
         return $elm$html$Html$Attributes$class(
             'col' + (A2(
                 $elm$core$Maybe$withDefault,
                 '',
                 A2(
                     $elm$core$Maybe$map,
                     function(v) {
@@ -7303,46 +7321,46 @@
         };
         return A2(
             $elm$core$List$filterMap,
             $elm$core$Basics$identity,
             A2($elm$core$List$map, width_, widths));
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$defaultColOptions = {
-        bk: $elm$core$Maybe$Nothing,
-        bl: $elm$core$Maybe$Nothing,
         bm: $elm$core$Maybe$Nothing,
         bn: $elm$core$Maybe$Nothing,
         bo: $elm$core$Maybe$Nothing,
-        bt: _List_Nil,
-        b4: $elm$core$Maybe$Nothing,
-        b5: $elm$core$Maybe$Nothing,
+        bp: $elm$core$Maybe$Nothing,
+        bq: $elm$core$Maybe$Nothing,
+        bv: _List_Nil,
         b6: $elm$core$Maybe$Nothing,
+        b7: $elm$core$Maybe$Nothing,
         b8: $elm$core$Maybe$Nothing,
-        b9: $elm$core$Maybe$Nothing,
-        cf: $elm$core$Maybe$Nothing,
-        cg: $elm$core$Maybe$Nothing,
+        ca: $elm$core$Maybe$Nothing,
+        cb: $elm$core$Maybe$Nothing,
         ch: $elm$core$Maybe$Nothing,
         ci: $elm$core$Maybe$Nothing,
         cj: $elm$core$Maybe$Nothing,
+        ck: $elm$core$Maybe$Nothing,
         cl: $elm$core$Maybe$Nothing,
-        cm: $elm$core$Maybe$Nothing,
         cn: $elm$core$Maybe$Nothing,
         co: $elm$core$Maybe$Nothing,
         cp: $elm$core$Maybe$Nothing,
         cq: $elm$core$Maybe$Nothing,
         cr: $elm$core$Maybe$Nothing,
         cs: $elm$core$Maybe$Nothing,
         ct: $elm$core$Maybe$Nothing,
         cu: $elm$core$Maybe$Nothing,
-        cE: $elm$core$Maybe$Nothing,
-        a8: $elm$core$Maybe$Nothing,
-        a9: $elm$core$Maybe$Nothing,
+        cv: $elm$core$Maybe$Nothing,
+        cw: $elm$core$Maybe$Nothing,
+        cG: $elm$core$Maybe$Nothing,
         ba: $elm$core$Maybe$Nothing,
         bb: $elm$core$Maybe$Nothing,
-        bc: $elm$core$Maybe$Nothing
+        bc: $elm$core$Maybe$Nothing,
+        bd: $elm$core$Maybe$Nothing,
+        be: $elm$core$Maybe$Nothing
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetCountOption = function(size) {
         switch (size) {
             case 0:
                 return '0';
             case 1:
                 return '1';
@@ -7374,16 +7392,16 @@
             var s = _v0.a;
             return '-' + (s + '-');
         } else {
             return '-';
         }
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetClass = function(_v0) {
-        var screenSize = _v0.e_;
-        var offsetCount = _v0.eC;
+        var screenSize = _v0.e$;
+        var offsetCount = _v0.eD;
         return $elm$html$Html$Attributes$class(
             'offset' + ($rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString(screenSize) + $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetCountOption(offsetCount)));
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetsToAttributes = function(offsets) {
         var offset_ = function(m) {
             return A2($elm$core$Maybe$map, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetClass, m);
         };
@@ -7423,15 +7441,15 @@
             default:
                 return 'last';
         }
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$orderToAttributes = function(orders) {
         var order_ = function(m) {
             if (!m.$) {
-                var screenSize = m.a.e_;
+                var screenSize = m.a.e$;
                 var moveCount = m.a.aF;
                 return $elm$core$Maybe$Just(
                     $elm$html$Html$Attributes$class(
                         'order' + ($rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString(screenSize) + $rundis$elm_bootstrap$Bootstrap$Grid$Internal$orderColOption(moveCount))));
             } else {
                 return $elm$core$Maybe$Nothing;
             }
@@ -7470,15 +7488,15 @@
             default:
                 return '12';
         }
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$pullsToAttributes = function(pulls) {
         var pull_ = function(m) {
             if (!m.$) {
-                var screenSize = m.a.e_;
+                var screenSize = m.a.e$;
                 var moveCount = m.a.aF;
                 return $elm$core$Maybe$Just(
                     $elm$html$Html$Attributes$class(
                         'pull' + ($rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString(screenSize) + $rundis$elm_bootstrap$Bootstrap$Grid$Internal$moveCountOption(moveCount))));
             } else {
                 return $elm$core$Maybe$Nothing;
             }
@@ -7487,15 +7505,15 @@
             $elm$core$List$filterMap,
             $elm$core$Basics$identity,
             A2($elm$core$List$map, pull_, pulls));
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$pushesToAttributes = function(pushes) {
         var push_ = function(m) {
             if (!m.$) {
-                var screenSize = m.a.e_;
+                var screenSize = m.a.e$;
                 var moveCount = m.a.aF;
                 return $elm$core$Maybe$Just(
                     $elm$html$Html$Attributes$class(
                         'push' + ($rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString(screenSize) + $rundis$elm_bootstrap$Bootstrap$Grid$Internal$moveCountOption(moveCount))));
             } else {
                 return $elm$core$Maybe$Nothing;
             }
@@ -7512,16 +7530,16 @@
             case 0:
                 return 'left';
             default:
                 return 'right';
         }
     };
     var $rundis$elm_bootstrap$Bootstrap$Internal$Text$textAlignClass = function(_v0) {
-        var dir = _v0.dY;
-        var size = _v0.e1;
+        var dir = _v0.d_;
+        var size = _v0.e2;
         return $elm$html$Html$Attributes$class(
             'text' + (A2(
                 $elm$core$Maybe$withDefault,
                 '-',
                 A2(
                     $elm$core$Maybe$map,
                     function(s) {
@@ -7537,16 +7555,16 @@
                 return 'center';
             default:
                 return 'end';
         }
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$vAlignClass = F2(
         function(prefix, _v0) {
-            var align = _v0.dL;
-            var screenSize = _v0.e_;
+            var align = _v0.dN;
+            var screenSize = _v0.e$;
             return $elm$html$Html$Attributes$class(
                 _Utils_ap(
                     prefix,
                     _Utils_ap(
                         A2(
                             $elm$core$Maybe$withDefault,
                             '',
@@ -7574,181 +7592,181 @@
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colAttributes = function(modifiers) {
         var options = A3($elm$core$List$foldl, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOption, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$defaultColOptions, modifiers);
         var shouldAddDefaultXs = !$elm$core$List$length(
             A2(
                 $elm$core$List$filterMap,
                 $elm$core$Basics$identity,
                 _List_fromArray(
-                    [options.bc, options.ba, options.a9, options.a8, options.bb])));
+                    [options.be, options.bc, options.bb, options.ba, options.bd])));
         return _Utils_ap(
             $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colWidthsToAttributes(
                 _List_fromArray(
                     [
                         shouldAddDefaultXs ? $elm$core$Maybe$Just(
-                            A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$Width, 0, 0)) : options.bc,
+                            A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$Width, 0, 0)) : options.be,
+                        options.bc,
+                        options.bb,
                         options.ba,
-                        options.a9,
-                        options.a8,
-                        options.bb
+                        options.bd
                     ])),
             _Utils_ap(
                 $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetsToAttributes(
                     _List_fromArray(
-                        [options.b9, options.b6, options.b5, options.b4, options.b8])),
+                        [options.cb, options.b8, options.b7, options.b6, options.ca])),
                 _Utils_ap(
                     $rundis$elm_bootstrap$Bootstrap$Grid$Internal$pullsToAttributes(
                         _List_fromArray(
-                            [options.cp, options.cn, options.cm, options.cl, options.co])),
+                            [options.cr, options.cp, options.co, options.cn, options.cq])),
                     _Utils_ap(
                         $rundis$elm_bootstrap$Bootstrap$Grid$Internal$pushesToAttributes(
                             _List_fromArray(
-                                [options.cu, options.cs, options.cr, options.cq, options.ct])),
+                                [options.cw, options.cu, options.ct, options.cs, options.cv])),
                         _Utils_ap(
                             $rundis$elm_bootstrap$Bootstrap$Grid$Internal$orderToAttributes(
                                 _List_fromArray(
-                                    [options.cj, options.ch, options.cg, options.cf, options.ci])),
+                                    [options.cl, options.cj, options.ci, options.ch, options.ck])),
                             _Utils_ap(
                                 A2(
                                     $rundis$elm_bootstrap$Bootstrap$Grid$Internal$vAlignsToAttributes,
                                     'align-self-',
                                     _List_fromArray(
-                                        [options.bo, options.bm, options.bl, options.bk, options.bn])),
+                                        [options.bq, options.bo, options.bn, options.bm, options.bp])),
                                 _Utils_ap(
                                     function() {
-                                        var _v0 = options.cE;
+                                        var _v0 = options.cG;
                                         if (!_v0.$) {
                                             var a = _v0.a;
                                             return _List_fromArray(
                                                 [
                                                     $rundis$elm_bootstrap$Bootstrap$Internal$Text$textAlignClass(a)
                                                 ]);
                                         } else {
                                             return _List_Nil;
                                         }
                                     }(),
-                                    options.bt)))))));
+                                    options.bv)))))));
     };
     var $elm$virtual_dom$VirtualDom$keyedNode = function(tag) {
         return _VirtualDom_keyedNode(
             _VirtualDom_noScript(tag));
     };
     var $elm$html$Html$Keyed$node = $elm$virtual_dom$VirtualDom$keyedNode;
     var $rundis$elm_bootstrap$Bootstrap$Grid$renderCol = function(column) {
         switch (column.$) {
             case 0:
-                var options = column.a.dh;
-                var children = column.a.dR;
+                var options = column.a.dj;
+                var children = column.a.dT;
                 return A2(
                     $elm$html$Html$div,
                     $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colAttributes(options),
                     children);
             case 1:
                 var e = column.a;
                 return e;
             default:
-                var options = column.a.dh;
-                var children = column.a.dR;
+                var options = column.a.dj;
+                var children = column.a.dT;
                 return A3(
                     $elm$html$Html$Keyed$node,
                     'div',
                     $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colAttributes(options),
                     children);
         }
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowHAlign = F2(
         function(align, options) {
-            var _v0 = align.e_;
+            var _v0 = align.e$;
             switch (_v0) {
                 case 0:
                     return _Utils_update(
                         options, {
-                            bS: $elm$core$Maybe$Just(align)
+                            bU: $elm$core$Maybe$Just(align)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            bQ: $elm$core$Maybe$Just(align)
+                            bS: $elm$core$Maybe$Just(align)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            bP: $elm$core$Maybe$Just(align)
+                            bR: $elm$core$Maybe$Just(align)
                         });
                 case 3:
                     return _Utils_update(
                         options, {
-                            bO: $elm$core$Maybe$Just(align)
+                            bQ: $elm$core$Maybe$Just(align)
                         });
                 default:
                     return _Utils_update(
                         options, {
-                            bR: $elm$core$Maybe$Just(align)
+                            bT: $elm$core$Maybe$Just(align)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowVAlign = F2(
         function(align_, options) {
-            var _v0 = align_.e_;
+            var _v0 = align_.e$;
             switch (_v0) {
                 case 0:
                     return _Utils_update(
                         options, {
-                            cO: $elm$core$Maybe$Just(align_)
+                            cP: $elm$core$Maybe$Just(align_)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            cM: $elm$core$Maybe$Just(align_)
+                            cN: $elm$core$Maybe$Just(align_)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            cL: $elm$core$Maybe$Just(align_)
+                            cM: $elm$core$Maybe$Just(align_)
                         });
                 case 3:
                     return _Utils_update(
                         options, {
-                            cK: $elm$core$Maybe$Just(align_)
+                            cL: $elm$core$Maybe$Just(align_)
                         });
                 default:
                     return _Utils_update(
                         options, {
-                            cN: $elm$core$Maybe$Just(align_)
+                            cO: $elm$core$Maybe$Just(align_)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowOption = F2(
         function(modifier, options) {
             switch (modifier.$) {
                 case 2:
                     var attrs = modifier.a;
                     return _Utils_update(
                         options, {
-                            bt: _Utils_ap(options.bt, attrs)
+                            bv: _Utils_ap(options.bv, attrs)
                         });
                 case 0:
                     var align = modifier.a;
                     return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowVAlign, align, options);
                 default:
                     var align = modifier.a;
                     return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowHAlign, align, options);
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$defaultRowOptions = {
-        bt: _List_Nil,
-        bO: $elm$core$Maybe$Nothing,
-        bP: $elm$core$Maybe$Nothing,
+        bv: _List_Nil,
         bQ: $elm$core$Maybe$Nothing,
         bR: $elm$core$Maybe$Nothing,
         bS: $elm$core$Maybe$Nothing,
-        cK: $elm$core$Maybe$Nothing,
+        bT: $elm$core$Maybe$Nothing,
+        bU: $elm$core$Maybe$Nothing,
         cL: $elm$core$Maybe$Nothing,
         cM: $elm$core$Maybe$Nothing,
         cN: $elm$core$Maybe$Nothing,
-        cO: $elm$core$Maybe$Nothing
+        cO: $elm$core$Maybe$Nothing,
+        cP: $elm$core$Maybe$Nothing
     };
     var $rundis$elm_bootstrap$Bootstrap$General$Internal$horizontalAlignOption = function(align) {
         switch (align) {
             case 0:
                 return 'start';
             case 1:
                 return 'center';
@@ -7757,16 +7775,16 @@
             case 3:
                 return 'around';
             default:
                 return 'between';
         }
     };
     var $rundis$elm_bootstrap$Bootstrap$General$Internal$hAlignClass = function(_v0) {
-        var align = _v0.dL;
-        var screenSize = _v0.e_;
+        var align = _v0.dN;
+        var screenSize = _v0.e$;
         return $elm$html$Html$Attributes$class(
             'justify-content-' + (A2(
                 $elm$core$Maybe$withDefault,
                 '',
                 A2(
                     $elm$core$Maybe$map,
                     function(v) {
@@ -7791,20 +7809,20 @@
                     $elm$html$Html$Attributes$class('row')
                 ]),
             _Utils_ap(
                 A2(
                     $rundis$elm_bootstrap$Bootstrap$Grid$Internal$vAlignsToAttributes,
                     'align-items-',
                     _List_fromArray(
-                        [options.cO, options.cM, options.cL, options.cK, options.cN])),
+                        [options.cP, options.cN, options.cM, options.cL, options.cO])),
                 _Utils_ap(
                     $rundis$elm_bootstrap$Bootstrap$Grid$Internal$hAlignsToAttributes(
                         _List_fromArray(
-                            [options.bS, options.bQ, options.bP, options.bO, options.bR])),
-                    options.bt)));
+                            [options.bU, options.bS, options.bR, options.bQ, options.bT])),
+                    options.bv)));
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$row = F2(
         function(options, cols) {
             return A2(
                 $elm$html$Html$div,
                 $rundis$elm_bootstrap$Bootstrap$Grid$Internal$rowAttributes(options),
                 A2($elm$core$List$map, $rundis$elm_bootstrap$Bootstrap$Grid$renderCol, cols));
@@ -7853,23 +7871,23 @@
                                                     [
                                                         A2(
                                                             $elm$html$Html$Attributes$style,
                                                             'color',
                                                             A2(
                                                                 $elm$core$Maybe$withDefault,
                                                                 'black',
-                                                                A2($elm$core$Maybe$map, $author$project$EpaCommon$getColorForLevel, currentReads.d0)))
+                                                                A2($elm$core$Maybe$map, $author$project$EpaCommon$getColorForLevel, currentReads.d1)))
                                                     ]),
                                                 _List_fromArray(
                                                     [
                                                         $elm$html$Html$text(
                                                             A2(
                                                                 $elm$core$Maybe$withDefault,
                                                                 'NA',
-                                                                A2($elm$core$Maybe$map, $elm$core$String$fromFloat, currentReads.en)))
+                                                                A2($elm$core$Maybe$map, $elm$core$String$fromFloat, currentReads.eo)))
                                                     ]))
                                         ]))
                             ])),
                     A2(
                         $rundis$elm_bootstrap$Bootstrap$Grid$row,
                         _List_fromArray(
                             [
@@ -7945,15 +7963,15 @@
                                         ]),
                                     _List_fromArray(
                                         [
                                             $elm$html$Html$text(
                                                 A2(
                                                     $elm$core$Maybe$withDefault,
                                                     'NA',
-                                                    A2($elm$core$Maybe$map, $elm$core$String$fromFloat, currentReads.ep)))
+                                                    A2($elm$core$Maybe$map, $elm$core$String$fromFloat, currentReads.eq)))
                                         ]))
                             ])),
                     A2(
                         $rundis$elm_bootstrap$Bootstrap$Grid$row,
                         _List_fromArray(
                             [
                                 $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
@@ -7991,15 +8009,15 @@
                                         ]),
                                     _List_fromArray(
                                         [
                                             $elm$html$Html$text(
                                                 A2(
                                                     $elm$core$Maybe$withDefault,
                                                     'NA',
-                                                    A2($elm$core$Maybe$map, $elm$core$String$fromFloat, currentReads.eq)))
+                                                    A2($elm$core$Maybe$map, $elm$core$String$fromFloat, currentReads.er)))
                                         ]))
                             ]))
                 ]));
     };
     var $author$project$DeviceStatus$deviceStatusColor = function(deviceStatus) {
         switch (deviceStatus) {
             case 0:
@@ -8127,15 +8145,15 @@
                                     _List_fromArray(
                                         [
                                             A2(
                                                 $elm$html$Html$img,
                                                 _List_fromArray(
                                                     [
                                                         $elm$html$Html$Attributes$src(
-                                                            $author$project$DeviceStatus$deviceStatusImage(deviceInfo.a1))
+                                                            $author$project$DeviceStatus$deviceStatusImage(deviceInfo.a3))
                                                     ]),
                                                 _List_Nil)
                                         ]))
                             ])),
                     A2(
                         $rundis$elm_bootstrap$Bootstrap$Grid$row,
                         _List_Nil,
@@ -8156,20 +8174,20 @@
                                             A2(
                                                 $elm$html$Html$h5,
                                                 _List_fromArray(
                                                     [
                                                         A2(
                                                             $elm$html$Html$Attributes$style,
                                                             'color',
-                                                            $author$project$DeviceStatus$deviceStatusColor(deviceInfo.a1))
+                                                            $author$project$DeviceStatus$deviceStatusColor(deviceInfo.a3))
                                                     ]),
                                                 _List_fromArray(
                                                     [
                                                         $elm$html$Html$text(
-                                                            $author$project$DeviceStatus$deviceStatusToString(deviceInfo.a1))
+                                                            $author$project$DeviceStatus$deviceStatusToString(deviceInfo.a3))
                                                     ]))
                                         ]))
                             ])),
                     A2(
                         $rundis$elm_bootstrap$Bootstrap$Grid$row,
                         _List_Nil,
                         _List_fromArray(
@@ -8183,15 +8201,15 @@
                                                     [
                                                         A2($elm$html$Html$Attributes$style, 'text-align', 'center')
                                                     ]))
                                         ]),
                                     _List_fromArray(
                                         [
                                             $elm$html$Html$text(
-                                                A2($elm$core$Maybe$withDefault, '', deviceInfo.eo))
+                                                A2($elm$core$Maybe$withDefault, '', deviceInfo.ep))
                                         ]))
                             ])),
                     A2(
                         $author$project$DeviceStatus$htmlIf,
                         A2(
                             $rundis$elm_bootstrap$Bootstrap$Grid$row,
                             _List_Nil,
@@ -8209,32 +8227,32 @@
                                             ]),
                                         _List_fromArray(
                                             [
                                                 $elm$html$Html$text(
                                                     'Next read in: ' + A2(
                                                         $elm$core$Maybe$withDefault,
                                                         '',
-                                                        A3($elm$core$Maybe$map2, $author$project$DeviceStatus$formatDuration, deviceInfo.dU, deviceInfo.eA)))
+                                                        A3($elm$core$Maybe$map2, $author$project$DeviceStatus$formatDuration, deviceInfo.dW, deviceInfo.eB)))
                                             ]))
                                 ])),
-                        $author$project$DeviceStatus$shouldShowTimer(deviceInfo.a1))
+                        $author$project$DeviceStatus$shouldShowTimer(deviceInfo.a3))
                 ]));
     };
     var $terezka$elm_charts$Internal$Svg$Start = 1;
     var $terezka$elm_charts$Chart$Attributes$alignLeft = function(config) {
         return _Utils_update(
             config, {
                 i: $elm$core$Maybe$Just(1)
             });
     };
     var $terezka$elm_charts$Chart$Attributes$background = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    fq: v
+                    fr: v
                 });
         });
     var $terezka$elm_charts$Internal$Helpers$blue = '#12A5ED';
     var $terezka$elm_charts$Chart$Attributes$blue = $terezka$elm_charts$Internal$Helpers$blue;
     var $terezka$elm_charts$Chart$Attributes$border = F2(
         function(v, config) {
             return _Utils_update(
@@ -8248,16 +8266,16 @@
                 config, {
                     x: v
                 });
         });
     var $terezka$elm_charts$Internal$Svg$Event = F2(
         function(name, handler) {
             return {
-                d8: handler,
-                fZ: name
+                d9: handler,
+                f_: name
             };
         });
     var $elm$core$List$any = F2(
         function(isOkay, list) {
             any: while (true) {
                 if (!list.b) {
                     return false;
@@ -8331,18 +8349,18 @@
     var $debois$elm_dom$DOM$boundingClientRect = A4(
         $elm$json$Json$Decode$map3,
         F3(
             function(_v0, width, height) {
                 var x = _v0.a;
                 var y = _v0.b;
                 return {
-                    ea: height,
-                    er: x,
-                    fb: y,
-                    fi: width
+                    eb: height,
+                    es: x,
+                    fc: y,
+                    fj: width
                 };
             }),
         A2($debois$elm_dom$DOM$position, 0, 0),
         $debois$elm_dom$DOM$offsetWidth,
         $debois$elm_dom$DOM$offsetHeight);
     var $elm$json$Json$Decode$lazy = function(thunk) {
         return A2(
@@ -8367,80 +8385,80 @@
                 ]));
     }
     var $terezka$elm_charts$Internal$Svg$decodePosition = $terezka$elm_charts$Internal$Svg$cyclic$decodePosition();
     $terezka$elm_charts$Internal$Svg$cyclic$decodePosition = function() {
         return $terezka$elm_charts$Internal$Svg$decodePosition;
     };
     var $terezka$elm_charts$Internal$Coordinates$innerLength = function(axis) {
-        return A2($elm$core$Basics$max, 1, (axis.O - axis.fW) - axis.fV);
+        return A2($elm$core$Basics$max, 1, (axis.O - axis.fX) - axis.fW);
     };
     var $terezka$elm_charts$Internal$Coordinates$innerWidth = function(plane) {
-        return $terezka$elm_charts$Internal$Coordinates$innerLength(plane.fj);
+        return $terezka$elm_charts$Internal$Coordinates$innerLength(plane.fk);
     };
     var $terezka$elm_charts$Internal$Coordinates$range = function(axis) {
-        var diff = axis.et - axis.ev;
+        var diff = axis.eu - axis.ew;
         return (diff > 0) ? diff : 1;
     };
     var $terezka$elm_charts$Internal$Coordinates$scaleCartesianX = F2(
         function(plane, value) {
-            return (value * $terezka$elm_charts$Internal$Coordinates$range(plane.fj)) / $terezka$elm_charts$Internal$Coordinates$innerWidth(plane);
+            return (value * $terezka$elm_charts$Internal$Coordinates$range(plane.fk)) / $terezka$elm_charts$Internal$Coordinates$innerWidth(plane);
         });
     var $terezka$elm_charts$Internal$Coordinates$toCartesianX = F2(
         function(plane, value) {
-            return A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, value - plane.fj.fW) + plane.fj.ev;
+            return A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, value - plane.fk.fX) + plane.fk.ew;
         });
     var $terezka$elm_charts$Internal$Coordinates$innerHeight = function(plane) {
-        return $terezka$elm_charts$Internal$Coordinates$innerLength(plane.fk);
+        return $terezka$elm_charts$Internal$Coordinates$innerLength(plane.fl);
     };
     var $terezka$elm_charts$Internal$Coordinates$scaleCartesianY = F2(
         function(plane, value) {
-            return (value * $terezka$elm_charts$Internal$Coordinates$range(plane.fk)) / $terezka$elm_charts$Internal$Coordinates$innerHeight(plane);
+            return (value * $terezka$elm_charts$Internal$Coordinates$range(plane.fl)) / $terezka$elm_charts$Internal$Coordinates$innerHeight(plane);
         });
     var $terezka$elm_charts$Internal$Coordinates$toCartesianY = F2(
         function(plane, value) {
-            return ($terezka$elm_charts$Internal$Coordinates$range(plane.fk) - A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, value - plane.fk.fW)) + plane.fk.ev;
+            return ($terezka$elm_charts$Internal$Coordinates$range(plane.fl) - A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, value - plane.fl.fX)) + plane.fl.ew;
         });
     var $terezka$elm_charts$Internal$Svg$fromSvg = F2(
         function(plane, point) {
             return {
-                fj: A2($terezka$elm_charts$Internal$Coordinates$toCartesianX, plane, point.fj),
-                fk: A2($terezka$elm_charts$Internal$Coordinates$toCartesianY, plane, point.fk)
+                fk: A2($terezka$elm_charts$Internal$Coordinates$toCartesianX, plane, point.fk),
+                fl: A2($terezka$elm_charts$Internal$Coordinates$toCartesianY, plane, point.fl)
             };
         });
     var $debois$elm_dom$DOM$target = function(decoder) {
         return A2($elm$json$Json$Decode$field, 'target', decoder);
     };
     var $terezka$elm_charts$Internal$Svg$decoder = F2(
         function(plane, toMsg) {
             var handle = F3(
                 function(mouseX, mouseY, box) {
-                    var yPrev = plane.fk;
-                    var xPrev = plane.fj;
-                    var widthPercent = box.fi / plane.fj.O;
-                    var heightPercent = box.ea / plane.fk.O;
+                    var yPrev = plane.fl;
+                    var xPrev = plane.fk;
+                    var widthPercent = box.fj / plane.fk.O;
+                    var heightPercent = box.eb / plane.fl.O;
                     var newPlane = _Utils_update(
                         plane, {
-                            fj: _Utils_update(
+                            fk: _Utils_update(
                                 xPrev, {
-                                    O: box.fi,
-                                    fV: plane.fj.fV * widthPercent,
-                                    fW: plane.fj.fW * widthPercent
+                                    O: box.fj,
+                                    fW: plane.fk.fW * widthPercent,
+                                    fX: plane.fk.fX * widthPercent
                                 }),
-                            fk: _Utils_update(
+                            fl: _Utils_update(
                                 yPrev, {
-                                    O: box.ea,
-                                    fV: plane.fk.fV * heightPercent,
-                                    fW: plane.fk.fW * heightPercent
+                                    O: box.eb,
+                                    fW: plane.fl.fW * heightPercent,
+                                    fX: plane.fl.fX * heightPercent
                                 })
                         });
                     var searched = A2(
                         $terezka$elm_charts$Internal$Svg$fromSvg,
                         newPlane, {
-                            fj: mouseX - box.er,
-                            fk: mouseY - box.fb
+                            fk: mouseX - box.es,
+                            fl: mouseY - box.fc
                         });
                     return A2(toMsg, newPlane, searched);
                 });
             return A4(
                 $elm$json$Json$Decode$map3,
                 handle,
                 A2($elm$json$Json$Decode$field, 'pageX', $elm$json$Json$Decode$float),
@@ -8482,79 +8500,79 @@
             A2($elm$core$String$replace, '.', '-'));
         return A2(
             $elm$core$String$join,
             '_',
             _List_fromArray(
                 [
                     'elm-charts__id',
-                    numToStr(plane.fj.O),
-                    numToStr(plane.fj.ev),
-                    numToStr(plane.fj.et),
-                    numToStr(plane.fj.fW),
-                    numToStr(plane.fj.fV),
                     numToStr(plane.fk.O),
-                    numToStr(plane.fk.ev),
-                    numToStr(plane.fk.et),
+                    numToStr(plane.fk.ew),
+                    numToStr(plane.fk.eu),
+                    numToStr(plane.fk.fX),
                     numToStr(plane.fk.fW),
-                    numToStr(plane.fk.fV)
+                    numToStr(plane.fl.O),
+                    numToStr(plane.fl.ew),
+                    numToStr(plane.fl.eu),
+                    numToStr(plane.fl.fX),
+                    numToStr(plane.fl.fW)
                 ]));
     };
     var $elm$svg$Svg$Attributes$viewBox = _VirtualDom_attribute('viewBox');
     var $elm$svg$Svg$Attributes$width = _VirtualDom_attribute('width');
     var $elm$svg$Svg$Attributes$x = _VirtualDom_attribute('x');
     var $elm$svg$Svg$Attributes$y = _VirtualDom_attribute('y');
     var $terezka$elm_charts$Internal$Svg$container = F5(
         function(plane, config, below, chartEls, above) {
             var toEvent = function(event) {
                 return A2(
                     $elm$svg$Svg$Events$on,
-                    event.fZ,
-                    A2($terezka$elm_charts$Internal$Svg$decoder, plane, event.d8));
+                    event.f_,
+                    A2($terezka$elm_charts$Internal$Svg$decoder, plane, event.d9));
             };
-            var svgAttrsSize = config.cw ? _List_fromArray(
+            var svgAttrsSize = config.cy ? _List_fromArray(
                 [
                     $elm$svg$Svg$Attributes$viewBox(
-                        '0 0 ' + ($elm$core$String$fromFloat(plane.fj.O) + (' ' + $elm$core$String$fromFloat(plane.fk.O)))),
+                        '0 0 ' + ($elm$core$String$fromFloat(plane.fk.O) + (' ' + $elm$core$String$fromFloat(plane.fl.O)))),
                     A2($elm$html$Html$Attributes$style, 'display', 'block')
                 ]) : _List_fromArray(
                 [
                     $elm$svg$Svg$Attributes$width(
-                        $elm$core$String$fromFloat(plane.fj.O)),
-                    $elm$svg$Svg$Attributes$height(
                         $elm$core$String$fromFloat(plane.fk.O)),
+                    $elm$svg$Svg$Attributes$height(
+                        $elm$core$String$fromFloat(plane.fl.O)),
                     A2($elm$html$Html$Attributes$style, 'display', 'block')
                 ]);
-            var htmlAttrsSize = config.cw ? _List_fromArray(
+            var htmlAttrsSize = config.cy ? _List_fromArray(
                 [
                     A2($elm$html$Html$Attributes$style, 'width', '100%'),
                     A2($elm$html$Html$Attributes$style, 'height', '100%')
                 ]) : _List_fromArray(
                 [
                     A2(
                         $elm$html$Html$Attributes$style,
                         'width',
-                        $elm$core$String$fromFloat(plane.fj.O) + 'px'),
+                        $elm$core$String$fromFloat(plane.fk.O) + 'px'),
                     A2(
                         $elm$html$Html$Attributes$style,
                         'height',
-                        $elm$core$String$fromFloat(plane.fk.O) + 'px')
+                        $elm$core$String$fromFloat(plane.fl.O) + 'px')
                 ]);
             var htmlAttrsDef = _List_fromArray(
                 [
                     $elm$html$Html$Attributes$class('elm-charts__container-inner')
                 ]);
             var htmlAttrs = _Utils_ap(
-                config.bX,
+                config.bZ,
                 _Utils_ap(htmlAttrsDef, htmlAttrsSize));
             var chartPosition = _List_fromArray(
                 [
                     $elm$svg$Svg$Attributes$x(
-                        $elm$core$String$fromFloat(plane.fj.fW)),
+                        $elm$core$String$fromFloat(plane.fk.fX)),
                     $elm$svg$Svg$Attributes$y(
-                        $elm$core$String$fromFloat(plane.fk.fW)),
+                        $elm$core$String$fromFloat(plane.fl.fX)),
                     $elm$svg$Svg$Attributes$width(
                         $elm$core$String$fromFloat(
                             $terezka$elm_charts$Internal$Coordinates$innerWidth(plane))),
                     $elm$svg$Svg$Attributes$height(
                         $elm$core$String$fromFloat(
                             $terezka$elm_charts$Internal$Coordinates$innerHeight(plane))),
                     $elm$svg$Svg$Attributes$fill('transparent')
@@ -8576,19 +8594,19 @@
                                     A2($elm$svg$Svg$rect, chartPosition, _List_Nil)
                                 ]))
                     ]));
             var catcher = A2(
                 $elm$svg$Svg$rect,
                 _Utils_ap(
                     chartPosition,
-                    A2($elm$core$List$map, toEvent, config.bL)),
+                    A2($elm$core$List$map, toEvent, config.bN)),
                 _List_Nil);
             var chart = A2(
                 $elm$svg$Svg$svg,
-                _Utils_ap(svgAttrsSize, config.bu),
+                _Utils_ap(svgAttrsSize, config.bw),
                 _Utils_ap(
                     _List_fromArray(
                         [clipPathDefs]),
                     _Utils_ap(
                         chartEls,
                         _List_fromArray(
                             [catcher]))));
@@ -8611,47 +8629,47 @@
                                         [chart]),
                                     above)))
                     ]));
         });
     var $terezka$elm_charts$Internal$Coordinates$Position = F4(
         function(x1, x2, y1, y2) {
             return {
-                aK: x1,
-                be: x2,
-                gA: y1,
-                dI: y2
+                aM: x1,
+                bg: x2,
+                gB: y1,
+                dK: y2
             };
         });
     var $elm$core$Basics$min = F2(
         function(x, y) {
             return (_Utils_cmp(x, y) < 0) ? x : y;
         });
     var $terezka$elm_charts$Internal$Coordinates$foldPosition = F2(
         function(func, data) {
             var fold = F2(
                 function(datum, posM) {
                     if (!posM.$) {
                         var pos = posM.a;
                         return $elm$core$Maybe$Just({
-                            aK: A2(
+                            aM: A2(
                                 $elm$core$Basics$min,
-                                func(datum).aK,
-                                pos.aK),
-                            be: A2(
+                                func(datum).aM,
+                                pos.aM),
+                            bg: A2(
                                 $elm$core$Basics$max,
-                                func(datum).be,
-                                pos.be),
-                            gA: A2(
+                                func(datum).bg,
+                                pos.bg),
+                            gB: A2(
                                 $elm$core$Basics$min,
-                                func(datum).gA,
-                                pos.gA),
-                            dI: A2(
+                                func(datum).gB,
+                                pos.gB),
+                            dK: A2(
                                 $elm$core$Basics$max,
-                                func(datum).dI,
-                                pos.dI)
+                                func(datum).dK,
+                                pos.dK)
                         });
                     } else {
                         return $elm$core$Maybe$Just(
                             func(datum));
                     }
                 });
             return A2(
@@ -8659,41 +8677,41 @@
                 A4($terezka$elm_charts$Internal$Coordinates$Position, 0, 0, 0, 0),
                 A3($elm$core$List$foldl, fold, $elm$core$Maybe$Nothing, data));
         });
     var $terezka$elm_charts$Chart$Attributes$lowest = F3(
         function(v, edit, b) {
             return _Utils_update(
                 b, {
-                    ev: A3(edit, v, b.ev, b.fz)
+                    ew: A3(edit, v, b.ew, b.fA)
                 });
         });
     var $terezka$elm_charts$Chart$Attributes$orLower = F3(
         function(least, real, _v0) {
             return (_Utils_cmp(real, least) > 0) ? least : real;
         });
     var $terezka$elm_charts$Chart$definePlane = F2(
         function(config, elements) {
-            var width = A2($elm$core$Basics$max, 1, (config.fi - config.S.er) - config.S.eW);
+            var width = A2($elm$core$Basics$max, 1, (config.fj - config.S.es) - config.S.eX);
             var toLimit = F5(
                 function(length, marginMin, marginMax, min, max) {
                     return {
-                        fy: max,
-                        fz: min,
+                        fz: max,
+                        fA: min,
                         O: length,
-                        fV: marginMax,
-                        fW: marginMin,
-                        et: max,
-                        ev: min
+                        fW: marginMax,
+                        fX: marginMin,
+                        eu: max,
+                        ew: min
                     };
                 });
-            var height = A2($elm$core$Basics$max, 1, (config.ea - config.S.dO) - config.S.fb);
+            var height = A2($elm$core$Basics$max, 1, (config.eb - config.S.dQ) - config.S.fc);
             var fixSingles = function(bs) {
-                return _Utils_eq(bs.ev, bs.et) ? _Utils_update(
+                return _Utils_eq(bs.ew, bs.eu) ? _Utils_update(
                     bs, {
-                        et: bs.ev + 10
+                        eu: bs.ew + 10
                     }) : bs;
             };
             var collectLimits = F2(
                 function(el, acc) {
                     switch (el.$) {
                         case 0:
                             return acc;
@@ -8726,83 +8744,83 @@
                             return acc;
                         default:
                             return acc;
                     }
                 });
             var limits_ = function(pos) {
                 return function(_v3) {
-                    var x = _v3.fj;
-                    var y = _v3.fk;
+                    var x = _v3.fk;
+                    var y = _v3.fl;
                     return {
-                        fj: fixSingles(x),
-                        fk: fixSingles(y)
+                        fk: fixSingles(x),
+                        fl: fixSingles(y)
                     };
                 }({
-                    fj: A5(toLimit, width, config.ap.er, config.ap.eW, pos.aK, pos.be),
-                    fk: A5(toLimit, height, config.ap.fb, config.ap.dO, pos.gA, pos.dI)
+                    fk: A5(toLimit, width, config.ap.es, config.ap.eX, pos.aM, pos.bg),
+                    fl: A5(toLimit, height, config.ap.fc, config.ap.dQ, pos.gB, pos.dK)
                 });
             }(
                 A2(
                     $terezka$elm_charts$Internal$Coordinates$foldPosition,
                     $elm$core$Basics$identity,
                     A3($elm$core$List$foldl, collectLimits, _List_Nil, elements)));
             var calcRange = function() {
-                var _v2 = config.dn;
+                var _v2 = config.dp;
                 if (!_v2.b) {
-                    return limits_.fj;
+                    return limits_.fk;
                 } else {
                     var some = _v2;
                     return A3(
                         $elm$core$List$foldl,
                         F2(
                             function(f, b) {
                                 return f(b);
                             }),
-                        limits_.fj,
+                        limits_.fk,
                         some);
                 }
             }();
             var calcDomain = function() {
-                var _v1 = config.cY;
+                var _v1 = config.cZ;
                 if (!_v1.b) {
-                    return A3($terezka$elm_charts$Chart$Attributes$lowest, 0, $terezka$elm_charts$Chart$Attributes$orLower, limits_.fk);
+                    return A3($terezka$elm_charts$Chart$Attributes$lowest, 0, $terezka$elm_charts$Chart$Attributes$orLower, limits_.fl);
                 } else {
                     var some = _v1;
                     return A3(
                         $elm$core$List$foldl,
                         F2(
                             function(f, b) {
                                 return f(b);
                             }),
-                        limits_.fk,
+                        limits_.fl,
                         some);
                 }
             }();
             var unpadded = {
-                fj: calcRange,
-                fk: calcDomain
+                fk: calcRange,
+                fl: calcDomain
             };
             var scalePadX = $terezka$elm_charts$Internal$Coordinates$scaleCartesianX(unpadded);
-            var xMax = calcRange.et + scalePadX(config.S.eW);
-            var xMin = calcRange.ev - scalePadX(config.S.er);
+            var xMax = calcRange.eu + scalePadX(config.S.eX);
+            var xMin = calcRange.ew - scalePadX(config.S.es);
             var scalePadY = $terezka$elm_charts$Internal$Coordinates$scaleCartesianY(unpadded);
-            var yMax = calcDomain.et + scalePadY(config.S.fb);
-            var yMin = calcDomain.ev - scalePadY(config.S.dO);
+            var yMax = calcDomain.eu + scalePadY(config.S.fc);
+            var yMin = calcDomain.ew - scalePadY(config.S.dQ);
             return {
-                fj: _Utils_update(
+                fk: _Utils_update(
                     calcRange, {
-                        O: config.fi,
-                        et: A2($elm$core$Basics$max, xMin, xMax),
-                        ev: A2($elm$core$Basics$min, xMin, xMax)
+                        O: config.fj,
+                        eu: A2($elm$core$Basics$max, xMin, xMax),
+                        ew: A2($elm$core$Basics$min, xMin, xMax)
                     }),
-                fk: _Utils_update(
+                fl: _Utils_update(
                     calcDomain, {
-                        O: config.ea,
-                        et: A2($elm$core$Basics$max, yMin, yMax),
-                        ev: A2($elm$core$Basics$min, yMin, yMax)
+                        O: config.eb,
+                        eu: A2($elm$core$Basics$max, yMin, yMax),
+                        ew: A2($elm$core$Basics$min, yMin, yMax)
                     })
             };
         });
     var $terezka$elm_charts$Chart$getItems = F2(
         function(plane, elements) {
             var toItems = F2(
                 function(el, acc) {
@@ -8885,17 +8903,17 @@
                 }
             });
         return A3($elm$core$List$foldl, toLegends, _List_Nil, elements);
     };
     var $terezka$elm_charts$Chart$TickValues = F4(
         function(xAxis, yAxis, xs, ys) {
             return {
-                bf: xAxis,
+                bh: xAxis,
                 A: xs,
-                bg: yAxis,
+                bi: yAxis,
                 J: ys
             };
         });
     var $terezka$elm_charts$Chart$getTickValues = F3(
         function(plane, items, elements) {
             var toValues = F2(
                 function(el, acc) {
@@ -8978,15 +8996,15 @@
             });
     };
     var $elm$svg$Svg$Attributes$class = _VirtualDom_attribute('class');
     var $terezka$elm_charts$Chart$Attributes$color = F2(
         function(v, config) {
             return (v === '') ? config : _Utils_update(
                 config, {
-                    bC: v
+                    bE: v
                 });
         });
     var $elm$core$List$append = F2(
         function(xs, ys) {
             if (!ys.b) {
                 return xs;
             } else {
@@ -9002,46 +9020,46 @@
                 A2($elm$core$List$map, f, list));
         });
     var $terezka$elm_charts$Internal$Helpers$darkGray = 'rgb(200 200 200)';
     var $terezka$elm_charts$Chart$Attributes$dashed = F2(
         function(value, config) {
             return _Utils_update(
                 config, {
-                    bF: value
+                    bH: value
                 });
         });
     var $terezka$elm_charts$Internal$Helpers$pink = '#ea60df';
     var $terezka$elm_charts$Internal$Svg$defaultDot = {
         v: '',
         x: 0,
-        bC: $terezka$elm_charts$Internal$Helpers$pink,
+        bE: $terezka$elm_charts$Internal$Helpers$pink,
         l: false,
-        fK: 0,
-        fL: '',
-        fM: 5,
+        fL: 0,
+        fM: '',
+        fN: 5,
         Q: 1,
         aG: $elm$core$Maybe$Nothing,
-        e1: 6
+        e2: 6
     };
     var $elm$svg$Svg$circle = $elm$svg$Svg$trustedNode('circle');
     var $elm$svg$Svg$Attributes$cx = _VirtualDom_attribute('cx');
     var $elm$svg$Svg$Attributes$cy = _VirtualDom_attribute('cy');
     var $elm$svg$Svg$Attributes$d = _VirtualDom_attribute('d');
     var $elm$svg$Svg$Attributes$fillOpacity = _VirtualDom_attribute('fill-opacity');
     var $elm$svg$Svg$g = $elm$svg$Svg$trustedNode('g');
     var $elm$core$Basics$clamp = F3(
         function(low, high, number) {
             return (_Utils_cmp(number, low) < 0) ? low : ((_Utils_cmp(number, high) > 0) ? high : number);
         });
     var $terezka$elm_charts$Internal$Svg$isWithinPlane = F3(
         function(plane, x, y) {
             return _Utils_eq(
-                A3($elm$core$Basics$clamp, plane.fj.ev, plane.fj.et, x),
+                A3($elm$core$Basics$clamp, plane.fk.ew, plane.fk.eu, x),
                 x) && _Utils_eq(
-                A3($elm$core$Basics$clamp, plane.fk.ev, plane.fk.et, y),
+                A3($elm$core$Basics$clamp, plane.fl.ew, plane.fl.eu, y),
                 y);
         });
     var $elm$core$Basics$not = _Basics_not;
     var $elm$svg$Svg$path = $elm$svg$Svg$trustedNode('path');
     var $elm$core$Basics$pi = _Basics_pi;
     var $elm$core$Basics$sqrt = _Basics_sqrt;
     var $terezka$elm_charts$Internal$Svg$plusPath = F4(
@@ -9073,27 +9091,27 @@
     var $elm$svg$Svg$Attributes$r = _VirtualDom_attribute('r');
     var $elm$svg$Svg$Attributes$stroke = _VirtualDom_attribute('stroke');
     var $elm$svg$Svg$Attributes$strokeOpacity = _VirtualDom_attribute('stroke-opacity');
     var $elm$svg$Svg$Attributes$strokeWidth = _VirtualDom_attribute('stroke-width');
     var $elm$svg$Svg$text = $elm$virtual_dom$VirtualDom$text;
     var $terezka$elm_charts$Internal$Coordinates$scaleSVGX = F2(
         function(plane, value) {
-            return (value * $terezka$elm_charts$Internal$Coordinates$innerWidth(plane)) / $terezka$elm_charts$Internal$Coordinates$range(plane.fj);
+            return (value * $terezka$elm_charts$Internal$Coordinates$innerWidth(plane)) / $terezka$elm_charts$Internal$Coordinates$range(plane.fk);
         });
     var $terezka$elm_charts$Internal$Coordinates$toSVGX = F2(
         function(plane, value) {
-            return A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, value - plane.fj.ev) + plane.fj.fW;
+            return A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, value - plane.fk.ew) + plane.fk.fX;
         });
     var $terezka$elm_charts$Internal$Coordinates$scaleSVGY = F2(
         function(plane, value) {
-            return (value * $terezka$elm_charts$Internal$Coordinates$innerHeight(plane)) / $terezka$elm_charts$Internal$Coordinates$range(plane.fk);
+            return (value * $terezka$elm_charts$Internal$Coordinates$innerHeight(plane)) / $terezka$elm_charts$Internal$Coordinates$range(plane.fl);
         });
     var $terezka$elm_charts$Internal$Coordinates$toSVGY = F2(
         function(plane, value) {
-            return A2($terezka$elm_charts$Internal$Coordinates$scaleSVGY, plane, plane.fk.et - value) + plane.fk.fW;
+            return A2($terezka$elm_charts$Internal$Coordinates$scaleSVGY, plane, plane.fl.eu - value) + plane.fl.fX;
         });
     var $elm$svg$Svg$Attributes$transform = _VirtualDom_attribute('transform');
     var $elm$core$Basics$degrees = function(angleInDegrees) {
         return (angleInDegrees * $elm$core$Basics$pi) / 180;
     };
     var $elm$core$Basics$tan = _Basics_tan;
     var $terezka$elm_charts$Internal$Svg$trianglePath = F4(
@@ -9124,38 +9142,38 @@
             var yOrg = toY(datum_);
             var y_ = A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, yOrg);
             var xOrg = toX(datum_);
             var x_ = A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, xOrg);
             var styleAttrs = _List_fromArray(
                 [
                     $elm$svg$Svg$Attributes$stroke(
-                        (config.v === '') ? config.bC : config.v),
+                        (config.v === '') ? config.bE : config.v),
                     $elm$svg$Svg$Attributes$strokeWidth(
                         $elm$core$String$fromFloat(config.x)),
                     $elm$svg$Svg$Attributes$fillOpacity(
                         $elm$core$String$fromFloat(config.Q)),
-                    $elm$svg$Svg$Attributes$fill(config.bC),
+                    $elm$svg$Svg$Attributes$fill(config.bE),
                     $elm$svg$Svg$Attributes$class('elm-charts__dot'),
                     config.l ? $terezka$elm_charts$Internal$Svg$withinChartArea(plane) : $elm$svg$Svg$Attributes$class('')
                 ]);
             var showDot = A3($terezka$elm_charts$Internal$Svg$isWithinPlane, plane, xOrg, yOrg) || config.l;
-            var highlightColor = (config.fL === '') ? config.bC : config.fL;
+            var highlightColor = (config.fM === '') ? config.bE : config.fM;
             var highlightAttrs = _List_fromArray(
                 [
                     $elm$svg$Svg$Attributes$stroke(highlightColor),
                     $elm$svg$Svg$Attributes$strokeWidth(
-                        $elm$core$String$fromFloat(config.fM)),
+                        $elm$core$String$fromFloat(config.fN)),
                     $elm$svg$Svg$Attributes$strokeOpacity(
-                        $elm$core$String$fromFloat(config.fK)),
+                        $elm$core$String$fromFloat(config.fL)),
                     $elm$svg$Svg$Attributes$fill('transparent'),
                     $elm$svg$Svg$Attributes$class('elm-charts__dot-highlight')
                 ]);
             var view = F3(
                 function(toEl, highlightOff, toAttrs) {
-                    return (config.fK > 0) ? A2(
+                    return (config.fL > 0) ? A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__dot-container')
                             ]),
                         _List_fromArray(
                             [
@@ -9174,29 +9192,29 @@
                             ])) : A2(
                         toEl,
                         _Utils_ap(
                             toAttrs(0),
                             styleAttrs),
                         _List_Nil);
                 });
-            var area_ = (2 * $elm$core$Basics$pi) * config.e1;
+            var area_ = (2 * $elm$core$Basics$pi) * config.e2;
             if (!showDot) {
                 return $elm$svg$Svg$text('');
             } else {
                 var _v0 = config.aG;
                 if (_v0.$ === 1) {
                     return $elm$svg$Svg$text('');
                 } else {
                     switch (_v0.a) {
                         case 0:
                             var _v1 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$circle,
-                                config.fM / 2,
+                                config.fN / 2,
                                 function(off) {
                                     var radius = $elm$core$Basics$sqrt(area_ / $elm$core$Basics$pi);
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$cx(
                                                 $elm$core$String$fromFloat(x_)),
                                             $elm$svg$Svg$Attributes$cy(
@@ -9206,28 +9224,28 @@
                                         ]);
                                 });
                         case 1:
                             var _v2 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$path,
-                                config.fM,
+                                config.fN,
                                 function(off) {
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$d(
                                                 A4($terezka$elm_charts$Internal$Svg$trianglePath, area_, off, x_, y_))
                                         ]);
                                 });
                         case 2:
                             var _v3 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$rect,
-                                config.fM,
+                                config.fN,
                                 function(off) {
                                     var side = $elm$core$Basics$sqrt(area_);
                                     var sideOff = side + off;
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$x(
                                                 $elm$core$String$fromFloat(x_ - (sideOff / 2))),
@@ -9240,15 +9258,15 @@
                                         ]);
                                 });
                         case 3:
                             var _v4 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$rect,
-                                config.fM,
+                                config.fN,
                                 function(off) {
                                     var side = $elm$core$Basics$sqrt(area_);
                                     var sideOff = side + off;
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$x(
                                                 $elm$core$String$fromFloat(x_ - (sideOff / 2))),
@@ -9263,30 +9281,30 @@
                                         ]);
                                 });
                         case 4:
                             var _v5 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$path,
-                                config.fM,
+                                config.fN,
                                 function(off) {
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$d(
                                                 A4($terezka$elm_charts$Internal$Svg$plusPath, area_, off, x_, y_)),
                                             $elm$svg$Svg$Attributes$transform(
                                                 'rotate(45 ' + ($elm$core$String$fromFloat(x_) + (' ' + ($elm$core$String$fromFloat(y_) + ')'))))
                                         ]);
                                 });
                         default:
                             var _v6 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$path,
-                                config.fM,
+                                config.fN,
                                 function(off) {
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$d(
                                                 A4($terezka$elm_charts$Internal$Svg$plusPath, area_, off, x_, y_))
                                         ]);
                                 });
@@ -9301,31 +9319,31 @@
                 plane,
                 toX,
                 toY,
                 A2($terezka$elm_charts$Internal$Helpers$apply, edits, $terezka$elm_charts$Internal$Svg$defaultDot));
         });
     var $terezka$elm_charts$Internal$Helpers$gray = '#EFF2FA';
     var $terezka$elm_charts$Internal$Svg$defaultLine = {
-        bu: _List_Nil,
-        ft: false,
-        bC: 'rgb(210, 210, 210)',
-        bF: _List_Nil,
+        bw: _List_Nil,
+        fu: false,
+        bE: 'rgb(210, 210, 210)',
+        bH: _List_Nil,
         e: false,
         l: false,
         Q: 1,
-        ge: -90,
-        gf: 0,
-        fi: 1,
-        aK: $elm$core$Maybe$Nothing,
-        be: $elm$core$Maybe$Nothing,
-        gz: $elm$core$Maybe$Nothing,
-        g: 0,
+        gf: -90,
+        gg: 0,
+        fj: 1,
+        aM: $elm$core$Maybe$Nothing,
+        bg: $elm$core$Maybe$Nothing,
         gA: $elm$core$Maybe$Nothing,
-        dI: $elm$core$Maybe$Nothing,
+        g: 0,
         gB: $elm$core$Maybe$Nothing,
+        dK: $elm$core$Maybe$Nothing,
+        gC: $elm$core$Maybe$Nothing,
         h: 0
     };
     var $terezka$elm_charts$Internal$Commands$Line = F2(
         function(a, b) {
             return {
                 $: 1,
                 a: a,
@@ -9597,33 +9615,33 @@
                     A2(
                         $elm$core$List$map,
                         $elm$html$Html$Attributes$map($elm$core$Basics$never),
                         attrs)));
         });
     var $terezka$elm_charts$Internal$Svg$line = F2(
         function(plane, config) {
-            var angle = $elm$core$Basics$degrees(config.ge);
+            var angle = $elm$core$Basics$degrees(config.gf);
             var _v0 = function() {
                 var _v3 = _Utils_Tuple3(
-                    _Utils_Tuple2(config.aK, config.be),
-                    _Utils_Tuple2(config.gA, config.dI),
-                    _Utils_Tuple2(config.gz, config.gB));
+                    _Utils_Tuple2(config.aM, config.bg),
+                    _Utils_Tuple2(config.gB, config.dK),
+                    _Utils_Tuple2(config.gA, config.gC));
                 if (!_v3.a.a.$) {
                     if (!_v3.a.b.$) {
                         if (_v3.b.a.$ === 1) {
                             if (_v3.b.b.$ === 1) {
                                 var _v4 = _v3.a;
                                 var a = _v4.a.a;
                                 var b = _v4.b.a;
                                 var _v5 = _v3.b;
                                 var _v6 = _v5.a;
                                 var _v7 = _v5.b;
                                 return _Utils_Tuple2(
                                     _Utils_Tuple2(a, b),
-                                    _Utils_Tuple2(plane.fk.ev, plane.fk.ev));
+                                    _Utils_Tuple2(plane.fl.ew, plane.fl.ew));
                             } else {
                                 var _v38 = _v3.a;
                                 var a = _v38.a.a;
                                 var b = _v38.b.a;
                                 var _v39 = _v3.b;
                                 var _v40 = _v39.a;
                                 var c = _v39.b.a;
@@ -9641,33 +9659,33 @@
                                 var _v43 = _v42.b;
                                 return _Utils_Tuple2(
                                     _Utils_Tuple2(a, b),
                                     _Utils_Tuple2(c, c));
                             } else {
                                 return _Utils_Tuple2(
                                     _Utils_Tuple2(
-                                        A2($elm$core$Maybe$withDefault, plane.fj.ev, config.aK),
-                                        A2($elm$core$Maybe$withDefault, plane.fj.et, config.be)),
+                                        A2($elm$core$Maybe$withDefault, plane.fk.ew, config.aM),
+                                        A2($elm$core$Maybe$withDefault, plane.fk.eu, config.bg)),
                                     _Utils_Tuple2(
-                                        A2($elm$core$Maybe$withDefault, plane.fk.ev, config.gA),
-                                        A2($elm$core$Maybe$withDefault, plane.fk.et, config.dI)));
+                                        A2($elm$core$Maybe$withDefault, plane.fl.ew, config.gB),
+                                        A2($elm$core$Maybe$withDefault, plane.fl.eu, config.dK)));
                             }
                         }
                     } else {
                         if (_v3.b.a.$ === 1) {
                             if (_v3.b.b.$ === 1) {
                                 var _v8 = _v3.a;
                                 var a = _v8.a.a;
                                 var _v9 = _v8.b;
                                 var _v10 = _v3.b;
                                 var _v11 = _v10.a;
                                 var _v12 = _v10.b;
                                 return _Utils_Tuple2(
                                     _Utils_Tuple2(a, a),
-                                    _Utils_Tuple2(plane.fk.ev, plane.fk.et));
+                                    _Utils_Tuple2(plane.fl.ew, plane.fl.eu));
                             } else {
                                 if (!_v3.c.a.$) {
                                     if (!_v3.c.b.$) {
                                         var _v51 = _v3.a;
                                         var a = _v51.a.a;
                                         var _v52 = _v51.b;
                                         var _v53 = _v3.b;
@@ -9707,15 +9725,15 @@
                                         var _v46 = _v3.b;
                                         var _v47 = _v46.a;
                                         var b = _v46.b.a;
                                         var _v48 = _v3.c;
                                         var _v49 = _v48.a;
                                         var _v50 = _v48.b;
                                         return _Utils_Tuple2(
-                                            _Utils_Tuple2(a, plane.fj.et),
+                                            _Utils_Tuple2(a, plane.fk.eu),
                                             _Utils_Tuple2(b, b));
                                     } else {
                                         var _v62 = _v3.a;
                                         var a = _v62.a.a;
                                         var _v63 = _v62.b;
                                         var _v64 = _v3.b;
                                         var _v65 = _v64.a;
@@ -9785,15 +9803,15 @@
                                         var _v70 = _v3.b;
                                         var b = _v70.a.a;
                                         var _v71 = _v70.b;
                                         var _v72 = _v3.c;
                                         var _v73 = _v72.a;
                                         var _v74 = _v72.b;
                                         return _Utils_Tuple2(
-                                            _Utils_Tuple2(a, plane.fj.et),
+                                            _Utils_Tuple2(a, plane.fk.eu),
                                             _Utils_Tuple2(b, b));
                                     } else {
                                         var _v86 = _v3.a;
                                         var a = _v86.a.a;
                                         var _v87 = _v86.b;
                                         var _v88 = _v3.b;
                                         var b = _v88.a.a;
@@ -9819,15 +9837,15 @@
                                 var _v14 = _v13.a;
                                 var b = _v13.b.a;
                                 var _v15 = _v3.b;
                                 var _v16 = _v15.a;
                                 var _v17 = _v15.b;
                                 return _Utils_Tuple2(
                                     _Utils_Tuple2(b, b),
-                                    _Utils_Tuple2(plane.fk.ev, plane.fk.et));
+                                    _Utils_Tuple2(plane.fl.ew, plane.fl.eu));
                             } else {
                                 if (!_v3.c.a.$) {
                                     if (!_v3.c.b.$) {
                                         var _v99 = _v3.a;
                                         var _v100 = _v99.a;
                                         var a = _v99.b.a;
                                         var _v101 = _v3.b;
@@ -9867,15 +9885,15 @@
                                         var _v94 = _v3.b;
                                         var _v95 = _v94.a;
                                         var b = _v94.b.a;
                                         var _v96 = _v3.c;
                                         var _v97 = _v96.a;
                                         var _v98 = _v96.b;
                                         return _Utils_Tuple2(
-                                            _Utils_Tuple2(a, plane.fj.et),
+                                            _Utils_Tuple2(a, plane.fk.eu),
                                             _Utils_Tuple2(b, b));
                                     } else {
                                         var _v110 = _v3.a;
                                         var _v111 = _v110.a;
                                         var a = _v110.b.a;
                                         var _v112 = _v3.b;
                                         var _v113 = _v112.a;
@@ -9945,15 +9963,15 @@
                                         var _v118 = _v3.b;
                                         var b = _v118.a.a;
                                         var _v119 = _v118.b;
                                         var _v120 = _v3.c;
                                         var _v121 = _v120.a;
                                         var _v122 = _v120.b;
                                         return _Utils_Tuple2(
-                                            _Utils_Tuple2(a, plane.fj.et),
+                                            _Utils_Tuple2(a, plane.fk.eu),
                                             _Utils_Tuple2(b, b));
                                     } else {
                                         var _v134 = _v3.a;
                                         var _v135 = _v134.a;
                                         var a = _v134.b.a;
                                         var _v136 = _v3.b;
                                         var b = _v136.a.a;
@@ -9976,48 +9994,48 @@
                                 var _v18 = _v3.a;
                                 var _v19 = _v18.a;
                                 var _v20 = _v18.b;
                                 var _v21 = _v3.b;
                                 var a = _v21.a.a;
                                 var b = _v21.b.a;
                                 return _Utils_Tuple2(
-                                    _Utils_Tuple2(plane.fj.ev, plane.fj.ev),
+                                    _Utils_Tuple2(plane.fk.ew, plane.fk.ew),
                                     _Utils_Tuple2(a, b));
                             } else {
                                 var _v22 = _v3.a;
                                 var _v23 = _v22.a;
                                 var _v24 = _v22.b;
                                 var _v25 = _v3.b;
                                 var a = _v25.a.a;
                                 var _v26 = _v25.b;
                                 return _Utils_Tuple2(
-                                    _Utils_Tuple2(plane.fj.ev, plane.fj.et),
+                                    _Utils_Tuple2(plane.fk.ew, plane.fk.eu),
                                     _Utils_Tuple2(a, a));
                             }
                         } else {
                             if (!_v3.b.b.$) {
                                 var _v27 = _v3.a;
                                 var _v28 = _v27.a;
                                 var _v29 = _v27.b;
                                 var _v30 = _v3.b;
                                 var _v31 = _v30.a;
                                 var b = _v30.b.a;
                                 return _Utils_Tuple2(
-                                    _Utils_Tuple2(plane.fj.ev, plane.fj.et),
+                                    _Utils_Tuple2(plane.fk.ew, plane.fk.eu),
                                     _Utils_Tuple2(b, b));
                             } else {
                                 var _v140 = _v3.a;
                                 var _v141 = _v140.a;
                                 var _v142 = _v140.b;
                                 var _v143 = _v3.b;
                                 var _v144 = _v143.a;
                                 var _v145 = _v143.b;
                                 return _Utils_Tuple2(
-                                    _Utils_Tuple2(plane.fj.ev, plane.fj.et),
-                                    _Utils_Tuple2(plane.fk.ev, plane.fk.et));
+                                    _Utils_Tuple2(plane.fk.ew, plane.fk.eu),
+                                    _Utils_Tuple2(plane.fl.ew, plane.fl.eu));
                             }
                         }
                     }
                 }
             }();
             var _v1 = _v0.a;
             var x1 = _v1.a;
@@ -10025,86 +10043,86 @@
             var _v2 = _v0.b;
             var y1 = _v2.a;
             var y2 = _v2.b;
             var x1_ = x1 + A2($terezka$elm_charts$Internal$Svg$lengthInCartesianX, plane, config.g);
             var x2_ = x2 + A2($terezka$elm_charts$Internal$Svg$lengthInCartesianX, plane, config.g);
             var y1_ = y1 - A2($terezka$elm_charts$Internal$Svg$lengthInCartesianY, plane, config.h);
             var y2_ = y2 - A2($terezka$elm_charts$Internal$Svg$lengthInCartesianY, plane, config.h);
-            var _v146 = (config.gf > 0) ? _Utils_Tuple2(
+            var _v146 = (config.gg > 0) ? _Utils_Tuple2(
                 A2(
                     $terezka$elm_charts$Internal$Svg$lengthInCartesianX,
                     plane,
-                    $elm$core$Basics$cos(angle) * config.gf),
+                    $elm$core$Basics$cos(angle) * config.gg),
                 A2(
                     $terezka$elm_charts$Internal$Svg$lengthInCartesianY,
                     plane,
-                    $elm$core$Basics$sin(angle) * config.gf)) : _Utils_Tuple2(0, 0);
+                    $elm$core$Basics$sin(angle) * config.gg)) : _Utils_Tuple2(0, 0);
             var tickOffsetX = _v146.a;
             var tickOffsetY = _v146.b;
             var cmds = config.e ? _Utils_ap(
-                (config.gf > 0) ? _List_fromArray(
+                (config.gg > 0) ? _List_fromArray(
                     [
                         A2($terezka$elm_charts$Internal$Commands$Move, x2_ + tickOffsetX, y2_ + tickOffsetY),
                         A2($terezka$elm_charts$Internal$Commands$Line, x2_, y2_)
                     ]) : _List_fromArray(
                     [
                         A2($terezka$elm_charts$Internal$Commands$Move, x2_, y2_)
                     ]),
                 _Utils_ap(
-                    config.ft ? _List_fromArray(
+                    config.fu ? _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x2_, y1_),
                             A2($terezka$elm_charts$Internal$Commands$Line, x1_, y1_)
                         ]) : _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x1_, y1_)
                         ]),
-                    (config.gf > 0) ? _List_fromArray(
+                    (config.gg > 0) ? _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x1_ + tickOffsetX, y1_ + tickOffsetY)
                         ]) : _List_Nil)) : _Utils_ap(
-                (config.gf > 0) ? _List_fromArray(
+                (config.gg > 0) ? _List_fromArray(
                     [
                         A2($terezka$elm_charts$Internal$Commands$Move, x1_ + tickOffsetX, y1_ + tickOffsetY),
                         A2($terezka$elm_charts$Internal$Commands$Line, x1_, y1_)
                     ]) : _List_fromArray(
                     [
                         A2($terezka$elm_charts$Internal$Commands$Move, x1_, y1_)
                     ]),
                 _Utils_ap(
-                    config.ft ? _List_fromArray(
+                    config.fu ? _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x1_, y2_),
                             A2($terezka$elm_charts$Internal$Commands$Line, x2_, y2_)
                         ]) : _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x2_, y2_)
                         ]),
-                    (config.gf > 0) ? _List_fromArray(
+                    (config.gg > 0) ? _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x2_ + tickOffsetX, y2_ + tickOffsetY)
                         ]) : _List_Nil));
             return A4(
                 $terezka$elm_charts$Internal$Svg$withAttrs,
-                config.bu,
+                config.bw,
                 $elm$svg$Svg$path,
                 _List_fromArray(
                     [
                         $elm$svg$Svg$Attributes$class('elm-charts__line'),
                         $elm$svg$Svg$Attributes$fill('transparent'),
-                        $elm$svg$Svg$Attributes$stroke(config.bC),
+                        $elm$svg$Svg$Attributes$stroke(config.bE),
                         $elm$svg$Svg$Attributes$strokeWidth(
-                            $elm$core$String$fromFloat(config.fi)),
+                            $elm$core$String$fromFloat(config.fj)),
                         $elm$svg$Svg$Attributes$strokeOpacity(
                             $elm$core$String$fromFloat(config.Q)),
                         $elm$svg$Svg$Attributes$strokeDasharray(
                             A2(
                                 $elm$core$String$join,
                                 ' ',
-                                A2($elm$core$List$map, $elm$core$String$fromFloat, config.bF))),
+                                A2($elm$core$List$map, $elm$core$String$fromFloat, config.bH))),
                         $elm$svg$Svg$Attributes$d(
                             A2($terezka$elm_charts$Internal$Commands$description, plane, cmds)),
                         config.l ? $terezka$elm_charts$Internal$Svg$withinChartArea(plane) : $elm$svg$Svg$Attributes$class('')
                     ]),
                 _List_Nil);
         });
     var $terezka$elm_charts$Chart$Svg$line = F2(
@@ -10123,109 +10141,109 @@
                 },
                 xs);
         });
     var $terezka$elm_charts$Chart$Attributes$size = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    e1: v
+                    e2: v
                 });
         });
     var $terezka$elm_charts$Chart$Attributes$width = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    fi: v
+                    fj: v
                 });
         });
     var $terezka$elm_charts$Chart$Attributes$x1 = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    aK: $elm$core$Maybe$Just(v)
+                    aM: $elm$core$Maybe$Just(v)
                 });
         });
     var $terezka$elm_charts$Chart$Attributes$y1 = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    gA: $elm$core$Maybe$Just(v)
+                    gB: $elm$core$Maybe$Just(v)
                 });
         });
     var $terezka$elm_charts$Chart$grid = function(edits) {
         var config = A2(
             $terezka$elm_charts$Internal$Helpers$apply,
             edits, {
-                bC: '',
-                bF: _List_Nil,
-                aP: false,
-                fi: 0
+                bE: '',
+                bH: _List_Nil,
+                aR: false,
+                fj: 0
             });
-        var width = (!config.fi) ? (config.aP ? 0.5 : 1) : config.fi;
-        var color = $elm$core$String$isEmpty(config.bC) ? (config.aP ? $terezka$elm_charts$Internal$Helpers$darkGray : $terezka$elm_charts$Internal$Helpers$gray) : config.bC;
+        var width = (!config.fj) ? (config.aR ? 0.5 : 1) : config.fj;
+        var color = $elm$core$String$isEmpty(config.bE) ? (config.aR ? $terezka$elm_charts$Internal$Helpers$darkGray : $terezka$elm_charts$Internal$Helpers$gray) : config.bE;
         var toDot = F4(
             function(vs, p, x, y) {
-                return (A2($elm$core$List$member, x, vs.bf) || A2($elm$core$List$member, y, vs.bg)) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
+                return (A2($elm$core$List$member, x, vs.bh) || A2($elm$core$List$member, y, vs.bi)) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
                     A5(
                         $terezka$elm_charts$Chart$Svg$dot,
                         p,
                         function($) {
-                            return $.fj;
+                            return $.fk;
                         },
                         function($) {
-                            return $.fk;
+                            return $.fl;
                         },
                         _List_fromArray(
                             [
                                 $terezka$elm_charts$Chart$Attributes$color(color),
                                 $terezka$elm_charts$Chart$Attributes$size(width),
                                 $terezka$elm_charts$Chart$Attributes$circle
                             ]), {
-                            fj: x,
-                            fk: y
+                            fk: x,
+                            fl: y
                         }));
             });
         var toXGrid = F3(
             function(vs, p, v) {
-                return A2($elm$core$List$member, v, vs.bf) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
+                return A2($elm$core$List$member, v, vs.bh) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
                     A2(
                         $terezka$elm_charts$Chart$Svg$line,
                         p,
                         _List_fromArray(
                             [
                                 $terezka$elm_charts$Chart$Attributes$color(color),
                                 $terezka$elm_charts$Chart$Attributes$width(width),
                                 $terezka$elm_charts$Chart$Attributes$x1(v),
-                                $terezka$elm_charts$Chart$Attributes$dashed(config.bF)
+                                $terezka$elm_charts$Chart$Attributes$dashed(config.bH)
                             ])));
             });
         var toYGrid = F3(
             function(vs, p, v) {
-                return A2($elm$core$List$member, v, vs.bg) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
+                return A2($elm$core$List$member, v, vs.bi) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
                     A2(
                         $terezka$elm_charts$Chart$Svg$line,
                         p,
                         _List_fromArray(
                             [
                                 $terezka$elm_charts$Chart$Attributes$color(color),
                                 $terezka$elm_charts$Chart$Attributes$width(width),
                                 $terezka$elm_charts$Chart$Attributes$y1(v),
-                                $terezka$elm_charts$Chart$Attributes$dashed(config.bF)
+                                $terezka$elm_charts$Chart$Attributes$dashed(config.bH)
                             ])));
             });
         return $terezka$elm_charts$Chart$GridElement(
             F2(
                 function(p, vs) {
                     return A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__grid')
                             ]),
-                        config.aP ? A2(
+                        config.aR ? A2(
                             $elm$core$List$concatMap,
                             function(x) {
                                 return A2(
                                     $elm$core$List$filterMap,
                                     A3(toDot, vs, p, x),
                                     vs.J);
                             },
@@ -10455,61 +10473,61 @@
                     $terezka$elm_charts$Chart$grid(_List_Nil),
                     indexedElements);
             }();
             var legends_ = $terezka$elm_charts$Chart$getLegends(elements);
             var config = A2(
                 $terezka$elm_charts$Internal$Helpers$apply,
                 edits, {
-                    bu: _List_fromArray(
+                    bw: _List_fromArray(
                         [
                             $elm$svg$Svg$Attributes$style('overflow: visible;')
                         ]),
-                    cY: _List_Nil,
-                    bL: _List_Nil,
-                    ea: 300,
-                    bX: _List_Nil,
+                    cZ: _List_Nil,
+                    bN: _List_Nil,
+                    eb: 300,
+                    bZ: _List_Nil,
                     ap: {
-                        dO: 0,
-                        er: 0,
-                        eW: 0,
-                        fb: 0
+                        dQ: 0,
+                        es: 0,
+                        eX: 0,
+                        fc: 0
                     },
                     S: {
-                        dO: 0,
-                        er: 0,
-                        eW: 0,
-                        fb: 0
+                        dQ: 0,
+                        es: 0,
+                        eX: 0,
+                        fc: 0
                     },
-                    dn: _List_Nil,
-                    cw: true,
-                    fi: 300
+                    dp: _List_Nil,
+                    cy: true,
+                    fj: 300
                 });
             var plane = A2($terezka$elm_charts$Chart$definePlane, config, elements);
             var items = A2($terezka$elm_charts$Chart$getItems, plane, elements);
             var toEvent = function(_v2) {
                 var event_ = _v2;
-                var _v1 = event_.fB;
+                var _v1 = event_.fC;
                 var decoder = _v1;
                 return A2(
                     $terezka$elm_charts$Internal$Svg$Event,
-                    event_.fZ,
+                    event_.f_,
                     decoder(items));
             };
             var tickValues = A3($terezka$elm_charts$Chart$getTickValues, plane, items, elements);
             var _v0 = A6($terezka$elm_charts$Chart$viewElements, config, plane, tickValues, items, legends_, elements);
             var beforeEls = _v0.a;
             var chartEls = _v0.b;
             var afterEls = _v0.c;
             return A5(
                 $terezka$elm_charts$Internal$Svg$container,
                 plane, {
-                    bu: config.bu,
-                    bL: A2($elm$core$List$map, toEvent, config.bL),
-                    bX: config.bX,
-                    cw: config.cw
+                    bw: config.bw,
+                    bN: A2($elm$core$List$map, toEvent, config.bN),
+                    bZ: config.bZ,
+                    cy: config.cy
                 },
                 beforeEls,
                 chartEls,
                 afterEls);
         });
     var $terezka$elm_charts$Internal$Many$Remodel = F2(
         function(a, b) {
@@ -10517,74 +10535,74 @@
                 $: 0,
                 a: a,
                 b: b
             };
         });
     var $terezka$elm_charts$Internal$Coordinates$center = function(pos) {
         return {
-            fj: pos.aK + ((pos.be - pos.aK) / 2),
-            fk: pos.gA + ((pos.dI - pos.gA) / 2)
+            fk: pos.aM + ((pos.bg - pos.aM) / 2),
+            fl: pos.gB + ((pos.dK - pos.gB) / 2)
         };
     };
     var $terezka$elm_charts$Internal$Many$fromPoint = function(point) {
         return {
-            aK: point.fj,
-            be: point.fj,
-            gA: point.fk,
-            dI: point.fk
+            aM: point.fk,
+            bg: point.fk,
+            gB: point.fl,
+            dK: point.fl
         };
     };
     var $terezka$elm_charts$Internal$Item$getPosition = F2(
         function(plane, _v0) {
             var item = _v0;
-            return A2(item.gp, plane, item.fv);
+            return A2(item.gq, plane, item.fw);
         });
     var $terezka$elm_charts$Internal$Item$Dot = function(a) {
         return {
             $: 0,
             a: a
         };
     };
     var $terezka$elm_charts$Internal$Item$Rendered = $elm$core$Basics$identity;
     var $terezka$elm_charts$Internal$Item$isDot = function(_v0) {
         var item = _v0;
-        var _v1 = item.fv.f1;
+        var _v1 = item.fw.f2;
         if (!_v1.$) {
             var dot = _v1.a;
             return $elm$core$Maybe$Just({
-                fv: {
-                    f1: dot,
-                    gk: $terezka$elm_charts$Internal$Item$Dot,
-                    cH: item.fv.cH,
-                    gv: item.fv.gv
+                fw: {
+                    f2: dot,
+                    gl: $terezka$elm_charts$Internal$Item$Dot,
+                    cI: item.fw.cI,
+                    gw: item.fw.gw
                 },
-                gl: function(c) {
-                    return item.gl(item.fv);
+                gm: function(c) {
+                    return item.gm(item.fw);
                 },
-                gm: function(_v2) {
-                    return item.gm(item.fv);
+                gn: function(_v2) {
+                    return item.gn(item.fw);
                 },
-                gp: F2(
+                gq: F2(
                     function(plane, _v3) {
-                        return A2(item.gp, plane, item.fv);
+                        return A2(item.gq, plane, item.fw);
                     }),
-                gq: F3(
+                gr: F3(
                     function(plane, config, pos) {
-                        return config.gv.fT ? A5(
+                        return config.gw.fU ? A5(
                             $terezka$elm_charts$Internal$Svg$dot,
                             plane,
                             function($) {
-                                return $.fj;
+                                return $.fk;
                             },
                             function($) {
-                                return $.fk;
+                                return $.fl;
                             },
-                            config.f1, {
-                                fj: config.gv.aK,
-                                fk: config.gv.fk
+                            config.f2, {
+                                fk: config.gw.aM,
+                                fl: config.gw.fl
                             }) : $elm$svg$Svg$text('');
                     })
             });
         } else {
             return $elm$core$Maybe$Nothing;
         }
     };
@@ -10656,27 +10674,42 @@
                 return '10';
             case 10:
                 return '11';
             default:
                 return '12';
         }
     };
+    var $elm$core$String$pad = F3(
+        function(n, _char, string) {
+            var half = (n - $elm$core$String$length(string)) / 2;
+            return _Utils_ap(
+                A2(
+                    $elm$core$String$repeat,
+                    $elm$core$Basics$ceiling(half),
+                    $elm$core$String$fromChar(_char)),
+                _Utils_ap(
+                    string,
+                    A2(
+                        $elm$core$String$repeat,
+                        $elm$core$Basics$floor(half),
+                        $elm$core$String$fromChar(_char))));
+        });
     var $elm$time$Time$flooredDiv = F2(
         function(numerator, denominator) {
             return $elm$core$Basics$floor(numerator / denominator);
         });
     var $elm$time$Time$toAdjustedMinutesHelp = F3(
         function(defaultOffset, posixMinutes, eras) {
             toAdjustedMinutesHelp: while (true) {
                 if (!eras.b) {
                     return posixMinutes + defaultOffset;
                 } else {
                     var era = eras.a;
                     var olderEras = eras.b;
-                    if (_Utils_cmp(era.dz, posixMinutes) < 0) {
+                    if (_Utils_cmp(era.dB, posixMinutes) < 0) {
                         return posixMinutes + era.b;
                     } else {
                         var $temp$defaultOffset = defaultOffset,
                             $temp$posixMinutes = posixMinutes,
                             $temp$eras = olderEras;
                         defaultOffset = $temp$defaultOffset;
                         posixMinutes = $temp$posixMinutes;
@@ -10706,23 +10739,23 @@
         var dayOfEra = rawDay - (era * 146097);
         var yearOfEra = ((((dayOfEra - ((dayOfEra / 1460) | 0)) + ((dayOfEra / 36524) | 0)) - ((dayOfEra / 146096) | 0)) / 365) | 0;
         var dayOfYear = dayOfEra - (((365 * yearOfEra) + ((yearOfEra / 4) | 0)) - ((yearOfEra / 100) | 0));
         var mp = (((5 * dayOfYear) + 2) / 153) | 0;
         var month = mp + ((mp < 10) ? 3 : (-9));
         var year = yearOfEra + (era * 400);
         return {
-            dW: (dayOfYear - ((((153 * mp) + 2) / 5) | 0)) + 1,
-            ex: month,
-            fl: year + ((month <= 2) ? 1 : 0)
+            dY: (dayOfYear - ((((153 * mp) + 2) / 5) | 0)) + 1,
+            ey: month,
+            fm: year + ((month <= 2) ? 1 : 0)
         };
     };
     var $elm$time$Time$toDay = F2(
         function(zone, time) {
             return $elm$time$Time$toCivil(
-                A2($elm$time$Time$toAdjustedMinutes, zone, time)).dW;
+                A2($elm$time$Time$toAdjustedMinutes, zone, time)).dY;
         });
     var $elm$time$Time$toHour = F2(
         function(zone, time) {
             return A2(
                 $elm$core$Basics$modBy,
                 24,
                 A2(
@@ -10748,15 +10781,15 @@
     var $elm$time$Time$May = 4;
     var $elm$time$Time$Nov = 10;
     var $elm$time$Time$Oct = 9;
     var $elm$time$Time$Sep = 8;
     var $elm$time$Time$toMonth = F2(
         function(zone, time) {
             var _v0 = $elm$time$Time$toCivil(
-                A2($elm$time$Time$toAdjustedMinutes, zone, time)).ex;
+                A2($elm$time$Time$toAdjustedMinutes, zone, time)).ey;
             switch (_v0) {
                 case 1:
                     return 0;
                 case 2:
                     return 1;
                 case 3:
                     return 2;
@@ -10789,59 +10822,134 @@
                     $elm$time$Time$flooredDiv,
                     $elm$time$Time$posixToMillis(time),
                     1000));
         });
     var $elm$time$Time$toYear = F2(
         function(zone, time) {
             return $elm$time$Time$toCivil(
-                A2($elm$time$Time$toAdjustedMinutes, zone, time)).fl;
+                A2($elm$time$Time$toAdjustedMinutes, zone, time)).fm;
         });
-    var $elm$time$Time$utc = A2($elm$time$Time$Zone, 0, _List_Nil);
-    var $author$project$Graph$formatTime = function(time) {
-        var milliTime = $elm$time$Time$millisToPosix(
-            $elm$core$Basics$floor(time) * 1000);
-        var minute = $elm$core$String$fromInt(
-            A2($elm$time$Time$toMinute, $elm$time$Time$utc, milliTime));
-        var month = $author$project$Graph$monthToString(
-            A2($elm$time$Time$toMonth, $elm$time$Time$utc, milliTime));
-        var second = $elm$core$String$fromInt(
-            A2($elm$time$Time$toSecond, $elm$time$Time$utc, milliTime));
-        var year = $elm$core$String$fromInt(
-            A2($elm$time$Time$toYear, $elm$time$Time$utc, milliTime));
-        var hour = $elm$core$String$fromInt(
-            A2($elm$time$Time$toHour, $elm$time$Time$utc, milliTime));
-        var day = $elm$core$String$fromInt(
-            A2($elm$time$Time$toDay, $elm$time$Time$utc, milliTime));
-        return month + ('/' + (day + (' ' + (hour + (':' + (minute + (':' + second)))))));
+    var $author$project$Graph$formatTime = F2(
+        function(time, timeZone) {
+            var milliTime = $elm$time$Time$millisToPosix(
+                $elm$core$Basics$floor(time) * 1000);
+            var minute = A3(
+                $elm$core$String$pad,
+                2,
+                '0',
+                $elm$core$String$fromInt(
+                    A2($elm$time$Time$toMinute, timeZone, milliTime)));
+            var month = $author$project$Graph$monthToString(
+                A2($elm$time$Time$toMonth, timeZone, milliTime));
+            var second = A3(
+                $elm$core$String$pad,
+                2,
+                '0',
+                $elm$core$String$fromInt(
+                    A2($elm$time$Time$toSecond, timeZone, milliTime)));
+            var year = $elm$core$String$fromInt(
+                A2($elm$time$Time$toYear, timeZone, milliTime));
+            var hour = A3(
+                $elm$core$String$pad,
+                2,
+                '0',
+                $elm$core$String$fromInt(
+                    A2($elm$time$Time$toHour, timeZone, milliTime)));
+            var day = $elm$core$String$fromInt(
+                A2($elm$time$Time$toDay, timeZone, milliTime));
+            return month + ('/' + (day + (' ' + (hour + (':' + (minute + (':' + second)))))));
+        });
+    var $elm$html$Html$br = _VirtualDom_node('br');
+    var $terezka$elm_charts$Internal$Item$getColor = function(_v0) {
+        var item = _v0;
+        return item.fw.cI.bE;
     };
+    var $terezka$elm_charts$Chart$Item$getColor = $terezka$elm_charts$Internal$Item$getColor;
+    var $terezka$elm_charts$Internal$Item$getDatum = function(_v0) {
+        var item = _v0;
+        return item.fw.gw.fB;
+    };
+    var $terezka$elm_charts$Chart$Item$getData = $terezka$elm_charts$Internal$Item$getDatum;
+    var $elm$html$Html$span = _VirtualDom_node('span');
+    var $author$project$Graph$getEpaToolTip = F2(
+        function(item, timeZone) {
+            var data = $terezka$elm_charts$Chart$Item$getData(item);
+            var formattedTime = A2($author$project$Graph$formatTime, data.aI, timeZone);
+            var value = $elm$core$String$fromFloat(data.c_);
+            var color = $terezka$elm_charts$Chart$Item$getColor(item);
+            return _List_fromArray(
+                [
+                    A2(
+                        $elm$html$Html$div,
+                        _List_Nil,
+                        _List_fromArray(
+                            [
+                                A2(
+                                    $elm$html$Html$span,
+                                    _List_fromArray(
+                                        [
+                                            A2($elm$html$Html$Attributes$style, 'color', color)
+                                        ]),
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$text('EPA')
+                                        ])),
+                                A2(
+                                    $elm$html$Html$span,
+                                    _List_Nil,
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$text(': ' + value)
+                                        ])),
+                                A2($elm$html$Html$br, _List_Nil, _List_Nil),
+                                A2(
+                                    $elm$html$Html$span,
+                                    _List_fromArray(
+                                        [
+                                            A2($elm$html$Html$Attributes$style, 'color', color)
+                                        ]),
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$text('Time')
+                                        ])),
+                                A2(
+                                    $elm$html$Html$span,
+                                    _List_Nil,
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$text(': ' + formattedTime)
+                                        ]))
+                            ]))
+                ]);
+        });
     var $terezka$elm_charts$Internal$Events$Decoder = $elm$core$Basics$identity;
     var $terezka$elm_charts$Internal$Many$apply = F2(
         function(_v0, items) {
             var func = _v0.b;
             return func(items);
         });
     var $terezka$elm_charts$Internal$Svg$closestPoint = F2(
         function(pos, searched) {
             return {
-                fj: A3($elm$core$Basics$clamp, pos.aK, pos.be, searched.fj),
-                fk: A3($elm$core$Basics$clamp, pos.gA, pos.dI, searched.fk)
+                fk: A3($elm$core$Basics$clamp, pos.aM, pos.bg, searched.fk),
+                fl: A3($elm$core$Basics$clamp, pos.gB, pos.dK, searched.fl)
             };
         });
     var $elm$core$Basics$abs = function(n) {
         return (n < 0) ? (-n) : n;
     };
     var $terezka$elm_charts$Internal$Svg$distanceX = F3(
         function(plane, searched, point) {
             return $elm$core$Basics$abs(
-                A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, point.fj) - A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, searched.fj));
+                A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, point.fk) - A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, searched.fk));
         });
     var $terezka$elm_charts$Internal$Svg$distanceY = F3(
         function(plane, searched, point) {
             return $elm$core$Basics$abs(
-                A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, point.fk) - A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, searched.fk));
+                A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, point.fl) - A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, searched.fl));
         });
     var $elm$core$Basics$pow = _Basics_pow;
     var $terezka$elm_charts$Internal$Svg$distanceSquared = F3(
         function(plane, searched, point) {
             return A2(
                 $elm$core$Basics$pow,
                 A3($terezka$elm_charts$Internal$Svg$distanceX, plane, searched, point),
@@ -10858,15 +10966,15 @@
         } else {
             return $elm$core$Maybe$Nothing;
         }
     };
     var $terezka$elm_charts$Internal$Svg$keepOne = function(toPosition) {
         var toArea = function(a) {
             return function(pos) {
-                return (pos.aK - pos.be) * (pos.gA - pos.dI);
+                return (pos.aM - pos.bg) * (pos.gB - pos.dK);
             }(
                 toPosition(a));
         };
         var func = F2(
             function(one, acc) {
                 var _v0 = $elm$core$List$head(acc);
                 if (_v0.$ === 1) {
@@ -10933,56 +11041,56 @@
             });
     };
     var $terezka$elm_charts$Chart$Events$getNearest = $terezka$elm_charts$Internal$Events$getNearest;
     var $terezka$elm_charts$Chart$Attributes$height = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    ea: v
+                    eb: v
                 });
         });
     var $terezka$elm_charts$Chart$Attributes$htmlAttrs = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    bX: v
+                    bZ: v
                 });
         });
     var $terezka$elm_charts$Internal$Svg$Linear = 0;
     var $terezka$elm_charts$Chart$Attributes$linear = function(config) {
         return _Utils_update(
             config, {
-                fX: $elm$core$Maybe$Just(0)
+                fY: $elm$core$Maybe$Just(0)
             });
     };
     var $terezka$elm_charts$Internal$Property$Property = function(a) {
         return {
             $: 0,
             a: a
         };
     };
     var $terezka$elm_charts$Internal$Property$property = F3(
         function(value, inter, attrs) {
             return $terezka$elm_charts$Internal$Property$Property({
-                bu: attrs,
-                d4: F5(
+                bw: attrs,
+                d5: F5(
                     function(_v0, _v1, _v2, _v3, _v4) {
                         return _List_Nil;
                     }),
                 F: A2(
                     $elm$core$Basics$composeR,
                     value,
                     A2(
                         $elm$core$Basics$composeR,
                         $elm$core$Maybe$map($elm$core$String$fromFloat),
                         $elm$core$Maybe$withDefault('N/A'))),
-                fR: inter,
-                eu: $elm$core$Maybe$Nothing,
+                fS: inter,
+                ev: $elm$core$Maybe$Nothing,
                 Z: value,
-                a7: value
+                a9: value
             });
         });
     var $terezka$elm_charts$Chart$interpolated = F2(
         function(y, inter) {
             return A2(
                 $terezka$elm_charts$Internal$Property$property,
                 A2($elm$core$Basics$composeR, y, $elm$core$Maybe$Just),
@@ -10996,21 +11104,21 @@
             $: 13,
             a: a
         };
     };
     var $terezka$elm_charts$Internal$Coordinates$Axis = F7(
         function(length, marginMin, marginMax, dataMin, dataMax, min, max) {
             return {
-                fy: dataMax,
-                fz: dataMin,
+                fz: dataMax,
+                fA: dataMin,
                 O: length,
-                fV: marginMax,
-                fW: marginMin,
-                et: max,
-                ev: min
+                fW: marginMax,
+                fX: marginMin,
+                eu: max,
+                ew: min
             };
         });
     var $terezka$elm_charts$Internal$Svg$apply = F2(
         function(funcs, _default) {
             var apply_ = F2(
                 function(f, a) {
                     return f(a);
@@ -11099,83 +11207,83 @@
             var _v0 = function() {
                 switch (design.$) {
                     case 0:
                         var edits = design.a;
                         var config = A2(
                             $terezka$elm_charts$Internal$Svg$apply,
                             edits, {
-                                bC: defaultColor,
+                                bE: defaultColor,
                                 o: 45,
-                                f9: 4,
-                                fi: 3
+                                ga: 4,
+                                fj: 3
                             });
                         var theId = toPatternId(
                             _List_fromArray(
                                 [
-                                    config.bC,
-                                    $elm$core$String$fromFloat(config.fi),
-                                    $elm$core$String$fromFloat(config.f9),
+                                    config.bE,
+                                    $elm$core$String$fromFloat(config.fj),
+                                    $elm$core$String$fromFloat(config.ga),
                                     $elm$core$String$fromFloat(config.o)
                                 ]));
                         return _Utils_Tuple2(
                             A4(
                                 toPatternDefs,
                                 theId,
-                                config.f9,
+                                config.ga,
                                 config.o,
                                 A2(
                                     $elm$svg$Svg$line,
                                     _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$x1('0'),
                                             $elm$svg$Svg$Attributes$y('0'),
                                             $elm$svg$Svg$Attributes$x2('0'),
                                             $elm$svg$Svg$Attributes$y2(
-                                                $elm$core$String$fromFloat(config.f9)),
-                                            $elm$svg$Svg$Attributes$stroke(config.bC),
+                                                $elm$core$String$fromFloat(config.ga)),
+                                            $elm$svg$Svg$Attributes$stroke(config.bE),
                                             $elm$svg$Svg$Attributes$strokeWidth(
-                                                $elm$core$String$fromFloat(config.fi))
+                                                $elm$core$String$fromFloat(config.fj))
                                         ]),
                                     _List_Nil)),
                             theId);
                     case 1:
                         var edits = design.a;
                         var config = A2(
                             $terezka$elm_charts$Internal$Svg$apply,
                             edits, {
-                                bC: defaultColor,
+                                bE: defaultColor,
                                 o: 45,
-                                f9: 4,
-                                fi: 3
+                                ga: 4,
+                                fj: 3
                             });
                         var theId = toPatternId(
                             _List_fromArray(
                                 [
-                                    config.bC,
-                                    $elm$core$String$fromFloat(config.fi),
-                                    $elm$core$String$fromFloat(config.f9),
+                                    config.bE,
+                                    $elm$core$String$fromFloat(config.fj),
+                                    $elm$core$String$fromFloat(config.ga),
                                     $elm$core$String$fromFloat(config.o)
                                 ]));
                         return _Utils_Tuple2(
                             A4(
                                 toPatternDefs,
                                 theId,
-                                config.f9,
+                                config.ga,
                                 config.o,
                                 A2(
                                     $elm$svg$Svg$circle,
                                     _List_fromArray(
                                         [
-                                            $elm$svg$Svg$Attributes$fill(config.bC),
+                                            $elm$svg$Svg$Attributes$fill(config.bE),
                                             $elm$svg$Svg$Attributes$cx(
-                                                $elm$core$String$fromFloat(config.fi / 3)),
+                                                $elm$core$String$fromFloat(config.fj / 3)),
                                             $elm$svg$Svg$Attributes$cy(
-                                                $elm$core$String$fromFloat(config.fi / 3)),
+                                                $elm$core$String$fromFloat(config.fj / 3)),
                                             $elm$svg$Svg$Attributes$r(
-                                                $elm$core$String$fromFloat(config.fi / 3))
+                                                $elm$core$String$fromFloat(config.fj / 3))
                                         ]),
                                     _List_Nil)),
                             theId);
                     default:
                         var edits = design.a;
                         var colors = _Utils_eq(edits, _List_Nil) ? _List_fromArray(
                             [defaultColor, 'white']) : edits;
@@ -11224,15 +11332,15 @@
         });
     var $terezka$elm_charts$Internal$Svg$bar = F3(
         function(plane, config, point) {
             var viewBar = F6(
                 function(fill, fillOpacity, border, borderWidth, strokeOpacity, cmds) {
                     return A4(
                         $terezka$elm_charts$Internal$Svg$withAttrs,
-                        config.bu,
+                        config.bw,
                         $elm$svg$Svg$path,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__bar'),
                                 $elm$svg$Svg$Attributes$fill(fill),
                                 $elm$svg$Svg$Attributes$fillOpacity(
                                     $elm$core$String$fromFloat(fillOpacity)),
@@ -11243,185 +11351,185 @@
                                     $elm$core$String$fromFloat(strokeOpacity)),
                                 $elm$svg$Svg$Attributes$d(
                                     A2($terezka$elm_charts$Internal$Commands$description, plane, cmds)),
                                 $terezka$elm_charts$Internal$Svg$withinChartArea(plane)
                             ]),
                         _List_Nil);
                 });
-            var highlightColor = (config.fL === '') ? config.bC : config.fL;
+            var highlightColor = (config.fM === '') ? config.bE : config.fM;
             var borderWidthCarY = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, config.x / 2);
-            var highlightWidthCarY = borderWidthCarY + A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, config.fM / 2);
+            var highlightWidthCarY = borderWidthCarY + A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, config.fN / 2);
             var borderWidthCarX = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, config.x / 2);
-            var highlightWidthCarX = borderWidthCarX + A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, config.fM / 2);
+            var highlightWidthCarX = borderWidthCarX + A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, config.fN / 2);
             var pos = {
-                aK: A2($elm$core$Basics$min, point.aK, point.be) + borderWidthCarX,
-                be: A2($elm$core$Basics$max, point.aK, point.be) - borderWidthCarX,
-                gA: A2($elm$core$Basics$min, point.gA, point.dI) + borderWidthCarY,
-                dI: A2($elm$core$Basics$max, point.gA, point.dI) - borderWidthCarY
+                aM: A2($elm$core$Basics$min, point.aM, point.bg) + borderWidthCarX,
+                bg: A2($elm$core$Basics$max, point.aM, point.bg) - borderWidthCarX,
+                gB: A2($elm$core$Basics$min, point.gB, point.dK) + borderWidthCarY,
+                dK: A2($elm$core$Basics$max, point.gB, point.dK) - borderWidthCarY
             };
-            var height = $elm$core$Basics$abs(pos.dI - pos.gA);
+            var height = $elm$core$Basics$abs(pos.dK - pos.gB);
             var highlightPos = {
-                aK: pos.aK - highlightWidthCarX,
-                be: pos.be + highlightWidthCarX,
-                gA: pos.gA - highlightWidthCarY,
-                dI: pos.dI + highlightWidthCarY
+                aM: pos.aM - highlightWidthCarX,
+                bg: pos.bg + highlightWidthCarX,
+                gB: pos.gB - highlightWidthCarY,
+                dK: pos.dK + highlightWidthCarY
             };
-            var width = $elm$core$Basics$abs(pos.be - pos.aK);
-            var roundingBottom = (A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, width) * 0.5) * A3($elm$core$Basics$clamp, 0, 1, config.f6);
+            var width = $elm$core$Basics$abs(pos.bg - pos.aM);
+            var roundingBottom = (A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, width) * 0.5) * A3($elm$core$Basics$clamp, 0, 1, config.f7);
             var radiusBottomX = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, roundingBottom);
             var radiusBottomY = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, roundingBottom);
-            var roundingTop = (A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, width) * 0.5) * A3($elm$core$Basics$clamp, 0, 1, config.f7);
+            var roundingTop = (A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, width) * 0.5) * A3($elm$core$Basics$clamp, 0, 1, config.f8);
             var radiusTopX = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, roundingTop);
             var radiusTopY = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, roundingTop);
-            var _v0 = ((((height - (radiusTopY * 0.8)) - (radiusBottomY * 0.8)) <= 0) || (((width - (radiusTopX * 0.8)) - (radiusBottomX * 0.8)) <= 0)) ? _Utils_Tuple2(0, 0) : _Utils_Tuple2(config.f7, config.f6);
+            var _v0 = ((((height - (radiusTopY * 0.8)) - (radiusBottomY * 0.8)) <= 0) || (((width - (radiusTopX * 0.8)) - (radiusBottomX * 0.8)) <= 0)) ? _Utils_Tuple2(0, 0) : _Utils_Tuple2(config.f8, config.f7);
             var roundTop = _v0.a;
             var roundBottom = _v0.b;
             var _v1 = function() {
-                if (_Utils_eq(pos.gA, pos.dI)) {
+                if (_Utils_eq(pos.gB, pos.dK)) {
                     return _Utils_Tuple2(_List_Nil, _List_Nil);
                 } else {
                     var _v2 = _Utils_Tuple2(roundTop > 0, roundBottom > 0);
                     if (!_v2.a) {
                         if (!_v2.b) {
                             return _Utils_Tuple2(
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aK, pos.gA),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.gA),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gA)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aM, pos.gB),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aM, pos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg, pos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg, pos.gB),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aM, pos.gB)
                                     ]),
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aK, pos.gA),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK, highlightPos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.be, highlightPos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.be, pos.gA),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.gA),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gA)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aM, pos.gB),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aM, highlightPos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bg, highlightPos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bg, pos.gB),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg, pos.gB),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg, pos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aM, pos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aM, pos.gB)
                                     ]));
                         } else {
                             return _Utils_Tuple2(
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aK + radiusBottomX, pos.gA),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.aK, pos.gA + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.gA + radiusBottomY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.be - radiusBottomX, pos.gA),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK + radiusBottomX, pos.gA)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aM + radiusBottomX, pos.gB),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.aM, pos.gB + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aM, pos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg, pos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg, pos.gB + radiusBottomY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.bg - radiusBottomX, pos.gB),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aM + radiusBottomX, pos.gB)
                                     ]),
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aK + radiusBottomX, highlightPos.gA),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.aK, highlightPos.gA + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK, highlightPos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.be, highlightPos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.be, highlightPos.gA + radiusBottomY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.be - radiusBottomX, highlightPos.gA),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK + radiusBottomX, highlightPos.gA),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be - radiusBottomX, pos.gA),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, false, pos.be, pos.gA + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gA + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.gA)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aM + radiusBottomX, highlightPos.gB),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.aM, highlightPos.gB + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aM, highlightPos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bg, highlightPos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bg, highlightPos.gB + radiusBottomY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.bg - radiusBottomX, highlightPos.gB),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aM + radiusBottomX, highlightPos.gB),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg - radiusBottomX, pos.gB),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, false, pos.bg, pos.gB + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg, pos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aM, pos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aM, pos.gB + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg, pos.gB)
                                     ]));
                         }
                     } else {
                         if (!_v2.b) {
                             return _Utils_Tuple2(
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aK, pos.gA),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dI - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.aK + radiusTopX, pos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be - radiusTopX, pos.dI),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.be, pos.dI - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.gA),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gA)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aM, pos.gB),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aM, pos.dK - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.aM + radiusTopX, pos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg - radiusTopX, pos.dK),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.bg, pos.dK - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg, pos.gB),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aM, pos.gB)
                                     ]),
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aK, pos.gA),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK, highlightPos.dI - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.aK + radiusTopX, highlightPos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.be - radiusTopX, highlightPos.dI),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.be, highlightPos.dI - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.be, pos.gA),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.gA),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.dI - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.be - radiusTopX, pos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK + radiusTopX, pos.dI),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.aK, pos.dI - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gA)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aM, pos.gB),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aM, highlightPos.dK - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.aM + radiusTopX, highlightPos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bg - radiusTopX, highlightPos.dK),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.bg, highlightPos.dK - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bg, pos.gB),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg, pos.gB),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg, pos.dK - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.bg - radiusTopX, pos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aM + radiusTopX, pos.dK),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.aM, pos.dK - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aM, pos.gB)
                                     ]));
                         } else {
                             return _Utils_Tuple2(
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aK + radiusBottomX, pos.gA),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.aK, pos.gA + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dI - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.aK + radiusTopX, pos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be - radiusTopX, pos.dI),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.be, pos.dI - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.gA + radiusBottomY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.be - radiusBottomX, pos.gA),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK + radiusBottomX, pos.gA)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aM + radiusBottomX, pos.gB),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.aM, pos.gB + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aM, pos.dK - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.aM + radiusTopX, pos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg - radiusTopX, pos.dK),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.bg, pos.dK - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg, pos.gB + radiusBottomY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.bg - radiusBottomX, pos.gB),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aM + radiusBottomX, pos.gB)
                                     ]),
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aK + radiusBottomX, highlightPos.gA),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.aK, highlightPos.gA + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK, highlightPos.dI - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.aK + radiusTopX, highlightPos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.be - radiusTopX, highlightPos.dI),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.be, highlightPos.dI - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.be, highlightPos.gA + radiusBottomY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.be - radiusBottomX, highlightPos.gA),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK + radiusBottomX, highlightPos.gA),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be - radiusBottomX, pos.gA),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, false, pos.be, pos.gA + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.dI - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.be - radiusTopX, pos.dI),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK + radiusTopX, pos.dI),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.aK, pos.dI - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gA + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.gA)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aM + radiusBottomX, highlightPos.gB),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.aM, highlightPos.gB + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aM, highlightPos.dK - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.aM + radiusTopX, highlightPos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bg - radiusTopX, highlightPos.dK),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.bg, highlightPos.dK - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bg, highlightPos.gB + radiusBottomY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.bg - radiusBottomX, highlightPos.gB),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aM + radiusBottomX, highlightPos.gB),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg - radiusBottomX, pos.gB),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, false, pos.bg, pos.gB + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg, pos.dK - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.bg - radiusTopX, pos.dK),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aM + radiusTopX, pos.dK),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.aM, pos.dK - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aM, pos.gB + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bg, pos.gB)
                                     ]));
                         }
                     }
                 }
             }();
             var commands = _v1.a;
             var highlightCommands = _v1.b;
             var viewAuraBar = function(fill) {
-                return (!config.fK) ? A6(viewBar, fill, config.Q, config.v, config.x, 1, commands) : A2(
+                return (!config.fL) ? A6(viewBar, fill, config.Q, config.v, config.x, 1, commands) : A2(
                     $elm$svg$Svg$g,
                     _List_fromArray(
                         [
                             $elm$svg$Svg$Attributes$class('elm-charts__bar-with-highlight')
                         ]),
                     _List_fromArray(
                         [
-                            A6(viewBar, highlightColor, config.fK, 'transparent', 0, 0, highlightCommands),
+                            A6(viewBar, highlightColor, config.fL, 'transparent', 0, 0, highlightCommands),
                             A6(viewBar, fill, config.Q, config.v, config.x, 1, commands)
                         ]));
             };
-            var _v3 = config.cW;
+            var _v3 = config.cX;
             if (_v3.$ === 1) {
-                return viewAuraBar(config.bC);
+                return viewAuraBar(config.bE);
             } else {
                 var design = _v3.a;
-                var _v4 = A2($terezka$elm_charts$Internal$Svg$toPattern, config.bC, design);
+                var _v4 = A2($terezka$elm_charts$Internal$Svg$toPattern, config.bE, design);
                 var patternDefs = _v4.a;
                 var fill = _v4.b;
                 return A2(
                     $elm$svg$Svg$g,
                     _List_fromArray(
                         [
                             $elm$svg$Svg$Attributes$class('elm-charts__bar-with-pattern')
@@ -11430,21 +11538,21 @@
                         [
                             patternDefs,
                             viewAuraBar(fill)
                         ]));
             }
         });
     var $terezka$elm_charts$Internal$Svg$defaultContainer = {
-        bu: _List_fromArray(
+        bw: _List_fromArray(
             [
                 $elm$svg$Svg$Attributes$style('overflow: visible;')
             ]),
-        bL: _List_Nil,
-        bX: _List_Nil,
-        cw: true
+        bN: _List_Nil,
+        bZ: _List_Nil,
+        cy: true
     };
     var $terezka$elm_charts$Internal$Svg$barLegend = F2(
         function(config, barConfig) {
             var fontStyle = function() {
                 var _v0 = config.k;
                 if (!_v0.$) {
                     var size_ = _v0.a;
@@ -11453,118 +11561,118 @@
                         'font-size',
                         $elm$core$String$fromInt(size_) + 'px');
                 } else {
                     return A2($elm$html$Html$Attributes$style, '', '');
                 }
             }();
             var fakePlane = {
-                fj: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.fi, 0, 0, 0, 10, 0, 10),
-                fk: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.ea, 0, 0, 0, 10, 0, 10)
+                fk: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.fj, 0, 0, 0, 10, 0, 10),
+                fl: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.eb, 0, 0, 0, 10, 0, 10)
             };
             return A2(
                 $elm$html$Html$div,
                 _Utils_ap(
                     _List_fromArray(
                         [
                             $elm$html$Html$Attributes$class('elm-charts__legend'),
                             A2($elm$html$Html$Attributes$style, 'display', 'flex'),
                             A2($elm$html$Html$Attributes$style, 'align-items', 'center')
                         ]),
-                    config.bX),
+                    config.bZ),
                 _List_fromArray(
                     [
                         A5(
                             $terezka$elm_charts$Internal$Svg$container,
                             fakePlane,
                             _Utils_update(
                                 $terezka$elm_charts$Internal$Svg$defaultContainer, {
-                                    cw: false
+                                    cy: false
                                 }),
                             _List_Nil,
                             _List_fromArray(
                                 [
                                     A3(
                                         $terezka$elm_charts$Internal$Svg$bar,
                                         fakePlane,
                                         barConfig, {
-                                            aK: 0,
-                                            be: 10,
-                                            gA: 0,
-                                            dI: 10
+                                            aM: 0,
+                                            bg: 10,
+                                            gB: 0,
+                                            dK: 10
                                         })
                                 ]),
                             _List_Nil),
                         A2(
                             $elm$html$Html$div,
                             _List_fromArray(
                                 [
                                     fontStyle,
                                     A2(
                                         $elm$html$Html$Attributes$style,
                                         'margin-left',
-                                        $elm$core$String$fromFloat(config.f9) + 'px')
+                                        $elm$core$String$fromFloat(config.ga) + 'px')
                                 ]),
                             _List_fromArray(
                                 [
-                                    $elm$html$Html$text(config.gi)
+                                    $elm$html$Html$text(config.gj)
                                 ]))
                     ]));
         });
     var $terezka$elm_charts$Internal$Svg$defaultBar = {
-        bu: _List_Nil,
+        bw: _List_Nil,
         v: 'white',
         x: 0,
-        bC: $terezka$elm_charts$Internal$Helpers$pink,
-        cW: $elm$core$Maybe$Nothing,
-        fK: 0,
-        fL: '',
-        fM: 10,
+        bE: $terezka$elm_charts$Internal$Helpers$pink,
+        cX: $elm$core$Maybe$Nothing,
+        fL: 0,
+        fM: '',
+        fN: 10,
         Q: 1,
-        f6: 0,
-        f7: 0
+        f7: 0,
+        f8: 0
     };
     var $terezka$elm_charts$Internal$Svg$defaultBarLegend = {
-        bC: '#808BAB',
+        bE: '#808BAB',
         k: $elm$core$Maybe$Nothing,
-        ea: 10,
-        bX: _List_Nil,
-        f9: 10,
-        gi: '',
-        fi: 10,
+        eb: 10,
+        bZ: _List_Nil,
+        ga: 10,
+        gj: '',
+        fj: 10,
         g: 0,
         h: 0
     };
     var $terezka$elm_charts$Chart$Svg$barLegend = F2(
         function(edits, barAttrs) {
             return A2(
                 $terezka$elm_charts$Internal$Svg$barLegend,
                 A2($terezka$elm_charts$Internal$Helpers$apply, edits, $terezka$elm_charts$Internal$Svg$defaultBarLegend),
                 A2($terezka$elm_charts$Internal$Helpers$apply, barAttrs, $terezka$elm_charts$Internal$Svg$defaultBar));
         });
     var $terezka$elm_charts$Internal$Svg$Row = 0;
     var $terezka$elm_charts$Internal$Svg$defaultLegends = {
-        dM: 0,
+        dO: 0,
         i: $elm$core$Maybe$Nothing,
-        fq: '',
+        fr: '',
         v: '',
         x: 0,
-        bX: _List_Nil,
-        f9: 10,
+        bZ: _List_Nil,
+        ga: 10,
         g: 0,
         h: 0
     };
     var $elm$virtual_dom$VirtualDom$node = function(tag) {
         return _VirtualDom_node(
             _VirtualDom_noScript(tag));
     };
     var $elm$html$Html$node = $elm$virtual_dom$VirtualDom$node;
     var $terezka$elm_charts$Internal$Svg$positionHtml = F7(
         function(plane, x, y, xOff, yOff, attrs, content) {
-            var yPercentage = ((A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, y) - yOff) * 100) / plane.fk.O;
-            var xPercentage = ((A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, x) + xOff) * 100) / plane.fj.O;
+            var yPercentage = ((A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, y) - yOff) * 100) / plane.fl.O;
+            var xPercentage = ((A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, x) + xOff) * 100) / plane.fk.O;
             var posititonStyles = _List_fromArray(
                 [
                     A2(
                         $elm$html$Html$Attributes$style,
                         'left',
                         $elm$core$String$fromFloat(xPercentage) + '%'),
                     A2(
@@ -11580,15 +11688,15 @@
                 content);
         });
     var $terezka$elm_charts$Internal$Svg$legendsAt = F5(
         function(plane, x, y, config, children) {
             var otherAttrs = _List_fromArray(
                 [
                     $elm$html$Html$Attributes$class('elm-charts__legends'),
-                    A2($elm$html$Html$Attributes$style, 'background', config.fq),
+                    A2($elm$html$Html$Attributes$style, 'background', config.fr),
                     A2($elm$html$Html$Attributes$style, 'border-color', config.v),
                     A2(
                         $elm$html$Html$Attributes$style,
                         'border-width',
                         $elm$core$String$fromFloat(config.x) + 'px'),
                     A2($elm$html$Html$Attributes$style, 'border-style', 'solid')
                 ]);
@@ -11619,15 +11727,15 @@
                                 [
                                     A2($elm$html$Html$Attributes$style, 'transform', 'translate(-50%, 0%)')
                                 ]);
                     }
                 }
             }();
             var _v0 = function() {
-                var _v1 = config.dM;
+                var _v1 = config.dO;
                 if (!_v1) {
                     return _Utils_Tuple2(
                         _List_fromArray(
                             [
                                 A2($elm$html$Html$Attributes$style, 'display', 'flex'),
                                 A2($elm$html$Html$Attributes$style, 'align-items', 'center')
                             ]),
@@ -11641,27 +11749,27 @@
                                 A2($elm$html$Html$Attributes$style, 'align-items', 'baseline')
                             ]),
                         'bottom');
                 }
             }();
             var alignmentAttrs = _v0.a;
             var direction = _v0.b;
-            var paddingStyle = ' .elm-charts__legends .elm-charts__legend {\n              margin-' + (direction + (':' + ($elm$core$String$fromFloat(config.f9) + ('px;\n            }\n\n            .elm-charts__legends .elm-charts__legend:last-child {\n              margin-' + (direction + ': 0px;\n            }\n        ')))));
+            var paddingStyle = ' .elm-charts__legends .elm-charts__legend {\n              margin-' + (direction + (':' + ($elm$core$String$fromFloat(config.ga) + ('px;\n            }\n\n            .elm-charts__legends .elm-charts__legend:last-child {\n              margin-' + (direction + ': 0px;\n            }\n        ')))));
             return A7(
                 $terezka$elm_charts$Internal$Svg$positionHtml,
                 plane,
                 x,
                 y,
                 config.g,
                 -config.h,
                 _Utils_ap(
                     anchorAttrs,
                     _Utils_ap(
                         alignmentAttrs,
-                        _Utils_ap(otherAttrs, config.bX))),
+                        _Utils_ap(otherAttrs, config.bZ))),
                 A2(
                     $elm$core$List$cons,
                     A3(
                         $elm$html$Html$node,
                         'style',
                         _List_Nil,
                         _List_fromArray(
@@ -11676,84 +11784,84 @@
                 $terezka$elm_charts$Internal$Svg$legendsAt,
                 plane,
                 x,
                 y,
                 A2($terezka$elm_charts$Internal$Helpers$apply, edits, $terezka$elm_charts$Internal$Svg$defaultLegends));
         });
     var $terezka$elm_charts$Internal$Svg$defaultInterpolation = {
-        bu: _List_Nil,
-        bC: $terezka$elm_charts$Internal$Helpers$pink,
-        bF: _List_Nil,
-        cW: $elm$core$Maybe$Nothing,
-        fX: $elm$core$Maybe$Nothing,
+        bw: _List_Nil,
+        bE: $terezka$elm_charts$Internal$Helpers$pink,
+        bH: _List_Nil,
+        cX: $elm$core$Maybe$Nothing,
+        fY: $elm$core$Maybe$Nothing,
         Q: 0,
-        fi: 1
+        fj: 1
     };
     var $terezka$elm_charts$Internal$Svg$defaultLineLegend = {
-        bC: '#808BAB',
+        bE: '#808BAB',
         k: $elm$core$Maybe$Nothing,
-        ea: 16,
-        bX: _List_Nil,
-        f9: 10,
-        gi: '',
-        fi: 30,
+        eb: 16,
+        bZ: _List_Nil,
+        ga: 10,
+        gj: '',
+        fj: 30,
         g: 0,
         h: 0
     };
     var $terezka$elm_charts$Internal$Svg$Point = F2(
         function(x, y) {
             return {
-                fj: x,
-                fk: y
+                fk: x,
+                fl: y
             };
         });
     var $elm$svg$Svg$Attributes$fillRule = _VirtualDom_attribute('fill-rule');
     var $terezka$elm_charts$Internal$Interpolation$linear = $elm$core$List$map(
         $elm$core$List$map(
             function(_v0) {
-                var x = _v0.fj;
-                var y = _v0.fk;
+                var x = _v0.fk;
+                var y = _v0.fl;
                 return A2($terezka$elm_charts$Internal$Commands$Line, x, y);
             }));
     var $terezka$elm_charts$Internal$Interpolation$First = {
         $: 0
     };
     var $terezka$elm_charts$Internal$Interpolation$Previous = function(a) {
         return {
             $: 1,
             a: a
         };
     };
     var $terezka$elm_charts$Internal$Interpolation$monotoneCurve = F4(
         function(point0, point1, tangent0, tangent1) {
-            var dx = (point1.fj - point0.fj) / 3;
-            return A6($terezka$elm_charts$Internal$Commands$CubicBeziers, point0.fj + dx, point0.fk + (dx * tangent0), point1.fj - dx, point1.fk - (dx * tangent1), point1.fj, point1.fk);
+            var dx = (point1.fk - point0.fk) / 3;
+            return A6($terezka$elm_charts$Internal$Commands$CubicBeziers, point0.fk + dx, point0.fl + (dx * tangent0), point1.fk - dx, point1.fl - (dx * tangent1), point1.fk, point1.fl);
         });
     var $elm$core$Basics$neq = _Utils_notEqual;
     var $terezka$elm_charts$Internal$Interpolation$slope2 = F3(
         function(point0, point1, t) {
-            var h = point1.fj - point0.fj;
-            return (!(!h)) ? ((((3 * (point1.fk - point0.fk)) / h) - t) / 2) : t;
+            var h = point1.fk - point0.fk;
+            return (!(!h)) ? ((((3 * (point1.fl - point0.fl)) / h) - t) / 2) : t;
         });
     var $elm$core$Basics$isNaN = _Basics_isNaN;
     var $terezka$elm_charts$Internal$Interpolation$sign = function(x) {
         return (x < 0) ? (-1) : 1;
     };
     var $terezka$elm_charts$Internal$Interpolation$toH = F2(
         function(h0, h1) {
             return (!h0) ? ((h1 < 0) ? (0 * (-1)) : h1) : h0;
         });
     var $terezka$elm_charts$Internal$Interpolation$slope3 = F3(
         function(point0, point1, point2) {
-            var h1 = point2.fj - point1.fj;
-            var h0 = point1.fj - point0.fj;
+            var h1 = point2.fk - point1.fk;
+            var h0 = point1.fk - point0.fk;
             var s0h = A2($terezka$elm_charts$Internal$Interpolation$toH, h0, h1);
-            var s0 = (point1.fk - point0.fk) / s0h;
+            var s0 = (point1.fl - point0.fl) / s0h;
             var s1h = A2($terezka$elm_charts$Internal$Interpolation$toH, h1, h0);
-            var s1 = (point2.fk - point1.fk) / s1h;
+            var s1 = (point2.fl - point1.fl) / s1h;
             var p = ((s0 * h1) + (s1 * h0)) / (h0 + h1);
             var slope = ($terezka$elm_charts$Internal$Interpolation$sign(s0) + $terezka$elm_charts$Internal$Interpolation$sign(s1)) * A2(
                 $elm$core$Basics$min,
                 A2(
                     $elm$core$Basics$min,
                     $elm$core$Basics$abs(s0),
                     $elm$core$Basics$abs(s1)),
@@ -11804,15 +11912,15 @@
                                 return _Utils_Tuple2(
                                     $terezka$elm_charts$Internal$Interpolation$Previous(t1),
                                     _Utils_ap(
                                         commands,
                                         _List_fromArray(
                                             [
                                                 A4($terezka$elm_charts$Internal$Interpolation$monotoneCurve, p0, p1, t1, t1),
-                                                A2($terezka$elm_charts$Internal$Commands$Line, p1.fj, p1.fk)
+                                                A2($terezka$elm_charts$Internal$Commands$Line, p1.fk, p1.fl)
                                             ])));
                             }
                         } else {
                             break _v1$4;
                         }
                     } else {
                         if (_v1.b.b && _v1.b.b.b) {
@@ -11850,15 +11958,15 @@
                                 return _Utils_Tuple2(
                                     $terezka$elm_charts$Internal$Interpolation$Previous(t1),
                                     _Utils_ap(
                                         commands,
                                         _List_fromArray(
                                             [
                                                 A4($terezka$elm_charts$Internal$Interpolation$monotoneCurve, p0, p1, t0, t1),
-                                                A2($terezka$elm_charts$Internal$Commands$Line, p1.fj, p1.fk)
+                                                A2($terezka$elm_charts$Internal$Commands$Line, p1.fk, p1.fl)
                                             ])));
                             }
                         } else {
                             break _v1$4;
                         }
                     }
                 }
@@ -11875,15 +11983,15 @@
                     return A2(
                         $terezka$elm_charts$Internal$Interpolation$monotonePart,
                         A2($elm$core$List$cons, p0, rest),
                         _Utils_Tuple2(
                             tangent,
                             _List_fromArray(
                                 [
-                                    A2($terezka$elm_charts$Internal$Commands$Line, p0.fj, p0.fk)
+                                    A2($terezka$elm_charts$Internal$Commands$Line, p0.fk, p0.fl)
                                 ])));
                 } else {
                     return _Utils_Tuple2(tangent, _List_Nil);
                 }
             }();
             var t0 = _v1.a;
             var commands = _v1.b;
@@ -11901,24 +12009,24 @@
             $terezka$elm_charts$Internal$Interpolation$monotoneSection,
             _Utils_Tuple2($terezka$elm_charts$Internal$Interpolation$First, _List_Nil),
             sections).b;
     };
     var $terezka$elm_charts$Internal$Interpolation$Point = F2(
         function(x, y) {
             return {
-                fj: x,
-                fk: y
+                fk: x,
+                fl: y
             };
         });
     var $terezka$elm_charts$Internal$Interpolation$after = F2(
         function(a, b) {
             return _List_fromArray(
                 [
                     a,
-                    A2($terezka$elm_charts$Internal$Interpolation$Point, b.fj, a.fk),
+                    A2($terezka$elm_charts$Internal$Interpolation$Point, b.fk, a.fl),
                     b
                 ]);
         });
     var $terezka$elm_charts$Internal$Interpolation$stepped = function(sections) {
         var expand = F2(
             function(result, section) {
                 expand: while (true) {
@@ -11947,16 +12055,16 @@
         return A2(
             $elm$core$List$map,
             A2(
                 $elm$core$Basics$composeR,
                 expand(_List_Nil),
                 $elm$core$List$map(
                     function(_v2) {
-                        var x = _v2.fj;
-                        var y = _v2.fk;
+                        var x = _v2.fk;
+                        var y = _v2.fl;
                         return A2($terezka$elm_charts$Internal$Commands$Line, x, y);
                     })),
             sections);
     };
     var $elm$core$List$drop = F2(
         function(n, list) {
             drop: while (true) {
@@ -12023,25 +12131,25 @@
                             var rest = acc.b;
                             return A2(
                                 $elm$core$List$cons,
                                 _Utils_ap(
                                     latest,
                                     _List_fromArray(
                                         [{
-                                            fj: toX(datum_),
-                                            fk: y_
+                                            fk: toX(datum_),
+                                            fl: y_
                                         }])),
                                 rest);
                         } else {
                             return A2(
                                 $elm$core$List$cons,
                                 _List_fromArray(
                                     [{
-                                        fj: toX(datum_),
-                                        fk: y_
+                                        fk: toX(datum_),
+                                        fl: y_
                                     }]),
                                 acc);
                         }
                     } else {
                         return A2($elm$core$List$cons, _List_Nil, acc);
                     }
                 });
@@ -12061,30 +12169,30 @@
                 $elm$core$List$filterMap,
                 $elm$core$Basics$identity,
                 A3($elm$core$List$map2, toSets, points, commands));
         });
     var $terezka$elm_charts$Internal$Svg$area = F6(
         function(plane, toX, toY2M, toY, config, data) {
             var _v0 = function() {
-                var _v1 = config.cW;
+                var _v1 = config.cX;
                 if (_v1.$ === 1) {
                     return _Utils_Tuple2(
                         $elm$svg$Svg$text(''),
-                        config.bC);
+                        config.bE);
                 } else {
                     var design = _v1.a;
-                    return A2($terezka$elm_charts$Internal$Svg$toPattern, config.bC, design);
+                    return A2($terezka$elm_charts$Internal$Svg$toPattern, config.bE, design);
                 }
             }();
             var patternDefs = _v0.a;
             var fill = _v0.b;
             var view = function(cmds) {
                 return A4(
                     $terezka$elm_charts$Internal$Svg$withAttrs,
-                    config.bu,
+                    config.bw,
                     $elm$svg$Svg$path,
                     _List_fromArray(
                         [
                             $elm$svg$Svg$Attributes$class('elm-charts__area-section'),
                             $elm$svg$Svg$Attributes$fill(fill),
                             $elm$svg$Svg$Attributes$fillOpacity(
                                 $elm$core$String$fromFloat(config.Q)),
@@ -12104,53 +12212,53 @@
                     var firstTop = _v6.a;
                     var cmdsTop = _v6.b;
                     var endTop = _v6.c;
                     return view(
                         _Utils_ap(
                             _List_fromArray(
                                 [
-                                    A2($terezka$elm_charts$Internal$Commands$Move, firstBottom.fj, firstBottom.fk),
-                                    A2($terezka$elm_charts$Internal$Commands$Line, firstTop.fj, firstTop.fk)
+                                    A2($terezka$elm_charts$Internal$Commands$Move, firstBottom.fk, firstBottom.fl),
+                                    A2($terezka$elm_charts$Internal$Commands$Line, firstTop.fk, firstTop.fl)
                                 ]),
                             _Utils_ap(
                                 cmdsTop,
                                 _Utils_ap(
                                     _List_fromArray(
                                         [
-                                            A2($terezka$elm_charts$Internal$Commands$Move, firstBottom.fj, firstBottom.fk)
+                                            A2($terezka$elm_charts$Internal$Commands$Move, firstBottom.fk, firstBottom.fl)
                                         ]),
                                     _Utils_ap(
                                         cmdsBottom,
                                         _List_fromArray(
                                             [
-                                                A2($terezka$elm_charts$Internal$Commands$Line, endTop.fj, endTop.fk)
+                                                A2($terezka$elm_charts$Internal$Commands$Line, endTop.fk, endTop.fl)
                                             ]))))));
                 });
             var withoutUnder = function(_v4) {
                 var first = _v4.a;
                 var cmds = _v4.b;
                 var end = _v4.c;
                 return view(
                     _Utils_ap(
                         _List_fromArray(
                             [
-                                A2($terezka$elm_charts$Internal$Commands$Move, first.fj, 0),
-                                A2($terezka$elm_charts$Internal$Commands$Line, first.fj, first.fk)
+                                A2($terezka$elm_charts$Internal$Commands$Move, first.fk, 0),
+                                A2($terezka$elm_charts$Internal$Commands$Line, first.fk, first.fl)
                             ]),
                         _Utils_ap(
                             cmds,
                             _List_fromArray(
                                 [
-                                    A2($terezka$elm_charts$Internal$Commands$Line, end.fj, 0)
+                                    A2($terezka$elm_charts$Internal$Commands$Line, end.fk, 0)
                                 ]))));
             };
             if (config.Q <= 0) {
                 return $elm$svg$Svg$text('');
             } else {
-                var _v2 = config.fX;
+                var _v2 = config.fY;
                 if (_v2.$ === 1) {
                     return $elm$svg$Svg$text('');
                 } else {
                     var method = _v2.a;
                     return A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
@@ -12184,41 +12292,41 @@
     var $terezka$elm_charts$Internal$Svg$interpolation = F5(
         function(plane, toX, toY, config, data) {
             var view = function(_v1) {
                 var first = _v1.a;
                 var cmds = _v1.b;
                 return A4(
                     $terezka$elm_charts$Internal$Svg$withAttrs,
-                    config.bu,
+                    config.bw,
                     $elm$svg$Svg$path,
                     _List_fromArray(
                         [
                             $elm$svg$Svg$Attributes$class('elm-charts__interpolation-section'),
                             $elm$svg$Svg$Attributes$fill('transparent'),
-                            $elm$svg$Svg$Attributes$stroke(config.bC),
+                            $elm$svg$Svg$Attributes$stroke(config.bE),
                             $elm$svg$Svg$Attributes$strokeDasharray(
                                 A2(
                                     $elm$core$String$join,
                                     ' ',
-                                    A2($elm$core$List$map, $elm$core$String$fromFloat, config.bF))),
+                                    A2($elm$core$List$map, $elm$core$String$fromFloat, config.bH))),
                             $elm$svg$Svg$Attributes$strokeWidth(
-                                $elm$core$String$fromFloat(config.fi)),
+                                $elm$core$String$fromFloat(config.fj)),
                             $elm$svg$Svg$Attributes$d(
                                 A2(
                                     $terezka$elm_charts$Internal$Commands$description,
                                     plane,
                                     A2(
                                         $elm$core$List$cons,
-                                        A2($terezka$elm_charts$Internal$Commands$Move, first.fj, first.fk),
+                                        A2($terezka$elm_charts$Internal$Commands$Move, first.fk, first.fl),
                                         cmds))),
                             $terezka$elm_charts$Internal$Svg$withinChartArea(plane)
                         ]),
                     _List_Nil);
             };
-            var _v0 = config.fX;
+            var _v0 = config.fY;
             if (_v0.$ === 1) {
                 return $elm$svg$Svg$text('');
             } else {
                 var method = _v0.a;
                 return A2(
                     $elm$svg$Svg$g,
                     _List_fromArray(
@@ -12253,15 +12361,15 @@
         });
     var $terezka$elm_charts$Internal$Svg$lineLegend = F3(
         function(config, interConfig, dotConfig) {
             var topMargin = function() {
                 var _v1 = dotConfig.aG;
                 if (!_v1.$) {
                     var shape = _v1.a;
-                    return A2($terezka$elm_charts$Internal$Svg$toRadius, dotConfig.e1, shape);
+                    return A2($terezka$elm_charts$Internal$Svg$toRadius, dotConfig.e2, shape);
                 } else {
                     return 0;
                 }
             }();
             var fontStyle = function() {
                 var _v0 = config.k;
                 if (!_v0.$) {
@@ -12271,103 +12379,103 @@
                         'font-size',
                         $elm$core$String$fromInt(size_) + 'px');
                 } else {
                     return A2($elm$html$Html$Attributes$style, '', '');
                 }
             }();
             var fakePlane = {
-                fj: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.fi, 0, 0, 0, 10, 0, 10),
-                fk: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.ea, 0, 0, 0, 10, 0, 10)
+                fk: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.fj, 0, 0, 0, 10, 0, 10),
+                fl: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.eb, 0, 0, 0, 10, 0, 10)
             };
             var bottomMargin = (!interConfig.Q) ? topMargin : 0;
             return A2(
                 $elm$html$Html$div,
                 _Utils_ap(
                     _List_fromArray(
                         [
                             $elm$html$Html$Attributes$class('elm-charts__legend'),
                             A2($elm$html$Html$Attributes$style, 'display', 'flex'),
                             A2($elm$html$Html$Attributes$style, 'align-items', 'center')
                         ]),
-                    config.bX),
+                    config.bZ),
                 _List_fromArray(
                     [
                         A5(
                             $terezka$elm_charts$Internal$Svg$container,
                             fakePlane,
                             _Utils_update(
                                 $terezka$elm_charts$Internal$Svg$defaultContainer, {
-                                    cw: false
+                                    cy: false
                                 }),
                             _List_Nil,
                             _List_fromArray(
                                 [
                                     A5(
                                         $terezka$elm_charts$Internal$Svg$interpolation,
                                         fakePlane,
                                         function($) {
-                                            return $.fj;
+                                            return $.fk;
                                         },
                                         A2(
                                             $elm$core$Basics$composeR,
                                             function($) {
-                                                return $.fk;
+                                                return $.fl;
                                             },
                                             $elm$core$Maybe$Just),
                                         interConfig,
                                         _List_fromArray(
                                             [
                                                 A2($terezka$elm_charts$Internal$Svg$Point, 0, 5),
                                                 A2($terezka$elm_charts$Internal$Svg$Point, 10, 5)
                                             ])),
                                     A6(
                                         $terezka$elm_charts$Internal$Svg$area,
                                         fakePlane,
                                         function($) {
-                                            return $.fj;
+                                            return $.fk;
                                         },
                                         $elm$core$Maybe$Nothing,
                                         A2(
                                             $elm$core$Basics$composeR,
                                             function($) {
-                                                return $.fk;
+                                                return $.fl;
                                             },
                                             $elm$core$Maybe$Just),
                                         interConfig,
                                         _List_fromArray(
                                             [
                                                 A2($terezka$elm_charts$Internal$Svg$Point, 0, 5),
                                                 A2($terezka$elm_charts$Internal$Svg$Point, 10, 5)
                                             ])),
                                     A5(
                                         $terezka$elm_charts$Internal$Svg$dot,
                                         fakePlane,
                                         function($) {
-                                            return $.fj;
+                                            return $.fk;
                                         },
                                         function($) {
-                                            return $.fk;
+                                            return $.fl;
                                         },
                                         dotConfig,
                                         A2($terezka$elm_charts$Internal$Svg$Point, 5, 5))
                                 ]),
                             _List_Nil),
                         A2(
                             $elm$html$Html$div,
                             _List_fromArray(
                                 [
                                     fontStyle,
                                     A2(
                                         $elm$html$Html$Attributes$style,
                                         'margin-left',
-                                        $elm$core$String$fromFloat(config.f9) + 'px')
+                                        $elm$core$String$fromFloat(config.ga) + 'px')
                                 ]),
                             _List_fromArray(
                                 [
-                                    $elm$html$Html$text(config.gi)
+                                    $elm$html$Html$text(config.gj)
                                 ]))
                     ]));
         });
     var $terezka$elm_charts$Chart$Attributes$opacity = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
@@ -12377,19 +12485,19 @@
     var $terezka$elm_charts$Chart$Svg$lineLegend = F3(
         function(edits, interAttrsOrg, dotAttrsOrg) {
             var interpolationConfigOrg = A2($terezka$elm_charts$Internal$Helpers$apply, interAttrsOrg, $terezka$elm_charts$Internal$Svg$defaultInterpolation);
             var dotConfigOrg = A2($terezka$elm_charts$Internal$Helpers$apply, dotAttrsOrg, $terezka$elm_charts$Internal$Svg$defaultDot);
             var adjustWidth = function(config) {
                 return _Utils_update(
                     config, {
-                        fi: 10
+                        fj: 10
                     });
             };
             var _v0 = function() {
-                var _v1 = _Utils_Tuple2(interpolationConfigOrg.fX, dotConfigOrg.aG);
+                var _v1 = _Utils_Tuple2(interpolationConfigOrg.fY, dotConfigOrg.aG);
                 if (!_v1.a.$) {
                     if (_v1.b.$ === 1) {
                         var _v2 = _v1.b;
                         return _Utils_Tuple3(
                             dotAttrsOrg,
                             interAttrsOrg,
                             A2(
@@ -12437,15 +12545,15 @@
                 A2($terezka$elm_charts$Internal$Helpers$apply, interAttrs, $terezka$elm_charts$Internal$Svg$defaultInterpolation),
                 A2($terezka$elm_charts$Internal$Helpers$apply, dotAttrs, $terezka$elm_charts$Internal$Svg$defaultDot));
         });
     var $terezka$elm_charts$Chart$Attributes$title = F2(
         function(value, config) {
             return _Utils_update(
                 config, {
-                    gi: value
+                    gj: value
                 });
         });
     var $terezka$elm_charts$Chart$legendsAt = F4(
         function(toX, toY, attrs, children) {
             return $terezka$elm_charts$Chart$HtmlElement(
                 F2(
                     function(p, legends_) {
@@ -12473,16 +12581,16 @@
                                     interAttrs,
                                     dotAttrs);
                             }
                         };
                         return A5(
                             $terezka$elm_charts$Chart$Svg$legendsAt,
                             p,
-                            toX(p.fj),
-                            toY(p.fk),
+                            toX(p.fk),
+                            toY(p.fl),
                             attrs,
                             A2($elm$core$List$map, viewLegend, legends_));
                     }));
         });
     var $terezka$elm_charts$Chart$Attributes$margin = F2(
         function(v, config) {
             return _Utils_update(
@@ -12490,15 +12598,15 @@
                     ap: v
                 });
         });
     var $terezka$elm_charts$Internal$Svg$Monotone = 1;
     var $terezka$elm_charts$Chart$Attributes$monotone = function(config) {
         return _Utils_update(
             config, {
-                fX: $elm$core$Maybe$Just(1)
+                fY: $elm$core$Maybe$Just(1)
             });
     };
     var $terezka$elm_charts$Internal$Property$Stacked = function(a) {
         return {
             $: 1,
             a: a
         };
@@ -12506,25 +12614,25 @@
     var $terezka$elm_charts$Internal$Property$meta = F2(
         function(value, prop) {
             if (!prop.$) {
                 var con = prop.a;
                 return $terezka$elm_charts$Internal$Property$Property(
                     _Utils_update(
                         con, {
-                            eu: $elm$core$Maybe$Just(value)
+                            ev: $elm$core$Maybe$Just(value)
                         }));
             } else {
                 var cons = prop.a;
                 return $terezka$elm_charts$Internal$Property$Stacked(
                     A2(
                         $elm$core$List$map,
                         function(con) {
                             return _Utils_update(
                                 con, {
-                                    eu: $elm$core$Maybe$Just(value)
+                                    ev: $elm$core$Maybe$Just(value)
                                 });
                         },
                         cons));
             }
         });
     var $terezka$elm_charts$Chart$named = function(name) {
         return $terezka$elm_charts$Internal$Property$meta(name);
@@ -12549,20 +12657,20 @@
         });
     var $terezka$elm_charts$Chart$Events$map = $terezka$elm_charts$Internal$Events$map;
     var $terezka$elm_charts$Internal$Events$Event = $elm$core$Basics$identity;
     var $terezka$elm_charts$Internal$Events$on = F3(
         function(name, decoder, config) {
             return _Utils_update(
                 config, {
-                    bL: A2(
+                    bN: A2(
                         $elm$core$List$cons, {
-                            fB: decoder,
-                            fZ: name
+                            fC: decoder,
+                            f_: name
                         },
-                        config.bL)
+                        config.bN)
                 });
         });
     var $terezka$elm_charts$Chart$Events$on = $terezka$elm_charts$Internal$Events$on;
     var $terezka$elm_charts$Chart$Events$onMouseLeave = function(onMsg) {
         return A2(
             $terezka$elm_charts$Chart$Events$on,
             'mouseleave',
@@ -12577,15 +12685,15 @@
                 $terezka$elm_charts$Chart$Events$on,
                 'mousemove',
                 A2($terezka$elm_charts$Chart$Events$map, onMsg, decoder));
         });
     var $terezka$elm_charts$Chart$Attributes$row = function(config) {
         return _Utils_update(
             config, {
-                dM: 0
+                dO: 0
             });
     };
     var $terezka$elm_charts$Chart$Indexed = function(a) {
         return {
             $: 0,
             a: a
         };
@@ -12598,100 +12706,100 @@
                 b: b,
                 c: c,
                 d: d
             };
         });
     var $terezka$elm_charts$Internal$Item$toHtml = function(_v0) {
         var item = _v0;
-        return item.gl(item.fv);
+        return item.gm(item.fw);
     };
     var $terezka$elm_charts$Internal$Item$toSvg = F2(
         function(plane, _v0) {
             var item = _v0;
             return A3(
-                item.gq,
+                item.gr,
                 plane,
-                item.fv,
-                A2(item.gp, plane, item.fv));
+                item.fw,
+                A2(item.gq, plane, item.fw));
         });
     var $terezka$elm_charts$Internal$Item$generalize = F2(
         function(toAny, _v0) {
             var item = _v0;
             return {
-                fv: {
-                    f1: toAny(item.fv.f1),
-                    gk: $elm$core$Basics$identity,
-                    cH: item.fv.cH,
-                    gv: item.fv.gv
+                fw: {
+                    f2: toAny(item.fw.f2),
+                    gl: $elm$core$Basics$identity,
+                    cI: item.fw.cI,
+                    gw: item.fw.gw
                 },
-                gl: function(c) {
+                gm: function(c) {
                     return $terezka$elm_charts$Internal$Item$toHtml(item);
                 },
-                gm: function(_v1) {
-                    return item.gm(item.fv);
+                gn: function(_v1) {
+                    return item.gn(item.fw);
                 },
-                gp: F2(
+                gq: F2(
                     function(plane, _v2) {
-                        return A2(item.gp, plane, item.fv);
+                        return A2(item.gq, plane, item.fw);
                     }),
-                gq: F3(
+                gr: F3(
                     function(plane, _v3, _v4) {
                         return A2($terezka$elm_charts$Internal$Item$toSvg, plane, item);
                     })
             };
         });
     var $terezka$elm_charts$Internal$Many$getMembers = function(_v0) {
         var group_ = _v0;
         return function(_v1) {
             var x = _v1.a;
             var xs = _v1.b;
             return A2($elm$core$List$cons, x, xs);
-        }(group_.fv.ek);
+        }(group_.fw.el);
     };
     var $terezka$elm_charts$Internal$Many$getGenerals = function(group_) {
         var generalize = function(_v0) {
             var item = _v0;
-            return A2($terezka$elm_charts$Internal$Item$generalize, item.fv.gk, item);
+            return A2($terezka$elm_charts$Internal$Item$generalize, item.fw.gl, item);
         };
         return A2(
             $elm$core$List$map,
             generalize,
             $terezka$elm_charts$Internal$Many$getMembers(group_));
     };
     var $terezka$elm_charts$Internal$Item$getLimits = function(_v0) {
         var item = _v0;
-        return item.gm(item.fv);
+        return item.gn(item.fw);
     };
     var $terezka$elm_charts$Internal$Item$map = F2(
         function(func, _v0) {
             var item = _v0;
             return {
-                fv: {
-                    f1: item.fv.f1,
-                    gk: item.fv.gk,
-                    cH: item.fv.cH,
-                    gv: {
-                        fA: func(item.fv.gv.fA),
-                        fT: item.fv.gv.fT,
-                        aK: item.fv.gv.aK,
-                        be: item.fv.gv.be,
-                        fk: item.fv.gv.fk
+                fw: {
+                    f2: item.fw.f2,
+                    gl: item.fw.gl,
+                    cI: item.fw.cI,
+                    gw: {
+                        fB: func(item.fw.gw.fB),
+                        fU: item.fw.gw.fU,
+                        aM: item.fw.gw.aM,
+                        bg: item.fw.gw.bg,
+                        fl: item.fw.gw.fl
                     }
                 },
-                gl: function(_v1) {
+                gm: function(_v1) {
                     return $terezka$elm_charts$Internal$Item$toHtml(item);
                 },
-                gm: function(_v2) {
-                    return item.gm(item.fv);
+                gn: function(_v2) {
+                    return item.gn(item.fw);
                 },
-                gp: F2(
+                gq: F2(
                     function(plane, _v3) {
-                        return A2(item.gp, plane, item.fv);
+                        return A2(item.gq, plane, item.fw);
                     }),
-                gq: F3(
+                gr: F3(
                     function(plane, _v4, _v5) {
                         return A2($terezka$elm_charts$Internal$Item$toSvg, plane, item);
                     })
             };
         });
     var $elm$virtual_dom$VirtualDom$map = _VirtualDom_map;
     var $elm$svg$Svg$map = $elm$virtual_dom$VirtualDom$map;
@@ -12784,27 +12892,27 @@
                     var interAttr = _Utils_ap(
                         _List_fromArray(
                             [
                                 $terezka$elm_charts$Chart$Attributes$color(
                                     $terezka$elm_charts$Internal$Helpers$toDefaultColor(colorIndex)),
                                 $terezka$elm_charts$Chart$Attributes$opacity(defaultOpacity)
                             ]),
-                        prop.fR);
+                        prop.fS);
                     var interConfig = toInterConfig(interAttr);
                     var defaultName = 'Property #' + $elm$core$String$fromInt(colorIndex + 1);
                     var defaultAttrs = _List_fromArray(
                         [
-                            $terezka$elm_charts$Chart$Attributes$color(interConfig.bC),
-                            $terezka$elm_charts$Chart$Attributes$border(interConfig.bC),
-                            _Utils_eq(interConfig.fX, $elm$core$Maybe$Nothing) ? $terezka$elm_charts$Chart$Attributes$circle : $elm$core$Basics$identity
+                            $terezka$elm_charts$Chart$Attributes$color(interConfig.bE),
+                            $terezka$elm_charts$Chart$Attributes$border(interConfig.bE),
+                            _Utils_eq(interConfig.fY, $elm$core$Maybe$Nothing) ? $terezka$elm_charts$Chart$Attributes$circle : $elm$core$Basics$identity
                         ]);
-                    var dotAttrs = _Utils_ap(defaultAttrs, prop.bu);
+                    var dotAttrs = _Utils_ap(defaultAttrs, prop.bw);
                     return A3(
                         $terezka$elm_charts$Internal$Legend$LineLegend,
-                        A2($elm$core$Maybe$withDefault, defaultName, prop.eu),
+                        A2($elm$core$Maybe$withDefault, defaultName, prop.ev),
                         interAttr,
                         dotAttrs);
                 });
             return A2(
                 $elm$core$List$indexedMap,
                 F2(
                     function(propIndex, f) {
@@ -12871,120 +12979,120 @@
                 return A2($terezka$elm_charts$Internal$Helpers$apply, attrs, $terezka$elm_charts$Internal$Svg$defaultDot);
             };
             var toDotItem = F7(
                 function(lineIndex, stackIndex, colorIndex, prop, interConfig, dataIndex, datum_) {
                     var y_ = A2(
                         $elm$core$Maybe$withDefault,
                         0,
-                        prop.a7(datum_));
+                        prop.a9(datum_));
                     var x_ = toX(datum_);
                     var defaultAttrs = _List_fromArray(
                         [
-                            $terezka$elm_charts$Chart$Attributes$color(interConfig.bC),
-                            $terezka$elm_charts$Chart$Attributes$border(interConfig.bC),
-                            _Utils_eq(interConfig.fX, $elm$core$Maybe$Nothing) ? $terezka$elm_charts$Chart$Attributes$circle : $elm$core$Basics$identity
+                            $terezka$elm_charts$Chart$Attributes$color(interConfig.bE),
+                            $terezka$elm_charts$Chart$Attributes$border(interConfig.bE),
+                            _Utils_eq(interConfig.fY, $elm$core$Maybe$Nothing) ? $terezka$elm_charts$Chart$Attributes$circle : $elm$core$Basics$identity
                         ]);
                     var dotAttrs = _Utils_ap(
                         defaultAttrs,
                         _Utils_ap(
-                            prop.bu,
-                            A5(prop.d4, lineIndex, stackIndex, dataIndex, prop.eu, datum_)));
+                            prop.bw,
+                            A5(prop.d5, lineIndex, stackIndex, dataIndex, prop.ev, datum_)));
                     var config = toDotConfig(dotAttrs);
                     return {
-                        fv: {
-                            f1: config,
-                            gk: $terezka$elm_charts$Internal$Item$Dot,
-                            cH: {
+                        fw: {
+                            f2: config,
+                            gl: $terezka$elm_charts$Internal$Item$Dot,
+                            cI: {
                                 v: config.v,
                                 x: config.x,
-                                bC: function() {
-                                    var _v6 = config.bC;
+                                bE: function() {
+                                    var _v6 = config.bE;
                                     if (_v6 === 'white') {
-                                        return interConfig.bC;
+                                        return interConfig.bE;
                                     } else {
-                                        return config.bC;
+                                        return config.bE;
                                     }
                                 }(),
-                                bG: dataIndex,
-                                fD: elIndex,
-                                d6: prop.F(datum_),
-                                fP: colorIndex,
-                                fZ: prop.eu,
-                                f2: lineIndex,
-                                ga: stackIndex
+                                bI: dataIndex,
+                                fE: elIndex,
+                                d7: prop.F(datum_),
+                                fQ: colorIndex,
+                                f_: prop.ev,
+                                f3: lineIndex,
+                                gb: stackIndex
                             },
-                            gv: {
-                                fA: datum_,
-                                fT: function() {
+                            gw: {
+                                fB: datum_,
+                                fU: function() {
                                     var _v7 = prop.Z(datum_);
                                     if (!_v7.$) {
                                         return true;
                                     } else {
                                         return false;
                                     }
                                 }(),
-                                aK: x_,
-                                be: x_,
-                                fk: y_
+                                aM: x_,
+                                bg: x_,
+                                fl: y_
                             }
                         },
-                        gl: function(c) {
+                        gm: function(c) {
                             return _List_fromArray(
                                 [
                                     A3(
                                         $terezka$elm_charts$Internal$Produce$tooltipRow,
-                                        c.cH.bC,
-                                        A2($terezka$elm_charts$Internal$Produce$toDefaultName, colorIndex, c.cH.fZ),
+                                        c.cI.bE,
+                                        A2($terezka$elm_charts$Internal$Produce$toDefaultName, colorIndex, c.cI.f_),
                                         prop.F(datum_))
                                 ]);
                         },
-                        gm: function(_v8) {
+                        gn: function(_v8) {
                             return {
-                                aK: x_,
-                                be: x_,
-                                gA: y_,
-                                dI: y_
+                                aM: x_,
+                                bg: x_,
+                                gB: y_,
+                                dK: y_
                             };
                         },
-                        gp: F2(
+                        gq: F2(
                             function(plane, _v9) {
                                 var radius = A2(
                                     $elm$core$Maybe$withDefault,
                                     0,
                                     A2(
                                         $elm$core$Maybe$map,
-                                        $terezka$elm_charts$Internal$Svg$toRadius(config.e1),
+                                        $terezka$elm_charts$Internal$Svg$toRadius(config.e2),
                                         config.aG));
                                 var radiusX_ = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, radius);
                                 var radiusY_ = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, radius);
                                 return {
-                                    aK: x_ - radiusX_,
-                                    be: x_ + radiusX_,
-                                    gA: y_ - radiusY_,
-                                    dI: y_ + radiusY_
+                                    aM: x_ - radiusX_,
+                                    bg: x_ + radiusX_,
+                                    gB: y_ - radiusY_,
+                                    dK: y_ + radiusY_
                                 };
                             }),
-                        gq: F3(
+                        gr: F3(
                             function(plane, _v10, _v11) {
                                 var _v12 = prop.Z(datum_);
                                 if (_v12.$ === 1) {
                                     return $elm$svg$Svg$text('');
                                 } else {
                                     return A5(
                                         $terezka$elm_charts$Internal$Svg$dot,
                                         plane,
                                         function($) {
-                                            return $.fj;
+                                            return $.fk;
                                         },
                                         function($) {
-                                            return $.fk;
+                                            return $.fl;
                                         },
                                         config, {
-                                            fj: x_,
-                                            fk: y_
+                                            fk: x_,
+                                            fl: y_
                                         });
                                 }
                             })
                     };
                 });
             var toSeriesItem = F5(
                 function(lineIndex, stacks, stackIndex, prop, colorIndex) {
@@ -12992,30 +13100,30 @@
                     var interAttr = _Utils_ap(
                         _List_fromArray(
                             [
                                 $terezka$elm_charts$Chart$Attributes$color(
                                     $terezka$elm_charts$Internal$Helpers$toDefaultColor(colorIndex)),
                                 $terezka$elm_charts$Chart$Attributes$opacity(defaultOpacity)
                             ]),
-                        prop.fR);
+                        prop.fS);
                     var interConfig = toInterConfig(interAttr);
                     var dotItems = A2(
                         $elm$core$List$indexedMap,
                         A5(toDotItem, lineIndex, stackIndex, colorIndex, prop, interConfig),
                         data);
                     if (!dotItems.b) {
                         return $elm$core$Maybe$Nothing;
                     } else {
                         var first = dotItems.a;
                         var rest = dotItems.b;
                         return $elm$core$Maybe$Just({
-                            fv: {
-                                ek: _Utils_Tuple2(first, rest)
+                            fw: {
+                                el: _Utils_Tuple2(first, rest)
                             },
-                            gl: function(c) {
+                            gm: function(c) {
                                 return _List_fromArray(
                                     [
                                         A2(
                                             $elm$html$Html$table,
                                             _List_fromArray(
                                                 [
                                                     A2($elm$html$Html$Attributes$style, 'margin', '0')
@@ -13023,67 +13131,67 @@
                                             A2(
                                                 $elm$core$List$concatMap,
                                                 $terezka$elm_charts$Internal$Item$toHtml,
                                                 function(_v1) {
                                                     var x = _v1.a;
                                                     var xs = _v1.b;
                                                     return A2($elm$core$List$cons, x, xs);
-                                                }(c.ek)))
+                                                }(c.el)))
                                     ]);
                             },
-                            gm: function(c) {
+                            gn: function(c) {
                                 return A2(
                                     $terezka$elm_charts$Internal$Coordinates$foldPosition,
                                     $terezka$elm_charts$Internal$Item$getLimits,
                                     function(_v2) {
                                         var x = _v2.a;
                                         var xs = _v2.b;
                                         return A2($elm$core$List$cons, x, xs);
-                                    }(c.ek));
+                                    }(c.el));
                             },
-                            gp: F2(
+                            gq: F2(
                                 function(plane, c) {
                                     return A2(
                                         $terezka$elm_charts$Internal$Coordinates$foldPosition,
                                         $terezka$elm_charts$Internal$Item$getPosition(plane),
                                         function(_v3) {
                                             var x = _v3.a;
                                             var xs = _v3.b;
                                             return A2($elm$core$List$cons, x, xs);
-                                        }(c.ek));
+                                        }(c.el));
                                 }),
-                            gq: F3(
+                            gr: F3(
                                 function(plane, _v4, _v5) {
                                     var toBottom = function(datum_) {
                                         return A3(
                                             $elm$core$Maybe$map2,
                                             F2(
                                                 function(real, visual) {
                                                     return visual - real;
                                                 }),
                                             prop.Z(datum_),
-                                            prop.a7(datum_));
+                                            prop.a9(datum_));
                                     };
                                     return A2(
                                         $elm$svg$Svg$g,
                                         _List_fromArray(
                                             [
                                                 $elm$svg$Svg$Attributes$class('elm-charts__series')
                                             ]),
                                         _List_fromArray(
                                             [
                                                 A6(
                                                     $terezka$elm_charts$Internal$Svg$area,
                                                     plane,
                                                     toX,
                                                     $elm$core$Maybe$Just(toBottom),
-                                                    prop.a7,
+                                                    prop.a9,
                                                     interConfig,
                                                     data),
-                                                A5($terezka$elm_charts$Internal$Svg$interpolation, plane, toX, prop.a7, interConfig, data),
+                                                A5($terezka$elm_charts$Internal$Svg$interpolation, plane, toX, prop.a9, interConfig, data),
                                                 A2(
                                                     $elm$svg$Svg$g,
                                                     _List_fromArray(
                                                         [
                                                             $elm$svg$Svg$Attributes$class('elm-charts__dots')
                                                         ]),
                                                     A2(
@@ -13156,62 +13264,62 @@
         function(toX, properties, data) {
             return A4($terezka$elm_charts$Chart$seriesMap, $elm$core$Basics$identity, toX, properties, data);
         });
     var $terezka$elm_charts$Chart$Attributes$spacing = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    f9: v
+                    ga: v
                 });
         });
     var $terezka$elm_charts$Chart$html = function(func) {
         return $terezka$elm_charts$Chart$HtmlElement(
             F2(
                 function(p, _v0) {
                     return func(p);
                 }));
     };
     var $terezka$elm_charts$Internal$Svg$defaultTooltip = {
         ax: true,
-        fq: 'white',
+        fr: 'white',
         v: '#D8D8D8',
         ac: $elm$core$Maybe$Nothing,
-        fG: $elm$core$Maybe$Nothing,
-        ea: 0,
+        fH: $elm$core$Maybe$Nothing,
+        eb: 0,
         b: 8,
-        fi: 0
+        fj: 0
     };
     var $terezka$elm_charts$Internal$Svg$Bottom = 3;
     var $terezka$elm_charts$Internal$Svg$Left = 1;
     var $terezka$elm_charts$Internal$Svg$Right = 2;
     var $terezka$elm_charts$Internal$Svg$Top = 0;
     var $elm$core$List$all = F2(
         function(isOkay, list) {
             return !A2(
                 $elm$core$List$any,
                 A2($elm$core$Basics$composeL, $elm$core$Basics$not, isOkay),
                 list);
         });
     var $terezka$elm_charts$Internal$Coordinates$bottom = function(pos) {
         return {
-            fj: pos.aK + ((pos.be - pos.aK) / 2),
-            fk: pos.gA
+            fk: pos.aM + ((pos.bg - pos.aM) / 2),
+            fl: pos.gB
         };
     };
     var $terezka$elm_charts$Internal$Coordinates$left = function(pos) {
         return {
-            fj: pos.aK,
-            fk: pos.gA + ((pos.dI - pos.gA) / 2)
+            fk: pos.aM,
+            fl: pos.gB + ((pos.dK - pos.gB) / 2)
         };
     };
     var $elm$html$Html$map = $elm$virtual_dom$VirtualDom$map;
     var $terezka$elm_charts$Internal$Coordinates$right = function(pos) {
         return {
-            fj: pos.be,
-            fk: pos.gA + ((pos.dI - pos.gA) / 2)
+            fk: pos.bg,
+            fl: pos.gB + ((pos.dK - pos.gB) / 2)
         };
     };
     var $terezka$elm_charts$Internal$Svg$tooltipPointerStyle = F4(
         function(direction, className, background, borderColor) {
             var config = function() {
                 switch (direction) {
                     case 0:
@@ -13240,34 +13348,34 @@
                         };
                 }
             }();
             return '\n  .' + (className + (':before, .' + (className + (':after {\n    content: "";\n    position: absolute;\n    border-' + (config.T + (': 5px solid transparent;\n    border-' + (config.aj + (': 5px solid transparent;\n    ' + (config.L + (': 100%;\n    ' + (config.T + (': 50%;\n    margin-' + (config.T + (': -5px;\n  }\n\n  .' + (className + (':after {\n    border-' + (config.L + (': 5px solid ' + (background + (';\n    margin-' + (config.L + (': -1px;\n    z-index: 1;\n    height: 0px;\n  }\n\n  .' + (className + (':before {\n    border-' + (config.L + (': 5px solid ' + (borderColor + ';\n    height: 0px;\n  }\n  ')))))))))))))))))))))))))));
         });
     var $terezka$elm_charts$Internal$Coordinates$top = function(pos) {
         return {
-            fj: pos.aK + ((pos.be - pos.aK) / 2),
-            fk: pos.dI
+            fk: pos.aM + ((pos.bg - pos.aM) / 2),
+            fl: pos.dK
         };
     };
     var $terezka$elm_charts$Internal$Svg$tooltip = F5(
         function(plane, pos, config, htmlAttrs, content) {
-            var distanceTop = A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, pos.dI);
-            var distanceRight = plane.fj.O - A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, pos.aK);
-            var distanceLeft = A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, pos.be);
-            var distanceBottom = plane.fk.O - A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, pos.gA);
+            var distanceTop = A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, pos.dK);
+            var distanceRight = plane.fk.O - A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, pos.aM);
+            var distanceLeft = A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, pos.bg);
+            var distanceBottom = plane.fl.O - A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, pos.gB);
             var direction = function() {
                 var _v5 = config.ac;
                 if (!_v5.$) {
                     switch (_v5.a) {
                         case 4:
                             var _v6 = _v5.a;
-                            return (config.fi > 0) ? ((_Utils_cmp(distanceLeft, config.fi + config.b) > 0) ? 1 : 2) : ((_Utils_cmp(distanceLeft, distanceRight) > 0) ? 1 : 2);
+                            return (config.fj > 0) ? ((_Utils_cmp(distanceLeft, config.fj + config.b) > 0) ? 1 : 2) : ((_Utils_cmp(distanceLeft, distanceRight) > 0) ? 1 : 2);
                         case 5:
                             var _v7 = _v5.a;
-                            return (config.ea > 0) ? ((_Utils_cmp(distanceTop, config.ea + config.b) > 0) ? 0 : 3) : ((_Utils_cmp(distanceTop, distanceBottom) > 0) ? 0 : 3);
+                            return (config.eb > 0) ? ((_Utils_cmp(distanceTop, config.eb + config.b) > 0) ? 0 : 3) : ((_Utils_cmp(distanceTop, distanceBottom) > 0) ? 0 : 3);
                         default:
                             var dir = _v5.a;
                             return dir;
                     }
                 } else {
                     var isLargest = function(a) {
                         return $elm$core$List$all(
@@ -13287,15 +13395,15 @@
                         isLargest,
                         distanceLeft,
                         _List_fromArray(
                             [distanceTop, distanceBottom, distanceRight])) ? 1 : 2));
                 }
             }();
             var focalPoint = function() {
-                var _v2 = config.fG;
+                var _v2 = config.fH;
                 if (!_v2.$) {
                     var focal = _v2.a;
                     switch (direction) {
                         case 0:
                             return $terezka$elm_charts$Internal$Coordinates$top(
                                 focal(pos));
                         case 3:
@@ -13369,33 +13477,33 @@
                 A3(
                     $elm$html$Html$node,
                     'style',
                     _List_Nil,
                     _List_fromArray(
                         [
                             $elm$html$Html$text(
-                                A4($terezka$elm_charts$Internal$Svg$tooltipPointerStyle, direction, className, config.fq, config.v))
+                                A4($terezka$elm_charts$Internal$Svg$tooltipPointerStyle, direction, className, config.fr, config.v))
                         ])),
                 content) : content;
             var attributes = _Utils_ap(
                 _List_fromArray(
                     [
                         $elm$html$Html$Attributes$class(className),
                         A2($elm$html$Html$Attributes$style, 'transform', transformation),
                         A2($elm$html$Html$Attributes$style, 'padding', '5px 8px'),
-                        A2($elm$html$Html$Attributes$style, 'background', config.fq),
+                        A2($elm$html$Html$Attributes$style, 'background', config.fr),
                         A2($elm$html$Html$Attributes$style, 'border', '1px solid ' + config.v),
                         A2($elm$html$Html$Attributes$style, 'border-radius', '3px'),
                         A2($elm$html$Html$Attributes$style, 'pointer-events', 'none')
                     ]),
                 htmlAttrs);
             return A2(
                 $elm$html$Html$map,
                 $elm$core$Basics$never,
-                A7($terezka$elm_charts$Internal$Svg$positionHtml, plane, focalPoint.fj, focalPoint.fk, xOff, yOff, attributes, children));
+                A7($terezka$elm_charts$Internal$Svg$positionHtml, plane, focalPoint.fk, focalPoint.fl, xOff, yOff, attributes, children));
         });
     var $terezka$elm_charts$Chart$Svg$tooltip = F3(
         function(plane, pos, edits) {
             return A3(
                 $terezka$elm_charts$Internal$Svg$tooltip,
                 plane,
                 pos,
@@ -13403,15 +13511,15 @@
         });
     var $terezka$elm_charts$Chart$tooltip = F4(
         function(i, edits, attrs_, content) {
             return $terezka$elm_charts$Chart$html(
                 function(p) {
                     var pos = $terezka$elm_charts$Internal$Item$getLimits(i);
                     var content_ = _Utils_eq(content, _List_Nil) ? $terezka$elm_charts$Internal$Item$toHtml(i) : content;
-                    return A3($terezka$elm_charts$Internal$Svg$isWithinPlane, p, pos.aK, pos.dI) ? A5(
+                    return A3($terezka$elm_charts$Internal$Svg$isWithinPlane, p, pos.aM, pos.dK) ? A5(
                         $terezka$elm_charts$Chart$Svg$tooltip,
                         p,
                         A2($terezka$elm_charts$Internal$Item$getPosition, p, i),
                         edits,
                         attrs_,
                         content_) : $elm$html$Html$text('');
                 });
@@ -13432,18 +13540,18 @@
                 a: a,
                 b: b,
                 c: c
             };
         });
     var $terezka$elm_charts$Internal$Svg$defaultLabel = {
         i: $elm$core$Maybe$Nothing,
-        bu: _List_Nil,
+        bw: _List_Nil,
         v: 'white',
         x: 0,
-        bC: '#808BAB',
+        bE: '#808BAB',
         j: $elm$core$Maybe$Nothing,
         k: $elm$core$Maybe$Nothing,
         l: false,
         o: 0,
         p: false,
         g: 0,
         h: 0
@@ -13802,15 +13910,15 @@
     var $terezka$intervals$Intervals$positions = F5(
         function(range, beginning, interval, m, acc) {
             positions: while (true) {
                 var nextPosition = A2(
                     $terezka$intervals$Intervals$correctFloat,
                     $terezka$intervals$Intervals$getPrecision(interval),
                     beginning + (m * interval));
-                if (_Utils_cmp(nextPosition, range.et) > 0) {
+                if (_Utils_cmp(nextPosition, range.eu) > 0) {
                     return acc;
                 } else {
                     var $temp$range = range,
                         $temp$beginning = beginning,
                         $temp$interval = interval,
                         $temp$m = m + 1,
                         $temp$acc = _Utils_ap(
@@ -13824,18 +13932,18 @@
                     acc = $temp$acc;
                     continue positions;
                 }
             }
         });
     var $terezka$intervals$Intervals$values = F4(
         function(allowDecimals, exact, amountRough, range) {
-            var intervalRough = (range.et - range.ev) / amountRough;
+            var intervalRough = (range.eu - range.ew) / amountRough;
             var interval = A3($terezka$intervals$Intervals$getInterval, intervalRough, allowDecimals, exact);
             var intervalSafe = (!interval) ? 1 : interval;
-            var beginning = A2($terezka$intervals$Intervals$getBeginning, range.ev, intervalSafe);
+            var beginning = A2($terezka$intervals$Intervals$getBeginning, range.ew, intervalSafe);
             var amountRoughSafe = (!amountRough) ? 1 : amountRough;
             return A5($terezka$intervals$Intervals$positions, range, beginning, intervalSafe, 0, _List_Nil);
         });
     var $terezka$intervals$Intervals$floats = function(amount) {
         if (!amount.$) {
             var number = amount.a;
             return A3($terezka$intervals$Intervals$values, true, true, number);
@@ -13845,28 +13953,28 @@
         }
     };
     var $terezka$elm_charts$Internal$Svg$floats = F2(
         function(i, b) {
             return A2(
                 $terezka$intervals$Intervals$floats,
                 $terezka$intervals$Intervals$around(i), {
-                    et: b.et,
-                    ev: b.ev
+                    eu: b.eu,
+                    ew: b.ew
                 });
         });
     var $terezka$elm_charts$Chart$Svg$floats = $terezka$elm_charts$Internal$Svg$floats;
     var $ryannhg$date_format$DateFormat$Language$Language = F6(
         function(toMonthName, toMonthAbbreviation, toWeekdayName, toWeekdayAbbreviation, toAmPm, toOrdinalSuffix) {
             return {
-                gj: toAmPm,
-                gn: toMonthAbbreviation,
-                go: toMonthName,
-                aI: toOrdinalSuffix,
-                gr: toWeekdayAbbreviation,
-                gs: toWeekdayName
+                gk: toAmPm,
+                go: toMonthAbbreviation,
+                gp: toMonthName,
+                aK: toOrdinalSuffix,
+                gs: toWeekdayAbbreviation,
+                gt: toWeekdayName
             };
         });
     var $ryannhg$date_format$DateFormat$Language$toEnglishAmPm = function(hour) {
         return (hour > 11) ? 'pm' : 'am';
     };
     var $ryannhg$date_format$DateFormat$Language$toEnglishMonthName = function(month) {
         switch (month) {
@@ -13949,15 +14057,15 @@
             $elm$core$Basics$composeR,
             $ryannhg$date_format$DateFormat$Language$toEnglishWeekdayName,
             $elm$core$String$left(3)),
         $ryannhg$date_format$DateFormat$Language$toEnglishAmPm,
         $ryannhg$date_format$DateFormat$Language$toEnglishSuffix);
     var $ryannhg$date_format$DateFormat$amPm = F3(
         function(language, zone, posix) {
-            return language.gj(
+            return language.gk(
                 A2($elm$time$Time$toHour, zone, posix));
         });
     var $ryannhg$date_format$DateFormat$dayOfMonth = $elm$time$Time$toDay;
     var $elm$time$Time$Sun = 6;
     var $elm$time$Time$Fri = 4;
     var $elm$time$Time$Mon = 0;
     var $elm$time$Time$Sat = 5;
@@ -14288,92 +14396,92 @@
                 case 0:
                     return $elm$core$String$fromInt(
                         A2($ryannhg$date_format$DateFormat$monthNumber_, zone, posix));
                 case 1:
                     return function(num) {
                         return _Utils_ap(
                             $elm$core$String$fromInt(num),
-                            language.aI(num));
+                            language.aK(num));
                     }(
                         A2($ryannhg$date_format$DateFormat$monthNumber_, zone, posix));
                 case 2:
                     return A2(
                         $ryannhg$date_format$DateFormat$toFixedLength,
                         2,
                         A2($ryannhg$date_format$DateFormat$monthNumber_, zone, posix));
                 case 3:
-                    return language.gn(
+                    return language.go(
                         A2($elm$time$Time$toMonth, zone, posix));
                 case 4:
-                    return language.go(
+                    return language.gp(
                         A2($elm$time$Time$toMonth, zone, posix));
                 case 17:
                     return $elm$core$String$fromInt(
                         1 + A2($ryannhg$date_format$DateFormat$quarter, zone, posix));
                 case 18:
                     return function(num) {
                         return _Utils_ap(
                             $elm$core$String$fromInt(num),
-                            language.aI(num));
+                            language.aK(num));
                     }(
                         1 + A2($ryannhg$date_format$DateFormat$quarter, zone, posix));
                 case 5:
                     return $elm$core$String$fromInt(
                         A2($ryannhg$date_format$DateFormat$dayOfMonth, zone, posix));
                 case 6:
                     return function(num) {
                         return _Utils_ap(
                             $elm$core$String$fromInt(num),
-                            language.aI(num));
+                            language.aK(num));
                     }(
                         A2($ryannhg$date_format$DateFormat$dayOfMonth, zone, posix));
                 case 7:
                     return A2(
                         $ryannhg$date_format$DateFormat$toFixedLength,
                         2,
                         A2($ryannhg$date_format$DateFormat$dayOfMonth, zone, posix));
                 case 8:
                     return $elm$core$String$fromInt(
                         A2($ryannhg$date_format$DateFormat$dayOfYear, zone, posix));
                 case 9:
                     return function(num) {
                         return _Utils_ap(
                             $elm$core$String$fromInt(num),
-                            language.aI(num));
+                            language.aK(num));
                     }(
                         A2($ryannhg$date_format$DateFormat$dayOfYear, zone, posix));
                 case 10:
                     return A2(
                         $ryannhg$date_format$DateFormat$toFixedLength,
                         3,
                         A2($ryannhg$date_format$DateFormat$dayOfYear, zone, posix));
                 case 11:
                     return $elm$core$String$fromInt(
                         A2($ryannhg$date_format$DateFormat$dayOfWeek, zone, posix));
                 case 12:
                     return function(num) {
                         return _Utils_ap(
                             $elm$core$String$fromInt(num),
-                            language.aI(num));
+                            language.aK(num));
                     }(
                         A2($ryannhg$date_format$DateFormat$dayOfWeek, zone, posix));
                 case 13:
-                    return language.gr(
+                    return language.gs(
                         A2($elm$time$Time$toWeekday, zone, posix));
                 case 14:
-                    return language.gs(
+                    return language.gt(
                         A2($elm$time$Time$toWeekday, zone, posix));
                 case 19:
                     return $elm$core$String$fromInt(
                         A2($ryannhg$date_format$DateFormat$weekOfYear, zone, posix));
                 case 20:
                     return function(num) {
                         return _Utils_ap(
                             $elm$core$String$fromInt(num),
-                            language.aI(num));
+                            language.aK(num));
                     }(
                         A2($ryannhg$date_format$DateFormat$weekOfYear, zone, posix));
                 case 21:
                     return A2(
                         $ryannhg$date_format$DateFormat$toFixedLength,
                         2,
                         A2($ryannhg$date_format$DateFormat$weekOfYear, zone, posix));
@@ -14540,30 +14648,30 @@
     };
     var $ryannhg$date_format$DateFormat$yearNumber = $ryannhg$date_format$DateFormat$YearNumber;
     var $terezka$elm_charts$Internal$Svg$formatYear = $ryannhg$date_format$DateFormat$format(
         _List_fromArray(
             [$ryannhg$date_format$DateFormat$yearNumber]));
     var $terezka$elm_charts$Internal$Svg$formatTime = F2(
         function(zone, time) {
-            var _v0 = A2($elm$core$Maybe$withDefault, time.gt, time.fu);
+            var _v0 = A2($elm$core$Maybe$withDefault, time.gu, time.fv);
             switch (_v0) {
                 case 0:
-                    return A2($terezka$elm_charts$Internal$Svg$formatClockMillis, zone, time.gh);
+                    return A2($terezka$elm_charts$Internal$Svg$formatClockMillis, zone, time.gi);
                 case 1:
-                    return A2($terezka$elm_charts$Internal$Svg$formatClockSecond, zone, time.gh);
+                    return A2($terezka$elm_charts$Internal$Svg$formatClockSecond, zone, time.gi);
                 case 2:
-                    return A2($terezka$elm_charts$Internal$Svg$formatClock, zone, time.gh);
+                    return A2($terezka$elm_charts$Internal$Svg$formatClock, zone, time.gi);
                 case 3:
-                    return A2($terezka$elm_charts$Internal$Svg$formatClock, zone, time.gh);
+                    return A2($terezka$elm_charts$Internal$Svg$formatClock, zone, time.gi);
                 case 4:
-                    return (time.fY === 7) ? A2($terezka$elm_charts$Internal$Svg$formatWeekday, zone, time.gh) : A2($terezka$elm_charts$Internal$Svg$formatDate, zone, time.gh);
+                    return (time.fZ === 7) ? A2($terezka$elm_charts$Internal$Svg$formatWeekday, zone, time.gi) : A2($terezka$elm_charts$Internal$Svg$formatDate, zone, time.gi);
                 case 5:
-                    return A2($terezka$elm_charts$Internal$Svg$formatMonth, zone, time.gh);
+                    return A2($terezka$elm_charts$Internal$Svg$formatMonth, zone, time.gi);
                 default:
-                    return A2($terezka$elm_charts$Internal$Svg$formatYear, zone, time.gh);
+                    return A2($terezka$elm_charts$Internal$Svg$formatYear, zone, time.gi);
             }
         });
     var $terezka$elm_charts$Chart$Svg$formatTime = $terezka$elm_charts$Internal$Svg$formatTime;
     var $terezka$elm_charts$Internal$Svg$generate = F3(
         function(amount, _v0, limits) {
             var func = _v0;
             return A2(func, amount, limits);
@@ -14585,16 +14693,16 @@
                 }());
         });
     var $terezka$elm_charts$Internal$Svg$ints = F2(
         function(i, b) {
             return A2(
                 $terezka$intervals$Intervals$ints,
                 $terezka$intervals$Intervals$around(i), {
-                    et: b.et,
-                    ev: b.ev
+                    eu: b.eu,
+                    ew: b.ew
                 });
         });
     var $terezka$elm_charts$Chart$Svg$ints = $terezka$elm_charts$Internal$Svg$ints;
     var $terezka$intervals$Intervals$Day = 4;
     var $terezka$intervals$Intervals$Hour = 3;
     var $terezka$intervals$Intervals$Millisecond = 0;
     var $terezka$intervals$Intervals$Minute = 2;
@@ -14746,17 +14854,17 @@
                         $temp$d = d - monthDays;
                     y = $temp$y;
                     m = $temp$m;
                     d = $temp$d;
                     continue toCalendarDateHelp;
                 } else {
                     return {
-                        dW: d,
-                        ex: m,
-                        fl: y
+                        dY: d,
+                        ey: m,
+                        fm: y
                     };
                 }
             }
         });
     var $justinmimbs$date$Date$divWithRemainder = F2(
         function(a, b) {
             return _Utils_Tuple2(
@@ -14780,38 +14888,38 @@
         var n = (!r1) ? 0 : 1;
         return ((((n400 * 400) + (n100 * 100)) + (n4 * 4)) + n1) + n;
     };
     var $justinmimbs$date$Date$toOrdinalDate = function(_v0) {
         var rd = _v0;
         var y = $justinmimbs$date$Date$year(rd);
         return {
-            di: rd - $justinmimbs$date$Date$daysBeforeYear(y),
-            fl: y
+            dk: rd - $justinmimbs$date$Date$daysBeforeYear(y),
+            fm: y
         };
     };
     var $justinmimbs$date$Date$toCalendarDate = function(_v0) {
         var rd = _v0;
         var date = $justinmimbs$date$Date$toOrdinalDate(rd);
-        return A3($justinmimbs$date$Date$toCalendarDateHelp, date.fl, 0, date.di);
+        return A3($justinmimbs$date$Date$toCalendarDateHelp, date.fm, 0, date.dk);
     };
     var $justinmimbs$date$Date$add = F3(
         function(unit, n, _v0) {
             var rd = _v0;
             switch (unit) {
                 case 0:
                     return A3($justinmimbs$date$Date$add, 1, 12 * n, rd);
                 case 1:
                     var date = $justinmimbs$date$Date$toCalendarDate(rd);
-                    var wholeMonths = ((12 * (date.fl - 1)) + ($justinmimbs$date$Date$monthToNumber(date.ex) - 1)) + n;
+                    var wholeMonths = ((12 * (date.fm - 1)) + ($justinmimbs$date$Date$monthToNumber(date.ey) - 1)) + n;
                     var m = $justinmimbs$date$Date$numberToMonth(
                         A2($elm$core$Basics$modBy, 12, wholeMonths) + 1);
                     var y = A2($justinmimbs$date$Date$floorDiv, wholeMonths, 12) + 1;
                     return ($justinmimbs$date$Date$daysBeforeYear(y) + A2($justinmimbs$date$Date$daysBeforeMonth, y, m)) + A2(
                         $elm$core$Basics$min,
-                        date.dW,
+                        date.dY,
                         A2($justinmimbs$date$Date$daysInMonth, y, m));
                 case 2:
                     return rd + (7 * n);
                 default:
                     return rd + n;
             }
         });
@@ -15032,15 +15140,15 @@
     var $justinmimbs$date$Date$firstOfYear = function(y) {
         return $justinmimbs$date$Date$daysBeforeYear(y) + 1;
     };
     var $justinmimbs$date$Date$month = A2(
         $elm$core$Basics$composeR,
         $justinmimbs$date$Date$toCalendarDate,
         function($) {
-            return $.ex;
+            return $.ey;
         });
     var $justinmimbs$date$Date$monthToQuarter = function(m) {
         return (($justinmimbs$date$Date$monthToNumber(m) + 2) / 3) | 0;
     };
     var $justinmimbs$date$Date$quarter = A2($elm$core$Basics$composeR, $justinmimbs$date$Date$month, $justinmimbs$date$Date$monthToQuarter);
     var $justinmimbs$date$Date$quarterToMonth = function(q) {
         return $justinmimbs$date$Date$numberToMonth((q * 3) - 2);
@@ -15166,62 +15274,62 @@
     var $terezka$intervals$Intervals$Time$ceilingDay = F3(
         function(zone, mult, stamp) {
             return (mult === 7) ? A3($justinmimbs$time_extra$Time$Extra$ceiling, 3, zone, stamp) : A3($justinmimbs$time_extra$Time$Extra$ceiling, 11, zone, stamp);
         });
     var $justinmimbs$time_extra$Time$Extra$Hour = 12;
     var $justinmimbs$time_extra$Time$Extra$partsToPosix = F2(
         function(zone, _v0) {
-            var year = _v0.fl;
-            var month = _v0.ex;
-            var day = _v0.dW;
-            var hour = _v0.c0;
-            var minute = _v0.dd;
-            var second = _v0.dr;
-            var millisecond = _v0.dc;
+            var year = _v0.fm;
+            var month = _v0.ey;
+            var day = _v0.dY;
+            var hour = _v0.c2;
+            var minute = _v0.df;
+            var second = _v0.dt;
+            var millisecond = _v0.de;
             return A3(
                 $justinmimbs$time_extra$Time$Extra$posixFromDateTime,
                 zone,
                 A3($justinmimbs$date$Date$fromCalendarDate, year, month, day),
                 A4(
                     $justinmimbs$time_extra$Time$Extra$timeFromClock,
                     A3($elm$core$Basics$clamp, 0, 23, hour),
                     A3($elm$core$Basics$clamp, 0, 59, minute),
                     A3($elm$core$Basics$clamp, 0, 59, second),
                     A3($elm$core$Basics$clamp, 0, 999, millisecond)));
         });
     var $justinmimbs$time_extra$Time$Extra$posixToParts = F2(
         function(zone, posix) {
             return {
-                dW: A2($elm$time$Time$toDay, zone, posix),
-                c0: A2($elm$time$Time$toHour, zone, posix),
-                dc: A2($elm$time$Time$toMillis, zone, posix),
-                dd: A2($elm$time$Time$toMinute, zone, posix),
-                ex: A2($elm$time$Time$toMonth, zone, posix),
-                dr: A2($elm$time$Time$toSecond, zone, posix),
-                fl: A2($elm$time$Time$toYear, zone, posix)
+                dY: A2($elm$time$Time$toDay, zone, posix),
+                c2: A2($elm$time$Time$toHour, zone, posix),
+                de: A2($elm$time$Time$toMillis, zone, posix),
+                df: A2($elm$time$Time$toMinute, zone, posix),
+                ey: A2($elm$time$Time$toMonth, zone, posix),
+                dt: A2($elm$time$Time$toSecond, zone, posix),
+                fm: A2($elm$time$Time$toYear, zone, posix)
             };
         });
     var $terezka$intervals$Intervals$Time$ceilingHour = F3(
         function(zone, mult, stamp) {
             var parts = A2(
                 $justinmimbs$time_extra$Time$Extra$posixToParts,
                 zone,
                 A3($justinmimbs$time_extra$Time$Extra$ceiling, 12, zone, stamp));
-            var rem = parts.c0 % mult;
+            var rem = parts.c2 % mult;
             var _new = A2($justinmimbs$time_extra$Time$Extra$partsToPosix, zone, parts);
             return (!rem) ? _new : A4($justinmimbs$time_extra$Time$Extra$add, 12, mult - rem, zone, _new);
         });
     var $justinmimbs$time_extra$Time$Extra$Minute = 13;
     var $terezka$intervals$Intervals$Time$ceilingMinute = F3(
         function(zone, mult, stamp) {
             var parts = A2(
                 $justinmimbs$time_extra$Time$Extra$posixToParts,
                 zone,
                 A3($justinmimbs$time_extra$Time$Extra$ceiling, 13, zone, stamp));
-            var rem = parts.dd % mult;
+            var rem = parts.df % mult;
             var _new = A2($justinmimbs$time_extra$Time$Extra$partsToPosix, zone, parts);
             return (!rem) ? _new : A4($justinmimbs$time_extra$Time$Extra$add, 13, mult - rem, zone, _new);
         });
     var $terezka$intervals$Intervals$Time$intAsMonth = function(_int) {
         switch (_int) {
             case 1:
                 return 0;
@@ -15281,61 +15389,61 @@
     };
     var $terezka$intervals$Intervals$Time$ceilingMonth = F3(
         function(zone, mult, stamp) {
             var parts = A2(
                 $justinmimbs$time_extra$Time$Extra$posixToParts,
                 zone,
                 A3($justinmimbs$time_extra$Time$Extra$ceiling, 2, zone, stamp));
-            var monthInt = $terezka$intervals$Intervals$Time$monthAsInt(parts.ex);
+            var monthInt = $terezka$intervals$Intervals$Time$monthAsInt(parts.ey);
             var rem = (monthInt - 1) % mult;
             var newMonth = (!rem) ? monthInt : ((monthInt - rem) + mult);
             return A2(
                 $justinmimbs$time_extra$Time$Extra$partsToPosix,
                 zone,
                 (newMonth > 12) ? _Utils_update(
                     parts, {
-                        ex: $terezka$intervals$Intervals$Time$intAsMonth(newMonth - 12),
-                        fl: parts.fl + 1
+                        ey: $terezka$intervals$Intervals$Time$intAsMonth(newMonth - 12),
+                        fm: parts.fm + 1
                     }) : _Utils_update(
                     parts, {
-                        ex: $terezka$intervals$Intervals$Time$intAsMonth(newMonth)
+                        ey: $terezka$intervals$Intervals$Time$intAsMonth(newMonth)
                     }));
         });
     var $terezka$intervals$Intervals$Time$ceilingMs = F3(
         function(zone, mult, stamp) {
             var parts = A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, stamp);
-            var rem = parts.dc % mult;
+            var rem = parts.de % mult;
             return (!rem) ? A2($justinmimbs$time_extra$Time$Extra$partsToPosix, zone, parts) : A4($justinmimbs$time_extra$Time$Extra$add, 15, mult - rem, zone, stamp);
         });
     var $justinmimbs$time_extra$Time$Extra$Second = 14;
     var $terezka$intervals$Intervals$Time$ceilingSecond = F3(
         function(zone, mult, stamp) {
             var parts = A2(
                 $justinmimbs$time_extra$Time$Extra$posixToParts,
                 zone,
                 A3($justinmimbs$time_extra$Time$Extra$ceiling, 14, zone, stamp));
-            var rem = parts.dr % mult;
+            var rem = parts.dt % mult;
             var _new = A2($justinmimbs$time_extra$Time$Extra$partsToPosix, zone, parts);
             return (!rem) ? _new : A4($justinmimbs$time_extra$Time$Extra$add, 14, mult - rem, zone, _new);
         });
     var $justinmimbs$time_extra$Time$Extra$Year = 0;
     var $terezka$intervals$Intervals$Time$ceilingYear = F3(
         function(zone, mult, stamp) {
             var parts = A2(
                 $justinmimbs$time_extra$Time$Extra$posixToParts,
                 zone,
                 A3($justinmimbs$time_extra$Time$Extra$ceiling, 0, zone, stamp));
-            var rem = parts.fl % mult;
-            var newYear = (!rem) ? parts.fl : ((parts.fl - rem) + mult);
+            var rem = parts.fm % mult;
+            var newYear = (!rem) ? parts.fm : ((parts.fm - rem) + mult);
             return A2(
                 $justinmimbs$time_extra$Time$Extra$partsToPosix,
                 zone,
                 _Utils_update(
                     parts, {
-                        fl: newYear
+                        fm: newYear
                     }));
         });
     var $terezka$intervals$Intervals$Time$ceilingUnit = F3(
         function(zone, unit, mult) {
             switch (unit) {
                 case 0:
                     return A2($terezka$intervals$Intervals$Time$ceilingMs, zone, mult);
@@ -15360,15 +15468,15 @@
     var $terezka$intervals$Intervals$Time$Month = 5;
     var $terezka$intervals$Intervals$Time$Second = 1;
     var $terezka$intervals$Intervals$Time$Year = 6;
     var $terezka$intervals$Intervals$Time$getChange = F3(
         function(zone, a, b) {
             var bP = A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, b);
             var aP = A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, a);
-            return (!_Utils_eq(aP.fl, bP.fl)) ? 6 : ((!_Utils_eq(aP.ex, bP.ex)) ? 5 : ((!_Utils_eq(aP.dW, bP.dW)) ? 4 : ((!_Utils_eq(aP.c0, bP.c0)) ? 3 : ((!_Utils_eq(aP.dd, bP.dd)) ? 2 : ((!_Utils_eq(aP.dr, bP.dr)) ? 1 : 0)))));
+            return (!_Utils_eq(aP.fm, bP.fm)) ? 6 : ((!_Utils_eq(aP.ey, bP.ey)) ? 5 : ((!_Utils_eq(aP.dY, bP.dY)) ? 4 : ((!_Utils_eq(aP.c2, bP.c2)) ? 3 : ((!_Utils_eq(aP.df, bP.df)) ? 2 : ((!_Utils_eq(aP.dt, bP.dt)) ? 1 : 0)))));
         });
     var $danhandrea$elm_time_extra$Util$isLeapYear = function(year) {
         return (!A2($elm$core$Basics$modBy, 400, year)) || ((!(!A2($elm$core$Basics$modBy, 100, year))) && (!A2($elm$core$Basics$modBy, 4, year)));
     };
     var $danhandrea$elm_time_extra$Month$days = F2(
         function(year, month) {
             switch (month) {
@@ -15407,36 +15515,36 @@
                 $terezka$intervals$Intervals$Time$toMs(b)) < 0) ? _Utils_Tuple2(
                 A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, a),
                 A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, b)) : _Utils_Tuple2(
                 A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, b),
                 A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, a));
             var aP = _v0.a;
             var bP = _v0.b;
-            var dMsX = bP.dc - aP.dc;
+            var dMsX = bP.de - aP.de;
             var dMs = (dMsX < 0) ? (1000 + dMsX) : dMsX;
-            var dSecondX = (bP.dr - aP.dr) + ((dMsX < 0) ? (-1) : 0);
-            var dMinuteX = (bP.dd - aP.dd) + ((dSecondX < 0) ? (-1) : 0);
-            var dHourX = (bP.c0 - aP.c0) + ((dMinuteX < 0) ? (-1) : 0);
-            var dDayX = (bP.dW - aP.dW) + ((dHourX < 0) ? (-1) : 0);
-            var dDay = (dDayX < 0) ? (A2($danhandrea$elm_time_extra$TimeExtra$daysInMonth, bP.fl, bP.ex) + dDayX) : dDayX;
-            var dMonthX = ($terezka$intervals$Intervals$Time$monthAsInt(bP.ex) - $terezka$intervals$Intervals$Time$monthAsInt(aP.ex)) + ((dDayX < 0) ? (-1) : 0);
+            var dSecondX = (bP.dt - aP.dt) + ((dMsX < 0) ? (-1) : 0);
+            var dMinuteX = (bP.df - aP.df) + ((dSecondX < 0) ? (-1) : 0);
+            var dHourX = (bP.c2 - aP.c2) + ((dMinuteX < 0) ? (-1) : 0);
+            var dDayX = (bP.dY - aP.dY) + ((dHourX < 0) ? (-1) : 0);
+            var dDay = (dDayX < 0) ? (A2($danhandrea$elm_time_extra$TimeExtra$daysInMonth, bP.fm, bP.ey) + dDayX) : dDayX;
+            var dMonthX = ($terezka$intervals$Intervals$Time$monthAsInt(bP.ey) - $terezka$intervals$Intervals$Time$monthAsInt(aP.ey)) + ((dDayX < 0) ? (-1) : 0);
             var dMonth = (dMonthX < 0) ? (12 + dMonthX) : dMonthX;
             var dHour = (dHourX < 0) ? (24 + dHourX) : dHourX;
             var dMinute = (dMinuteX < 0) ? (60 + dMinuteX) : dMinuteX;
             var dSecond = (dSecondX < 0) ? (60 + dSecondX) : dSecondX;
-            var dYearX = (bP.fl - aP.fl) + ((dMonthX < 0) ? (-1) : 0);
-            var dYear = (dYearX < 0) ? ($terezka$intervals$Intervals$Time$monthAsInt(bP.ex) + dYearX) : dYearX;
+            var dYearX = (bP.fm - aP.fm) + ((dMonthX < 0) ? (-1) : 0);
+            var dYear = (dYearX < 0) ? ($terezka$intervals$Intervals$Time$monthAsInt(bP.ey) + dYearX) : dYearX;
             return {
-                dW: dDay,
-                c0: dHour,
-                dc: dMs,
-                dd: dMinute,
-                ex: dMonth,
-                dr: dSecond,
-                fl: dYear
+                dY: dDay,
+                c2: dHour,
+                de: dMs,
+                df: dMinute,
+                ey: dMonth,
+                dt: dSecond,
+                fm: dYear
             };
         });
     var $terezka$intervals$Intervals$Time$oneSecond = 1000;
     var $terezka$intervals$Intervals$Time$oneMinute = $terezka$intervals$Intervals$Time$oneSecond * 60;
     var $terezka$intervals$Intervals$Time$oneHour = $terezka$intervals$Intervals$Time$oneMinute * 60;
     var $terezka$intervals$Intervals$Time$oneDay = $terezka$intervals$Intervals$Time$oneHour * 24;
     var $terezka$intervals$Intervals$Time$oneMs = 1;
@@ -15478,20 +15586,20 @@
                 case 3:
                     return timeDiff($terezka$intervals$Intervals$Time$oneHour) + 1;
                 case 4:
                     return timeDiff($terezka$intervals$Intervals$Time$oneDay) + 1;
                 case 5:
                     return diff(
                         function(d) {
-                            return d.ex + (d.fl * 12);
+                            return d.ey + (d.fm * 12);
                         }) + 1;
                 default:
                     return diff(
                         function($) {
-                            return $.fl;
+                            return $.fm;
                         }) + 1;
             }
         });
     var $terezka$intervals$Intervals$Time$largerUnit = function(unit) {
         switch (unit) {
             case 0:
                 return $elm$core$Maybe$Just(1);
@@ -15613,22 +15721,22 @@
             var mult = _v0.b;
             var amount = A5($terezka$intervals$Intervals$Time$getNumOfTicks, zone, unit, mult, min, max);
             var initial = A4($terezka$intervals$Intervals$Time$ceilingUnit, zone, unit, mult, min);
             var tUnit = $terezka$intervals$Intervals$Time$toExtraUnit(unit);
             var toTick = F3(
                 function(x, timestamp, change) {
                     return {
-                        fu: (_Utils_cmp(
+                        fv: (_Utils_cmp(
                             $terezka$intervals$Intervals$Time$unitToInt(change),
                             $terezka$intervals$Intervals$Time$unitToInt(unit)) > 0) ? $elm$core$Maybe$Just(change) : $elm$core$Maybe$Nothing,
-                        da: !x,
-                        fY: mult,
-                        gh: timestamp,
-                        gt: unit,
-                        dJ: zone
+                        dc: !x,
+                        fZ: mult,
+                        gi: timestamp,
+                        gu: unit,
+                        dL: zone
                     };
                 });
             var toTicks = F2(
                 function(xs, acc) {
                     toTicks: while (true) {
                         if (xs.b) {
                             var x = xs.a;
@@ -15673,57 +15781,57 @@
                         return 5;
                     default:
                         return 6;
                 }
             };
             var translateUnit = function(time) {
                 return {
-                    fu: A2($elm$core$Maybe$map, toUnit, time.fu),
-                    da: time.da,
-                    fY: time.fY,
-                    gh: time.gh,
-                    gt: toUnit(time.gt),
-                    dJ: time.dJ
+                    fv: A2($elm$core$Maybe$map, toUnit, time.fv),
+                    dc: time.dc,
+                    fZ: time.fZ,
+                    gi: time.gi,
+                    gu: toUnit(time.gu),
+                    dL: time.dL
                 };
             };
             var fromMs = function(ts) {
                 return $elm$time$Time$millisToPosix(
                     $elm$core$Basics$round(ts));
             };
             return A2(
                 $elm$core$List$map,
                 translateUnit,
                 A4(
                     $terezka$intervals$Intervals$Time$values,
                     zone,
                     amount,
-                    fromMs(range.ev),
-                    fromMs(range.et)));
+                    fromMs(range.ew),
+                    fromMs(range.eu)));
         });
     var $terezka$elm_charts$Internal$Svg$times = function(zone) {
         return F2(
             function(i, b) {
                 return A3(
                     $terezka$intervals$Intervals$times,
                     zone,
                     i, {
-                        et: b.et,
-                        ev: b.ev
+                        eu: b.eu,
+                        ew: b.ew
                     });
             });
     };
     var $terezka$elm_charts$Chart$Svg$times = $terezka$elm_charts$Internal$Svg$times;
     var $terezka$elm_charts$Chart$generateValues = F4(
         function(amount, tick, maybeFormat, axis) {
             var toTickValues = F2(
                 function(toValue, toString) {
                     return $elm$core$List$map(
                         function(i) {
                             return {
-                                em: function() {
+                                en: function() {
                                     if (!maybeFormat.$) {
                                         var formatter = maybeFormat.a;
                                         return formatter(
                                             toValue(i));
                                     } else {
                                         return toString(i);
                                     }
@@ -15749,15 +15857,15 @@
                     var zone = tick.a;
                     return A3(
                         toTickValues,
                         A2(
                             $elm$core$Basics$composeL,
                             A2($elm$core$Basics$composeL, $elm$core$Basics$toFloat, $elm$time$Time$posixToMillis),
                             function($) {
-                                return $.gh;
+                                return $.gi;
                             }),
                         $terezka$elm_charts$Chart$Svg$formatTime(zone),
                         A3(
                             $terezka$elm_charts$Chart$Svg$generate,
                             amount,
                             $terezka$elm_charts$Chart$Svg$times(zone),
                             axis));
@@ -15822,24 +15930,24 @@
                                 return 'text-anchor: middle;';
                         }
                     }
                 }();
                 return withOverflowWrap(
                     A4(
                         $terezka$elm_charts$Internal$Svg$withAttrs,
-                        config.bu,
+                        config.bw,
                         $elm$svg$Svg$text_,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__label'),
                                 $elm$svg$Svg$Attributes$stroke(config.v),
                                 $elm$svg$Svg$Attributes$strokeWidth(
                                     $elm$core$String$fromFloat(config.x)),
-                                $elm$svg$Svg$Attributes$fill(config.bC),
-                                A6($terezka$elm_charts$Internal$Svg$position, plane, -config.o, point.fj, point.fk, config.g, config.h),
+                                $elm$svg$Svg$Attributes$fill(config.bE),
+                                A6($terezka$elm_charts$Internal$Svg$position, plane, -config.o, point.fk, point.fl, config.g, config.h),
                                 $elm$svg$Svg$Attributes$style(
                                     A2(
                                         $elm$core$String$join,
                                         ' ',
                                         _List_fromArray(
                                             ['pointer-events: none;', fontStyle, anchorStyle, uppercaseStyle])))
                             ]),
@@ -15848,26 +15956,26 @@
                                 A2($elm$svg$Svg$tspan, _List_Nil, inner)
                             ])));
             } else {
                 var ellipsis = _v0.a;
                 var xOffWithAnchor = function() {
                     var _v11 = config.i;
                     if (_v11.$ === 1) {
-                        return config.g - (ellipsis.fi / 2);
+                        return config.g - (ellipsis.fj / 2);
                     } else {
                         switch (_v11.a) {
                             case 0:
                                 var _v12 = _v11.a;
-                                return config.g - ellipsis.fi;
+                                return config.g - ellipsis.fj;
                             case 1:
                                 var _v13 = _v11.a;
                                 return config.g;
                             default:
                                 var _v14 = _v11.a;
-                                return config.g - (ellipsis.fi / 2);
+                                return config.g - (ellipsis.fj / 2);
                         }
                     }
                 }();
                 var withOverflowWrap = function(el) {
                     return config.l ? A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
@@ -15907,49 +16015,49 @@
                                 return A2($elm$html$Html$Attributes$style, 'text-align', 'center');
                         }
                     }
                 }();
                 return withOverflowWrap(
                     A4(
                         $terezka$elm_charts$Internal$Svg$withAttrs,
-                        config.bu,
+                        config.bw,
                         $elm$svg$Svg$foreignObject,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__label'),
                                 $elm$svg$Svg$Attributes$class('elm-charts__html-label'),
                                 $elm$svg$Svg$Attributes$width(
-                                    $elm$core$String$fromFloat(ellipsis.fi)),
+                                    $elm$core$String$fromFloat(ellipsis.fj)),
                                 $elm$svg$Svg$Attributes$height(
-                                    $elm$core$String$fromFloat(ellipsis.ea)),
-                                A6($terezka$elm_charts$Internal$Svg$position, plane, -config.o, point.fj, point.fk, xOffWithAnchor, config.h - 10)
+                                    $elm$core$String$fromFloat(ellipsis.eb)),
+                                A6($terezka$elm_charts$Internal$Svg$position, plane, -config.o, point.fk, point.fl, xOffWithAnchor, config.h - 10)
                             ]),
                         _List_fromArray(
                             [
                                 A2(
                                     $elm$html$Html$div,
                                     _List_fromArray(
                                         [
                                             A2($elm$html$Html$Attributes$attribute, 'xmlns', 'http://www.w3.org/1999/xhtml'),
                                             A2($elm$html$Html$Attributes$style, 'white-space', 'nowrap'),
                                             A2($elm$html$Html$Attributes$style, 'overflow', 'hidden'),
                                             A2($elm$html$Html$Attributes$style, 'text-overflow', 'ellipsis'),
                                             A2($elm$html$Html$Attributes$style, 'height', '100%'),
                                             A2($elm$html$Html$Attributes$style, 'pointer-events', 'none'),
-                                            A2($elm$html$Html$Attributes$style, 'color', config.bC),
+                                            A2($elm$html$Html$Attributes$style, 'color', config.bE),
                                             fontStyle,
                                             uppercaseStyle,
                                             anchorStyle
                                         ]),
                                     inner)
                             ])));
             }
         });
     var $terezka$elm_charts$Chart$Attributes$zero = function(b) {
-        return A3($elm$core$Basics$clamp, b.ev, b.et, 0);
+        return A3($elm$core$Basics$clamp, b.ew, b.eu, 0);
     };
     var $terezka$elm_charts$Chart$xLabels = function(edits) {
         var toTicks = F2(
             function(p, config) {
                 return A4(
                     $terezka$elm_charts$Chart$generateValues,
                     config.K,
@@ -15957,15 +16065,15 @@
                     config.F,
                     A3(
                         $elm$core$List$foldl,
                         F2(
                             function(f, x) {
                                 return f(x);
                             }),
-                        p.fj,
+                        p.fk,
                         config.t));
             });
         var toTickValues = F3(
             function(p, config, ts) {
                 return (!config.f) ? ts : _Utils_update(
                     ts, {
                         A: _Utils_ap(
@@ -15980,16 +16088,16 @@
             });
         var toConfig = function(p) {
             return A2(
                 $terezka$elm_charts$Internal$Helpers$apply,
                 edits, {
                     K: 5,
                     i: $elm$core$Maybe$Nothing,
-                    bu: _List_Nil,
-                    bC: '#808BAB',
+                    bw: _List_Nil,
+                    bE: '#808BAB',
                     j: $elm$core$Maybe$Nothing,
                     e: false,
                     k: $elm$core$Maybe$Nothing,
                     F: $elm$core$Maybe$Nothing,
                     N: $terezka$elm_charts$Internal$Svg$Floats,
                     f: false,
                     l: false,
@@ -16011,30 +16119,30 @@
                     var toLabel = function(item) {
                         return A4(
                             $terezka$elm_charts$Internal$Svg$label,
                             p,
                             _Utils_update(
                                 _default, {
                                     i: config.i,
-                                    bu: config.bu,
-                                    bC: config.bC,
+                                    bw: config.bw,
+                                    bE: config.bE,
                                     j: config.j,
                                     k: config.k,
                                     l: config.l,
                                     o: config.o,
                                     p: config.p,
                                     g: config.g,
                                     h: config.e ? ((-config.h) + 10) : config.h
                                 }),
                             _List_fromArray(
                                 [
-                                    $elm$svg$Svg$text(item.em)
+                                    $elm$svg$Svg$text(item.en)
                                 ]), {
-                                fj: item.Z,
-                                fk: config.n(p.fk)
+                                fk: item.Z,
+                                fl: config.n(p.fl)
                             });
                     };
                     return A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__x-labels')
@@ -16056,15 +16164,15 @@
                     config.F,
                     A3(
                         $elm$core$List$foldl,
                         F2(
                             function(f, y) {
                                 return f(y);
                             }),
-                        p.fk,
+                        p.fl,
                         config.t));
             });
         var toTickValues = F3(
             function(p, config, ts) {
                 return (!config.f) ? ts : _Utils_update(
                     ts, {
                         J: _Utils_ap(
@@ -16079,16 +16187,16 @@
             });
         var toConfig = function(p) {
             return A2(
                 $terezka$elm_charts$Internal$Helpers$apply,
                 edits, {
                     K: 5,
                     i: $elm$core$Maybe$Nothing,
-                    bu: _List_Nil,
-                    bC: '#808BAB',
+                    bw: _List_Nil,
+                    bE: '#808BAB',
                     j: $elm$core$Maybe$Nothing,
                     e: false,
                     k: $elm$core$Maybe$Nothing,
                     F: $elm$core$Maybe$Nothing,
                     N: $terezka$elm_charts$Internal$Svg$Floats,
                     f: false,
                     l: false,
@@ -16119,30 +16227,30 @@
                                             return $elm$core$Maybe$Just(
                                                 config.e ? 1 : 0);
                                         } else {
                                             var anchor = _v0.a;
                                             return $elm$core$Maybe$Just(anchor);
                                         }
                                     }(),
-                                    bu: config.bu,
-                                    bC: config.bC,
+                                    bw: config.bw,
+                                    bE: config.bE,
                                     j: config.j,
                                     k: config.k,
                                     l: config.l,
                                     o: config.o,
                                     p: config.p,
                                     g: config.e ? (-config.g) : config.g,
                                     h: config.h
                                 }),
                             _List_fromArray(
                                 [
-                                    $elm$svg$Svg$text(item.em)
+                                    $elm$svg$Svg$text(item.en)
                                 ]), {
-                                fj: config.n(p.fj),
-                                fk: item.Z
+                                fk: config.n(p.fk),
+                                fl: item.Z
                             });
                     };
                     return A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__y-labels')
@@ -16158,18 +16266,18 @@
             return A2(
                 $terezka$elm_charts$Chart$chart,
                 _List_fromArray(
                     [
                         $terezka$elm_charts$Chart$Attributes$height(200),
                         $terezka$elm_charts$Chart$Attributes$width(800),
                         $terezka$elm_charts$Chart$Attributes$margin({
-                            dO: 0,
-                            er: 40,
-                            eW: 20,
-                            fb: 0
+                            dQ: 0,
+                            es: 40,
+                            eX: 20,
+                            fc: 0
                         }),
                         A2(
                             $terezka$elm_charts$Chart$Events$onMouseMove,
                             onHover,
                             $terezka$elm_charts$Chart$Events$getNearest($terezka$elm_charts$Chart$Item$dots)),
                         $terezka$elm_charts$Chart$Events$onMouseLeave(
                             onHover(_List_Nil))
@@ -16177,66 +16285,74 @@
                 _List_fromArray(
                     [
                         $terezka$elm_charts$Chart$xLabels(
                             _List_fromArray(
                                 [
                                     $terezka$elm_charts$Chart$Attributes$fontSize(10),
                                     $terezka$elm_charts$Chart$Attributes$withGrid,
-                                    $terezka$elm_charts$Chart$Attributes$format($author$project$Graph$formatTime)
+                                    $terezka$elm_charts$Chart$Attributes$format(
+                                        function(time) {
+                                            return A2($author$project$Graph$formatTime, time, graphModel.aJ);
+                                        })
                                 ])),
                         $terezka$elm_charts$Chart$yLabels(
                             _List_fromArray(
                                 [
                                     $terezka$elm_charts$Chart$Attributes$fontSize(10),
                                     $terezka$elm_charts$Chart$Attributes$withGrid
                                 ])),
                         A3(
                             $terezka$elm_charts$Chart$series,
                             function($) {
-                                return $.cF;
+                                return $.aI;
                             },
                             _List_fromArray(
                                 [
                                     A2(
                                         $terezka$elm_charts$Chart$named,
                                         'EPA',
                                         A3(
                                             $terezka$elm_charts$Chart$interpolated,
                                             function($) {
-                                                return $.d$;
+                                                return $.c_;
                                             },
                                             _List_fromArray(
                                                 [
                                                     $terezka$elm_charts$Chart$Attributes$monotone,
                                                     $terezka$elm_charts$Chart$Attributes$color($terezka$elm_charts$Chart$Attributes$blue)
                                                 ]),
                                             _List_fromArray(
                                                 [
                                                     $terezka$elm_charts$Chart$Attributes$circle,
                                                     $terezka$elm_charts$Chart$Attributes$size(3)
                                                 ])))
                                 ]),
-                            graphModel.bM),
+                            graphModel.bO),
                         A2(
                             $terezka$elm_charts$Chart$each,
-                            graphModel.bD,
+                            graphModel.bF,
                             F2(
                                 function(p, item) {
                                     return _List_fromArray(
                                         [
-                                            A4($terezka$elm_charts$Chart$tooltip, item, _List_Nil, _List_Nil, _List_Nil)
+                                            A4(
+                                                $terezka$elm_charts$Chart$tooltip,
+                                                item,
+                                                _List_Nil,
+                                                _List_Nil,
+                                                A2($author$project$Graph$getEpaToolTip, item, graphModel.aJ))
                                         ]);
                                 })),
                         A4(
                             $terezka$elm_charts$Chart$legendsAt,
                             function($) {
-                                return $.ev;
+                                return $.ew;
                             },
                             function($) {
-                                return $.et;
+                                return $.eu;
                             },
                             _List_fromArray(
                                 [
                                     $terezka$elm_charts$Chart$Attributes$row,
                                     $terezka$elm_charts$Chart$Attributes$alignLeft,
                                     $terezka$elm_charts$Chart$Attributes$spacing(5),
                                     $terezka$elm_charts$Chart$Attributes$background('Azure'),
@@ -16362,29 +16478,97 @@
                         $author$project$EpaLevel$getRow,
                         5,
                         _Utils_eq(
                             currentLevel,
                             $elm$core$Maybe$Just(5)))
                 ]));
     };
+    var $terezka$elm_charts$Internal$Item$getName = function(_v0) {
+        var item = _v0;
+        var _v1 = item.fw.cI.f_;
+        if (!_v1.$) {
+            var name = _v1.a;
+            return name;
+        } else {
+            return 'Property #' + $elm$core$String$fromInt(item.fw.cI.fQ + 1);
+        }
+    };
+    var $terezka$elm_charts$Chart$Item$getName = $terezka$elm_charts$Internal$Item$getName;
+    var $terezka$elm_charts$Internal$Item$getTooltipValue = function(_v0) {
+        var item = _v0;
+        return item.fw.cI.d7;
+    };
+    var $terezka$elm_charts$Chart$Item$getTooltipValue = $terezka$elm_charts$Internal$Item$getTooltipValue;
+    var $author$project$Graph$getPmToolTip = F2(
+        function(item, timeZone) {
+            var value = $terezka$elm_charts$Chart$Item$getTooltipValue(item);
+            var label = $terezka$elm_charts$Chart$Item$getName(item);
+            var data = $terezka$elm_charts$Chart$Item$getData(item);
+            var formattedTime = A2($author$project$Graph$formatTime, data.aI, timeZone);
+            var color = $terezka$elm_charts$Chart$Item$getColor(item);
+            return _List_fromArray(
+                [
+                    A2(
+                        $elm$html$Html$div,
+                        _List_Nil,
+                        _List_fromArray(
+                            [
+                                A2(
+                                    $elm$html$Html$span,
+                                    _List_fromArray(
+                                        [
+                                            A2($elm$html$Html$Attributes$style, 'color', color)
+                                        ]),
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$text(label)
+                                        ])),
+                                A2(
+                                    $elm$html$Html$span,
+                                    _List_Nil,
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$text(': ' + value)
+                                        ])),
+                                A2($elm$html$Html$br, _List_Nil, _List_Nil),
+                                A2(
+                                    $elm$html$Html$span,
+                                    _List_fromArray(
+                                        [
+                                            A2($elm$html$Html$Attributes$style, 'color', color)
+                                        ]),
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$text('Time')
+                                        ])),
+                                A2(
+                                    $elm$html$Html$span,
+                                    _List_Nil,
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$text(': ' + formattedTime)
+                                        ]))
+                            ]))
+                ]);
+        });
     var $terezka$elm_charts$Chart$Attributes$red = $terezka$elm_charts$Internal$Helpers$red;
     var $terezka$elm_charts$Chart$Attributes$yellow = $terezka$elm_charts$Internal$Helpers$yellow;
     var $author$project$Graph$getReadChart = F2(
         function(graphModel, onHover) {
             return A2(
                 $terezka$elm_charts$Chart$chart,
                 _List_fromArray(
                     [
                         $terezka$elm_charts$Chart$Attributes$height(200),
                         $terezka$elm_charts$Chart$Attributes$width(800),
                         $terezka$elm_charts$Chart$Attributes$margin({
-                            dO: 0,
-                            er: 40,
-                            eW: 20,
-                            fb: 0
+                            dQ: 0,
+                            es: 40,
+                            eX: 20,
+                            fc: 0
                         }),
                         A2(
                             $terezka$elm_charts$Chart$Events$onMouseMove,
                             onHover,
                             $terezka$elm_charts$Chart$Events$getNearest($terezka$elm_charts$Chart$Item$dots)),
                         $terezka$elm_charts$Chart$Events$onMouseLeave(
                             onHover(_List_Nil))
@@ -16392,36 +16576,39 @@
                 _List_fromArray(
                     [
                         $terezka$elm_charts$Chart$xLabels(
                             _List_fromArray(
                                 [
                                     $terezka$elm_charts$Chart$Attributes$fontSize(10),
                                     $terezka$elm_charts$Chart$Attributes$withGrid,
-                                    $terezka$elm_charts$Chart$Attributes$format($author$project$Graph$formatTime)
+                                    $terezka$elm_charts$Chart$Attributes$format(
+                                        function(time) {
+                                            return A2($author$project$Graph$formatTime, time, graphModel.aJ);
+                                        })
                                 ])),
                         $terezka$elm_charts$Chart$yLabels(
                             _List_fromArray(
                                 [
                                     $terezka$elm_charts$Chart$Attributes$fontSize(10),
                                     $terezka$elm_charts$Chart$Attributes$withGrid
                                 ])),
                         A3(
                             $terezka$elm_charts$Chart$series,
                             function($) {
-                                return $.cF;
+                                return $.aI;
                             },
                             _List_fromArray(
                                 [
                                     A2(
                                         $terezka$elm_charts$Chart$named,
                                         'PM2.5',
                                         A3(
                                             $terezka$elm_charts$Chart$interpolated,
                                             function($) {
-                                                return $.eG;
+                                                return $.eH;
                                             },
                                             _List_fromArray(
                                                 [
                                                     $terezka$elm_charts$Chart$Attributes$monotone,
                                                     $terezka$elm_charts$Chart$Attributes$color($terezka$elm_charts$Chart$Attributes$yellow)
                                                 ]),
                                             _List_fromArray(
@@ -16431,45 +16618,50 @@
                                                 ]))),
                                     A2(
                                         $terezka$elm_charts$Chart$named,
                                         'PM10',
                                         A3(
                                             $terezka$elm_charts$Chart$interpolated,
                                             function($) {
-                                                return $.eF;
+                                                return $.eG;
                                             },
                                             _List_fromArray(
                                                 [
                                                     $terezka$elm_charts$Chart$Attributes$monotone,
                                                     $terezka$elm_charts$Chart$Attributes$color($terezka$elm_charts$Chart$Attributes$red)
                                                 ]),
                                             _List_fromArray(
                                                 [
                                                     $terezka$elm_charts$Chart$Attributes$circle,
                                                     $terezka$elm_charts$Chart$Attributes$size(3)
                                                 ])))
                                 ]),
-                            graphModel.bM),
+                            graphModel.bO),
                         A2(
                             $terezka$elm_charts$Chart$each,
-                            graphModel.bD,
+                            graphModel.bF,
                             F2(
                                 function(p, item) {
                                     return _List_fromArray(
                                         [
-                                            A4($terezka$elm_charts$Chart$tooltip, item, _List_Nil, _List_Nil, _List_Nil)
+                                            A4(
+                                                $terezka$elm_charts$Chart$tooltip,
+                                                item,
+                                                _List_Nil,
+                                                _List_Nil,
+                                                A2($author$project$Graph$getPmToolTip, item, graphModel.aJ))
                                         ]);
                                 })),
                         A4(
                             $terezka$elm_charts$Chart$legendsAt,
                             function($) {
-                                return $.ev;
+                                return $.ew;
                             },
                             function($) {
-                                return $.et;
+                                return $.eu;
                             },
                             _List_fromArray(
                                 [
                                     $terezka$elm_charts$Chart$Attributes$row,
                                     $terezka$elm_charts$Chart$Attributes$alignLeft,
                                     $terezka$elm_charts$Chart$Attributes$spacing(5),
                                     $terezka$elm_charts$Chart$Attributes$background('Azure'),
@@ -16485,15 +16677,15 @@
                                 [
                                     $terezka$elm_charts$Chart$Attributes$fontSize(12)
                                 ]))
                     ]));
         });
     var $author$project$Main$ChangeWindow = function(a) {
         return {
-            $: 6,
+            $: 7,
             a: a
         };
     };
     var $rundis$elm_bootstrap$Bootstrap$Internal$Button$Attrs = function(a) {
         return {
             $: 4,
             a: a
@@ -16560,57 +16752,57 @@
     var $rundis$elm_bootstrap$Bootstrap$Internal$Button$applyModifier = F2(
         function(modifier, options) {
             switch (modifier.$) {
                 case 0:
                     var size = modifier.a;
                     return _Utils_update(
                         options, {
-                            e1: $elm$core$Maybe$Just(size)
+                            e2: $elm$core$Maybe$Just(size)
                         });
                 case 1:
                     var coloring = modifier.a;
                     return _Utils_update(
                         options, {
                             ab: $elm$core$Maybe$Just(coloring)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            bw: true
+                            by: true
                         });
                 case 3:
                     var val = modifier.a;
                     return _Utils_update(
                         options, {
-                            bI: val
+                            bK: val
                         });
                 default:
                     var attrs = modifier.a;
                     return _Utils_update(
                         options, {
-                            bt: _Utils_ap(options.bt, attrs)
+                            bv: _Utils_ap(options.bv, attrs)
                         });
             }
         });
     var $elm$html$Html$Attributes$classList = function(classes) {
         return $elm$html$Html$Attributes$class(
             A2(
                 $elm$core$String$join,
                 ' ',
                 A2(
                     $elm$core$List$map,
                     $elm$core$Tuple$first,
                     A2($elm$core$List$filter, $elm$core$Tuple$second, classes))));
     };
     var $rundis$elm_bootstrap$Bootstrap$Internal$Button$defaultOptions = {
-        bt: _List_Nil,
-        bw: false,
+        bv: _List_Nil,
+        by: false,
         ab: $elm$core$Maybe$Nothing,
-        bI: false,
-        e1: $elm$core$Maybe$Nothing
+        bK: false,
+        e2: $elm$core$Maybe$Nothing
     };
     var $elm$json$Json$Encode$bool = _Json_wrap;
     var $elm$html$Html$Attributes$boolProperty = F2(
         function(key, bool) {
             return A2(
                 _VirtualDom_property,
                 key,
@@ -16644,22 +16836,22 @@
         return _Utils_ap(
             _List_fromArray(
                 [
                     $elm$html$Html$Attributes$classList(
                         _List_fromArray(
                             [
                                 _Utils_Tuple2('btn', true),
-                                _Utils_Tuple2('btn-block', options.bw),
-                                _Utils_Tuple2('disabled', options.bI)
+                                _Utils_Tuple2('btn-block', options.by),
+                                _Utils_Tuple2('disabled', options.bK)
                             ])),
-                    $elm$html$Html$Attributes$disabled(options.bI)
+                    $elm$html$Html$Attributes$disabled(options.bK)
                 ]),
             _Utils_ap(
                 function() {
-                    var _v0 = A2($elm$core$Maybe$andThen, $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption, options.e1);
+                    var _v0 = A2($elm$core$Maybe$andThen, $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption, options.e2);
                     if (!_v0.$) {
                         var s = _v0.a;
                         return _List_fromArray(
                             [
                                 $elm$html$Html$Attributes$class('btn-' + s)
                             ]);
                     } else {
@@ -16685,15 +16877,15 @@
                                             'btn-outline-' + $rundis$elm_bootstrap$Bootstrap$Internal$Button$roleClass(role))
                                     ]);
                             }
                         } else {
                             return _List_Nil;
                         }
                     }(),
-                    options.bt)));
+                    options.bv)));
     };
     var $elm$html$Html$Attributes$checked = $elm$html$Html$Attributes$boolProperty('checked');
     var $elm$html$Html$input = _VirtualDom_node('input');
     var $elm$html$Html$label = _VirtualDom_node('label');
     var $elm$html$Html$Attributes$type_ = $elm$html$Html$Attributes$stringProperty('type');
     var $rundis$elm_bootstrap$Bootstrap$Button$radioButton = F3(
         function(checked, options, children) {
@@ -16741,14 +16933,20 @@
                     ]),
                 _List_fromArray(
                     [
                         $elm$html$Html$text(textDuration)
                     ]));
         });
     var $elm$html$Html$h2 = _VirtualDom_node('h2');
+    var $elm$html$Html$Attributes$height = function(n) {
+        return A2(
+            _VirtualDom_attribute,
+            'height',
+            $elm$core$String$fromInt(n));
+    };
     var $author$project$Main$htmlIf = F2(
         function(el, cond) {
             return cond ? el : $elm$html$Html$text('');
         });
     var $rundis$elm_bootstrap$Bootstrap$Form$Select$Item = $elm$core$Basics$identity;
     var $elm$html$Html$option = _VirtualDom_node('option');
     var $rundis$elm_bootstrap$Bootstrap$Form$Select$item = F2(
@@ -16783,64 +16981,64 @@
     var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$applyModifier = F2(
         function(modifier, options) {
             switch (modifier.$) {
                 case 0:
                     var size = modifier.a;
                     return _Utils_update(
                         options, {
-                            e1: $elm$core$Maybe$Just(size)
+                            e2: $elm$core$Maybe$Just(size)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            cQ: true
+                            cR: true
                         });
                 default:
                     var attrs_ = modifier.a;
                     return _Utils_update(
                         options, {
-                            bt: _Utils_ap(options.bt, attrs_)
+                            bv: _Utils_ap(options.bv, attrs_)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$defaultOptions = {
-        bt: _List_Nil,
-        e1: $elm$core$Maybe$Nothing,
-        cQ: false
+        bv: _List_Nil,
+        e2: $elm$core$Maybe$Nothing,
+        cR: false
     };
     var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$groupAttributes = F2(
         function(toggle, modifiers) {
             var options = A3($elm$core$List$foldl, $rundis$elm_bootstrap$Bootstrap$ButtonGroup$applyModifier, $rundis$elm_bootstrap$Bootstrap$ButtonGroup$defaultOptions, modifiers);
             return _Utils_ap(
                 _List_fromArray(
                     [
                         A2($elm$html$Html$Attributes$attribute, 'role', 'group'),
                         $elm$html$Html$Attributes$classList(
                             _List_fromArray(
                                 [
                                     _Utils_Tuple2('btn-group', true),
                                     _Utils_Tuple2('btn-group-toggle', toggle),
-                                    _Utils_Tuple2('btn-group-vertical', options.cQ)
+                                    _Utils_Tuple2('btn-group-vertical', options.cR)
                                 ])),
                         A2($elm$html$Html$Attributes$attribute, 'data-toggle', 'buttons')
                     ]),
                 _Utils_ap(
                     function() {
-                        var _v0 = A2($elm$core$Maybe$andThen, $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption, options.e1);
+                        var _v0 = A2($elm$core$Maybe$andThen, $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption, options.e2);
                         if (!_v0.$) {
                             var s = _v0.a;
                             return _List_fromArray(
                                 [
                                     $elm$html$Html$Attributes$class('btn-group-' + s)
                                 ]);
                         } else {
                             return _List_Nil;
                         }
                     }(),
-                    options.bt));
+                    options.bv));
         });
     var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButtonGroupItem = F2(
         function(options, items) {
             return A2(
                 $elm$html$Html$div,
                 A2($rundis$elm_bootstrap$Bootstrap$ButtonGroup$groupAttributes, true, options),
                 A2(
@@ -16860,62 +17058,62 @@
             return $rundis$elm_bootstrap$Bootstrap$ButtonGroup$renderGroup(
                 A2($rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButtonGroupItem, options, items));
         });
     var $rundis$elm_bootstrap$Bootstrap$Form$Select$Select = $elm$core$Basics$identity;
     var $rundis$elm_bootstrap$Bootstrap$Form$Select$create = F2(
         function(options, items) {
             return {
-                ek: items,
-                dh: options
+                el: items,
+                dj: options
             };
         });
     var $elm$html$Html$select = _VirtualDom_node('select');
     var $rundis$elm_bootstrap$Bootstrap$Form$Select$applyModifier = F2(
         function(modifier, options) {
             switch (modifier.$) {
                 case 0:
                     var size_ = modifier.a;
                     return _Utils_update(
                         options, {
-                            e1: $elm$core$Maybe$Just(size_)
+                            e2: $elm$core$Maybe$Just(size_)
                         });
                 case 1:
                     var id_ = modifier.a;
                     return _Utils_update(
                         options, {
-                            aT: $elm$core$Maybe$Just(id_)
+                            aV: $elm$core$Maybe$Just(id_)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
                             C: true
                         });
                 case 3:
                     var val = modifier.a;
                     return _Utils_update(
                         options, {
-                            bI: val
+                            bK: val
                         });
                 case 4:
                     var onChange_ = modifier.a;
                     return _Utils_update(
                         options, {
-                            ca: $elm$core$Maybe$Just(onChange_)
+                            cc: $elm$core$Maybe$Just(onChange_)
                         });
                 case 5:
                     var validation_ = modifier.a;
                     return _Utils_update(
                         options, {
-                            cP: $elm$core$Maybe$Just(validation_)
+                            cQ: $elm$core$Maybe$Just(validation_)
                         });
                 default:
                     var attrs_ = modifier.a;
                     return _Utils_update(
                         options, {
-                            bt: _Utils_ap(options.bt, attrs_)
+                            bv: _Utils_ap(options.bv, attrs_)
                         });
             }
         });
     var $elm$json$Json$Decode$at = F2(
         function(fields, decoder) {
             return A3($elm$core$List$foldr, $elm$json$Json$Decode$field, decoder, fields);
         });
@@ -16927,21 +17125,21 @@
     var $rundis$elm_bootstrap$Bootstrap$Form$Select$customEventOnChange = function(tagger) {
         return A2(
             $elm$html$Html$Events$on,
             'change',
             A2($elm$json$Json$Decode$map, tagger, $elm$html$Html$Events$targetValue));
     };
     var $rundis$elm_bootstrap$Bootstrap$Form$Select$defaultOptions = {
-        bt: _List_Nil,
+        bv: _List_Nil,
         C: false,
-        bI: false,
-        aT: $elm$core$Maybe$Nothing,
-        ca: $elm$core$Maybe$Nothing,
-        e1: $elm$core$Maybe$Nothing,
-        cP: $elm$core$Maybe$Nothing
+        bK: false,
+        aV: $elm$core$Maybe$Nothing,
+        cc: $elm$core$Maybe$Nothing,
+        e2: $elm$core$Maybe$Nothing,
+        cQ: $elm$core$Maybe$Nothing
     };
     var $elm$html$Html$Attributes$id = $elm$html$Html$Attributes$stringProperty('id');
     var $rundis$elm_bootstrap$Bootstrap$Form$Select$sizeAttribute = F2(
         function(isCustom, size_) {
             var prefix = isCustom ? 'custom-select-' : 'form-control-';
             return A2(
                 $elm$core$Maybe$map,
@@ -16969,35 +17167,35 @@
                 [
                     $elm$html$Html$Attributes$classList(
                         _List_fromArray(
                             [
                                 _Utils_Tuple2('form-control', !options.C),
                                 _Utils_Tuple2('custom-select', options.C)
                             ])),
-                    $elm$html$Html$Attributes$disabled(options.bI)
+                    $elm$html$Html$Attributes$disabled(options.bK)
                 ]),
             _Utils_ap(
                 A2(
                     $elm$core$List$filterMap,
                     $elm$core$Basics$identity,
                     _List_fromArray(
                         [
-                            A2($elm$core$Maybe$map, $elm$html$Html$Attributes$id, options.aT),
+                            A2($elm$core$Maybe$map, $elm$html$Html$Attributes$id, options.aV),
                             A2(
                                 $elm$core$Maybe$andThen,
                                 $rundis$elm_bootstrap$Bootstrap$Form$Select$sizeAttribute(options.C),
-                                options.e1),
-                            A2($elm$core$Maybe$map, $rundis$elm_bootstrap$Bootstrap$Form$Select$customEventOnChange, options.ca),
-                            A2($elm$core$Maybe$map, $rundis$elm_bootstrap$Bootstrap$Form$Select$validationAttribute, options.cP)
+                                options.e2),
+                            A2($elm$core$Maybe$map, $rundis$elm_bootstrap$Bootstrap$Form$Select$customEventOnChange, options.cc),
+                            A2($elm$core$Maybe$map, $rundis$elm_bootstrap$Bootstrap$Form$Select$validationAttribute, options.cQ)
                         ])),
-                options.bt));
+                options.bv));
     };
     var $rundis$elm_bootstrap$Bootstrap$Form$Select$view = function(_v0) {
-        var options = _v0.dh;
-        var items = _v0.ek;
+        var options = _v0.dj;
+        var items = _v0.el;
         return A2(
             $elm$html$Html$select,
             $rundis$elm_bootstrap$Bootstrap$Form$Select$toAttributes(options),
             A2(
                 $elm$core$List$map,
                 function(_v1) {
                     var e = _v1;
@@ -17007,14 +17205,20 @@
     };
     var $rundis$elm_bootstrap$Bootstrap$Form$Select$select = F2(
         function(options, items) {
             return $rundis$elm_bootstrap$Bootstrap$Form$Select$view(
                 A2($rundis$elm_bootstrap$Bootstrap$Form$Select$create, options, items));
         });
     var $elm$html$Html$Attributes$value = $elm$html$Html$Attributes$stringProperty('value');
+    var $elm$html$Html$Attributes$width = function(n) {
+        return A2(
+            _VirtualDom_attribute,
+            'width',
+            $elm$core$String$fromInt(n));
+    };
     var $author$project$Main$view = function(model) {
         return A2(
             $elm$html$Html$div,
             _List_Nil,
             _List_fromArray(
                 [
                     A2(
@@ -17040,17 +17244,33 @@
                                             A2(
                                                 $rundis$elm_bootstrap$Bootstrap$Grid$col,
                                                 _List_Nil,
                                                 _List_fromArray(
                                                     [
                                                         A2(
                                                             $elm$html$Html$h1,
-                                                            _List_Nil,
                                                             _List_fromArray(
                                                                 [
+                                                                    $elm$html$Html$Attributes$class('d-flex'),
+                                                                    $elm$html$Html$Attributes$class('align-items-center')
+                                                                ]),
+                                                            _List_fromArray(
+                                                                [
+                                                                    A2(
+                                                                        $elm$html$Html$img,
+                                                                        _List_fromArray(
+                                                                            [
+                                                                                $elm$html$Html$Attributes$src('/static/images/aqimon.png'),
+                                                                                A2($elm$html$Html$Attributes$style, 'margin-right', '0.5em'),
+                                                                                $elm$html$Html$Attributes$width(75),
+                                                                                $elm$html$Html$Attributes$height(75),
+                                                                                $elm$html$Html$Attributes$class('d-inline-block'),
+                                                                                $elm$html$Html$Attributes$class('align-text-top')
+                                                                            ]),
+                                                                        _List_Nil),
                                                                     $elm$html$Html$text('AQI Monitor')
                                                                 ]))
                                                     ]))
                                         ])),
                                 A2(
                                     $rundis$elm_bootstrap$Bootstrap$Grid$row,
                                     _List_fromArray(
@@ -17073,18 +17293,18 @@
                                                                     A2($elm$html$Html$Attributes$style, 'background-color', '#D9D9D9'),
                                                                     A2($elm$html$Html$Attributes$style, 'margin', '1em')
                                                                 ]))
                                                     ]),
                                                 _List_fromArray(
                                                     [
                                                         $author$project$CurrentReads$getCurrentReads({
-                                                            d0: model.ad.d0,
-                                                            en: model.ad.d$,
-                                                            ep: model.ad.eF,
-                                                            eq: model.ad.eG
+                                                            d1: model.ad.d1,
+                                                            eo: model.ad.c_,
+                                                            eq: model.ad.eG,
+                                                            er: model.ad.eH
                                                         })
                                                     ])),
                                             A2(
                                                 $rundis$elm_bootstrap$Bootstrap$Grid$col,
                                                 _List_fromArray(
                                                     [
                                                         $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
@@ -17094,15 +17314,15 @@
                                                                     $elm$html$Html$Attributes$class('d-flex'),
                                                                     A2($elm$html$Html$Attributes$style, 'background-color', '#D9D9D9'),
                                                                     A2($elm$html$Html$Attributes$style, 'margin', '1em')
                                                                 ]))
                                                     ]),
                                                 _List_fromArray(
                                                     [
-                                                        $author$project$EpaLevel$getEpaLevel(model.ad.d0)
+                                                        $author$project$EpaLevel$getEpaLevel(model.ad.d1)
                                                     ])),
                                             A2(
                                                 $rundis$elm_bootstrap$Bootstrap$Grid$col,
                                                 _List_fromArray(
                                                     [
                                                         $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
                                                             _List_fromArray(
@@ -17256,22 +17476,23 @@
                                                                     [
                                                                         A2($elm$html$Html$Attributes$style, 'height', '400px')
                                                                     ]),
                                                                 _List_fromArray(
                                                                     [
                                                                         A2(
                                                                             $author$project$Graph$getEpaChart, {
-                                                                                bD: model.bV,
-                                                                                bM: model.bp
+                                                                                bF: model.bX,
+                                                                                bO: model.br,
+                                                                                aJ: model.aJ
                                                                             },
                                                                             $author$project$Main$OnEpaHover)
                                                                     ]))
                                                         ]))
                                             ])),
-                                    !model.aO),
+                                    !model.aQ),
                                 A2(
                                     $author$project$Main$htmlIf,
                                     A2(
                                         $rundis$elm_bootstrap$Bootstrap$Grid$row,
                                         _List_fromArray(
                                             [
                                                 $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
@@ -17296,30 +17517,31 @@
                                                                     [
                                                                         A2($elm$html$Html$Attributes$style, 'height', '400px')
                                                                     ]),
                                                                 _List_fromArray(
                                                                     [
                                                                         A2(
                                                                             $author$project$Graph$getReadChart, {
-                                                                                bD: model.bW,
-                                                                                bM: model.bq
+                                                                                bF: model.bY,
+                                                                                bO: model.bs,
+                                                                                aJ: model.aJ
                                                                             },
                                                                             $author$project$Main$OnReadHover)
                                                                     ]))
                                                         ]))
                                             ])),
-                                    model.aO === 1)
+                                    model.aQ === 1)
                             ]))
                 ]));
     };
     var $author$project$Main$main = $elm$browser$Browser$element({
-        fQ: $author$project$Main$init,
-        gd: $author$project$Main$subscriptions,
-        gu: $author$project$Main$update,
-        gw: $author$project$Main$view
+        fR: $author$project$Main$init,
+        ge: $author$project$Main$subscriptions,
+        gv: $author$project$Main$update,
+        gx: $author$project$Main$view
     });
     _Platform_export({
         'Main': {
             'init': $author$project$Main$main(
                 $elm$json$Json$Decode$succeed(0))(0)
         }
     });
```

### Comparing `aqimon-0.5.1/aqimon/static/favicon-32x32.png` & `aqimon-0.6.0/aqimon/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.5.1/aqimon/static/images/failing.png` & `aqimon-0.6.0/aqimon/static/images/failing.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.5.1/aqimon/static/images/idle.png` & `aqimon-0.6.0/aqimon/static/images/idle.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.5.1/aqimon/static/images/loading.gif` & `aqimon-0.6.0/aqimon/static/images/loading.gif`

 * *Files identical despite different names*

### Comparing `aqimon-0.5.1/aqimon/static/images/warmingup.gif` & `aqimon-0.6.0/aqimon/static/images/warmingup.gif`

 * *Files identical despite different names*

### Comparing `aqimon-0.5.1/aqimon/static/index.html` & `aqimon-0.6.0/aqimon/static/index.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <!-- Required meta tags -->
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
+    <link rel="icon" href="/static/favicon.ico" sizes="32x32">
 
     <!-- Bootstrap CSS -->
     <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">
   </head>
   <body>
 
     <div id="elm-app"></div>
```

#### html2text {}

```diff
@@ -1,3 +1,4 @@
 
 
 
+
```

### Comparing `aqimon-0.5.1/pyproject.toml` & `aqimon-0.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aqimon"
-version = "0.5.1"
+version = "0.6.0"
 description = "Air Quality Index Monitor"
 authors = ["Tim Orme"]
 readme = "README.md"
 include = ["aqimon/static/elm.js"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `aqimon-0.5.1/PKG-INFO` & `aqimon-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqimon
-Version: 0.5.1
+Version: 0.6.0
 Summary: Air Quality Index Monitor
 Author: Tim Orme
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,15 +12,15 @@
 Requires-Dist: fastapi (>=0.92.0,<0.93.0)
 Requires-Dist: fastapi-utils (>=0.2.1,<0.3.0)
 Requires-Dist: pyserial (>=3.5,<4.0)
 Requires-Dist: sds011lib (>=0.4.0,<0.5.0)
 Requires-Dist: uvicorn (>=0.21.0,<0.22.0)
 Description-Content-Type: text/markdown
 
-# AQIMON
+# ![AQIMON](header.png) 
 
 A simple Air Quality Index monitor, designed to work on the Raspberry Pi with the SDS011 Nova PM Sensor.
 
 - [AQIMON](#aqimon)
   - [Screenshot](#screenshot) 
   - [Installation](#installation)
     - [Pre-Requisites](#pre-requisites)
```

