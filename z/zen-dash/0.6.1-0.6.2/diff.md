# Comparing `tmp/zen_dash-0.6.1.tar.gz` & `tmp/zen_dash-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zen_dash-0.6.1.tar", max compression
+gzip compressed data, was "zen_dash-0.6.2.tar", max compression
```

## Comparing `zen_dash-0.6.1.tar` & `zen_dash-0.6.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1070 2023-02-09 14:33:40.121808 zen_dash-0.6.1/LICENSE
--rw-r--r--   0        0        0     7781 2023-05-05 01:59:51.099742 zen_dash-0.6.1/README.md
--rw-r--r--   0        0        0     1288 2023-07-30 20:53:03.392198 zen_dash-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       41 2023-04-12 05:50:21.332964 zen_dash-0.6.1/zen_dash/__init__.py
--rw-r--r--   0        0        0     1521 2023-07-30 20:54:39.317930 zen_dash-0.6.1/zen_dash/auth/__init__.py
--rw-r--r--   0        0        0        0 2023-01-07 16:56:11.285785 zen_dash-0.6.1/zen_dash/cli/__init__.py
--rw-r--r--   0        0        0      219 2023-04-14 03:33:36.095076 zen_dash-0.6.1/zen_dash/cli/main.py
--rw-r--r--   0        0        0     5879 2023-04-14 03:33:25.986936 zen_dash-0.6.1/zen_dash/cli/project_management.py
--rw-r--r--   0        0        0      203 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/flex_data.py
--rw-r--r--   0        0        0      196 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/instances.py
--rw-r--r--   0        0        0     1403 2023-07-22 15:37:24.864370 zen_dash-0.6.1/zen_dash/objects/__init__.py
--rw-r--r--   0        0        0      291 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/objects/flex_data.py
--rw-r--r--   0        0        0    13136 2023-07-24 00:51:23.343274 zen_dash-0.6.1/zen_dash/objects/instances.py
--rw-r--r--   0        0        0      255 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/objects/page.py
--rw-r--r--   0        0        0      768 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/objects/scripts.py
--rw-r--r--   0        0        0      750 2023-06-16 02:37:03.983233 zen_dash-0.6.1/zen_dash/objects/sidebar.py
--rw-r--r--   0        0        0      919 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/page.py
--rw-r--r--   0        0        0        0 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/route.py
--rw-r--r--   0        0        0      191 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/scripts.py
--rw-r--r--   0        0        0      195 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/sidebar.py
--rw-r--r--   0        0        0  1017714 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/275.44cd52f9d992445f.js
--rw-r--r--   0        0        0    57081 2023-07-24 00:55:40.695293 zen_dash-0.6.1/zen_dash/static/3rdpartylicenses.txt
--rw-r--r--   0        0        0   128180 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf
--rw-r--r--   0        0        0   143258 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot
--rw-r--r--   0        0        0    44300 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2
--rw-r--r--   0        0        0    57620 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff
--rw-r--r--   0        0        0      948 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/favicon.ico
--rw-r--r--   0        0        0     2137 2023-07-24 00:55:41.423305 zen_dash-0.6.1/zen_dash/static/index.html
--rw-r--r--   0        0        0    92621 2023-07-24 00:55:40.695293 zen_dash-0.6.1/zen_dash/static/main.b01efffb503d168d.js
--rw-r--r--   0        0        0    33759 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/polyfills.0a8881ff36766b1e.js
--rw-r--r--   0        0        0     3285 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/runtime.6a9b461ae5a72237.js
--rw-r--r--   0        0        0   152653 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/styles.362a8260c32d36d9.css
--rw-r--r--   0        0        0  3060723 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/vendor.3c67e76b6e4a9ca3.js
--rw-r--r--   0        0        0      621 2022-10-23 00:15:15.909625 zen_dash-0.6.1/zen_dash/support/__init__.py
--rw-r--r--   0        0        0      217 2023-04-12 05:50:21.352964 zen_dash-0.6.1/zen_dash/support/encoder.py
--rw-r--r--   0        0        0     7055 2023-05-29 16:12:36.409345 zen_dash-0.6.1/zen_dash/tag/__init__.py
--rw-r--r--   0        0        0     1513 2023-04-12 05:50:21.352964 zen_dash-0.6.1/zen_dash/websocket/__init__.py
--rw-r--r--   0        0        0     8861 1970-01-01 00:00:00.000000 zen_dash-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-02-09 14:33:40.121808 zen_dash-0.6.2/LICENSE
+-rw-r--r--   0        0        0     7781 2023-05-05 01:59:51.099742 zen_dash-0.6.2/README.md
+-rw-r--r--   0        0        0     1288 2023-08-08 03:05:17.162111 zen_dash-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-04-12 05:50:21.332964 zen_dash-0.6.2/zen_dash/__init__.py
+-rw-r--r--   0        0        0     1521 2023-07-30 20:54:39.317930 zen_dash-0.6.2/zen_dash/auth/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-07 16:56:11.285785 zen_dash-0.6.2/zen_dash/cli/__init__.py
+-rw-r--r--   0        0        0      219 2023-04-14 03:33:36.095076 zen_dash-0.6.2/zen_dash/cli/main.py
+-rw-r--r--   0        0        0     5879 2023-04-14 03:33:25.986936 zen_dash-0.6.2/zen_dash/cli/project_management.py
+-rw-r--r--   0        0        0      203 2023-04-12 05:50:21.336964 zen_dash-0.6.2/zen_dash/flex_data.py
+-rw-r--r--   0        0        0      196 2023-04-12 05:50:21.336964 zen_dash-0.6.2/zen_dash/instances.py
+-rw-r--r--   0        0        0     1403 2023-07-22 15:37:24.864370 zen_dash-0.6.2/zen_dash/objects/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-12 05:50:21.336964 zen_dash-0.6.2/zen_dash/objects/flex_data.py
+-rw-r--r--   0        0        0    13136 2023-07-24 00:51:23.343274 zen_dash-0.6.2/zen_dash/objects/instances.py
+-rw-r--r--   0        0        0      255 2023-04-12 05:50:21.336964 zen_dash-0.6.2/zen_dash/objects/page.py
+-rw-r--r--   0        0        0      768 2023-04-12 05:50:21.336964 zen_dash-0.6.2/zen_dash/objects/scripts.py
+-rw-r--r--   0        0        0      750 2023-06-16 02:37:03.983233 zen_dash-0.6.2/zen_dash/objects/sidebar.py
+-rw-r--r--   0        0        0      919 2023-04-12 05:50:21.336964 zen_dash-0.6.2/zen_dash/page.py
+-rw-r--r--   0        0        0        0 2023-04-12 05:50:21.336964 zen_dash-0.6.2/zen_dash/route.py
+-rw-r--r--   0        0        0      191 2023-04-12 05:50:21.336964 zen_dash-0.6.2/zen_dash/scripts.py
+-rw-r--r--   0        0        0      195 2023-04-12 05:50:21.336964 zen_dash-0.6.2/zen_dash/sidebar.py
+-rw-r--r--   0        0        0  1017714 2023-08-04 23:38:23.199118 zen_dash-0.6.2/zen_dash/static/275.44cd52f9d992445f.js
+-rw-r--r--   0        0        0    57081 2023-08-05 03:43:32.396520 zen_dash-0.6.2/zen_dash/static/3rdpartylicenses.txt
+-rw-r--r--   0        0        0   128180 2023-08-04 23:38:23.199118 zen_dash-0.6.2/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf
+-rw-r--r--   0        0        0   143258 2023-08-04 23:38:23.199118 zen_dash-0.6.2/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot
+-rw-r--r--   0        0        0    44300 2023-08-04 23:38:23.199118 zen_dash-0.6.2/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2
+-rw-r--r--   0        0        0    57620 2023-08-04 23:38:23.199118 zen_dash-0.6.2/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff
+-rw-r--r--   0        0        0      948 2023-08-04 23:38:23.199118 zen_dash-0.6.2/zen_dash/static/favicon.ico
+-rw-r--r--   0        0        0     2137 2023-08-05 03:43:33.160532 zen_dash-0.6.2/zen_dash/static/index.html
+-rw-r--r--   0        0        0    93278 2023-08-05 03:43:32.396520 zen_dash-0.6.2/zen_dash/static/main.2ca5ecb496656cbf.js
+-rw-r--r--   0        0        0    33759 2023-08-04 23:38:23.199118 zen_dash-0.6.2/zen_dash/static/polyfills.0a8881ff36766b1e.js
+-rw-r--r--   0        0        0     3285 2023-08-04 23:38:23.199118 zen_dash-0.6.2/zen_dash/static/runtime.6a9b461ae5a72237.js
+-rw-r--r--   0        0        0   152653 2023-08-04 23:38:23.199118 zen_dash-0.6.2/zen_dash/static/styles.362a8260c32d36d9.css
+-rw-r--r--   0        0        0  3060723 2023-08-04 23:38:23.199118 zen_dash-0.6.2/zen_dash/static/vendor.3c67e76b6e4a9ca3.js
+-rw-r--r--   0        0        0      621 2022-10-23 00:15:15.909625 zen_dash-0.6.2/zen_dash/support/__init__.py
+-rw-r--r--   0        0        0      217 2023-04-12 05:50:21.352964 zen_dash-0.6.2/zen_dash/support/encoder.py
+-rw-r--r--   0        0        0     7055 2023-05-29 16:12:36.409345 zen_dash-0.6.2/zen_dash/tag/__init__.py
+-rw-r--r--   0        0        0     1513 2023-04-12 05:50:21.352964 zen_dash-0.6.2/zen_dash/websocket/__init__.py
+-rw-r--r--   0        0        0     8861 1970-01-01 00:00:00.000000 zen_dash-0.6.2/PKG-INFO
```

### Comparing `zen_dash-0.6.1/LICENSE` & `zen_dash-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/README.md` & `zen_dash-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/pyproject.toml` & `zen_dash-0.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zen_dash"
-version = "0.6.1"
+version = "0.6.2"
 license = "MIT"
 description = "Simple yet scable and production ready python dashboard that is better than shiny application for business."
 readme = "README.md"
 authors = ["Zen <zenreportz@pm.me>"]
 homepage = "https://zen-reportz.github.io/zen_dash/index.html"
 repository = "https://github.com/Zen-Reportz/zen_dash"
 include = [
```

### Comparing `zen_dash-0.6.1/zen_dash/auth/__init__.py` & `zen_dash-0.6.2/zen_dash/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/cli/project_management.py` & `zen_dash-0.6.2/zen_dash/cli/project_management.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/objects/__init__.py` & `zen_dash-0.6.2/zen_dash/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/objects/instances.py` & `zen_dash-0.6.2/zen_dash/objects/instances.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/objects/scripts.py` & `zen_dash-0.6.2/zen_dash/objects/scripts.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/objects/sidebar.py` & `zen_dash-0.6.2/zen_dash/objects/sidebar.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/page.py` & `zen_dash-0.6.2/zen_dash/page.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/static/275.44cd52f9d992445f.js` & `zen_dash-0.6.2/zen_dash/static/275.44cd52f9d992445f.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/static/3rdpartylicenses.txt` & `zen_dash-0.6.2/zen_dash/static/3rdpartylicenses.txt`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf` & `zen_dash-0.6.2/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot` & `zen_dash-0.6.2/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2` & `zen_dash-0.6.2/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff` & `zen_dash-0.6.2/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/static/favicon.ico` & `zen_dash-0.6.2/zen_dash/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/static/index.html` & `zen_dash-0.6.2/zen_dash/static/index.html`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,14 @@
   <title>Frontend</title>
   <base href="./">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <link rel="icon" type="image/x-icon" href="favicon.ico">
   <!-- <link rel="preconnect" href="https://fonts.gstatic.com">
   <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500&display=swap" rel="stylesheet">
   <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet"> -->
-  <style type="text/css">@font-face{font-family:'Material Symbols Outlined';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialsymbolsoutlined/v127/kJF1BvYX7BgnkSrUwT8OhrdQw4oELdPIeeII9v6oDMzByHX9rA6RzaxHMPdY43zj-jCxv3fzvRNU22ZXGJpEpjC_1n-q_4MrImHCIJIZrDCvHOelbd5zrDAt.woff) format('woff');}.material-symbols-outlined{font-family:'Material Symbols Outlined';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased;}</style>
+  <style type="text/css">@font-face{font-family:'Material Symbols Outlined';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialsymbolsoutlined/v129/kJF1BvYX7BgnkSrUwT8OhrdQw4oELdPIeeII9v6oDMzByHX9rA6RzaxHMPdY43zj-jCxv3fzvRNU22ZXGJpEpjC_1n-q_4MrImHCIJIZrDCvHOelbd5zrDAt.woff) format('woff');}.material-symbols-outlined{font-family:'Material Symbols Outlined';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased;}</style>
 <style>.mat-typography{font:400 14px/20px Roboto,Helvetica Neue,sans-serif;letter-spacing:normal}.mat-typography{font:400 14px/20px Roboto,Helvetica Neue,sans-serif;letter-spacing:normal}body{font-family:Roboto,Helvetica Neue,sans-serif;margin:0;position:relative;overflow:auto;display:inline-block;overflow:hidden}html{margin:0;height:100%;width:100%}body{margin:0;min-height:100%;width:100%}</style><link rel="stylesheet" href="styles.362a8260c32d36d9.css" media="print" onload="this.media='all'"><noscript><link rel="stylesheet" href="styles.362a8260c32d36d9.css"></noscript></head>
 <body class="mat-typography">
   <app-root></app-root>
-<script src="runtime.6a9b461ae5a72237.js" type="module"></script><script src="polyfills.0a8881ff36766b1e.js" type="module"></script><script src="vendor.3c67e76b6e4a9ca3.js" type="module"></script><script src="main.b01efffb503d168d.js" type="module"></script>
+<script src="runtime.6a9b461ae5a72237.js" type="module"></script><script src="polyfills.0a8881ff36766b1e.js" type="module"></script><script src="vendor.3c67e76b6e4a9ca3.js" type="module"></script><script src="main.2ca5ecb496656cbf.js" type="module"></script>
 
 </body></html>
```

### Comparing `zen_dash-0.6.1/zen_dash/static/main.b01efffb503d168d.js` & `zen_dash-0.6.2/zen_dash/static/main.2ca5ecb496656cbf.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -52,271 +52,271 @@
             p.d(I, {
                 D: () => pt
             });
             var T = p(64537),
                 t = p(21312);
             let pt = (() => {
                 class S {
-                    constructor(c, u) {
-                        this.router = c, this.activatedRoute = u, this.defaul_page = "page_0", this.all_input = new Map, this.input_emitter = new T.vpe, this.data = {
+                    constructor(d, u) {
+                        this.router = d, this.activatedRoute = u, this.defaul_page = "page_0", this.all_input = new Map, this.input_emitter = new T.vpe, this.data = {
                             global: {
                                 device_information: ["device_information", {
                                     browser: navigator.userAgent,
                                     screen_info: {
                                         height: screen.availHeight,
                                         width: screen.availWidth
                                     }
                                 }]
                             }
                         }, this.data_setter = new T.vpe, this.refresh = new T.vpe, window.data_service = this, window.data_service_get_page = this.get_page, window.data_service_get_all = this.get_all, this.data_setter.subscribe(h => {
                             this.reset_path(u), void 0 === this.data[h.page] && (this.data[h.page] = {}), this.data[h.page][h.url] = [h.key, h.value]
                         })
                     }
-                    reset_path(c) {
+                    reset_path(d) {
                         let h = {};
                         h = {
                             page: this.get_page()[0]
                         };
                         let C = new URL(window.location.href),
                             v = new URLSearchParams(C.search);
                         null !== v.get("document_id") && (null !== v.get("page") ? this.router.navigate([], {
-                            relativeTo: c,
+                            relativeTo: d,
                             queryParams: {
                                 page: v.get("page")
                             }
                         }) : this.router.navigate([], {
-                            relativeTo: c,
+                            relativeTo: d,
                             queryParams: {}
                         }))
                     }
                     get_page() {
-                        let c = new URL(window.location.href),
-                            u = new URLSearchParams(c.search),
+                        let d = new URL(window.location.href),
+                            u = new URLSearchParams(d.search),
                             h = "page_0";
                         return h = null !== u.get("page") ? u.get("page") : this.defaul_page, h
                     }
-                    get_data(c, u) {
-                        if (void 0 !== this.data[c]) return this.data[c][u]
+                    get_data(d, u) {
+                        if (void 0 !== this.data[d]) return this.data[d][u]
                     }
                     get_all() {
-                        let c;
+                        let d;
                         try {
-                            c = this.get_page()
+                            d = this.get_page()
                         } catch {
-                            c = window.data_service_get_page()
+                            d = window.data_service_get_page()
                         }
                         let h, C, u = {
                             url: window.location.href
                         };
                         try {
-                            h = this.data[c] ?? {}
+                            h = this.data[d] ?? {}
                         } catch {
-                            h = window.data_service.data[c] ?? {}
+                            h = window.data_service.data[d] ?? {}
                         }
                         Object.entries(h).forEach(([v, U]) => {
                             u[U[0]] = U[1]
                         });
                         try {
                             C = this.data.global ?? {}
                         } catch {
                             C = window.data_service.data.global ?? {}
                         }
                         return Object.entries(C).forEach(([v, U]) => {
                             "page" === v ? u[v] = U : u[U[0]] = U[1]
                         }), u
                     }
-                    get_input_data(c) {
-                        return this.all_input.get(c)
+                    get_input_data(d) {
+                        return this.all_input.get(d)
                     }
-                    set_data(c, u, h) {
-                        void 0 === this.data[c] && (this.data[c] = {}), this.data[c][u] = h
+                    set_data(d, u, h) {
+                        void 0 === this.data[d] && (this.data[d] = {}), this.data[d][u] = h
                     }
-                    input_lookup(c, u) {
-                        return u + "$ZenLookup$" + c
+                    input_lookup(d, u) {
+                        return u + "$ZenLookup$" + d
                     }
-                    trueTypeOf(c) {
-                        return Object.prototype.toString.call(c).slice(8, -1).toLowerCase()
+                    trueTypeOf(d) {
+                        return Object.prototype.toString.call(d).slice(8, -1).toLowerCase()
                     }
-                    dataLookup(c) {
-                        return c ? "global" : this.get_page()
+                    dataLookup(d) {
+                        return d ? "global" : this.get_page()
                     }
                     reset_data() {
                         this.all_input = new Map
                     }
-                    save_instance(c, u, h) {
-                        switch (c.type) {
+                    save_instance(d, u, h) {
+                        switch (d.type) {
                             case "date":
-                                let C = c.date_data;
-                                C.second_date ? (C.first_date = u[0], C.second_date = u[1]) : C.first_date = u, c.date_data = C, this.all_input.set(h, c);
+                                let C = d.date_data;
+                                C.second_date ? (C.first_date = u[0], C.second_date = u[1]) : C.first_date = u, d.date_data = C, this.all_input.set(h, d);
                                 break;
                             case "radio":
-                                let v = c.radio_data;
-                                v.selected = u, c.radio_data = v, this.all_input.set(h, c);
+                                let v = d.radio_data;
+                                v.selected = u, d.radio_data = v, this.all_input.set(h, d);
                                 break;
                             case "checkbox":
-                                let U = c.checkbox_data;
-                                U.data = u, c.checkbox_data = U, this.all_input.set(h, c);
+                                let U = d.checkbox_data;
+                                U.data = u, d.checkbox_data = U, this.all_input.set(h, d);
                                 break;
                             case "slider":
-                                let P = c.slider_data;
-                                P.value = u, c.slider_data = P, this.all_input.set(h, c);
+                                let P = d.slider_data;
+                                P.value = u, d.slider_data = P, this.all_input.set(h, d);
                                 break;
                             case "button_toggle":
-                                let K = c.button_toggle_data;
+                                let K = d.button_toggle_data;
                                 if (K.multi)
-                                    for (let N of K.data) N.selected = -1 !== u.indexOf(N.name);
+                                    for (let E of K.data) E.selected = -1 !== u.indexOf(E.name);
                                 else
-                                    for (let N of K.data) N.selected = N.name === u;
-                                c.button_toggle_data = K, this.all_input.set(h, c);
+                                    for (let E of K.data) E.selected = E.name === u;
+                                d.button_toggle_data = K, this.all_input.set(h, d);
                                 break;
                             case "toggle":
-                                let ct = c.toggle_data;
-                                ct.checked = u, c.toggle_data = ct, this.all_input.set(h, c);
+                                let ct = d.toggle_data;
+                                ct.checked = u, d.toggle_data = ct, this.all_input.set(h, d);
                                 break;
                             case "simple_filter":
-                                let X = c.simple_filter_data;
-                                X.selected = X.multi ? u : [u], c.simple_filter_data = X, this.all_input.set(h, c);
+                                let X = d.simple_filter_data;
+                                X.selected = X.multi ? u : [u], d.simple_filter_data = X, this.all_input.set(h, d);
                                 break;
                             case "simple_server_filter":
-                                let W = c.simple_server_filter_data;
-                                W.selected = W.multi ? u : [u], c.simple_server_filter_data = W, this.all_input.set(h, c);
+                                let W = d.simple_server_filter_data;
+                                W.selected = W.multi ? u : [u], d.simple_server_filter_data = W, this.all_input.set(h, d);
                                 break;
                             case "group_filter":
-                                let $ = c.group_filter_data;
-                                $.selected = $.multi ? u : [u], c.group_filter_data = $, this.all_input.set(h, c);
+                                let $ = d.group_filter_data;
+                                $.selected = $.multi ? u : [u], d.group_filter_data = $, this.all_input.set(h, d);
                                 break;
                             case "input":
-                                let dt = c.input_data;
-                                dt.value = u, c.input_data = dt, this.all_input.set(h, c);
+                                let dt = d.input_data;
+                                dt.value = u, d.input_data = dt, this.all_input.set(h, d);
                                 break;
                             default:
-                                console.error(c.type)
+                                console.error(d.type)
                         }
                     }
                     save_default() {
-                        let c = this.get_page();
+                        let d = this.get_page();
                         for (const [u, h] of Object.entries(this.data.global)) {
                             console.log(u + h);
                             try {
                                 if ("page" !== u) {
                                     let C = h,
                                         v = this.all_input.get(u);
                                     this.save_instance(v, C[1], u)
                                 }
                             } catch {}
                         }
                         try {
-                            for (const [u, h] of Object.entries(this.data[c])) {
+                            for (const [u, h] of Object.entries(this.data[d])) {
                                 let C = h,
                                     v = this.all_input.get(u);
                                 this.save_instance(v, C[1], u)
                             }
                         } catch {}
                     }
-                    isFullCustom(c) {
-                        return null != this.all_input.get(c)?.custom_html_data?.full_custom && this.all_input.get(c)?.custom_html_data?.full_custom
+                    isFullCustom(d) {
+                        return null != this.all_input.get(d)?.custom_html_data?.full_custom && this.all_input.get(d)?.custom_html_data?.full_custom
                     }
-                    makeid(c) {
+                    makeid(d) {
                         let u = "";
                         const h = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789",
                             C = h.length;
                         let v = 0;
-                        for (; v < c;) u += h.charAt(Math.floor(Math.random() * C)), v += 1;
+                        for (; v < d;) u += h.charAt(Math.floor(Math.random() * C)), v += 1;
                         return u
                     }
                 }
-                return S.\u0275fac = function(c) {
-                    return new(c || S)(T.LFG(t.F0), T.LFG(t.gz))
+                return S.\u0275fac = function(d) {
+                    return new(d || S)(T.LFG(t.F0), T.LFG(t.gz))
                 }, S.\u0275prov = T.Yz7({
                     token: S,
                     factory: S.\u0275fac,
                     providedIn: "root"
                 }), S
             })()
         },
         24269: (O, I, p) => {
             var T = p(5998),
                 t = p(64537),
                 pt = p(68014),
                 S = p(52612);
             class b {}
             class Gt {}
-            var E = p(7666),
+            var N = p(7666),
                 g = p(88692);
 
-            function jt(n, s) {
-                if (1 & n && (t.TgZ(0, "span", 3)(1, "span", 4), t._uU(2), t.qZA(), t._UZ(3, "br"), t.TgZ(4, "span", 4), t._uU(5, " Built using Zen Dash "), t.qZA()()), 2 & n) {
+            function jt(a, s) {
+                if (1 & a && (t.TgZ(0, "span", 3)(1, "span", 4), t._uU(2), t.qZA(), t._UZ(3, "br"), t.TgZ(4, "span", 4), t._uU(5, " Built using Zen Dash "), t.qZA()()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(2), t.hij(" ", e.data.message, "")
                 }
             }
 
-            function Bt(n, s) {
-                if (1 & n && (t.TgZ(0, "span")(1, "span", 5), t._uU(2), t.qZA()()), 2 & n) {
+            function Bt(a, s) {
+                if (1 & a && (t.TgZ(0, "span")(1, "span", 5), t._uU(2), t.qZA()()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(2), t.hij(" ", e.data.message, "")
                 }
             }
 
-            function zt(n, s) {
-                if (1 & n && (t.TgZ(0, "span")(1, "span", 6), t._uU(2), t.qZA()()), 2 & n) {
+            function zt(a, s) {
+                if (1 & a && (t.TgZ(0, "span")(1, "span", 6), t._uU(2), t.qZA()()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(2), t.hij(" ", e.data.message, "")
                 }
             }
 
-            function Kt(n, s) {
-                1 & n && (t.TgZ(0, "span", 3)(1, "span", 4), t._uU(2, " Built using Zen Dash "), t.qZA()())
+            function Kt(a, s) {
+                1 & a && (t.TgZ(0, "span", 3)(1, "span", 4), t._uU(2, " Built using Zen Dash "), t.qZA()())
             }
             let F = (() => {
-                class n {
+                class a {
                     constructor(e) {
                         this.data = e
                     }
                     ngOnInit() {}
                 }
-                return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(E.qD))
-                }, n.\u0275cmp = t.Xpm({
-                    type: n,
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.Y36(N.qD))
+                }, a.\u0275cmp = t.Xpm({
+                    type: a,
                     selectors: [
                         ["app-loading"]
                     ],
                     decls: 4,
                     vars: 4,
                     consts: [
                         ["style", " width: 100%; display: inline-block;", 4, "ngIf"],
                         [4, "ngIf"],
                         ["style", "width: 100%; display: inline-block;", 4, "ngIf"],
                         [2, "width", "100%", "display", "inline-block"],
                         [1, "success"],
                         [1, "warn"],
                         [1, "error"]
                     ],
-                    template: function(e, a) {
-                        1 & e && (t.YNc(0, jt, 6, 1, "span", 0), t.YNc(1, Bt, 3, 1, "span", 1), t.YNc(2, zt, 3, 1, "span", 1), t.YNc(3, Kt, 3, 0, "span", 2)), 2 & e && (t.Q6J("ngIf", "success" === a.data.status), t.xp6(1), t.Q6J("ngIf", "warn" === a.data.status), t.xp6(1), t.Q6J("ngIf", "error" === a.data.status), t.xp6(1), t.Q6J("ngIf", "loading" === a.data.status))
+                    template: function(e, n) {
+                        1 & e && (t.YNc(0, jt, 6, 1, "span", 0), t.YNc(1, Bt, 3, 1, "span", 1), t.YNc(2, zt, 3, 1, "span", 1), t.YNc(3, Kt, 3, 0, "span", 2)), 2 & e && (t.Q6J("ngIf", "success" === n.data.status), t.xp6(1), t.Q6J("ngIf", "warn" === n.data.status), t.xp6(1), t.Q6J("ngIf", "error" === n.data.status), t.xp6(1), t.Q6J("ngIf", "loading" === n.data.status))
                     },
                     dependencies: [g.O5],
                     styles: [".warn[_ngcontent-%COMP%]{color:#ffffe0}.error[_ngcontent-%COMP%]{color:#ff69b4}.success[_ngcontent-%COMP%]{color:#90ee90;margin:auto;width:50%;padding:10px}"]
-                }), n
+                }), a
             })();
             var Dt = p(21444),
-                Y = p(35732),
+                Q = p(35732),
                 f = p(52468),
                 J = p(21312),
                 ut = p(87241),
                 _t = p(84945),
                 at = p(33568),
                 mt = p(95990),
                 ht = p(44551),
                 Xt = p(98826);
             let kt = (() => {
-                    class n {
-                        constructor(e, a) {
-                            this.aRoute = e, this.ds = a
+                    class a {
+                        constructor(e, n) {
+                            this.aRoute = e, this.ds = n
                         }
                         request_change() {
                             let e = this.ds.get_all();
                             void 0 !== this.subject && this.subject.next(e)
                         }
                         ws_or_wss() {
                             if (window.location.href.split("/?")[0].includes("https")) {
@@ -324,59 +324,59 @@
                                 return e = e.substring(0, e.length - 1), "wss://" + e
                             } {
                                 let e = window.location.href.split("?")[0].split("http://")[1];
                                 return e = e.substring(0, e.length - 1), "ws://" + e
                             }
                         }
                         delay(e) {
-                            return new Promise(a => setTimeout(a, e))
+                            return new Promise(n => setTimeout(n, e))
                         }
-                        save_data(e, a) {
+                        save_data(e, n) {
                             for (const [i, o] of Object.entries(e)) {
                                 let l = JSON.parse(o);
-                                a.input_emitter.emit({
+                                n.input_emitter.emit({
                                     calling: !0,
                                     lookup: i,
                                     t: void 0,
                                     message: void 0
-                                }), new Promise(d => setTimeout(d, 2e3)).then(() => {
-                                    a.all_input.delete(i), a.all_input.set(i, l), a.input_emitter.emit({
+                                }), new Promise(c => setTimeout(c, 2e3)).then(() => {
+                                    n.all_input.delete(i), n.all_input.set(i, l), n.input_emitter.emit({
                                         calling: !1,
                                         lookup: i,
                                         t: l,
                                         message: void 0
                                     })
                                 })
                             }
                         }
-                        connect(e, a) {
-                            "complete" === a && delete this.subject, void 0 !== a && console.log(a);
+                        connect(e, n) {
+                            "complete" === n && delete this.subject, void 0 !== n && console.log(n);
                             let i = this.ws_or_wss() + e,
                                 o = this.ds.get_all();
                             new Promise(r => setTimeout(r, 1e4)).then(() => {
                                 this.subject = (0, Xt.j)(i), this.subject.subscribe({
                                     next: r => this.save_data(r, this.ds),
                                     error: r => this.connect(i, r),
                                     complete: () => this.connect(i, "complete")
                                 }), this.subject.next(o)
                             })
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.LFG(J.gz), t.LFG(f.D))
-                    }, n.\u0275prov = t.Yz7({
-                        token: n,
-                        factory: n.\u0275fac,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.LFG(J.gz), t.LFG(f.D))
+                    }, a.\u0275prov = t.Yz7({
+                        token: a,
+                        factory: a.\u0275fac,
                         providedIn: "root"
-                    }), n
+                    }), a
                 })(),
                 D = (() => {
-                    class n {
-                        constructor(e, a, i) {
-                            this.http = e, this.dataService = a, this.ws = i, this.refresh_listener = new t.vpe, this.config = {
+                    class a {
+                        constructor(e, n, i) {
+                            this.http = e, this.dataService = n, this.ws = i, this.refresh_listener = new t.vpe, this.config = {
                                 retry_count: 2,
                                 show_right_sidebar: !1,
                                 refresh: {
                                     refresh: !0,
                                     rate_in_seconds: 300
                                 },
                                 websocket: {
@@ -385,153 +385,153 @@
                                 auth: {
                                     SSO: !1,
                                     UP_Login: !1
                                 }
                             }
                         }
                         get_url(e) {
-                            let a;
-                            if (e.includes("http")) a = e;
+                            let n;
+                            if (e.includes("http")) n = e;
                             else {
                                 let i = this.my_url();
-                                "/" === e[0] && (e = e.substring(1)), a = i + e
+                                "/" === e[0] && (e = e.substring(1)), n = i + e
                             }
-                            return a
+                            return n
                         }
                         pullConfiguration(e = "/backend/configuration") {
-                            e = this.get_url(e), this.http.get(e).subscribe(a => {
-                                this.config = a, this.config.websocket.active && this.ws.connect("/backend/ws"), this.config.refresh.refresh && this.refresh_listener.emit(!0)
+                            e = this.get_url(e), this.http.get(e).subscribe(n => {
+                                this.config = n, this.config.websocket.active && this.ws.connect("/backend/ws"), this.config.refresh.refresh && this.refresh_listener.emit(!0)
                             })
                         }
                         show_right_sidebar() {
                             return this.config.show_right_sidebar
                         }
                         get_retry() {
                             let e;
                             try {
                                 e = this.config.retry_count
                             } catch {
                                 e = 2
                             }
                             return e
                         }
-                        call_response(e, a, i) {
+                        call_response(e, n, i) {
                             let o = this.get_url(e),
                                 l = {};
                             if (void 0 !== i) {
                                 l = i;
                                 let y = this.dataService.get_all();
-                                Object.entries(y).forEach((w, Q) => {
-                                    l.append(Q, w)
+                                Object.entries(y).forEach((w, Y) => {
+                                    l.append(Y, w)
                                 })
                             } else l = this.dataService.get_all();
-                            let r, d = {
+                            let r, c = {
                                     error: "Error or Unathorized"
                                 },
                                 _ = this.get_retry();
-                            return r = void 0 === a ? this.http.post(o, l).pipe((0, at.K)((y, w) => _-- > 0 && 401 !== y.status ? (0, _t.of)(y).pipe((0, mt.g)(2e3), (0, ht.b)(() => w)) : new ut.y(Q => {
-                                Q.next(d)
-                            }))) : this.http.post(o, l, a).pipe((0, at.K)((y, w) => _-- > 0 && 401 !== y.status ? (0, _t.of)(y).pipe((0, mt.g)(1e3), (0, ht.b)(() => w)) : new ut.y(Q => {
-                                Q.next(d)
+                            return r = void 0 === n ? this.http.post(o, l).pipe((0, at.K)((y, w) => _-- > 0 && 401 !== y.status ? (0, _t.of)(y).pipe((0, mt.g)(2e3), (0, ht.b)(() => w)) : new ut.y(Y => {
+                                Y.next(c)
+                            }))) : this.http.post(o, l, n).pipe((0, at.K)((y, w) => _-- > 0 && 401 !== y.status ? (0, _t.of)(y).pipe((0, mt.g)(1e3), (0, ht.b)(() => w)) : new ut.y(Y => {
+                                Y.next(c)
                             }))), r
                         }
-                        second_call_response(e, a, i) {
+                        second_call_response(e, n, i) {
                             let o = this.get_url(e),
                                 l = this.dataService.get_all();
-                            void 0 !== a && (l[a] = i);
-                            let r, d = this.get_retry(),
+                            void 0 !== n && (l[n] = i);
+                            let r, c = this.get_retry(),
                                 _ = {
                                     error: "Error or Unathorized"
                                 };
-                            return r = this.http.post(o, l).pipe((0, at.K)((y, w) => d-- > 0 && 401 !== y.status ? (0, _t.of)(y).pipe((0, mt.g)(1e3), (0, ht.b)(() => w)) : new ut.y(Q => {
-                                Q.next(_)
+                            return r = this.http.post(o, l).pipe((0, at.K)((y, w) => c-- > 0 && 401 !== y.status ? (0, _t.of)(y).pipe((0, mt.g)(1e3), (0, ht.b)(() => w)) : new ut.y(Y => {
+                                Y.next(_)
                             }))), r
                         }
                         my_url() {
                             return window.location.href.split("?")[0]
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.LFG(Y.eN), t.LFG(f.D), t.LFG(kt))
-                    }, n.\u0275prov = t.Yz7({
-                        token: n,
-                        factory: n.\u0275fac,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.LFG(Q.eN), t.LFG(f.D), t.LFG(kt))
+                    }, a.\u0275prov = t.Yz7({
+                        token: a,
+                        factory: a.\u0275fac,
                         providedIn: "root"
-                    }), n
+                    }), a
                 })();
             var gt = p(24580),
                 At = p(44083);
             let Jt = (() => {
-                class n {
+                class a {
                     constructor(e) {
                         this.cookie = e
                     }
                     not_logged() {
                         return "" === this.cookie.get("auth_token")
                     }
                     removed_cookie() {
                         this.cookie.delete("auth_token")
                     }
                 }
-                return n.\u0275fac = function(e) {
-                    return new(e || n)(t.LFG(At.N))
-                }, n.\u0275prov = t.Yz7({
-                    token: n,
-                    factory: n.\u0275fac,
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.LFG(At.N))
+                }, a.\u0275prov = t.Yz7({
+                    token: a,
+                    factory: a.\u0275fac,
                     providedIn: "root"
-                }), n
+                }), a
             })();
             var Z = p(46842),
                 L = p(9638),
                 H = p(83331),
                 G = p(50814),
                 V = p(83319),
                 it = p(42094),
                 ft = p(64639),
                 Ot = p(25295),
                 Mt = p(46438),
                 R = p(47408);
             const Wt = ["script"];
 
-            function $t(n, s) {
-                if (1 & n && (t.TgZ(0, "mat-card-footer", 4), t._uU(1), t.qZA()), 2 & n) {
+            function $t(a, s) {
+                if (1 & a && (t.TgZ(0, "mat-card-footer", 4), t._uU(1), t.qZA()), 2 & a) {
                     const e = t.oxw(2);
                     t.xp6(1), t.hij(" ", e.getFooter(), " ")
                 }
             }
 
-            function Vt(n, s) {
-                if (1 & n) {
+            function Vt(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "mat-card")(1, "mat-card-header", 1)(2, "h4"), t._uU(3), t.qZA()(), t.TgZ(4, "mat-card-content")(5, "app-sub-entry-point", 2), t.NdJ("rd", function(i) {
                         t.CHM(e);
                         const o = t.oxw();
                         return t.KtG(o.rd.emit(i))
                     })("fd", function(i) {
                         t.CHM(e);
                         const o = t.oxw();
                         return t.KtG(o.fx.emit(i))
                     }), t.qZA()(), t.YNc(6, $t, 2, 1, "mat-card-footer", 3), t.qZA()
                 }
-                if (2 & n) {
+                if (2 & a) {
                     const e = t.oxw();
                     t.xp6(3), t.Oqu(e.getTitle()), t.xp6(2), t.Q6J("url", e.url)("isSidebar", e.isSidebar), t.xp6(1), t.Q6J("ngIf", e.getFooter())
                 }
             }
 
-            function te(n, s) {
-                if (1 & n && (t.TgZ(0, "span"), t._UZ(1, "app-custom-html", 5), t.qZA()), 2 & n) {
+            function te(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-custom-html", 5), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.url)
                 }
             }
             let tt = (() => {
-                class n {
-                    constructor(e, a) {
-                        this.ds = e, this.cd = a, this.fx = new t.vpe, this.rd = new t.vpe, this.pulled = !1, this.script_code = ""
+                class a {
+                    constructor(e, n) {
+                        this.ds = e, this.cd = n, this.fx = new t.vpe, this.rd = new t.vpe, this.pulled = !1, this.script_code = ""
                     }
                     ngOnInit() {
                         let e = "";
                         e = this.isSidebar ? "sidebar" : this.ds.get_page(), this.look_up = this.ds.input_lookup(e, this.url)
                     }
                     ngAfterViewInit() {
                         this.cd.detectChanges()
@@ -540,29 +540,29 @@
                         return void 0 !== this.ds.all_input.get(this.look_up) && this.ds.all_input.get(this.look_up)?.footer
                     }
                     getTitle() {
                         return void 0 !== this.ds.all_input.get(this.look_up) ? this.ds.all_input.get(this.look_up)?.title : ""
                     }
                     get_lookup_url() {
                         this.ds.get_page();
-                        let a = "";
-                        a = this.isSidebar ? "sidebar" : this.ds.get_page(), this.look_up = this.ds.input_lookup(a, this.url)
+                        let n = "";
+                        n = this.isSidebar ? "sidebar" : this.ds.get_page(), this.look_up = this.ds.input_lookup(n, this.url)
                     }
                 }
-                return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(f.D), t.Y36(t.sBO))
-                }, n.\u0275cmp = t.Xpm({
-                    type: n,
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.Y36(f.D), t.Y36(t.sBO))
+                }, a.\u0275cmp = t.Xpm({
+                    type: a,
                     selectors: [
                         ["app-entry-point"]
                     ],
-                    viewQuery: function(e, a) {
+                    viewQuery: function(e, n) {
                         if (1 & e && t.Gf(Wt, 5), 2 & e) {
                             let i;
-                            t.iGM(i = t.CRH()) && (a.script = i.first)
+                            t.iGM(i = t.CRH()) && (n.script = i.first)
                         }
                     },
                     inputs: {
                         url: "url",
                         isSidebar: "isSidebar"
                     },
                     outputs: {
@@ -575,141 +575,141 @@
                         [4, "ngIf"],
                         [2, "display", "flex", "justify-content", "center", "align-items", "center"],
                         [3, "url", "isSidebar", "rd", "fd"],
                         ["style", "font-size: 10px; text-align: center", 4, "ngIf"],
                         [2, "font-size", "10px", "text-align", "center"],
                         [3, "url"]
                     ],
-                    template: function(e, a) {
-                        1 & e && (t.YNc(0, Vt, 7, 4, "mat-card", 0), t.YNc(1, te, 2, 1, "span", 0)), 2 & e && (t.Q6J("ngIf", !a.ds.isFullCustom(a.look_up)), t.xp6(1), t.Q6J("ngIf", a.ds.isFullCustom(a.look_up)))
+                    template: function(e, n) {
+                        1 & e && (t.YNc(0, Vt, 7, 4, "mat-card", 0), t.YNc(1, te, 2, 1, "span", 0)), 2 & e && (t.Q6J("ngIf", !n.ds.isFullCustom(n.look_up)), t.xp6(1), t.Q6J("ngIf", n.ds.isFullCustom(n.look_up)))
                     }
-                }), n
+                }), a
             })();
 
-            function ee(n, s) {
-                1 & n && t._UZ(0, "p")
+            function ee(a, s) {
+                1 & a && t._UZ(0, "p")
             }
-            const It = function(n) {
+            const It = function(a) {
                 return {
-                    page: n
+                    page: a
                 }
             };
 
-            function ne(n, s) {
-                if (1 & n && (t.TgZ(0, "mat-list-option", 6)(1, "a", 7)(2, "mat-icon"), t._uU(3), t.qZA(), t._uU(4), t.qZA()()), 2 & n) {
+            function ne(a, s) {
+                if (1 & a && (t.TgZ(0, "mat-list-option", 6)(1, "a", 7)(2, "mat-icon"), t._uU(3), t.qZA(), t._uU(4), t.qZA()()), 2 & a) {
                     const e = t.oxw(),
-                        a = e.index,
+                        n = e.index,
                         i = e.$implicit,
                         o = t.oxw(4);
-                    t.Q6J("selected", "page_" + a === o.page), t.xp6(1), t.Udp("height", "45px"), t.Q6J("routerLink", ".")("queryParams", t.VKq(7, It, "page_" + a)), t.xp6(2), t.hij("", i.icon, " "), t.xp6(1), t.hij(" ", i.label, " ")
+                    t.Q6J("selected", "page_" + n === o.page), t.xp6(1), t.Udp("height", "45px"), t.Q6J("routerLink", ".")("queryParams", t.VKq(7, It, "page_" + n)), t.xp6(2), t.hij("", i.icon, " "), t.xp6(1), t.hij(" ", i.label, " ")
                 }
             }
 
-            function ae(n, s) {
-                if (1 & n && (t.TgZ(0, "mat-list-option", 6)(1, "a", 7)(2, "mat-icon"), t._uU(3), t.qZA(), t._uU(4), t.qZA()()), 2 & n) {
+            function ae(a, s) {
+                if (1 & a && (t.TgZ(0, "mat-list-option", 6)(1, "a", 7)(2, "mat-icon"), t._uU(3), t.qZA(), t._uU(4), t.qZA()()), 2 & a) {
                     const e = s.$implicit,
-                        a = s.index,
+                        n = s.index,
                         i = t.oxw(2).index,
                         o = t.oxw(4);
-                    t.Q6J("selected", "page_" + i + "_" + a === o.page), t.xp6(1), t.Udp("height", "45px"), t.Q6J("routerLink", ".")("queryParams", t.VKq(7, It, "page_" + i + "_" + a)), t.xp6(2), t.hij("", e.icon, " "), t.xp6(1), t.hij(" ", e.label, " ")
+                    t.Q6J("selected", "page_" + i + "_" + n === o.page), t.xp6(1), t.Udp("height", "45px"), t.Q6J("routerLink", ".")("queryParams", t.VKq(7, It, "page_" + i + "_" + n)), t.xp6(2), t.hij("", e.icon, " "), t.xp6(1), t.hij(" ", e.label, " ")
                 }
             }
 
-            function ie(n, s) {
-                if (1 & n && (t.TgZ(0, "mat-expansion-panel")(1, "mat-expansion-panel-header"), t._uU(2), t.qZA(), t.TgZ(3, "mat-nav-list"), t.YNc(4, ae, 5, 9, "mat-list-option", 8), t.qZA()()), 2 & n) {
+            function ie(a, s) {
+                if (1 & a && (t.TgZ(0, "mat-expansion-panel")(1, "mat-expansion-panel-header"), t._uU(2), t.qZA(), t.TgZ(3, "mat-nav-list"), t.YNc(4, ae, 5, 9, "mat-list-option", 8), t.qZA()()), 2 & a) {
                     const e = t.oxw().$implicit;
                     t.ekj("mat-elevation-z0", !0), t.xp6(2), t.hij(" ", e.name, " "), t.xp6(2), t.Q6J("ngForOf", e.subtabs)
                 }
             }
 
-            function se(n, s) {
-                if (1 & n && (t.TgZ(0, "span"), t.YNc(1, ee, 1, 0, "p", 3), t.YNc(2, ne, 5, 9, "ng-template", null, 4, t.W1O), t.YNc(4, ie, 5, 4, "ng-template", null, 5, t.W1O), t.qZA()), 2 & n) {
+            function se(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t.YNc(1, ee, 1, 0, "p", 3), t.YNc(2, ne, 5, 9, "ng-template", null, 4, t.W1O), t.YNc(4, ie, 5, 4, "ng-template", null, 5, t.W1O), t.qZA()), 2 & a) {
                     const e = s.$implicit,
-                        a = t.MAs(3),
+                        n = t.MAs(3),
                         i = t.MAs(5);
-                    t.xp6(1), t.Q6J("ngIf", e.icon)("ngIfThen", a)("ngIfElse", i)
+                    t.xp6(1), t.Q6J("ngIf", e.icon)("ngIfThen", n)("ngIfElse", i)
                 }
             }
 
-            function oe(n, s) {
-                if (1 & n && (t.TgZ(0, "span"), t.YNc(1, se, 6, 3, "span", 2), t.qZA()), 2 & n) {
+            function oe(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t.YNc(1, se, 6, 3, "span", 2), t.qZA()), 2 & a) {
                     const e = t.oxw(3);
                     t.xp6(1), t.Q6J("ngForOf", e.getSideData())
                 }
             }
 
-            function le(n, s) {
-                if (1 & n) {
+            function le(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.ynx(0), t._UZ(1, "mat-divider")(2, "br"), t.TgZ(3, "app-entry-point", 9), t.NdJ("fx", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(3);
                         return t.KtG(r.setFlex(l.url, i))
                     })("rd", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(3);
                         return t.KtG(r.setReactivity(l.url, i))
                     }), t.qZA(), t._UZ(4, "br"), t.BQk()
                 }
-                if (2 & n) {
+                if (2 & a) {
                     const e = s.$implicit,
-                        a = t.oxw(3);
+                        n = t.oxw(3);
                     let i;
-                    t.xp6(3), t.Q6J("hidden", null == (i = a.reactivityData.get(e.url)) ? null : i.hidden)("url", e.url)("isSidebar", !0)
+                    t.xp6(3), t.Q6J("hidden", null == (i = n.reactivityData.get(e.url)) ? null : i.hidden)("url", e.url)("isSidebar", !0)
                 }
             }
 
-            function re(n, s) {
-                if (1 & n && (t.TgZ(0, "span")(1, "mat-selection-list", 1), t.YNc(2, oe, 2, 1, "span", 0), t.qZA(), t._UZ(3, "br")(4, "br"), t.YNc(5, le, 5, 3, "ng-container", 2), t._UZ(6, "br"), t.qZA()), 2 & n) {
+            function re(a, s) {
+                if (1 & a && (t.TgZ(0, "span")(1, "mat-selection-list", 1), t.YNc(2, oe, 2, 1, "span", 0), t.qZA(), t._UZ(3, "br")(4, "br"), t.YNc(5, le, 5, 3, "ng-container", 2), t._UZ(6, "br"), t.qZA()), 2 & a) {
                     const e = t.oxw(2);
                     t.xp6(1), t.Q6J("multiple", !1), t.xp6(1), t.Q6J("ngIf", e.isSideData()), t.xp6(3), t.Q6J("ngForOf", e.side_data.filters)
                 }
             }
 
-            function pe(n, s) {
-                if (1 & n && (t.TgZ(0, "span"), t.YNc(1, re, 7, 3, "span", 0), t.qZA()), 2 & n) {
+            function pe(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t.YNc(1, re, 7, 3, "span", 0), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("ngIf", void 0 !== e.side_data)
                 }
             }
             let ce = (() => {
-                class n {
-                    constructor(e, a, i, o, l) {
-                        this.http = e, this.aRoute = a, this.call = i, this.auth = o, this.ds = l, this.size = new t.vpe, this.reactivityData = new Map, this.flexData = new Map, this.page = null, this.aRoute.queryParamMap.subscribe(r => {
+                class a {
+                    constructor(e, n, i, o, l) {
+                        this.http = e, this.aRoute = n, this.call = i, this.auth = o, this.ds = l, this.size = new t.vpe, this.reactivityData = new Map, this.flexData = new Map, this.page = null, this.aRoute.queryParamMap.subscribe(r => {
                             this.page = r.get("page")
                         })
                     }
                     ngOnInit() {
                         this.http.get(this.call.my_url() + this.url).subscribe(e => {
                             this.side_data = e, console.log(`Python library version is ${this.side_data.library_version}`);
                             try {
-                                this.side_data.tabs.forEach(a => {
-                                    throw void 0 !== a.label ? (this.page = "page_0", this.ds.defaul_page = "page_0") : void 0 !== a.name && (this.page = "page_0_0", this.ds.defaul_page = "page_0_0"), "break"
+                                this.side_data.tabs.forEach(n => {
+                                    throw void 0 !== n.label ? (this.page = "page_0", this.ds.defaul_page = "page_0") : void 0 !== n.name && (this.page = "page_0_0", this.ds.defaul_page = "page_0_0"), "break"
                                 })
                             } catch {}
                             this.size.emit(this.side_data.size)
                         })
                     }
                     getSideData() {
                         return this.side_data?.tabs
                     }
                     isSideData() {
                         return this.side_data?.tabs.length > 0
                     }
-                    setFlex(e, a) {
-                        this.flexData.set(e, a)
+                    setFlex(e, n) {
+                        this.flexData.set(e, n)
                     }
-                    setReactivity(e, a) {
-                        this.reactivityData.set(e, a)
+                    setReactivity(e, n) {
+                        this.reactivityData.set(e, n)
                     }
                 }
-                return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(Y.eN), t.Y36(J.gz), t.Y36(D), t.Y36(Jt), t.Y36(f.D))
-                }, n.\u0275cmp = t.Xpm({
-                    type: n,
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.Y36(Q.eN), t.Y36(J.gz), t.Y36(D), t.Y36(Jt), t.Y36(f.D))
+                }, a.\u0275cmp = t.Xpm({
+                    type: a,
                     selectors: [
                         ["app-sidebar"]
                     ],
                     inputs: {
                         url: "url"
                     },
                     outputs: {
@@ -725,117 +725,117 @@
                         ["thenBlock2", ""],
                         ["elseBlock2", ""],
                         [3, "selected"],
                         ["mat-list-item", "", "type", "button", 3, "routerLink", "queryParams"],
                         [3, "selected", 4, "ngFor", "ngForOf"],
                         [3, "hidden", "url", "isSidebar", "fx", "rd"]
                     ],
-                    template: function(e, a) {
-                        1 & e && t.YNc(0, pe, 2, 1, "span", 0), 2 & e && t.Q6J("ngIf", !((a.call.config.auth.SSO || a.call.config.auth.UP_Login) && a.auth.not_logged()))
+                    template: function(e, n) {
+                        1 & e && t.YNc(0, pe, 2, 1, "span", 0), 2 & e && t.Q6J("ngIf", !((n.call.config.auth.SSO || n.call.config.auth.UP_Login) && n.auth.not_logged()))
                     },
                     dependencies: [Mt.d, R.ib, R.yz, H.Hw, G.Hk, G.Tg, G.Ub, G.vS, g.sg, g.O5, J.yS, tt],
                     styles: [".mat-icon[_ngcontent-%COMP%]{vertical-align:middle}.toolbar-item-spacer[_ngcontent-%COMP%]{flex:1 1 auto}.app-container[_ngcontent-%COMP%]{height:90%;margin:0}.app-sidenav[_ngcontent-%COMP%]{width:230px}.app-sidenav-content[_ngcontent-%COMP%]{display:flex;height:100%;align-items:center;justify-content:center}"]
-                }), n
+                }), a
             })();
             var m = p(20092),
                 A = p(11997),
                 x = p(88659),
                 j = p(39665);
 
-            function de(n, s) {
-                if (1 & n) {
+            function de(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "mat-card")(1, "mat-card-content")(2, "h2"), t._uU(3, "Login with Username and Password"), t.qZA(), t.TgZ(4, "form")(5, "mat-form-field", 2)(6, "mat-label"), t._uU(7, "Username"), t.qZA(), t._UZ(8, "input", 3), t.qZA(), t.TgZ(9, "mat-form-field", 2)(10, "mat-label"), t._uU(11, "Password"), t.qZA(), t._UZ(12, "input", 4), t.qZA(), t.TgZ(13, "div", 5)(14, "button", 6), t.NdJ("click", function() {
                         t.CHM(e);
                         const i = t.oxw();
                         return t.KtG(i.login_logic())
                     }), t._uU(15, "Login"), t.qZA()()()()()
                 }
             }
 
-            function ue(n, s) {
-                if (1 & n) {
+            function ue(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "mat-card")(1, "mat-card-content")(2, "h2"), t._uU(3, "Login with Single Sign-On (SSO)"), t.qZA(), t.TgZ(4, "form")(5, "div", 5)(6, "button", 6), t.NdJ("click", function() {
                         t.CHM(e);
                         const i = t.oxw();
                         return t.KtG(i.sso_logic())
                     }), t._uU(7, "Login with SSO"), t.qZA()()()()()
                 }
             }
             let _e = (() => {
-                class n {
-                    constructor(e, a, i, o) {
-                        this.router = e, this.http = a, this.call = i, this._snackBar = o, this.is_sso = !0
+                class a {
+                    constructor(e, n, i, o) {
+                        this.router = e, this.http = n, this.call = i, this._snackBar = o, this.is_sso = !0
                     }
                     ngOnInit() {}
                     login_logic() {
                         let e = this.call.get_url("/auth/up_login");
-                        this.http.post(e, {}).subscribe(a => {
+                        this.http.post(e, {}).subscribe(n => {
                             this._snackBar.openFromComponent(F, {
                                 duration: 1e4,
                                 data: {
                                     message: "Authentication Failure",
                                     status: "error"
                                 }
                             })
                         })
                     }
                     sso_logic() {
                         let e = this.call.get_url("/auth/login");
                         window.location.replace(e)
                     }
                 }
-                return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(J.F0), t.Y36(Y.eN), t.Y36(D), t.Y36(E.ux))
-                }, n.\u0275cmp = t.Xpm({
-                    type: n,
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.Y36(J.F0), t.Y36(Q.eN), t.Y36(D), t.Y36(N.ux))
+                }, a.\u0275cmp = t.Xpm({
+                    type: a,
                     selectors: [
                         ["app-login"]
                     ],
                     decls: 3,
                     vars: 2,
                     consts: [
                         [2, "display", "flex", "justify-content", "center", "align-items", "center", "min-height", "100vh"],
                         [4, "ngIf"],
                         ["appearance", "fill"],
                         ["matInput", "", "type", "text"],
                         ["matInput", "", "type", "password"],
                         [2, "display", "flex", "justify-content", "center", "align-items", "center"],
                         ["mat-raised-button", "", "color", "primary", 3, "click"]
                     ],
-                    template: function(e, a) {
-                        1 & e && (t.TgZ(0, "div", 0), t.YNc(1, de, 16, 0, "mat-card", 1), t.YNc(2, ue, 8, 0, "mat-card", 1), t.qZA()), 2 & e && (t.xp6(1), t.Q6J("ngIf", !a.is_sso), t.xp6(1), t.Q6J("ngIf", a.is_sso))
+                    template: function(e, n) {
+                        1 & e && (t.TgZ(0, "div", 0), t.YNc(1, de, 16, 0, "mat-card", 1), t.YNc(2, ue, 8, 0, "mat-card", 1), t.qZA()), 2 & e && (t.xp6(1), t.Q6J("ngIf", !n.is_sso), t.xp6(1), t.Q6J("ngIf", n.is_sso))
                     },
                     dependencies: [m._Y, m.JL, m.F, L.lW, A.a8, A.dn, x.KE, x.hX, j.Nt, g.O5]
-                }), n
+                }), a
             })();
 
-            function me(n, s) {
-                if (1 & n) {
+            function me(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "span")(1, "button", 1), t.NdJ("click", function() {
                         t.CHM(e), t.oxw();
                         const i = t.MAs(27);
                         return t.KtG(i.toggle())
                     }), t.TgZ(2, "mat-icon"), t._uU(3, "menu"), t.qZA()()()
                 }
             }
 
-            function he(n, s) {
-                1 & n && (t.TgZ(0, "span"), t._UZ(1, "app-login"), t.qZA())
+            function he(a, s) {
+                1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-login"), t.qZA())
             }
 
-            function ge(n, s) {
-                1 & n && t._UZ(0, "router-outlet")
+            function ge(a, s) {
+                1 & a && t._UZ(0, "router-outlet")
             }
             let fe = (() => {
-                    class n {
-                        constructor(e, a, i, o, l, r, d, _, y, w, Q) {
-                            this.http = i, this.ds = o, this._snackBar = l, this.aRoute = r, this.call = d, this.titleService = _, this.clipboard = y, this.ws = w, this.auth = Q, this.durationInSeconds = 5, this.mySize = "500px", this.mySize2 = "500px", this.color = "primary", this.checked = !1, this.mobileQuery = a.matchMedia("(max-width: 600px)"), this._mobileQueryListener = () => e.detectChanges(), this.mobileQuery.addListener(this._mobileQueryListener)
+                    class a {
+                        constructor(e, n, i, o, l, r, c, _, y, w, Y) {
+                            this.http = i, this.ds = o, this._snackBar = l, this.aRoute = r, this.call = c, this.titleService = _, this.clipboard = y, this.ws = w, this.auth = Y, this.durationInSeconds = 5, this.mySize = "500px", this.mySize2 = "500px", this.color = "primary", this.checked = !1, this.mobileQuery = n.matchMedia("(max-width: 600px)"), this._mobileQueryListener = () => e.detectChanges(), this.mobileQuery.addListener(this._mobileQueryListener)
                         }
                         ngOnDestroy() {
                             this.mobileQuery.removeListener(this._mobileQueryListener)
                         }
                         setTitle() {
                             this.http.get(this.call.my_url() + "backend/title").subscribe(e => {
                                 this.titleService.setTitle(e), this.title = e
@@ -875,67 +875,67 @@
                                 duration: 1e3 * this.durationInSeconds,
                                 data: {
                                     message: "Refreshing data",
                                     status: "success"
                                 }
                             })
                         }
-                        loadExternalScript(e, a, i, o, l, r) {
-                            const d = document.head;
+                        loadExternalScript(e, n, i, o, l, r) {
+                            const c = document.head;
                             if ("javascript" === i) {
                                 const _ = document.createElement("script");
-                                _.id = this.ds.makeid(5), _.type = "text/javascript", void 0 !== e && (_.src = e), void 0 !== a && (_.text = a), _.async = l, _.defer = r, d.appendChild(_)
+                                _.id = this.ds.makeid(5), _.type = "text/javascript", void 0 !== e && (_.src = e), void 0 !== n && (_.text = n), _.async = l, _.defer = r, c.appendChild(_)
                             }
                             if ("link" === i) {
                                 const _ = document.createElement("link");
-                                _.id = this.ds.makeid(5), _.rel = o, _.href = e, d.appendChild(_)
+                                _.id = this.ds.makeid(5), _.rel = o, _.href = e, c.appendChild(_)
                             }
                         }
                         getScripts() {
                             this.http.post(this.call.my_url() + "backend/scripts", this.ds.get_all()).subscribe(e => {
-                                let a = e.scripts;
-                                for (let i of a) this.loadExternalScript(i.url, i.text, i.type, i.rel, i.async, i.defer)
+                                let n = e.scripts;
+                                for (let i of n) this.loadExternalScript(i.url, i.text, i.type, i.rel, i.async, i.defer)
                             })
                         }
-                        set_size(e, a) {
-                            a ? this.mySize2 = e : this.mySize = e
+                        set_size(e, n) {
+                            n ? this.mySize2 = e : this.mySize = e
                         }
                         saveReport() {
                             this.document_id = this.ds.makeid(32);
                             let e = new b;
-                            e.key = "document_id", e.value = this.document_id, this.ds.data_setter.emit(e), this.refresh_data(), this.call.call_response(this.call.my_url() + "backend/document", void 0, void 0).subscribe(a => {
+                            e.key = "document_id", e.value = this.document_id, this.ds.data_setter.emit(e), this.refresh_data(), this.call.call_response(this.call.my_url() + "backend/document", void 0, void 0).subscribe(n => {
                                 const i = new URL(window.location.href);
                                 i.searchParams.set("document_id", this.document_id), this.clipboard.copy(i.href), this._snackBar.openFromComponent(F, {
                                     duration: 1e3 * this.durationInSeconds,
                                     data: {
                                         message: "Document URL copied",
                                         status: "success"
                                     }
                                 })
-                            }, a => {
+                            }, n => {
                                 this._snackBar.openFromComponent(F, {
                                     duration: 1e3 * this.durationInSeconds,
                                     data: {
                                         message: "Saving report failed",
                                         status: "error"
                                     }
                                 })
                             })
                         }
-                        call_refresh(e, a, i) {
-                            console.log("call refresh"), e.config.websocket.active ? i.request_change() : a.refresh.emit("AutoRefresh")
+                        call_refresh(e, n, i) {
+                            console.log("call refresh"), e.config.websocket.active ? i.request_change() : n.refresh.emit("AutoRefresh")
                         }
                         set_auto(e) {
                             e.checked ? this.runRefresh = setInterval(this.call_refresh, 1e3 * this.call.config.refresh.rate_in_seconds, this.call, this.ds, this.ws) : clearInterval(this.runRefresh)
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(t.sBO), t.Y36(Dt.vx), t.Y36(Y.eN), t.Y36(f.D), t.Y36(E.ux), t.Y36(J.gz), t.Y36(D), t.Y36(T.Dx), t.Y36(gt.TU), t.Y36(kt), t.Y36(Jt))
-                    }, n.\u0275cmp = t.Xpm({
-                        type: n,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.Y36(t.sBO), t.Y36(Dt.vx), t.Y36(Q.eN), t.Y36(f.D), t.Y36(N.ux), t.Y36(J.gz), t.Y36(D), t.Y36(T.Dx), t.Y36(gt.TU), t.Y36(kt), t.Y36(Jt))
+                    }, a.\u0275cmp = t.Xpm({
+                        type: a,
                         selectors: [
                             ["app-root"]
                         ],
                         decls: 41,
                         vars: 16,
                         consts: [
                             ["color", "primary", "layout", "row"],
@@ -957,158 +957,158 @@
                             ["layout", "row", 2, "width", "100%", "z-index", "5"],
                             ["flex", ""],
                             [2, "float", "right"],
                             ["mat-mini-fab", "", "aria-label", "Example icon button with a filter list icon", 1, "float", 3, "color", "click"],
                             [4, "ngIf", "ngIfElse"],
                             ["withoutLogin", ""]
                         ],
-                        template: function(e, a) {
+                        template: function(e, n) {
                             if (1 & e) {
                                 const i = t.EpF();
                                 t.TgZ(0, "mat-toolbar", 0)(1, "button", 1), t.NdJ("click", function() {
                                     t.CHM(i);
                                     const l = t.MAs(23);
                                     return t.KtG(l.toggle())
                                 }), t.TgZ(2, "mat-icon"), t._uU(3, "menu"), t.qZA()(), t.TgZ(4, "span"), t._uU(5), t.qZA(), t.TgZ(6, "div", 2), t.YNc(7, me, 4, 0, "span", 3), t.TgZ(8, "button", 4)(9, "mat-icon"), t._uU(10, "more_vert"), t.qZA()()(), t.TgZ(11, "mat-menu", null, 5)(13, "button", 6), t.NdJ("click", function() {
-                                    return a.saveReport()
+                                    return n.saveReport()
                                 }), t.TgZ(14, "mat-icon"), t._uU(15, "saved_search"), t.qZA(), t.TgZ(16, "span"), t._uU(17, "Save Report"), t.qZA()(), t.TgZ(18, "button", 7)(19, "mat-slide-toggle", 8), t.NdJ("change", function(l) {
-                                    return a.set_auto(l)
+                                    return n.set_auto(l)
                                 }), t._uU(20, " Auto Refresh "), t.qZA()()()(), t.TgZ(21, "mat-sidenav-container", 9)(22, "mat-sidenav", 10, 11)(24, "mat-nav-list")(25, "app-sidebar", 12), t.NdJ("size", function(l) {
-                                    return a.set_size(l, !1)
+                                    return n.set_size(l, !1)
                                 }), t.qZA()()(), t.TgZ(26, "mat-sidenav", 13, 14)(28, "mat-nav-list")(29, "app-sidebar", 12), t.NdJ("size", function(l) {
-                                    return a.set_size(l, !0)
+                                    return n.set_size(l, !0)
                                 }), t.qZA()()(), t.TgZ(30, "mat-sidenav-content")(31, "div", 15)(32, "div", 16)(33, "div", 17)(34, "div", 18)(35, "button", 19), t.NdJ("click", function() {
-                                    return a.refresh_data()
+                                    return n.refresh_data()
                                 }), t.TgZ(36, "mat-icon"), t._uU(37, "refresh"), t.qZA()()()()()(), t.YNc(38, he, 2, 0, "span", 20), t.YNc(39, ge, 1, 0, "ng-template", null, 21, t.W1O), t.qZA()()
                             }
                             if (2 & e) {
                                 const i = t.MAs(12),
                                     o = t.MAs(40);
-                                t.xp6(5), t.Oqu(a.title), t.xp6(2), t.Q6J("ngIf", a.call.show_right_sidebar()), t.xp6(1), t.Q6J("matMenuTriggerFor", i), t.xp6(11), t.Q6J("checked", a.checked), t.xp6(3), t.Udp("width", a.mySize), t.Q6J("mode", "over"), t.xp6(3), t.Q6J("url", "backend/sidebar"), t.xp6(1), t.Udp("width", a.mySize2), t.Q6J("position", "end")("mode", "over"), t.xp6(3), t.Q6J("url", "backend/sidebar2"), t.xp6(6), t.Q6J("color", a.color), t.xp6(3), t.Q6J("ngIf", (a.call.config.auth.SSO || a.call.config.auth.UP_Login) && a.auth.not_logged())("ngIfElse", o)
+                                t.xp6(5), t.Oqu(n.title), t.xp6(2), t.Q6J("ngIf", n.call.show_right_sidebar()), t.xp6(1), t.Q6J("matMenuTriggerFor", i), t.xp6(11), t.Q6J("checked", n.checked), t.xp6(3), t.Udp("width", n.mySize), t.Q6J("mode", "over"), t.xp6(3), t.Q6J("url", "backend/sidebar"), t.xp6(1), t.Udp("width", n.mySize2), t.Q6J("position", "end")("mode", "over"), t.xp6(3), t.Q6J("url", "backend/sidebar2"), t.xp6(6), t.Q6J("color", n.color), t.xp6(3), t.Q6J("ngIf", (n.call.config.auth.SSO || n.call.config.auth.UP_Login) && n.auth.not_logged())("ngIfElse", o)
                             }
                         },
                         dependencies: [Z.Wh, Z.yH, L.lW, H.Hw, G.Hk, V.VK, V.OP, V.p6, it.JX, it.TM, it.Rh, ft.Rr, Ot.Ye, g.O5, J.lC, ce, _e],
                         styles: ["[_nghost-%COMP%]{position:absolute;left:0;right:0;bottom:0;top:0}mat-sidenav-container[_ngcontent-%COMP%]{margin:0;min-height:100%;height:100%;width:100%;display:inline-block}.increase-size[_ngcontent-%COMP%]{width:200px}mat-sidenav[_ngcontent-%COMP%]{min-width:200px}.float[_ngcontent-%COMP%]{position:fixed;bottom:1rem;right:1rem;z-index:5}.app-container[_ngcontent-%COMP%]{height:90%;margin:0}.app-sidenav[_ngcontent-%COMP%]{width:230px}.app-sidenav-content[_ngcontent-%COMP%]{display:flex;height:100%;align-items:center;justify-content:center}.toolbar-item-spacer[_ngcontent-%COMP%]{flex:1 1 auto}"]
-                    }), n
+                    }), a
                 })(),
                 xe = (() => {
-                    class n {
+                    class a {
                         constructor() {}
-                        set_title(e, a, i) {
+                        set_title(e, n, i) {
                             e.fragment.subscribe(o => {
-                                null !== o ? a.setTitle(o) : i.get("/backend/title").subscribe(l => {
-                                    a.setTitle(l)
+                                null !== o ? n.setTitle(o) : i.get("/backend/title").subscribe(l => {
+                                    n.setTitle(l)
                                 })
                             })
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)
-                    }, n.\u0275prov = t.Yz7({
-                        token: n,
-                        factory: n.\u0275fac,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)
+                    }, a.\u0275prov = t.Yz7({
+                        token: a,
+                        factory: a.\u0275fac,
                         providedIn: "root"
-                    }), n
+                    }), a
                 })();
 
-            function be(n, s) {
-                if (1 & n) {
+            function be(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "app-entry-point", 5), t.NdJ("fx", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(3);
                         return t.KtG(r.setFlex(l.url, i))
                     })("rd", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(3);
                         return t.KtG(r.setReactivity(l.url, i))
                     }), t.qZA()
                 }
-                if (2 & n) {
+                if (2 & a) {
                     const e = s.$implicit,
-                        a = t.oxw(3);
-                    let i, o, l, r, d;
-                    t.Q6J("hidden", null == (i = a.reactivityData.get(e.url)) ? null : i.hidden)("url", e.url)("isSidebar", !1)("fxFlex", (null == (o = a.flexData.get(e.url)) ? null : o.fxFlex) || "33%")("fxFlex.md", (null == (l = a.flexData.get(e.url)) ? null : l.fxFlex_md) || "33%")("fxFlex.sm", (null == (r = a.flexData.get(e.url)) ? null : r.fxFlex_sm) || "50%")("fxFlex.xs", (null == (d = a.flexData.get(e.url)) ? null : d.fxFlex_sm) || "100%")
+                        n = t.oxw(3);
+                    let i, o, l, r, c;
+                    t.Q6J("hidden", null == (i = n.reactivityData.get(e.url)) ? null : i.hidden)("url", e.url)("isSidebar", !1)("fxFlex", (null == (o = n.flexData.get(e.url)) ? null : o.fxFlex) || "33%")("fxFlex.md", (null == (l = n.flexData.get(e.url)) ? null : l.fxFlex_md) || "33%")("fxFlex.sm", (null == (r = n.flexData.get(e.url)) ? null : r.fxFlex_sm) || "50%")("fxFlex.xs", (null == (c = n.flexData.get(e.url)) ? null : c.fxFlex_sm) || "100%")
                 }
             }
 
-            function Ce(n, s) {
-                if (1 & n && (t.TgZ(0, "div", 2)(1, "mat-card")(2, "mat-card-content")(3, "div", 3), t.YNc(4, be, 1, 7, "app-entry-point", 4), t.qZA()()()()), 2 & n) {
+            function Ce(a, s) {
+                if (1 & a && (t.TgZ(0, "div", 2)(1, "mat-card")(2, "mat-card-content")(3, "div", 3), t.YNc(4, be, 1, 7, "app-entry-point", 4), t.qZA()()()()), 2 & a) {
                     const e = s.$implicit;
                     t.xp6(4), t.Q6J("ngForOf", e.data)
                 }
             }
 
-            function ve(n, s) {
-                if (1 & n && (t.TgZ(0, "div"), t.YNc(1, Ce, 5, 1, "div", 1), t.qZA()), 2 & n) {
+            function ve(a, s) {
+                if (1 & a && (t.TgZ(0, "div"), t.YNc(1, Ce, 5, 1, "div", 1), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("ngForOf", null == e.page ? null : e.page.rows)
                 }
             }
             const ye = [{
                 path: "**",
                 component: (() => {
-                    class n {
-                        constructor(e, a, i, o, l) {
-                            this.http = e, this.titleService = a, this.aRoute = i, this.call = o, this.dataService = l, this.page = void 0, this.reactivityData = new Map, this.flexData = new Map
+                    class a {
+                        constructor(e, n, i, o, l) {
+                            this.http = e, this.titleService = n, this.aRoute = i, this.call = o, this.dataService = l, this.page = void 0, this.reactivityData = new Map, this.flexData = new Map
                         }
                         ngOnInit() {
                             (new xe).set_title(this.aRoute, this.titleService, this.http), this.aRoute.queryParamMap.subscribe(e => {
-                                let a = this.dataService.get_page(),
-                                    i = (new Y.LE).set("fragment", a);
+                                let n = this.dataService.get_page(),
+                                    i = (new Q.LE).set("fragment", n);
                                 this.http.get(this.call.my_url() + "backend/page_detail", {
                                     params: i
                                 }).subscribe(o => {
                                     this.page = o
                                 })
                             })
                         }
-                        setFlex(e, a) {
-                            this.flexData.set(e, a)
+                        setFlex(e, n) {
+                            this.flexData.set(e, n)
                         }
-                        setReactivity(e, a) {
-                            this.reactivityData.set(e, a)
+                        setReactivity(e, n) {
+                            this.reactivityData.set(e, n)
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(Y.eN), t.Y36(T.Dx), t.Y36(J.gz), t.Y36(D), t.Y36(f.D))
-                    }, n.\u0275cmp = t.Xpm({
-                        type: n,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.Y36(Q.eN), t.Y36(T.Dx), t.Y36(J.gz), t.Y36(D), t.Y36(f.D))
+                    }, a.\u0275cmp = t.Xpm({
+                        type: a,
                         selectors: [
                             ["app-page"]
                         ],
                         decls: 1,
                         vars: 1,
                         consts: [
                             [4, "ngIf"],
                             ["style", "padding: 10px", 4, "ngFor", "ngForOf"],
                             [2, "padding", "10px"],
                             ["fxLayout", "row wrap", "fxLayout.lt-sm", "column", "fxLayoutGap", "row_data.layoutGap", "fxLayoutAlign", "space-around center", "fxLayoutAlign.lt-sm", "space-around stretch", "fxFlexFill", ""],
                             ["class", "padding", 3, "hidden", "url", "isSidebar", "fxFlex", "fxFlex.md", "fxFlex.sm", "fxFlex.xs", "fx", "rd", 4, "ngFor", "ngForOf"],
                             [1, "padding", 3, "hidden", "url", "isSidebar", "fxFlex", "fxFlex.md", "fxFlex.sm", "fxFlex.xs", "fx", "rd"]
                         ],
-                        template: function(e, a) {
-                            1 & e && t.YNc(0, ve, 2, 1, "div", 0), 2 & e && t.Q6J("ngIf", a.page)
+                        template: function(e, n) {
+                            1 & e && t.YNc(0, ve, 2, 1, "div", 0), 2 & e && t.Q6J("ngIf", n.page)
                         },
                         dependencies: [Z.xw, Z.SQ, Z.Wh, Z.s9, Z.yH, A.a8, A.dn, g.sg, g.O5, tt],
                         styles: [".padding[_ngcontent-%COMP%]{padding:5px;margin-bottom:1em;min-width:100px}.max[_ngcontent-%COMP%]{max-height:200px}"]
-                    }), n
+                    }), a
                 })()
             }];
             let Te = (() => {
-                class n {}
-                return n.\u0275fac = function(e) {
-                    return new(e || n)
-                }, n.\u0275mod = t.oAB({
-                    type: n
-                }), n.\u0275inj = t.cJS({
+                class a {}
+                return a.\u0275fac = function(e) {
+                    return new(e || a)
+                }, a.\u0275mod = t.oAB({
+                    type: a
+                }), a.\u0275inj = t.cJS({
                     imports: [J.Bz.forRoot(ye, {
                         relativeLinkResolution: "legacy"
                     }), J.Bz]
-                }), n
+                }), a
             })();
             var Se = p(25544),
                 we = p(38954),
                 Ze = p(58698),
                 Fe = p(27165),
                 De = p(18632),
                 ke = p(76342),
@@ -1123,299 +1123,299 @@
                 Ie = p(27084),
                 Pe = p(65429),
                 q = p(83704),
                 et = p(88696),
                 nt = p(25237),
                 vt = p(53538),
                 B = p(40827),
-                Yt = p(8697),
+                Qt = p(8697),
                 yt = p(53556),
                 st = p(18033),
-                Qt = p(96219),
+                Yt = p(96219),
                 ot = p(56558),
                 M = p(80418),
                 Tt = p(72516),
                 Ut = p(2940),
-                Ye = p(18849),
-                Qe = p(19596),
+                Qe = p(18849),
+                Ye = p(19596),
                 Ue = p(96100),
-                Nt = p(40512);
+                Et = p(40512);
 
-            function Ne(n, s) {
-                if (1 & n) {
+            function Ee(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "app-entry-point", 5), t.NdJ("fx", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(3);
                         return t.KtG(r.setFlex(l.url, i))
                     })("rd", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(3);
                         return t.KtG(r.setReactivity(l.url, i))
                     }), t.qZA()
                 }
-                if (2 & n) {
+                if (2 & a) {
                     const e = s.$implicit,
-                        a = t.oxw(3);
-                    let i, o, l, r, d;
-                    t.Q6J("hidden", null == (i = a.reactivityData.get(e.url)) ? null : i.hidden)("url", e.url)("isSidebar", !1)("fxFlex", (null == (o = a.flexData.get(e.url)) ? null : o.fxFlex) || "33%")("fxFlex.md", (null == (l = a.flexData.get(e.url)) ? null : l.fxFlex_md) || "33%")("fxFlex.sm", (null == (r = a.flexData.get(e.url)) ? null : r.fxFlex_sm) || "50%")("fxFlex.xs", (null == (d = a.flexData.get(e.url)) ? null : d.fxFlex_sm) || "100%")
+                        n = t.oxw(3);
+                    let i, o, l, r, c;
+                    t.Q6J("hidden", null == (i = n.reactivityData.get(e.url)) ? null : i.hidden)("url", e.url)("isSidebar", !1)("fxFlex", (null == (o = n.flexData.get(e.url)) ? null : o.fxFlex) || "33%")("fxFlex.md", (null == (l = n.flexData.get(e.url)) ? null : l.fxFlex_md) || "33%")("fxFlex.sm", (null == (r = n.flexData.get(e.url)) ? null : r.fxFlex_sm) || "50%")("fxFlex.xs", (null == (c = n.flexData.get(e.url)) ? null : c.fxFlex_sm) || "100%")
                 }
             }
 
-            function Ee(n, s) {
-                if (1 & n && (t.TgZ(0, "div", 2)(1, "mat-card")(2, "mat-card-content")(3, "div", 3), t.YNc(4, Ne, 1, 7, "app-entry-point", 4), t.qZA()()()()), 2 & n) {
+            function Ne(a, s) {
+                if (1 & a && (t.TgZ(0, "div", 2)(1, "mat-card")(2, "mat-card-content")(3, "div", 3), t.YNc(4, Ee, 1, 7, "app-entry-point", 4), t.qZA()()()()), 2 & a) {
                     const e = s.$implicit;
                     t.xp6(4), t.Q6J("ngForOf", e.data)
                 }
             }
 
-            function Le(n, s) {
-                if (1 & n && (t.TgZ(0, "div"), t.YNc(1, Ee, 5, 1, "div", 1), t.qZA()), 2 & n) {
+            function Le(a, s) {
+                if (1 & a && (t.TgZ(0, "div"), t.YNc(1, Ne, 5, 1, "div", 1), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("ngForOf", null == e.page ? null : e.page.rows)
                 }
             }
             let Re = (() => {
-                class n {
-                    constructor(e, a, i, o, l, r) {
-                        this.dialogRef = e, this.dialog_url = a, this.http = i, this.aRoute = o, this.call = l, this.dataService = r, this.page = void 0, this.reactivityData = new Map, this.flexData = new Map
+                class a {
+                    constructor(e, n, i, o, l, r) {
+                        this.dialogRef = e, this.dialog_url = n, this.http = i, this.aRoute = o, this.call = l, this.dataService = r, this.page = void 0, this.reactivityData = new Map, this.flexData = new Map
                     }
                     ngOnInit() {
                         let e;
                         if (this.dialog_url.includes("http")) e = this.dialog_url;
                         else {
                             let i = this.call.my_url();
                             "/" === this.dialog_url[0] && (this.dialog_url = this.dialog_url.substring(1)), e = i + this.dialog_url
                         }
-                        let a = this.dataService.get_all();
-                        this.http.post(e, a).subscribe(i => {
+                        let n = this.dataService.get_all();
+                        this.http.post(e, n).subscribe(i => {
                             this.page = i
                         })
                     }
-                    setFlex(e, a) {
-                        this.flexData.set(e, a)
+                    setFlex(e, n) {
+                        this.flexData.set(e, n)
                     }
-                    setReactivity(e, a) {
-                        this.reactivityData.set(e, a)
+                    setReactivity(e, n) {
+                        this.reactivityData.set(e, n)
                     }
                 }
-                return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(et.so), t.Y36(et.WI), t.Y36(Y.eN), t.Y36(J.gz), t.Y36(D), t.Y36(f.D))
-                }, n.\u0275cmp = t.Xpm({
-                    type: n,
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.Y36(et.so), t.Y36(et.WI), t.Y36(Q.eN), t.Y36(J.gz), t.Y36(D), t.Y36(f.D))
+                }, a.\u0275cmp = t.Xpm({
+                    type: a,
                     selectors: [
                         ["app-dialog"]
                     ],
                     decls: 1,
                     vars: 1,
                     consts: [
                         [4, "ngIf"],
                         ["style", "padding: 10px", 4, "ngFor", "ngForOf"],
                         [2, "padding", "10px"],
                         ["fxLayout", "row wrap", "fxLayout.lt-sm", "column", "fxLayoutGap", "row_data.layoutGap", "fxLayoutAlign", "space-around center", "fxLayoutAlign.lt-sm", "space-around stretch", "fxFlexFill", ""],
                         ["class", "padding", 3, "hidden", "url", "isSidebar", "fxFlex", "fxFlex.md", "fxFlex.sm", "fxFlex.xs", "fx", "rd", 4, "ngFor", "ngForOf"],
                         [1, "padding", 3, "hidden", "url", "isSidebar", "fxFlex", "fxFlex.md", "fxFlex.sm", "fxFlex.xs", "fx", "rd"]
                     ],
-                    template: function(e, a) {
-                        1 & e && t.YNc(0, Le, 2, 1, "div", 0), 2 & e && t.Q6J("ngIf", a.page)
+                    template: function(e, n) {
+                        1 & e && t.YNc(0, Le, 2, 1, "div", 0), 2 & e && t.Q6J("ngIf", n.page)
                     },
                     dependencies: [Z.xw, Z.SQ, Z.Wh, Z.s9, Z.yH, A.a8, A.dn, g.sg, g.O5, tt]
-                }), n
+                }), a
             })();
             var qe = p(8239);
-            let Et = (() => {
-                    class n {
-                        constructor(e, a, i) {
-                            this.ds = e, this.callService = a, this.dialog = i, this.input_types = ["date", "checkbox", "radio", "simple_filter", "simple_server_filter", "group_filter", "slider", "button_toggle", "toggle", "input", "download", "upload", "button", "form"], this.subscription_lookup = {}, this.d = new Map, this.data_type = ["box", "table", "chart", "image", "highchart", "custom_html"], this.call_this = new t.vpe, this.call_api = {}, this.data_ = {}, this.call_this.subscribe(o => {
+            let Nt = (() => {
+                    class a {
+                        constructor(e, n, i) {
+                            this.ds = e, this.callService = n, this.dialog = i, this.input_types = ["date", "checkbox", "radio", "simple_filter", "simple_server_filter", "group_filter", "slider", "button_toggle", "toggle", "input", "download", "upload", "button", "form"], this.subscription_lookup = {}, this.d = new Map, this.data_type = ["box", "table", "chart", "image", "highchart", "custom_html"], this.call_this = new t.vpe, this.call_api = {}, this.data_ = {}, this.call_this.subscribe(o => {
                                 this.getData(o.forced, o.url, o.look_up, o.page, o.isSidebar, "")
                             })
                         }
                         get_multi_url(e) {
-                            let a = [];
+                            let n = [];
                             switch (e.type) {
                                 case "multi_list":
                                 case "multi_tabs":
                                 case "multi_expand":
-                                    a = e.multi_data?.urls;
+                                    n = e.multi_data?.urls;
                                     break;
                                 default:
-                                    a = []
+                                    n = []
                             }
-                            return a
+                            return n
                         }
                         set_name(e) {
-                            let a = "";
+                            let n = "";
                             switch (e.type) {
                                 case "box":
-                                    a = e.box_data?.name;
+                                    n = e.box_data?.name;
                                     break;
                                 case "date":
-                                    a = e.date_data?.name;
+                                    n = e.date_data?.name;
                                     break;
                                 case "table":
-                                    a = e.table_data?.name;
+                                    n = e.table_data?.name;
                                     break;
                                 case "chart":
-                                    a = e.chart_data?.name;
+                                    n = e.chart_data?.name;
                                     break;
                                 case "radio":
-                                    a = e.radio_data?.name;
+                                    n = e.radio_data?.name;
                                     break;
                                 case "checkbox":
-                                    a = e.checkbox_data?.name;
+                                    n = e.checkbox_data?.name;
                                     break;
                                 case "slider":
-                                    a = e.slider_data?.name;
+                                    n = e.slider_data?.name;
                                     break;
                                 case "button_toggle":
                                 case "toggle":
-                                    a = e.button_toggle_data?.name;
+                                    n = e.button_toggle_data?.name;
                                     break;
                                 case "simple_filter":
                                 case "simple_server_filter":
-                                    a = e.simple_filter_data?.name;
+                                    n = e.simple_filter_data?.name;
                                     break;
                                 case "group_filter":
-                                    a = e.group_filter_data?.name;
+                                    n = e.group_filter_data?.name;
                                     break;
                                 case "input":
-                                    a = e.input_data?.name;
+                                    n = e.input_data?.name;
                                     break;
                                 case "custom_html":
-                                    a = e.custom_html?.name;
+                                    n = e.custom_html?.name;
                                     break;
                                 default:
-                                    a = ""
+                                    n = ""
                             }
-                            return a
+                            return n
                         }
-                        updateData(e, a, i, o, l) {
-                            this.saveData(e, a, i);
+                        updateData(e, n, i, o, l) {
+                            this.saveData(e, n, i);
                             let r = o?.reactive,
-                                d = o?.type,
+                                c = o?.type,
                                 _ = this.set_name(o);
-                            this.unsubscribe(l), this.subscribe(d, l, a, r, _, i, e), this.ds.all_input.set(l, o), this.ds.input_emitter.emit({
+                            this.unsubscribe(l), this.subscribe(c, l, n, r, _, i, e), this.ds.all_input.set(l, o), this.ds.input_emitter.emit({
                                 calling: !1,
                                 lookup: l,
                                 t: o,
                                 message: void 0
                             })
                         }
-                        getData(e, a, i, o, l, r) {
-                            var d = this;
+                        getData(e, n, i, o, l, r) {
+                            var c = this;
                             return (0, qe.Z)(function*() {
-                                let _ = d.ds.all_input.get(i);
-                                if (void 0 !== _ && !e) return void d.ds.input_emitter.emit({
+                                let _ = c.ds.all_input.get(i);
+                                if (void 0 !== _ && !e) return void c.ds.input_emitter.emit({
                                     calling: !1,
                                     lookup: i,
                                     t: _,
                                     message: void 0
                                 });
-                                if (d.input_types.includes(_?.type) && "Reactive" !== r && "SpecificReactive" !== r) return void d.ds.input_emitter.emit({
+                                if (c.input_types.includes(_?.type) && "Reactive" !== r && "SpecificReactive" !== r) return void c.ds.input_emitter.emit({
                                     calling: !1,
                                     lookup: i,
                                     t: _,
                                     message: void 0
                                 });
-                                void 0 !== d.subscription_lookup[i] && d.subscription_lookup[i].unsubscribe();
-                                let y = d.callService.call_response(a, void 0, void 0);
-                                return d.ds.input_emitter.emit({
+                                void 0 !== c.subscription_lookup[i] && c.subscription_lookup[i].unsubscribe();
+                                let y = c.callService.call_response(n, void 0, void 0);
+                                return c.ds.input_emitter.emit({
                                     calling: !0,
                                     lookup: i,
                                     t: void 0,
                                     message: void 0
-                                }), d.ds.all_input.delete(i), d.subscription_lookup[i] = yield y.subscribe({
+                                }), c.ds.all_input.delete(i), c.subscription_lookup[i] = yield y.subscribe({
                                     next: w => {
-                                        void 0 === w?.error ? d.updateData(l, a, o, w, i) : d.ds.input_emitter.emit({
+                                        void 0 === w?.error ? c.updateData(l, n, o, w, i) : c.ds.input_emitter.emit({
                                             calling: !1,
                                             lookup: i,
                                             t: void 0,
                                             message: w.error
                                         })
                                     },
                                     error: w => {
-                                        d.ds.input_emitter.emit({
+                                        c.ds.input_emitter.emit({
                                             calling: !1,
                                             lookup: i,
                                             t: void 0,
                                             message: w.message
                                         })
                                     }
                                 }), {
                                     error: "not called"
                                 }
                             })()
                         }
                         unsubscribe(e) {
                             this.d.get("refresh_" + e)?.unsubscribe(), this.d.get("reactive_" + e)?.unsubscribe(), this.d.get("specific_reactive_" + e)?.unsubscribe()
                         }
-                        callGetData(e, a, i, o, l) {
+                        callGetData(e, n, i, o, l) {
                             if (this.ds.get_page() === i) {
-                                let d = !1;
-                                if ("PageRefresh" === o) d = !0;
-                                else if ("RefreshButton" === o) d = !0;
-                                else if ("AutoRefresh" === o) d = !0;
-                                else if ("Reactive" === o) d = !0;
+                                let c = !1;
+                                if ("PageRefresh" === o) c = !0;
+                                else if ("RefreshButton" === o) c = !0;
+                                else if ("AutoRefresh" === o) c = !0;
+                                else if ("Reactive" === o) c = !0;
                                 else {
                                     if ("SpecificReactive" !== o) return;
-                                    d = !0
+                                    c = !0
                                 }
-                                this.getData(d, a, e, i, l, o)
+                                this.getData(c, n, e, i, l, o)
                             }
                         }
-                        subscribe(e, a, i, o, l, r, d) {
-                            this.data_type.indexOf(e) >= 0 && this.d.set("refresh_" + a, this.ds.refresh.subscribe(_ => {
-                                this.callGetData(a, i, r, _, d)
-                            })), o.full_reactive ? this.d.set("reactive_" + a, this.ds.data_setter.subscribe(_ => {
-                                _.key !== l && this.callGetData(a, i, r, "Reactive", d)
-                            })) : o.reactive_ids.length > 0 && this.d.set("specific_reactive_" + a, this.ds.data_setter.subscribe(_ => {
-                                o.reactive_ids.indexOf(_.key) >= 0 && this.callGetData(a, i, r, "SpecificReactive", d)
+                        subscribe(e, n, i, o, l, r, c) {
+                            this.data_type.indexOf(e) >= 0 && this.d.set("refresh_" + n, this.ds.refresh.subscribe(_ => {
+                                this.callGetData(n, i, r, _, c)
+                            })), o.full_reactive ? this.d.set("reactive_" + n, this.ds.data_setter.subscribe(_ => {
+                                _.key !== l && this.callGetData(n, i, r, "Reactive", c)
+                            })) : o.reactive_ids.length > 0 && this.d.set("specific_reactive_" + n, this.ds.data_setter.subscribe(_ => {
+                                o.reactive_ids.indexOf(_.key) >= 0 && this.callGetData(n, i, r, "SpecificReactive", c)
                             }))
                         }
-                        lookup(e, a) {
+                        lookup(e, n) {
                             let i = "";
-                            return i = e ? "sidebar" : this.ds.get_page(), this.ds.input_lookup(i, a)
+                            return i = e ? "sidebar" : this.ds.get_page(), this.ds.input_lookup(i, n)
                         }
-                        needToPull(e, a, i) {
-                            let o = this.lookup(e, a),
+                        needToPull(e, n, i) {
+                            let o = this.lookup(e, n),
                                 l = !1,
                                 r = this.data_[o],
-                                d = {
+                                c = {
                                     global: this.ds.data.global,
                                     page: this.ds.data[i]
                                 };
                             try {
-                                delete d.page[o], 0 === Object.keys(d.page).length && delete d.page
+                                delete c.page[o], 0 === Object.keys(c.page).length && delete c.page
                             } catch {}
-                            let _ = JSON.stringify(d);
+                            let _ = JSON.stringify(c);
                             return null !== r ? _ !== r && (l = !0) : l = !0, l
                         }
-                        saveData(e, a, i) {
-                            let o = this.lookup(e, a),
+                        saveData(e, n, i) {
+                            let o = this.lookup(e, n),
                                 l = {
                                     global: this.ds.data.global,
                                     page: this.ds.data[i]
                                 };
                             try {
                                 delete l.page[o], 0 === Object.keys(l.page).length && delete l.page
                             } catch {}
                             let r = JSON.stringify(l);
                             this.data_[o] = r
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.LFG(f.D), t.LFG(D), t.LFG(et.uw))
-                    }, n.\u0275prov = t.Yz7({
-                        token: n,
-                        factory: n.\u0275fac,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.LFG(f.D), t.LFG(D), t.LFG(et.uw))
+                    }, a.\u0275prov = t.Yz7({
+                        token: a,
+                        factory: a.\u0275fac,
                         providedIn: "root"
-                    }), n
+                    }), a
                 })(),
                 He = (() => {
-                    class n {
+                    class a {
                         constructor(e) {
                             this.ds = e
                         }
                         ngOnDestroy() {}
                         ngOnInit() {}
                         getIcon() {
                             return this.ds.all_input.get(this.url)?.box_data?.icon
@@ -1423,18 +1423,18 @@
                         getValue() {
                             return this.ds.all_input.get(this.url)?.box_data?.value
                         }
                         getName() {
                             return this.ds.all_input.get(this.url)?.box_data?.name
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(f.D))
-                    }, n.\u0275cmp = t.Xpm({
-                        type: n,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.Y36(f.D))
+                    }, a.\u0275cmp = t.Xpm({
+                        type: a,
                         selectors: [
                             ["app-box"]
                         ],
                         inputs: {
                             url: "url"
                         },
                         decls: 10,
@@ -1442,90 +1442,90 @@
                         consts: [
                             ["cols", "2", "rowHeight", "3:1"],
                             [3, "colspan", "rowspan"],
                             [1, "material-symbols-outlined"],
                             [2, "font-size", "30px", "text-align", "right"],
                             [2, "font-size", "12px", "text-align", "right"]
                         ],
-                        template: function(e, a) {
-                            1 & e && (t.TgZ(0, "mat-grid-list", 0)(1, "mat-grid-tile", 1)(2, "span", 2), t._uU(3), t.qZA()(), t.TgZ(4, "mat-grid-tile", 1)(5, "div", 3), t._uU(6), t.qZA()(), t.TgZ(7, "mat-grid-tile", 1)(8, "div", 4), t._uU(9), t.qZA()()()), 2 & e && (t.xp6(1), t.Q6J("colspan", 1)("rowspan", 2), t.xp6(2), t.hij(" ", a.getIcon(), " "), t.xp6(1), t.Q6J("colspan", 1)("rowspan", 1), t.xp6(2), t.hij(" ", a.getValue(), " "), t.xp6(1), t.Q6J("colspan", 1)("rowspan", 1), t.xp6(2), t.hij(" ", a.getName(), " "))
+                        template: function(e, n) {
+                            1 & e && (t.TgZ(0, "mat-grid-list", 0)(1, "mat-grid-tile", 1)(2, "span", 2), t._uU(3), t.qZA()(), t.TgZ(4, "mat-grid-tile", 1)(5, "div", 3), t._uU(6), t.qZA()(), t.TgZ(7, "mat-grid-tile", 1)(8, "div", 4), t._uU(9), t.qZA()()()), 2 & e && (t.xp6(1), t.Q6J("colspan", 1)("rowspan", 2), t.xp6(2), t.hij(" ", n.getIcon(), " "), t.xp6(1), t.Q6J("colspan", 1)("rowspan", 1), t.xp6(2), t.hij(" ", n.getValue(), " "), t.xp6(1), t.Q6J("colspan", 1)("rowspan", 1), t.xp6(2), t.hij(" ", n.getName(), " "))
                         },
                         dependencies: [nt.Il, nt.DX],
                         styles: [".material-symbols-outlined[_ngcontent-%COMP%]{font-size:50px;height:50px;width:50px;line-height:50px}"]
-                    }), n
+                    }), a
                 })();
 
-            function Ge(n, s) {
-                if (1 & n) {
+            function Ge(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "div")(1, "mat-form-field", 3)(2, "mat-label"), t._uU(3), t.qZA(), t.TgZ(4, "mat-date-range-input", 4)(5, "input", 5), t.NdJ("dateChange", function(i) {
                         t.CHM(e);
                         const o = t.oxw();
                         return t.KtG(o.changeValue(i))
                     }), t.qZA(), t.TgZ(6, "input", 6), t.NdJ("dateChange", function(i) {
                         t.CHM(e);
                         const o = t.oxw();
                         return t.KtG(o.changeValue(i))
                     }), t.qZA()(), t.TgZ(7, "mat-hint"), t._uU(8, "MM/DD/YYYY \u2013 MM/DD/YYYY"), t.qZA(), t._UZ(9, "mat-datepicker-toggle", 7)(10, "mat-date-range-picker", null, 8), t.qZA()()
                 }
-                if (2 & n) {
+                if (2 & a) {
                     const e = t.MAs(11),
-                        a = t.oxw();
-                    t.xp6(3), t.Oqu(a.getLabel()), t.xp6(1), t.Q6J("formGroup", a.getForm())("rangePicker", e)("comparisonStart", a.form_data.value.start)("comparisonEnd", a.form_data.value.end), t.xp6(5), t.Q6J("for", e)
+                        n = t.oxw();
+                    t.xp6(3), t.Oqu(n.getLabel()), t.xp6(1), t.Q6J("formGroup", n.getForm())("rangePicker", e)("comparisonStart", n.form_data.value.start)("comparisonEnd", n.form_data.value.end), t.xp6(5), t.Q6J("for", e)
                 }
             }
 
-            function je(n, s) {
-                if (1 & n) {
+            function je(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "div")(1, "mat-form-field", 9)(2, "mat-label"), t._uU(3), t.qZA(), t.TgZ(4, "input", 10), t.NdJ("dateChange", function(i) {
                         t.CHM(e);
                         const o = t.oxw();
                         return t.KtG(o.changeValue(i))
                     }), t.qZA(), t.TgZ(5, "mat-hint"), t._uU(6, "MM/DD/YYYY"), t.qZA(), t._UZ(7, "mat-datepicker-toggle", 7)(8, "mat-datepicker", null, 11), t.qZA()()
                 }
-                if (2 & n) {
+                if (2 & a) {
                     const e = t.MAs(9),
-                        a = t.oxw();
-                    t.xp6(3), t.Oqu(a.getLabel()), t.xp6(1), t.Q6J("matDatepicker", e)("formControl", a.form_control), t.xp6(3), t.Q6J("for", e)
+                        n = t.oxw();
+                    t.xp6(3), t.Oqu(n.getLabel()), t.xp6(1), t.Q6J("matDatepicker", e)("formControl", n.form_control), t.xp6(3), t.Q6J("for", e)
                 }
             }
             let Be = (() => {
-                class n {
+                class a {
                     constructor(e) {
                         this.ds = e
                     }
                     ngOnInit() {
                         this.getData()
                     }
                     getData() {
                         this.data = this.ds.all_input.get(this.url)?.date_data, this.data.second_date ? (this.single = !1, this.form_data = new m.nJ({
-                            start: new m.p4(new Date(this.data.first_date + "T00:00:00")),
-                            end: new m.p4(new Date(this.data.second_date + "T00:00:00"))
-                        })) : (this.single = !0, this.form_control = new m.p4(new Date(this.data.first_date + "T00:00:00")))
+                            start: new m.p4(new Date(this.data.first_date + "T00:00:00Z")),
+                            end: new m.p4(new Date(this.data.second_date + "T00:00:00Z"))
+                        })) : (this.single = !0, this.form_control = new m.p4(new Date(this.data.first_date + "T00:00:00Z")))
                     }
                     getForm() {
                         return this.form_data
                     }
                     isSingle() {
                         return this.single
                     }
                     getLabel() {
                         return this.data.name
                     }
                     changeValue(e) {
-                        let a = new b,
+                        let n = new b,
                             i = !0;
-                        a.key = this.data.name, a.url = this.url, a.page = this.ds.dataLookup(this.isSidebar), this.single ? (a.value = this.form_control.value.toISOString().substring(0, 10), a.page = this.ds.dataLookup(this.isSidebar)) : this.form_data.value.end && this.form_data.value.start ? a.value = [this.form_data.value.start.toISOString().substring(0, 10), this.form_data.value.end.toISOString().substring(0, 10)] : i = !1, i && this.ds.data_setter.emit(a)
+                        n.key = this.data.name, n.url = this.url, n.page = this.ds.dataLookup(this.isSidebar), this.single ? (n.value = this.form_control.value.toISOString().substring(0, 10), n.page = this.ds.dataLookup(this.isSidebar)) : this.form_data.value.end && this.form_data.value.start ? n.value = [this.form_data.value.start.toISOString().substring(0, 10), this.form_data.value.end.toISOString().substring(0, 10)] : i = !1, i && this.ds.data_setter.emit(n)
                     }
                 }
-                return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(f.D))
-                }, n.\u0275cmp = t.Xpm({
-                    type: n,
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.Y36(f.D))
+                }, a.\u0275cmp = t.Xpm({
+                    type: a,
                     selectors: [
                         ["app-datetime"]
                     ],
                     inputs: {
                         url: "url",
                         isSidebar: "isSidebar"
                     },
@@ -1541,83 +1541,83 @@
                         ["matEndDate", "", "placeholder", "End date", "formControlName", "end", 3, "dateChange"],
                         ["matSuffix", "", 3, "for"],
                         ["campaignOnePicker", ""],
                         ["appearance", "standard", "floatLabel", "always"],
                         ["matInput", "", 3, "matDatepicker", "formControl", "dateChange"],
                         ["dp", ""]
                     ],
-                    template: function(e, a) {
-                        1 & e && (t.TgZ(0, "mat-grid-list", 0)(1, "mat-grid-tile", 1), t.YNc(2, Ge, 12, 6, "div", 2), t.YNc(3, je, 10, 4, "div", 2), t._UZ(4, "br"), t.qZA()()), 2 & e && (t.xp6(1), t.Q6J("colspan", 4)("rowspan", 1), t.xp6(1), t.Q6J("ngIf", !a.isSingle()), t.xp6(1), t.Q6J("ngIf", a.isSingle()))
+                    template: function(e, n) {
+                        1 & e && (t.TgZ(0, "mat-grid-list", 0)(1, "mat-grid-tile", 1), t.YNc(2, Ge, 12, 6, "div", 2), t.YNc(3, je, 10, 4, "div", 2), t._UZ(4, "br"), t.qZA()()), 2 & e && (t.xp6(1), t.Q6J("colspan", 4)("rowspan", 1), t.xp6(1), t.Q6J("ngIf", !n.isSingle()), t.xp6(1), t.Q6J("ngIf", n.isSingle()))
                     },
                     dependencies: [m.Fj, m.JJ, m.JL, m.oH, m.sg, m.u, q.Mq, q.hl, q.nW, q.wx, q.zY, q.By, q._g, nt.Il, nt.DX, x.KE, x.bx, x.hX, x.R9, j.Nt, g.O5]
-                }), n
+                }), a
             })();
             var ze = p(95834);
 
-            function Ke(n, s) {
-                if (1 & n) {
+            function Ke(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "button", 14), t.NdJ("click", function() {
                         t.CHM(e);
                         const i = t.oxw();
                         return t.KtG(i.value = "")
                     }), t.TgZ(1, "mat-icon"), t._uU(2, "close"), t.qZA()()
                 }
             }
 
-            function Xe(n, s) {
-                if (1 & n && (t.TgZ(0, "mat-header-cell", 18), t._uU(1), t.qZA()), 2 & n) {
+            function Xe(a, s) {
+                if (1 & a && (t.TgZ(0, "mat-header-cell", 18), t._uU(1), t.qZA()), 2 & a) {
                     const e = t.oxw().$implicit;
                     t.xp6(1), t.Oqu(e.header)
                 }
             }
 
-            function We(n, s) {
-                if (1 & n && (t.TgZ(0, "mat-cell"), t._uU(1), t.qZA()), 2 & n) {
+            function We(a, s) {
+                if (1 & a && (t.TgZ(0, "mat-cell"), t._uU(1), t.qZA()), 2 & a) {
                     const e = s.$implicit,
-                        a = t.oxw().$implicit;
-                    t.xp6(1), t.Oqu(e[a.columnDef])
+                        n = t.oxw().$implicit;
+                    t.xp6(1), t.Oqu(e[n.columnDef])
                 }
             }
 
-            function $e(n, s) {
-                1 & n && (t.ynx(0, 15), t.YNc(1, Xe, 2, 1, "mat-header-cell", 16), t.YNc(2, We, 2, 1, "mat-cell", 17), t.BQk()), 2 & n && t.Q6J("matColumnDef", s.$implicit.columnDef)
+            function $e(a, s) {
+                1 & a && (t.ynx(0, 15), t.YNc(1, Xe, 2, 1, "mat-header-cell", 16), t.YNc(2, We, 2, 1, "mat-cell", 17), t.BQk()), 2 & a && t.Q6J("matColumnDef", s.$implicit.columnDef)
             }
 
-            function Ve(n, s) {
-                1 & n && t._UZ(0, "mat-header-row")
+            function Ve(a, s) {
+                1 & a && t._UZ(0, "mat-header-row")
             }
 
-            function tn(n, s) {
-                1 & n && t._UZ(0, "mat-row")
+            function tn(a, s) {
+                1 & a && t._UZ(0, "mat-row")
             }
 
-            function en(n, s) {
-                if (1 & n) {
+            function en(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "div", 19)(1, "div", 20)(2, "button", 21), t.NdJ("click", function() {
                         t.CHM(e);
                         const i = t.oxw();
                         return t.KtG(i.download())
                     }), t._uU(3, "Download"), t.qZA()(), t.TgZ(4, "div", 22), t._UZ(5, "mat-paginator", 23), t.qZA()()
                 }
-                if (2 & n) {
+                if (2 & a) {
                     const e = t.oxw();
                     t.xp6(5), t.Q6J("pageSizeOptions", e.items_per_page_options)("pageSize", e.items_per_page)
                 }
             }
 
-            function nn(n, s) {
-                if (1 & n && (t.TgZ(0, "div"), t._UZ(1, "mat-paginator", 23), t.qZA()), 2 & n) {
+            function nn(a, s) {
+                if (1 & a && (t.TgZ(0, "div"), t._UZ(1, "mat-paginator", 23), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("pageSizeOptions", e.items_per_page_options)("pageSize", e.items_per_page)
                 }
             }
             let an = (() => {
-                    class n {
+                    class a {
                         constructor(e) {
                             this.dataService = e, this.selection = new ze.Ov(!0, []), this.displayedColumns = []
                         }
                         ngOnInit() {
                             this.columns = this.dataService.all_input.get(this.url)?.table_data?.columns, this.dataSource = new M.by(this.dataService.all_input.get(this.url)?.table_data?.data), this.allow_download = this.dataService.all_input.get(this.url)?.table_data?.allow_download, this.items_per_page = this.dataService.all_input.get(this.url)?.table_data?.items_per_page, this.items_per_page_options = this.dataService.all_input.get(this.url)?.table_data?.items_per_page_options, this.displayedColumns = this.displayedColumns.concat(this.columns.map(e => e.columnDef))
                         }
                         ngAfterViewInit() {
@@ -1630,39 +1630,39 @@
                             this.isAllSelected() ? this.selection.clear() : this.dataSource.data.forEach(e => this.selection.select(e))
                         }
                         applyFilter(e) {
                             this.dataSource.filter = e.target.value.trim().toLowerCase()
                         }
                         download() {
                             let e = "",
-                                a = [];
-                            for (let _ = 0; _ < this.columns.length; _++) e += this.columns[_].header + ",", a.push(this.columns[_].columnDef), e = e.replace(/\n/g, "");
+                                n = [];
+                            for (let _ = 0; _ < this.columns.length; _++) e += this.columns[_].header + ",", n.push(this.columns[_].columnDef), e = e.replace(/\n/g, "");
                             e = e.substring(0, e.length - 1) + "\n";
                             const i = this.dataService.all_input.get(this.url)?.table_data?.data;
                             for (let _ = 0; _ < i.length; _++) {
-                                for (let y = 0; y < a.length; y++) e += i[_][a[y]] + ",";
+                                for (let y = 0; y < n.length; y++) e += i[_][n[y]] + ",";
                                 e = e.substring(0, e.length - 1) + "\n"
                             }
                             e = e.substring(0, e.length - 1) + "\n";
                             const o = document.createElement("a"),
-                                d = "download_file".concat(".csv");
-                            o.href = "data:text/csv;charset=utf-8," + encodeURI("\ufeff" + e), o.target = "_blank", o.download = d, o.click()
+                                c = "download_file".concat(".csv");
+                            o.href = "data:text/csv;charset=utf-8," + encodeURI("\ufeff" + e), o.target = "_blank", o.download = c, o.click()
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(f.D))
-                    }, n.\u0275cmp = t.Xpm({
-                        type: n,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.Y36(f.D))
+                    }, a.\u0275cmp = t.Xpm({
+                        type: a,
                         selectors: [
                             ["app-table"]
                         ],
-                        viewQuery: function(e, a) {
+                        viewQuery: function(e, n) {
                             if (1 & e && (t.Gf(vt.NW, 5), t.Gf(ot.YE, 5)), 2 & e) {
                                 let i;
-                                t.iGM(i = t.CRH()) && (a.paginator = i.first), t.iGM(i = t.CRH()) && (a.sort = i.first)
+                                t.iGM(i = t.CRH()) && (n.paginator = i.first), t.iGM(i = t.CRH()) && (n.sort = i.first)
                             }
                         },
                         inputs: {
                             url: "url"
                         },
                         decls: 18,
                         vars: 8,
@@ -1688,108 +1688,108 @@
                             ["mat-sort-header", ""],
                             [2, "display", "flex", "flex-wrap", "wrap"],
                             [2, "width", "15%", "padding", "1%", "margin", "2px"],
                             ["mat-raised-button", "", "color", "primary", 3, "click"],
                             [2, "width", "80%", "padding", "1%", "margin", "1px"],
                             ["showFirstLastButtons", "", 3, "pageSizeOptions", "pageSize"]
                         ],
-                        template: function(e, a) {
+                        template: function(e, n) {
                             1 & e && (t.TgZ(0, "div", 0)(1, "div", 1)(2, "mat-form-field", 2)(3, "mat-icon", 3), t._uU(4, "search"), t.qZA(), t.TgZ(5, "mat-label"), t._uU(6, "Search"), t.qZA(), t.TgZ(7, "input", 4), t.NdJ("ngModelChange", function(o) {
-                                return a.value = o
+                                return n.value = o
                             })("keyup", function(o) {
-                                return a.applyFilter(o)
-                            }), t.qZA(), t.YNc(8, Ke, 3, 0, "button", 5), t.qZA()()(), t.TgZ(9, "div", 6)(10, "mat-table", 7, 8), t.YNc(12, $e, 3, 1, "ng-container", 9), t.YNc(13, Ve, 1, 0, "mat-header-row", 10), t.YNc(14, tn, 1, 0, "mat-row", 11), t.qZA(), t.TgZ(15, "div"), t.YNc(16, en, 6, 2, "div", 12), t.YNc(17, nn, 2, 2, "div", 13), t.qZA()()), 2 & e && (t.xp6(7), t.Q6J("ngModel", a.value), t.xp6(1), t.Q6J("ngIf", a.value), t.xp6(2), t.Q6J("dataSource", a.dataSource), t.xp6(2), t.Q6J("ngForOf", a.columns), t.xp6(1), t.Q6J("matHeaderRowDef", a.displayedColumns), t.xp6(1), t.Q6J("matRowDefColumns", a.displayedColumns), t.xp6(2), t.Q6J("ngIf", a.allow_download), t.xp6(1), t.Q6J("ngIf", !a.allow_download))
+                                return n.applyFilter(o)
+                            }), t.qZA(), t.YNc(8, Ke, 3, 0, "button", 5), t.qZA()()(), t.TgZ(9, "div", 6)(10, "mat-table", 7, 8), t.YNc(12, $e, 3, 1, "ng-container", 9), t.YNc(13, Ve, 1, 0, "mat-header-row", 10), t.YNc(14, tn, 1, 0, "mat-row", 11), t.qZA(), t.TgZ(15, "div"), t.YNc(16, en, 6, 2, "div", 12), t.YNc(17, nn, 2, 2, "div", 13), t.qZA()()), 2 & e && (t.xp6(7), t.Q6J("ngModel", n.value), t.xp6(1), t.Q6J("ngIf", n.value), t.xp6(2), t.Q6J("dataSource", n.dataSource), t.xp6(2), t.Q6J("ngForOf", n.columns), t.xp6(1), t.Q6J("matHeaderRowDef", n.displayedColumns), t.xp6(1), t.Q6J("matRowDefColumns", n.displayedColumns), t.xp6(2), t.Q6J("ngIf", n.allow_download), t.xp6(1), t.Q6J("ngIf", !n.allow_download))
                         },
                         dependencies: [m.Fj, m.JJ, m.On, xt.O_, xt.D5, L.lW, H.Hw, x.KE, x.hX, x.qo, x.R9, j.Nt, vt.NW, ot.YE, ot.nU, M.BZ, M.as, M.w1, M.nj, M.ge, M.ev, M.XQ, M.Gk, g.sg, g.O5],
                         styles: ['.search-box[_ngcontent-%COMP%]   mat-form-field[_ngcontent-%COMP%]{width:100%}.table-responsive[_ngcontent-%COMP%]{display:block;overflow-x:scroll}.table-responsive[_ngcontent-%COMP%]   .mat-table[_ngcontent-%COMP%]{width:100%;max-width:100%;margin-bottom:1rem;display:table;border-collapse:collapse;margin:0}.table-responsive[_ngcontent-%COMP%]   .mat-row[_ngcontent-%COMP%], .table-responsive[_ngcontent-%COMP%]   .mat-header-row[_ngcontent-%COMP%]{display:table-row}.table-responsive[_ngcontent-%COMP%]   .mat-cell[_ngcontent-%COMP%], .table-responsive[_ngcontent-%COMP%]   .mat-header-cell[_ngcontent-%COMP%]{word-wrap:initial;display:table-cell;padding:0 5px;line-break:unset;width:auto;white-space:nowrap;overflow:hidden;vertical-align:middle}.material-symbols-outlined[_ngcontent-%COMP%]{font-variation-settings:"FILL" 1,"wght" 700,"GRAD" 200,"opsz" 48}']
-                    }), n
+                    }), a
                 })(),
                 sn = (() => {
-                    class n {
+                    class a {
                         constructor(e) {
                             this.dataService = e
                         }
                         ngOnInit() {}
                         get_options() {
                             return this.dataService.all_input.get(this.url)?.chart_data?.data
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(f.D))
-                    }, n.\u0275cmp = t.Xpm({
-                        type: n,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.Y36(f.D))
+                    }, a.\u0275cmp = t.Xpm({
+                        type: a,
                         selectors: [
                             ["app-plot"]
                         ],
                         inputs: {
                             url: "url"
                         },
                         decls: 1,
                         vars: 1,
                         consts: [
                             ["echarts", "", 1, "demo-chart", 3, "options"]
                         ],
-                        template: function(e, a) {
-                            1 & e && t._UZ(0, "div", 0), 2 & e && t.Q6J("options", a.get_options())
+                        template: function(e, n) {
+                            1 & e && t._UZ(0, "div", 0), 2 & e && t.Q6J("options", n.get_options())
                         },
-                        dependencies: [Nt._w]
-                    }), n
+                        dependencies: [Et._w]
+                    }), a
                 })();
 
-            function on(n, s) {
-                if (1 & n) {
+            function on(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "div")(1, "mat-checkbox", 4), t.NdJ("ngModelChange", function(i) {
                         const l = t.CHM(e).$implicit;
                         return t.KtG(l.selected = i)
                     })("ngModelChange", function() {
                         t.CHM(e);
                         const i = t.oxw(2);
                         return t.KtG(i.update())
                     }), t._uU(2), t.qZA()()
                 }
-                if (2 & n) {
+                if (2 & a) {
                     const e = s.$implicit;
                     t.xp6(1), t.Q6J("ngModel", e.selected), t.xp6(1), t.hij(" ", e.name, " ")
                 }
             }
 
-            function ln(n, s) {
-                if (1 & n && (t.TgZ(0, "section", 2), t.YNc(1, on, 3, 2, "div", 3), t.qZA()), 2 & n) {
+            function ln(a, s) {
+                if (1 & a && (t.TgZ(0, "section", 2), t.YNc(1, on, 3, 2, "div", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("ngForOf", e.my_data())
                 }
             }
 
-            function rn(n, s) {
-                if (1 & n) {
+            function rn(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "li")(1, "mat-checkbox", 5), t.NdJ("ngModelChange", function(i) {
                         const l = t.CHM(e).$implicit;
                         return t.KtG(l.selected = i)
                     })("ngModelChange", function() {
                         t.CHM(e);
                         const i = t.oxw(2);
                         return t.KtG(i.update())
                     }), t._uU(2), t.qZA()()
                 }
-                if (2 & n) {
+                if (2 & a) {
                     const e = s.$implicit;
                     t.xp6(1), t.Q6J("ngModel", e.selected), t.xp6(1), t.hij(" ", e.name, " ")
                 }
             }
 
-            function pn(n, s) {
-                if (1 & n && (t.TgZ(0, "section")(1, "ul"), t.YNc(2, rn, 3, 2, "li", 3), t.qZA()()), 2 & n) {
+            function pn(a, s) {
+                if (1 & a && (t.TgZ(0, "section")(1, "ul"), t.YNc(2, rn, 3, 2, "li", 3), t.qZA()()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(2), t.Q6J("ngForOf", e.my_data())
                 }
             }
             let cn = (() => {
-                class n {
+                class a {
                     constructor(e) {
                         this.ds = e
                     }
                     ngOnInit() {
                         this.getData()
                     }
                     getData() {
@@ -1802,18 +1802,18 @@
                     get_style() {
                         return this.getData().style
                     }
                     my_data() {
                         return this.getData().data
                     }
                 }
-                return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(f.D))
-                }, n.\u0275cmp = t.Xpm({
-                    type: n,
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.Y36(f.D))
+                }, a.\u0275cmp = t.Xpm({
+                    type: a,
                     selectors: [
                         ["app-checkbox"]
                     ],
                     inputs: {
                         url: "url",
                         isSidebar: "isSidebar"
                     },
@@ -1823,75 +1823,75 @@
                         ["class", "example-section", 4, "ngIf"],
                         [4, "ngIf"],
                         [1, "example-section"],
                         [4, "ngFor", "ngForOf"],
                         [1, "example-margin", 3, "ngModel", "ngModelChange"],
                         [1, "example-margin-top", 3, "ngModel", "ngModelChange"]
                     ],
-                    template: function(e, a) {
-                        1 & e && (t.YNc(0, ln, 2, 1, "section", 0), t.YNc(1, pn, 3, 1, "section", 1)), 2 & e && (t.Q6J("ngIf", "Horizontal" === a.get_style()), t.xp6(1), t.Q6J("ngIf", "Vertical" === a.get_style()))
+                    template: function(e, n) {
+                        1 & e && (t.YNc(0, ln, 2, 1, "section", 0), t.YNc(1, pn, 3, 1, "section", 1)), 2 & e && (t.Q6J("ngIf", "Horizontal" === n.get_style()), t.xp6(1), t.Q6J("ngIf", "Vertical" === n.get_style()))
                     },
                     dependencies: [m.JJ, m.On, Pt.oG, g.sg, g.O5],
                     styles: [".example-margin[_ngcontent-%COMP%]{margin-left:10px}.example-margin-top[_ngcontent-%COMP%]{margin-bottom:10px}ul[_ngcontent-%COMP%]{list-style-type:none;margin-top:4px}.example-section[_ngcontent-%COMP%]{display:flex;align-content:center;align-items:center;height:60px}"]
-                }), n
+                }), a
             })();
 
-            function dn(n, s) {
-                if (1 & n && (t.TgZ(0, "mat-radio-button", 5), t._uU(1), t.qZA()), 2 & n) {
+            function dn(a, s) {
+                if (1 & a && (t.TgZ(0, "mat-radio-button", 5), t._uU(1), t.qZA()), 2 & a) {
                     const e = s.$implicit;
                     t.Q6J("value", e), t.xp6(1), t.Oqu(e)
                 }
             }
 
-            function un(n, s) {
-                if (1 & n) {
+            function un(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "section", 2)(1, "mat-radio-group", 3), t.NdJ("ngModelChange", function(i) {
                         t.CHM(e);
                         const o = t.oxw();
                         return t.KtG(o.selected = i)
                     })("change", function() {
                         t.CHM(e);
                         const i = t.oxw();
                         return t.KtG(i.update())
                     }), t.YNc(2, dn, 2, 2, "mat-radio-button", 4), t.qZA()()
                 }
-                if (2 & n) {
+                if (2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("ngModel", e.selected), t.xp6(1), t.Q6J("ngForOf", e.getData())
                 }
             }
 
-            function _n(n, s) {
-                if (1 & n && (t.TgZ(0, "li")(1, "mat-radio-button", 7), t._uU(2), t.qZA()()), 2 & n) {
+            function _n(a, s) {
+                if (1 & a && (t.TgZ(0, "li")(1, "mat-radio-button", 7), t._uU(2), t.qZA()()), 2 & a) {
                     const e = s.$implicit;
                     t.xp6(1), t.Q6J("value", e), t.xp6(1), t.Oqu(e)
                 }
             }
 
-            function mn(n, s) {
-                if (1 & n) {
+            function mn(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "section")(1, "mat-radio-group", 3), t.NdJ("ngModelChange", function(i) {
                         t.CHM(e);
                         const o = t.oxw();
                         return t.KtG(o.selected = i)
                     })("change", function() {
                         t.CHM(e);
                         const i = t.oxw();
                         return t.KtG(i.update())
                     }), t.TgZ(2, "ul"), t.YNc(3, _n, 3, 2, "li", 6), t.qZA()()()
                 }
-                if (2 & n) {
+                if (2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("ngModel", e.selected), t.xp6(2), t.Q6J("ngForOf", e.getData())
                 }
             }
             let hn = (() => {
-                    class n {
+                    class a {
                         constructor(e) {
                             this.ds = e
                         }
                         ngOnInit() {
                             this.selected = this.ds.all_input.get(this.url)?.radio_data?.selected
                         }
                         getStyle() {
@@ -1901,18 +1901,18 @@
                             let e = new b;
                             e.page = this.ds.dataLookup(this.isSidebar), e.key = this.ds.all_input.get(this.url)?.radio_data?.name, e.value = this.selected, e.url = this.url, this.ds.data_setter.emit(e)
                         }
                         getData() {
                             return this.ds.all_input.get(this.url)?.radio_data?.data
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(f.D))
-                    }, n.\u0275cmp = t.Xpm({
-                        type: n,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.Y36(f.D))
+                    }, a.\u0275cmp = t.Xpm({
+                        type: a,
                         selectors: [
                             ["app-radio"]
                         ],
                         inputs: {
                             url: "url",
                             isSidebar: "isSidebar"
                         },
@@ -1924,23 +1924,23 @@
                             [1, "example-section"],
                             [3, "ngModel", "ngModelChange", "change"],
                             ["class", "example-radio-button", 3, "value", 4, "ngFor", "ngForOf"],
                             [1, "example-radio-button", 3, "value"],
                             [4, "ngFor", "ngForOf"],
                             [1, "example-radio-button-bottom", 3, "value"]
                         ],
-                        template: function(e, a) {
-                            1 & e && (t.YNc(0, un, 3, 2, "section", 0), t.YNc(1, mn, 4, 2, "section", 1)), 2 & e && (t.Q6J("ngIf", "Horizontal" === a.getStyle()), t.xp6(1), t.Q6J("ngIf", "Vertical" === a.getStyle()))
+                        template: function(e, n) {
+                            1 & e && (t.YNc(0, un, 3, 2, "section", 0), t.YNc(1, mn, 4, 2, "section", 1)), 2 & e && (t.Q6J("ngIf", "Horizontal" === n.getStyle()), t.xp6(1), t.Q6J("ngIf", "Vertical" === n.getStyle()))
                         },
                         dependencies: [m.JJ, m.On, yt.VQ, yt.U0, g.sg, g.O5],
                         styles: [".mat-radio-button[_ngcontent-%COMP%] ~ .mat-radio-button[_ngcontent-%COMP%]{margin-left:16px}.example-radio-group[_ngcontent-%COMP%]{display:flex;flex-direction:column;margin:15px 0;align-items:flex-start}.example-radio-button[_ngcontent-%COMP%]{margin:5px}.example-radio-button-bottom[_ngcontent-%COMP%]{margin-bottom:5px}ul[_ngcontent-%COMP%]{list-style-type:none;margin-top:4px}"]
-                    }), n
+                    }), a
                 })(),
                 gn = (() => {
-                    class n {
+                    class a {
                         constructor(e) {
                             this.ds = e
                         }
                         ngOnInit() {
                             this.value = this.ds.all_input.get(this.url)?.slider_data?.value
                         }
                         isInverted() {
@@ -1962,59 +1962,59 @@
                             return this.ds.all_input.get(this.url)?.slider_data?.vertical
                         }
                         detectChange() {
                             let e = new b;
                             e.page = this.ds.dataLookup(this.isSidebar), e.key = this.ds.all_input.get(this.url)?.slider_data?.name, e.value = this.value, e.url = this.url, this.ds.data_setter.emit(e)
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(f.D))
-                    }, n.\u0275cmp = t.Xpm({
-                        type: n,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.Y36(f.D))
+                    }, a.\u0275cmp = t.Xpm({
+                        type: a,
                         selectors: [
                             ["app-slider"]
                         ],
                         inputs: {
                             url: "url",
                             isSidebar: "isSidebar"
                         },
                         decls: 1,
                         vars: 7,
                         consts: [
                             ["aria-labelledby", "example-name-label", 1, "example-margin", 3, "invert", "max", "min", "step", "thumbLabel", "ngModel", "vertical", "ngModelChange", "change"]
                         ],
-                        template: function(e, a) {
+                        template: function(e, n) {
                             1 & e && (t.TgZ(0, "mat-slider", 0), t.NdJ("ngModelChange", function(o) {
-                                return a.value = o
+                                return n.value = o
                             })("change", function() {
-                                return a.detectChange()
-                            }), t.qZA()), 2 & e && t.Q6J("invert", a.isInverted())("max", a.isMax())("min", a.isMin())("step", a.step())("thumbLabel", a.isThumbLabel())("ngModel", a.value)("vertical", a.isVertical())
+                                return n.detectChange()
+                            }), t.qZA()), 2 & e && t.Q6J("invert", n.isInverted())("max", n.isMax())("min", n.isMin())("step", n.step())("thumbLabel", n.isThumbLabel())("ngModel", n.value)("vertical", n.isVertical())
                         },
-                        dependencies: [m.JJ, m.On, Qt.pH],
+                        dependencies: [m.JJ, m.On, Yt.pH],
                         styles: [".mat-slider-horizontal[_ngcontent-%COMP%]{width:300px}.mat-slider-vertical[_ngcontent-%COMP%]{height:150px}"]
-                    }), n
+                    }), a
                 })();
 
-            function fn(n, s) {
-                if (1 & n && (t.TgZ(0, "mat-button-toggle", 2), t._uU(1), t.qZA()), 2 & n) {
+            function fn(a, s) {
+                if (1 & a && (t.TgZ(0, "mat-button-toggle", 2), t._uU(1), t.qZA()), 2 & a) {
                     const e = s.$implicit;
                     t.Q6J("value", e.name), t.xp6(1), t.hij(" ", e.name, "")
                 }
             }
             let xn = (() => {
-                    class n {
+                    class a {
                         constructor(e) {
                             this.ds = e
                         }
                         ngOnInit() {
                             this.selected_data = this.isMultiple() ? [] : ""
                         }
                         updateData(e) {
-                            let a = new b;
-                            if (a.page = this.ds.dataLookup(this.isSidebar), a.key = this.ds.all_input.get(this.url)?.button_toggle_data?.name, a.value = e, a.url = this.url, this.ds.data_setter.emit(a), "string" == this.ds.trueTypeOf(e))
+                            let n = new b;
+                            if (n.page = this.ds.dataLookup(this.isSidebar), n.key = this.ds.all_input.get(this.url)?.button_toggle_data?.name, n.value = e, n.url = this.url, this.ds.data_setter.emit(n), "string" == this.ds.trueTypeOf(e))
                                 for (let i of this.get_buton_data()) i.selected = i.name === e;
                             else if ("array" == this.ds.trueTypeOf(e))
                                 for (let i of this.get_buton_data()) i.selected = -1 != e.indexOf(i.name)
                         }
                         onChange(e) {
                             this.updateData(e.value)
                         }
@@ -2023,124 +2023,124 @@
                         }
                         get_buton_data() {
                             return this.ds.all_input.get(this.url)?.button_toggle_data?.data
                         }
                         get_value() {
                             if (this.ds.all_input.get(this.url)?.button_toggle_data?.data) {
                                 let e = [];
-                                for (let a of this.get_buton_data()) a.selected && (this.isMultiple() ? e.push(a.name) : this.selected_data = a.name);
+                                for (let n of this.get_buton_data()) n.selected && (this.isMultiple() ? e.push(n.name) : this.selected_data = n.name);
                                 e.length > 0 && (this.selected_data = e)
                             }
                             return this.selected_data
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(f.D))
-                    }, n.\u0275cmp = t.Xpm({
-                        type: n,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.Y36(f.D))
+                    }, a.\u0275cmp = t.Xpm({
+                        type: a,
                         selectors: [
                             ["app-button-toggle"]
                         ],
                         inputs: {
                             url: "url",
                             isSidebar: "isSidebar"
                         },
                         decls: 2,
                         vars: 3,
                         consts: [
                             [3, "value", "multiple", "change"],
                             [3, "value", 4, "ngFor", "ngForOf"],
                             [3, "value"]
                         ],
-                        template: function(e, a) {
+                        template: function(e, n) {
                             1 & e && (t.TgZ(0, "mat-button-toggle-group", 0), t.NdJ("change", function(o) {
-                                return a.onChange(o)
-                            }), t.YNc(1, fn, 2, 2, "mat-button-toggle", 1), t.qZA()), 2 & e && (t.Q6J("value", a.get_value())("multiple", a.isMultiple()), t.xp6(1), t.Q6J("ngForOf", a.get_buton_data()))
+                                return n.onChange(o)
+                            }), t.YNc(1, fn, 2, 2, "mat-button-toggle", 1), t.qZA()), 2 & e && (t.Q6J("value", n.get_value())("multiple", n.isMultiple()), t.xp6(1), t.Q6J("ngForOf", n.get_buton_data()))
                         },
                         dependencies: [Ct.A9, Ct.Yi, g.sg]
-                    }), n
+                    }), a
                 })(),
                 bn = (() => {
-                    class n {
+                    class a {
                         constructor(e) {
                             this.ds = e
                         }
                         ngOnInit() {}
                         checkData() {
                             return this.ds.all_input.get(this.url)?.toggle_data?.checked
                         }
                         saveData(e) {
                             this.update(e.checked)
                         }
                         update(e) {
-                            let a = new b;
-                            a.key = this.ds.all_input.get(this.url)?.toggle_data?.name, a.value = e, a.url = this.url, a.page = this.ds.dataLookup(this.isSidebar), this.ds.data_setter.emit(a)
+                            let n = new b;
+                            n.key = this.ds.all_input.get(this.url)?.toggle_data?.name, n.value = e, n.url = this.url, n.page = this.ds.dataLookup(this.isSidebar), this.ds.data_setter.emit(n)
                         }
                         get_name() {
                             return this.ds.all_input.get(this.url)?.toggle_data?.name
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(f.D))
-                    }, n.\u0275cmp = t.Xpm({
-                        type: n,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.Y36(f.D))
+                    }, a.\u0275cmp = t.Xpm({
+                        type: a,
                         selectors: [
                             ["app-toggle"]
                         ],
                         inputs: {
                             url: "url",
                             isSidebar: "isSidebar"
                         },
                         decls: 2,
                         vars: 2,
                         consts: [
                             [3, "checked", "change"]
                         ],
-                        template: function(e, a) {
+                        template: function(e, n) {
                             1 & e && (t.TgZ(0, "mat-slide-toggle", 0), t.NdJ("change", function(o) {
-                                return a.saveData(o)
-                            }), t._uU(1), t.qZA()), 2 & e && (t.Q6J("checked", a.checkData()), t.xp6(1), t.Oqu(a.get_name()))
+                                return n.saveData(o)
+                            }), t._uU(1), t.qZA()), 2 & e && (t.Q6J("checked", n.checkData()), t.xp6(1), t.Oqu(n.get_name()))
                         },
                         dependencies: [ft.Rr]
-                    }), n
+                    }), a
                 })();
             var St = p(5557),
                 wt = p(38023),
                 Lt = p(65598),
                 z = p(13528),
                 lt = p(64325);
             const Cn = ["dataSelect"];
 
-            function vn(n, s) {
-                if (1 & n && (t.TgZ(0, "mat-option", 5), t._uU(1), t.qZA()), 2 & n) {
+            function vn(a, s) {
+                if (1 & a && (t.TgZ(0, "mat-option", 5), t._uU(1), t.qZA()), 2 & a) {
                     const e = s.$implicit;
                     t.Q6J("value", e), t.xp6(1), t.hij(" ", e, " ")
                 }
             }
             let yn = (() => {
-                class n {
+                class a {
                     constructor(e) {
-                        this.ds = e, this.dataForm = new m.p4, this.compareFn = (a, i) => a && i && a.id === i.id, this.data_select_control = new m.p4, this.data_search_control = new m.p4, this.data_search = new St.t(1), this.searching = !1, this._onDestroy = new wt.x
+                        this.ds = e, this.dataForm = new m.p4, this.compareFn = (n, i) => n && i && n.id === i.id, this.data_select_control = new m.p4, this.data_search_control = new m.p4, this.data_search = new St.t(1), this.searching = !1, this._onDestroy = new wt.x
                     }
                     ngOnInit() {
                         this.originalData(), this.searchData()
                     }
                     ngAfterViewInit() {}
                     ngOnDestroy() {
                         this._onDestroy.next(), this._onDestroy.complete()
                     }
                     setInitialValue() {
                         this.data_search.pipe((0, Lt.q)(1), (0, z.R)(this._onDestroy)).subscribe(() => {
-                            this.dataSelect.compareWith = (e, a) => e === a
+                            this.dataSelect.compareWith = (e, n) => e === n
                         })
                     }
                     filterMulti() {
                         if (!this.data) return;
                         let e = this.data_search_control.value;
-                        e ? (e = e.toLowerCase(), this.data_search.next(this.data.filter(a => a.toLowerCase().indexOf(e) > -1))) : this.data_search.next(this.data.slice())
+                        e ? (e = e.toLowerCase(), this.data_search.next(this.data.filter(n => n.toLowerCase().indexOf(e) > -1))) : this.data_search.next(this.data.slice())
                     }
                     selectedData() {
                         return this.ds.all_input.get(this.url)?.simple_filter_data?.selected
                     }
                     isMulti() {
                         return this.ds.all_input.get(this.url)?.simple_filter_data?.multi
                     }
@@ -2152,29 +2152,29 @@
                             this.filterMulti()
                         }), this.setInitialValue()
                     }
                     getLabel() {
                         return this.ds.all_input.get(this.url)?.simple_filter_data?.name
                     }
                     detectChange(e) {
-                        let a = new b;
-                        a.key = this.ds.all_input.get(this.url)?.simple_filter_data?.name, a.value = e.value, a.page = this.ds.dataLookup(this.isSidebar), a.url = this.url, this.ds.data_setter.emit(a)
+                        let n = new b;
+                        n.key = this.ds.all_input.get(this.url)?.simple_filter_data?.name, n.value = e.value, n.page = this.ds.dataLookup(this.isSidebar), n.url = this.url, this.ds.data_setter.emit(n)
                     }
                 }
-                return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(f.D))
-                }, n.\u0275cmp = t.Xpm({
-                    type: n,
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.Y36(f.D))
+                }, a.\u0275cmp = t.Xpm({
+                    type: a,
                     selectors: [
                         ["app-simple-filter"]
                     ],
-                    viewQuery: function(e, a) {
+                    viewQuery: function(e, n) {
                         if (1 & e && t.Gf(Cn, 7), 2 & e) {
                             let i;
-                            t.iGM(i = t.CRH()) && (a.dataSelect = i.first)
+                            t.iGM(i = t.CRH()) && (n.dataSelect = i.first)
                         }
                     },
                     inputs: {
                         url: "url",
                         isSidebar: "isSidebar"
                     },
                     decls: 9,
@@ -2183,98 +2183,98 @@
                         ["appearance", "fill"],
                         ["placeholder", "getLabel()", 3, "formControl", "multiple", "selectionChange"],
                         ["dataSelect", ""],
                         [3, "formControl"],
                         [3, "value", 4, "ngFor", "ngForOf"],
                         [3, "value"]
                     ],
-                    template: function(e, a) {
+                    template: function(e, n) {
                         1 & e && (t.TgZ(0, "mat-form-field", 0)(1, "mat-label"), t._uU(2), t.qZA(), t.TgZ(3, "mat-select", 1, 2), t.NdJ("selectionChange", function(o) {
-                            return a.detectChange(o)
-                        }), t.TgZ(5, "mat-option"), t._UZ(6, "ngx-mat-select-search", 3), t.qZA(), t.YNc(7, vn, 2, 2, "mat-option", 4), t.ALo(8, "async"), t.qZA()()), 2 & e && (t.xp6(2), t.Oqu(a.getLabel()), t.xp6(1), t.Q6J("formControl", a.data_select_control)("multiple", a.isMulti()), t.xp6(3), t.Q6J("formControl", a.data_search_control), t.xp6(1), t.Q6J("ngForOf", t.lcZ(8, 5, a.data_search)))
+                            return n.detectChange(o)
+                        }), t.TgZ(5, "mat-option"), t._UZ(6, "ngx-mat-select-search", 3), t.qZA(), t.YNc(7, vn, 2, 2, "mat-option", 4), t.ALo(8, "async"), t.qZA()()), 2 & e && (t.xp6(2), t.Oqu(n.getLabel()), t.xp6(1), t.Q6J("formControl", n.data_select_control)("multiple", n.isMulti()), t.xp6(3), t.Q6J("formControl", n.data_search_control), t.xp6(1), t.Q6J("ngForOf", t.lcZ(8, 5, n.data_search)))
                     },
                     dependencies: [m.JJ, m.oH, S.ey, x.KE, x.hX, st.gD, g.sg, lt.nu, g.Ov]
-                }), n
+                }), a
             })();
             const Tn = ["dataSelect"];
 
-            function Sn(n, s) {
-                if (1 & n && (t.TgZ(0, "mat-option", 7), t._uU(1), t.qZA()), 2 & n) {
+            function Sn(a, s) {
+                if (1 & a && (t.TgZ(0, "mat-option", 7), t._uU(1), t.qZA()), 2 & a) {
                     const e = s.$implicit;
                     t.Q6J("value", e), t.xp6(1), t.hij(" ", e, " ")
                 }
             }
 
-            function wn(n, s) {
-                if (1 & n && (t.TgZ(0, "mat-optgroup", 5), t.YNc(1, Sn, 2, 2, "mat-option", 6), t.qZA()), 2 & n) {
+            function wn(a, s) {
+                if (1 & a && (t.TgZ(0, "mat-optgroup", 5), t.YNc(1, Sn, 2, 2, "mat-option", 6), t.qZA()), 2 & a) {
                     const e = s.$implicit;
                     t.Q6J("label", e.group_name), t.xp6(1), t.Q6J("ngForOf", e.group_data)
                 }
             }
             let Zn = (() => {
-                class n {
+                class a {
                     constructor(e) {
                         this.ds = e, this.dataForm = new m.p4, this.data_select_control = new m.p4, this.data_search_control = new m.p4, this.data_search = new St.t(1), this._onDestroy = new wt.x
                     }
                     ngOnInit() {
                         this.myData()
                     }
                     ngAfterViewInit() {}
                     ngOnDestroy() {
                         this._onDestroy.next(), this._onDestroy.complete()
                     }
                     setInitialValue() {
                         this.data_search.pipe((0, Lt.q)(1), (0, z.R)(this._onDestroy)).subscribe(() => {
-                            this.dataSelect.compareWith = (e, a) => e === a
+                            this.dataSelect.compareWith = (e, n) => e === n
                         })
                     }
                     filterMulti() {
                         if (!this.group_data) return;
                         let e = this.data_search_control.value;
-                        const a = this.copyGroups(this.group_data);
-                        e ? (e = e.toLowerCase(), this.data_search.next(a.filter(i => (i.group_name.toLowerCase().indexOf(e) > -1 || (i.group_data = i.group_data.filter(l => l.toLowerCase().indexOf(e) > -1)), i.group_data.length > 0)))) : this.data_search.next(this.group_data.slice())
+                        const n = this.copyGroups(this.group_data);
+                        e ? (e = e.toLowerCase(), this.data_search.next(n.filter(i => (i.group_name.toLowerCase().indexOf(e) > -1 || (i.group_data = i.group_data.filter(l => l.toLowerCase().indexOf(e) > -1)), i.group_data.length > 0)))) : this.data_search.next(this.group_data.slice())
                     }
                     myData() {
                         this.data = this.ds.all_input.get(this.url)?.group_filter_data, this.multi = this.ds.all_input.get(this.url)?.group_filter_data?.multi, this.group_data = this.data.data;
                         let e = this.ds.all_input.get(this.url)?.group_filter_data?.selected;
                         void 0 !== e && e.length > 0 && (this.isMulti() ? this.data_select_control.setValue(e) : this.data_select_control.setValue(e[0])), this.data_search.next(this.group_data.slice()), this.data_search_control.valueChanges.pipe((0, z.R)(this._onDestroy)).subscribe(() => {
                             this.filterMulti()
                         }), this.setInitialValue()
                     }
                     getLabel() {
                         return this.ds.all_input.get(this.url)?.group_filter_data?.name
                     }
                     detectChange(e) {
-                        let a = new b;
-                        a.key = this.ds.all_input.get(this.url)?.group_filter_data?.name, a.value = e.value, a.page = this.ds.dataLookup(this.isSidebar), a.url = this.url, this.ds.data_setter.emit(a)
+                        let n = new b;
+                        n.key = this.ds.all_input.get(this.url)?.group_filter_data?.name, n.value = e.value, n.page = this.ds.dataLookup(this.isSidebar), n.url = this.url, this.ds.data_setter.emit(n)
                     }
                     isMulti() {
                         return this.ds.all_input.get(this.url)?.group_filter_data?.multi
                     }
                     copyGroups(e) {
-                        let a = [];
+                        let n = [];
                         return e.forEach(i => {
-                            a.push({
+                            n.push({
                                 group_name: i.group_name,
                                 group_data: i.group_data.slice()
                             })
-                        }), a
+                        }), n
                     }
                 }
-                return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(f.D))
-                }, n.\u0275cmp = t.Xpm({
-                    type: n,
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.Y36(f.D))
+                }, a.\u0275cmp = t.Xpm({
+                    type: a,
                     selectors: [
                         ["app-group-filter"]
                     ],
-                    viewQuery: function(e, a) {
+                    viewQuery: function(e, n) {
                         if (1 & e && t.Gf(Tn, 7), 2 & e) {
                             let i;
-                            t.iGM(i = t.CRH()) && (a.dataSelect = i.first)
+                            t.iGM(i = t.CRH()) && (n.dataSelect = i.first)
                         }
                     },
                     inputs: {
                         url: "url",
                         isSidebar: "isSidebar"
                     },
                     decls: 9,
@@ -2285,35 +2285,36 @@
                         ["dataSelect", ""],
                         [3, "formControl"],
                         [3, "label", 4, "ngFor", "ngForOf"],
                         [3, "label"],
                         [3, "value", 4, "ngFor", "ngForOf"],
                         [3, "value"]
                     ],
-                    template: function(e, a) {
+                    template: function(e, n) {
                         1 & e && (t.TgZ(0, "mat-form-field", 0)(1, "mat-label"), t._uU(2), t.qZA(), t.TgZ(3, "mat-select", 1, 2), t.NdJ("selectionChange", function(o) {
-                            return a.detectChange(o)
-                        }), t.TgZ(5, "mat-option"), t._UZ(6, "ngx-mat-select-search", 3), t.qZA(), t.YNc(7, wn, 2, 2, "mat-optgroup", 4), t.ALo(8, "async"), t.qZA()()), 2 & e && (t.xp6(2), t.Oqu(a.getLabel()), t.xp6(1), t.Q6J("formControl", a.data_select_control)("multiple", a.multi), t.xp6(3), t.Q6J("formControl", a.data_search_control), t.xp6(1), t.Q6J("ngForOf", t.lcZ(8, 5, a.data_search)))
+                            return n.detectChange(o)
+                        }), t.TgZ(5, "mat-option"), t._UZ(6, "ngx-mat-select-search", 3), t.qZA(), t.YNc(7, wn, 2, 2, "mat-optgroup", 4), t.ALo(8, "async"), t.qZA()()), 2 & e && (t.xp6(2), t.Oqu(n.getLabel()), t.xp6(1), t.Q6J("formControl", n.data_select_control)("multiple", n.multi), t.xp6(3), t.Q6J("formControl", n.data_search_control), t.xp6(1), t.Q6J("ngForOf", t.lcZ(8, 5, n.data_search)))
                     },
                     dependencies: [m.JJ, m.oH, S.ey, S.Nv, x.KE, x.hX, st.gD, g.sg, lt.nu, g.Ov]
-                }), n
+                }), a
             })();
+            const Fn = ["inputModel"];
 
-            function Fn(n, s) {
-                if (1 & n) {
+            function Dn(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
-                    t.TgZ(0, "button", 3), t.NdJ("click", function() {
+                    t.TgZ(0, "button", 4), t.NdJ("click", function() {
                         t.CHM(e);
                         const i = t.oxw();
                         return t.KtG(i.clearData())
                     }), t.TgZ(1, "mat-icon"), t._uU(2, "close"), t.qZA()()
                 }
             }
-            let Dn = (() => {
-                class n {
+            let kn = (() => {
+                class a {
                     constructor(e) {
                         this.ds = e
                     }
                     ngOnInit() {
                         let e = this.ds.all_input.get(this.url)?.input_data?.value;
                         void 0 !== e && (this.data = e)
                     }
@@ -2328,84 +2329,114 @@
                         e.key = this.ds.all_input.get(this.url)?.input_data?.name, e.value = this.data, e.page = this.ds.dataLookup(this.isSidebar), e.url = this.url, this.ds.data_setter.emit(e)
                     }
                     clearData() {
                         this.data = "";
                         let e = new b;
                         e.key = this.ds.all_input.get(this.url)?.input_data?.name, e.value = this.data, e.page = this.ds.dataLookup(this.isSidebar), this.ds.data_setter.emit(e)
                     }
-                }
-                return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(f.D))
-                }, n.\u0275cmp = t.Xpm({
-                    type: n,
+                    onPaste(e, n) {
+                        e.preventDefault();
+                        const i = n.selectionStart;
+                        console.log(i);
+                        const o = n.selectionEnd;
+                        if (console.log(o), e.clipboardData) {
+                            let l = e.clipboardData.getData("text/plain");
+                            if (console.log(l), null !== i && null !== o) {
+                                const r = this.data.substring(0, i),
+                                    c = this.data.substring(o);
+                                console.log("bst"), console.log(this.data), console.log(r), console.log(c), console.log("ast"), this.data = r + l + c
+                            } else this.data += l
+                        }
+                        this.saveData()
+                    }
+                }
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.Y36(f.D))
+                }, a.\u0275cmp = t.Xpm({
+                    type: a,
                     selectors: [
                         ["app-input"]
                     ],
+                    viewQuery: function(e, n) {
+                        if (1 & e && t.Gf(Fn, 5), 2 & e) {
+                            let i;
+                            t.iGM(i = t.CRH()) && (n.inputModel = i.first)
+                        }
+                    },
                     inputs: {
                         url: "url",
                         isSidebar: "isSidebar"
                     },
-                    decls: 5,
+                    decls: 6,
                     vars: 3,
                     consts: [
                         ["appearance", "fill", 1, "example-form-field"],
-                        ["matInput", "", "type", "text", 3, "ngModel", "ngModelChange"],
+                        ["matInput", "", "type", "text", 3, "ngModel", "ngModelChange", "paste"],
+                        ["inputModel", ""],
                         ["matSuffix", "", "mat-icon-button", "", "aria-label", "Clear", 3, "click", 4, "ngIf"],
                         ["matSuffix", "", "mat-icon-button", "", "aria-label", "Clear", 3, "click"]
                     ],
-                    template: function(e, a) {
-                        1 & e && (t.TgZ(0, "mat-form-field", 0)(1, "mat-label"), t._uU(2), t.qZA(), t.TgZ(3, "input", 1), t.NdJ("ngModelChange", function(o) {
-                            return a.data = o
-                        })("ngModelChange", function() {
-                            return a.saveData()
-                        }), t.qZA(), t.YNc(4, Fn, 3, 0, "button", 2), t.qZA()), 2 & e && (t.xp6(2), t.hij(" ", a.getLabel(), ""), t.xp6(1), t.Q6J("ngModel", a.data), t.xp6(1), t.Q6J("ngIf", a.data))
+                    template: function(e, n) {
+                        if (1 & e) {
+                            const i = t.EpF();
+                            t.TgZ(0, "mat-form-field", 0)(1, "mat-label"), t._uU(2), t.qZA(), t.TgZ(3, "input", 1, 2), t.NdJ("ngModelChange", function(l) {
+                                return n.data = l
+                            })("ngModelChange", function() {
+                                return n.saveData()
+                            })("paste", function(l) {
+                                t.CHM(i);
+                                const r = t.MAs(4);
+                                return t.KtG(n.onPaste(l, r))
+                            }), t.qZA(), t.YNc(5, Dn, 3, 0, "button", 3), t.qZA()
+                        }
+                        2 & e && (t.xp6(2), t.hij(" ", n.getLabel(), ""), t.xp6(1), t.Q6J("ngModel", n.data), t.xp6(2), t.Q6J("ngIf", n.data))
                     },
                     dependencies: [m.Fj, m.JJ, m.On, L.lW, H.Hw, x.KE, x.hX, x.R9, j.Nt, g.O5]
-                }), n
+                }), a
             })();
             var Rt = p(33441);
 
-            function kn(n, s) {
-                1 & n && (t.TgZ(0, "span"), t._UZ(1, "br")(2, "br")(3, "br")(4, "mat-progress-bar", 2), t.qZA())
+            function An(a, s) {
+                1 & a && (t.TgZ(0, "span"), t._UZ(1, "br")(2, "br")(3, "br")(4, "mat-progress-bar", 2), t.qZA())
             }
-            let An = (() => {
-                class n {
-                    constructor(e, a, i, o) {
-                        this.ds = e, this.fileSaverService = a, this.callService = i, this._snackBar = o, this.show = !1
+            let Jn = (() => {
+                class a {
+                    constructor(e, n, i, o) {
+                        this.ds = e, this.fileSaverService = n, this.callService = i, this._snackBar = o, this.show = !1
                     }
                     getFileName(e) {
-                        let a = /filename\*=UTF-8''([\w%\-\.]+)(?:; ?|$)/i,
+                        let n = /filename\*=UTF-8''([\w%\-\.]+)(?:; ?|$)/i,
                             i = /^filename=(["']?)(.*?[^\\])\1(?:; ?|$)/i,
                             o = null;
-                        if (a.test(e)) {
-                            let l = a.exec(e);
+                        if (n.test(e)) {
+                            let l = n.exec(e);
                             o = decodeURIComponent(l[1])
                         } else {
                             const l = e.toLowerCase().indexOf("filename=");
                             if (l >= 0) {
                                 const r = e.slice(l),
-                                    d = i.exec(r);
-                                null != d && d[2] && (o = d[2])
+                                    c = i.exec(r);
+                                null != c && c[2] && (o = c[2])
                             }
                         }
                         return o
                     }
                     onSave() {
                         this.show = !0, void 0 !== this.downloadCall && this.downloadCall.unsubscribe();
                         let e = this.callService.call_response(this.data?.url, {
                             responseType: "blob",
                             observe: "response"
                         }, void 0);
-                        this.downloadCall = e.subscribe(a => {
+                        this.downloadCall = e.subscribe(n => {
                             let i = new b;
                             i.page = this.ds.dataLookup(!1), i.key = this.ds.all_input.get(this.url)?.download_data?.name, i.value = this.ds.makeid(2), i.url = this.url, this.ds.data_setter.emit(i);
-                            let o = a.headers.get("content-disposition"),
+                            let o = n.headers.get("content-disposition"),
                                 l = this.getFileName(o);
-                            this.fileSaverService.save(a.body, l), this.show = !1
-                        }, a => {
+                            this.fileSaverService.save(n.body, l), this.show = !1
+                        }, n => {
                             this.show = !1, this._snackBar.openFromComponent(F, {
                                 duration: 5e3,
                                 data: {
                                     message: "Failed download",
                                     status: "error"
                                 }
                             })
@@ -2416,63 +2447,63 @@
                     }
                     fileLabel() {
                         return this.data?.label
                     }
                     onSuc(e) {}
                     onErr(e) {}
                 }
-                return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(f.D), t.Y36(Rt.m9), t.Y36(D), t.Y36(E.ux))
-                }, n.\u0275cmp = t.Xpm({
-                    type: n,
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.Y36(f.D), t.Y36(Rt.m9), t.Y36(D), t.Y36(N.ux))
+                }, a.\u0275cmp = t.Xpm({
+                    type: a,
                     selectors: [
                         ["app-app-download"]
                     ],
                     inputs: {
                         url: "url"
                     },
                     decls: 3,
                     vars: 2,
                     consts: [
                         ["mat-raised-button", "", "color", "primary", 3, "click", "success", "error"],
                         [4, "ngIf"],
                         ["mode", "indeterminate"]
                     ],
-                    template: function(e, a) {
+                    template: function(e, n) {
                         1 & e && (t.TgZ(0, "button", 0), t.NdJ("click", function() {
-                            return a.onSave()
+                            return n.onSave()
                         })("success", function(o) {
-                            return a.onSuc(o)
+                            return n.onSuc(o)
                         })("error", function(o) {
-                            return a.onErr(o)
-                        }), t._uU(1), t.qZA(), t.YNc(2, kn, 5, 0, "span", 1)), 2 & e && (t.xp6(1), t.hij(" Download ", a.fileLabel(), "\n"), t.xp6(1), t.Q6J("ngIf", a.show))
+                            return n.onErr(o)
+                        }), t._uU(1), t.qZA(), t.YNc(2, An, 5, 0, "span", 1)), 2 & e && (t.xp6(1), t.hij(" Download ", n.fileLabel(), "\n"), t.xp6(1), t.Q6J("ngIf", n.show))
                     },
                     dependencies: [L.lW, B.pW, g.O5]
-                }), n
+                }), a
             })();
 
-            function Jn(n, s) {
-                1 & n && (t.TgZ(0, "span"), t._UZ(1, "br")(2, "br")(3, "br")(4, "mat-progress-bar", 2), t.qZA())
+            function On(a, s) {
+                1 & a && (t.TgZ(0, "span"), t._UZ(1, "br")(2, "br")(3, "br")(4, "mat-progress-bar", 2), t.qZA())
             }
-            let On = (() => {
-                    class n {
-                        constructor(e, a, i) {
-                            this.ds = e, this.callService = a, this._snackBar = i, this.myFiles = [], this.show = !1
+            let Mn = (() => {
+                    class a {
+                        constructor(e, n, i) {
+                            this.ds = e, this.callService = n, this._snackBar = i, this.myFiles = [], this.show = !1
                         }
                         ngOnInit() {
                             this.data = this.ds.all_input.get(this.url)?.upload_data
                         }
                         getMultiple() {
                             return this.data?.multi
                         }
                         saveData(e) {
                             this.show = !0;
-                            for (var a = 0; a < e.target.files.length; a++) this.myFiles.push(e.target.files[a]);
+                            for (var n = 0; n < e.target.files.length; n++) this.myFiles.push(e.target.files[n]);
                             const i = new FormData;
-                            for (a = 0; a < this.myFiles.length; a++) i.append("files", this.myFiles[a]);
+                            for (n = 0; n < this.myFiles.length; n++) i.append("files", this.myFiles[n]);
                             void 0 !== this.uploadCall && this.uploadCall.unsubscribe();
                             let o = this.callService.call_response(this.data?.url, void 0, i);
                             this.uploadCall = o.subscribe(l => {
                                 this._snackBar.openFromComponent(F, {
                                     duration: 5e3,
                                     data: {
                                         message: "Sucessfully Uploaded file",
@@ -2488,101 +2519,101 @@
                                         message: "Failed Uploaded file",
                                         status: "error"
                                     }
                                 })
                             })
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(f.D), t.Y36(D), t.Y36(E.ux))
-                    }, n.\u0275cmp = t.Xpm({
-                        type: n,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.Y36(f.D), t.Y36(D), t.Y36(N.ux))
+                    }, a.\u0275cmp = t.Xpm({
+                        type: a,
                         selectors: [
                             ["app-app-upload"]
                         ],
                         inputs: {
                             url: "url"
                         },
                         decls: 2,
                         vars: 2,
                         consts: [
                             ["type", "file", 1, "file-upload", 3, "multiple", "change"],
                             [4, "ngIf"],
                             ["mode", "indeterminate"]
                         ],
-                        template: function(e, a) {
+                        template: function(e, n) {
                             1 & e && (t.TgZ(0, "input", 0), t.NdJ("change", function(o) {
-                                return a.saveData(o)
-                            }), t.qZA(), t.YNc(1, Jn, 5, 0, "span", 1)), 2 & e && (t.Q6J("multiple", a.getMultiple()), t.xp6(1), t.Q6J("ngIf", a.show))
+                                return n.saveData(o)
+                            }), t.qZA(), t.YNc(1, On, 5, 0, "span", 1)), 2 & e && (t.Q6J("multiple", n.getMultiple()), t.xp6(1), t.Q6J("ngIf", n.show))
                         },
                         dependencies: [B.pW, g.O5]
-                    }), n
+                    }), a
                 })(),
-                Mn = (() => {
-                    class n {
-                        constructor(e, a, i) {
-                            this.dataService = e, this.sanitizer = a, this.callService = i
+                In = (() => {
+                    class a {
+                        constructor(e, n, i) {
+                            this.dataService = e, this.sanitizer = n, this.callService = i
                         }
                         get_data() {
                             this.data = this.dataService.get_input_data(this.url)?.image_data
                         }
                         get_image() {
                             this.height = this.data.height, this.width = this.data.width, void 0 !== this.imageCall && this.imageCall.unsubscribe();
                             let e = this.callService.call_response(this.data.url, {
                                 responseType: "blob",
                                 observe: "response"
                             }, void 0);
-                            this.imageCall = e.subscribe(a => {
-                                this.image = a.body, null !== this.image && (this.imageURL = this.sanitizer.bypassSecurityTrustUrl(URL.createObjectURL(this.image)))
+                            this.imageCall = e.subscribe(n => {
+                                this.image = n.body, null !== this.image && (this.imageURL = this.sanitizer.bypassSecurityTrustUrl(URL.createObjectURL(this.image)))
                             })
                         }
                         ngOnInit() {
                             this.get_data(), this.get_image()
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(f.D), t.Y36(T.H7), t.Y36(D))
-                    }, n.\u0275cmp = t.Xpm({
-                        type: n,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.Y36(f.D), t.Y36(T.H7), t.Y36(D))
+                    }, a.\u0275cmp = t.Xpm({
+                        type: a,
                         selectors: [
                             ["app-app-image"]
                         ],
                         inputs: {
                             url: "url"
                         },
                         decls: 2,
                         vars: 5,
                         consts: [
                             ["mat-card-sm-image", "", 3, "src"]
                         ],
-                        template: function(e, a) {
-                            1 & e && (t.TgZ(0, "span"), t._UZ(1, "img", 0), t.qZA()), 2 & e && (t.xp6(1), t.Udp("height", a.height)("width", a.width), t.Q6J("src", a.imageURL, t.LSH))
+                        template: function(e, n) {
+                            1 & e && (t.TgZ(0, "span"), t._UZ(1, "img", 0), t.qZA()), 2 & e && (t.xp6(1), t.Udp("height", n.height)("width", n.width), t.Q6J("src", n.imageURL, t.LSH))
                         },
                         dependencies: [A.vP]
-                    }), n
+                    }), a
                 })();
-            var In = p(63156),
-                Pn = p(74970),
+            var Pn = p(63156),
+                Qn = p(74970),
                 Yn = p(98168),
-                Qn = p(83151),
-                Un = p(27969);
+                Un = p(83151),
+                En = p(27969);
 
-            function Nn(n, s) {
-                if (1 & n && (t.TgZ(0, "mat-option", 5), t._uU(1), t.qZA()), 2 & n) {
+            function Nn(a, s) {
+                if (1 & a && (t.TgZ(0, "mat-option", 5), t._uU(1), t.qZA()), 2 & a) {
                     const e = s.$implicit;
                     t.Q6J("value", e), t.xp6(1), t.hij(" ", e, " ")
                 }
             }
-            let En = (() => {
-                    class n {
-                        constructor(e, a) {
-                            this.ds = e, this.callService = a, this.multi = !1, this.compareFn = (i, o) => i && o && i.id === o.id, this.items = [], this.ServerSideCtrl = new m.p4, this.ServerSideFilteringCtrl = new m.p4, this.searching = !1, this.filteredServerSideBanks = new St.t(1), this._onDestroy = new wt.x
+            let Ln = (() => {
+                    class a {
+                        constructor(e, n) {
+                            this.ds = e, this.callService = n, this.multi = !1, this.compareFn = (i, o) => i && o && i.id === o.id, this.items = [], this.ServerSideCtrl = new m.p4, this.ServerSideFilteringCtrl = new m.p4, this.searching = !1, this.filteredServerSideBanks = new St.t(1), this._onDestroy = new wt.x
                         }
                         ngOnInit() {
-                            this.originalData(), this.ServerSideFilteringCtrl.valueChanges.pipe((0, Pn.h)(e => !!e), (0, Yn.b)(() => this.searching = !0), (0, z.R)(this._onDestroy), (0, Qn.b)(200), (0, Un.U)(e => this.items && e ? e : []), (0, z.R)(this._onDestroy)).subscribe(e => {
+                            this.originalData(), this.ServerSideFilteringCtrl.valueChanges.pipe((0, Qn.h)(e => !!e), (0, Yn.b)(() => this.searching = !0), (0, z.R)(this._onDestroy), (0, Un.b)(200), (0, En.U)(e => this.items && e ? e : []), (0, z.R)(this._onDestroy)).subscribe(e => {
                                 this.pullData(e).subscribe(i => {
                                     this.searching = !1;
                                     let r, o = this.ServerSideCtrl.value,
                                         l = i.simple_fitler_data;
                                     r = null !== o ? l.concat(o) : l, this.filteredServerSideBanks.next(r)
                                 }, i => {
                                     this.searching = !1
@@ -2602,22 +2633,22 @@
                             let e = this.ds.all_input.get(this.url)?.simple_server_filter_data?.data;
                             e = e.concat(this.selectedData()), this.data = [...new Set(e)], this.name = this.ds.all_input.get(this.url)?.simple_server_filter_data?.name, this.server_url = this.ds.all_input.get(this.url)?.simple_server_filter_data?.url, void 0 !== this.selectedData() && this.selectedData().length > 0 && (this.isMulti() ? this.ServerSideCtrl.setValue(this.selectedData()) : this.ServerSideCtrl.setValue(this.selectedData()[0])), this.filteredServerSideBanks.next(this.data.slice())
                         }
                         pullData(e) {
                             return this.callService.second_call_response(this.server_url, this.name, e)
                         }
                         detectChange(e) {
-                            let a = new b;
-                            a.key = this.ds.all_input.get(this.url)?.simple_server_filter_data?.name, a.value = e.value, a.page = this.ds.dataLookup(this.isSidebar), a.url = this.url, this.ds.data_setter.emit(a)
+                            let n = new b;
+                            n.key = this.ds.all_input.get(this.url)?.simple_server_filter_data?.name, n.value = e.value, n.page = this.ds.dataLookup(this.isSidebar), n.url = this.url, this.ds.data_setter.emit(n)
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(f.D), t.Y36(D))
-                    }, n.\u0275cmp = t.Xpm({
-                        type: n,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.Y36(f.D), t.Y36(D))
+                    }, a.\u0275cmp = t.Xpm({
+                        type: a,
                         selectors: [
                             ["app-simple-server-filter"]
                         ],
                         inputs: {
                             url: "url",
                             isSidebar: "isSidebar"
                         },
@@ -2627,81 +2658,81 @@
                             ["appearance", "fill"],
                             [3, "formControl", "multiple", "selectionChange"],
                             ["dataSelect", ""],
                             [3, "formControl", "searching"],
                             [3, "value", 4, "ngFor", "ngForOf"],
                             [3, "value"]
                         ],
-                        template: function(e, a) {
+                        template: function(e, n) {
                             1 & e && (t.TgZ(0, "mat-form-field", 0)(1, "mat-select", 1, 2), t.NdJ("selectionChange", function(o) {
-                                return a.detectChange(o)
-                            }), t.TgZ(3, "mat-option"), t._UZ(4, "ngx-mat-select-search", 3), t.qZA(), t.YNc(5, Nn, 2, 2, "mat-option", 4), t.ALo(6, "async"), t.qZA()()), 2 & e && (t.xp6(1), t.Q6J("formControl", a.ServerSideCtrl)("multiple", a.isMulti()), t.xp6(3), t.Q6J("formControl", a.ServerSideFilteringCtrl)("searching", a.searching), t.xp6(1), t.Q6J("ngForOf", t.lcZ(6, 5, a.filteredServerSideBanks)))
+                                return n.detectChange(o)
+                            }), t.TgZ(3, "mat-option"), t._UZ(4, "ngx-mat-select-search", 3), t.qZA(), t.YNc(5, Nn, 2, 2, "mat-option", 4), t.ALo(6, "async"), t.qZA()()), 2 & e && (t.xp6(1), t.Q6J("formControl", n.ServerSideCtrl)("multiple", n.isMulti()), t.xp6(3), t.Q6J("formControl", n.ServerSideFilteringCtrl)("searching", n.searching), t.xp6(1), t.Q6J("ngForOf", t.lcZ(6, 5, n.filteredServerSideBanks)))
                         },
                         dependencies: [m.JJ, m.oH, S.ey, x.KE, st.gD, g.sg, lt.nu, g.Ov]
-                    }), n
+                    }), a
                 })(),
-                Ln = (() => {
-                    class n {
+                Rn = (() => {
+                    class a {
                         constructor(e) {
                             this.sanitizer = e
                         }
                         transform(e) {
                             return this.sanitizer.bypassSecurityTrustResourceUrl(e)
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(T.H7, 16))
-                    }, n.\u0275pipe = t.Yjl({
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.Y36(T.H7, 16))
+                    }, a.\u0275pipe = t.Yjl({
                         name: "safe",
-                        type: n,
+                        type: a,
                         pure: !0
-                    }), n
+                    }), a
                 })(),
-                Rn = (() => {
-                    class n {
-                        constructor(e, a) {
-                            this.sanitizer = e, this.ds = a
+                qn = (() => {
+                    class a {
+                        constructor(e, n) {
+                            this.sanitizer = e, this.ds = n
                         }
                         ngOnInit() {
                             this.data = this.ds.get_input_data(this.url)?.iframe_data
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(T.H7), t.Y36(f.D))
-                    }, n.\u0275cmp = t.Xpm({
-                        type: n,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.Y36(T.H7), t.Y36(f.D))
+                    }, a.\u0275cmp = t.Xpm({
+                        type: a,
                         selectors: [
                             ["app-app-iframe"]
                         ],
                         inputs: {
                             url: "url"
                         },
                         decls: 2,
                         vars: 5,
                         consts: [
                             [3, "src", "height", "width"]
                         ],
-                        template: function(e, a) {
-                            1 & e && (t._UZ(0, "iframe", 0), t.ALo(1, "safe")), 2 & e && t.Q6J("src", t.lcZ(1, 3, a.data.url), t.uOi)("height", a.data.height)("width", a.data.width)
+                        template: function(e, n) {
+                            1 & e && (t._UZ(0, "iframe", 0), t.ALo(1, "safe")), 2 & e && t.Q6J("src", t.lcZ(1, 3, n.data.url), t.uOi)("height", n.data.height)("width", n.data.width)
                         },
-                        dependencies: [Ln]
-                    }), n
+                        dependencies: [Rn]
+                    }), a
                 })(),
                 qt = (() => {
-                    class n {
-                        constructor(e, a, i, o, l) {
-                            this.ds = e, this.sanitizer = a, this.api = i, this.renderer = o, this.document = l, this.loading = !0
+                    class a {
+                        constructor(e, n, i, o, l) {
+                            this.ds = e, this.sanitizer = n, this.api = i, this.renderer = o, this.document = l, this.loading = !0
                         }
                         ngOnInit() {
-                            this.look_up = this.api.lookup(!1, this.url), this.page = this.ds.get_page(), this.ds.input_emitter.subscribe(a => {
-                                if (a.lookup === this.look_up)
-                                    if (void 0 !== a.message) this.loading = !0;
-                                    else if (a.calling) this.loading = !0;
+                            this.look_up = this.api.lookup(!1, this.url), this.page = this.ds.get_page(), this.ds.input_emitter.subscribe(n => {
+                                if (n.lookup === this.look_up)
+                                    if (void 0 !== n.message) this.loading = !0;
+                                    else if (n.calling) this.loading = !0;
                                 else {
-                                    let i = a.t;
+                                    let i = n.t;
                                     if (this.loading = !1, this.htmlStr = this.sanitizer.bypassSecurityTrustHtml(i.custom_html_data?.html), void 0 !== i?.custom_html_data?.script) {
                                         const o = this.renderer.createElement("script");
                                         this.renderer.setProperty(o, "text", i?.custom_html_data?.script), this.renderer.appendChild(this.document.body, o)
                                     }
                                 }
                             });
                             let e = this.api.needToPull(!1, this.url, this.page);
@@ -2713,58 +2744,58 @@
                                 isSidebar: !1
                             })
                         }
                         striptHide() {
                             return void 0 === this.scriptStr
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(f.D), t.Y36(T.H7), t.Y36(Et), t.Y36(t.Qsj), t.Y36(g.K0))
-                    }, n.\u0275cmp = t.Xpm({
-                        type: n,
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.Y36(f.D), t.Y36(T.H7), t.Y36(Nt), t.Y36(t.Qsj), t.Y36(g.K0))
+                    }, a.\u0275cmp = t.Xpm({
+                        type: a,
                         selectors: [
                             ["app-custom-html"]
                         ],
                         inputs: {
                             url: "url"
                         },
                         decls: 2,
                         vars: 1,
                         consts: [
                             [3, "innerHTML"],
                             ["css", ""]
                         ],
-                        template: function(e, a) {
-                            1 & e && t._UZ(0, "span", 0, 1), 2 & e && t.Q6J("innerHTML", a.htmlStr, t.oJD)
+                        template: function(e, n) {
+                            1 & e && t._UZ(0, "span", 0, 1), 2 & e && t.Q6J("innerHTML", n.htmlStr, t.oJD)
                         }
-                    }), n
+                    }), a
                 })();
 
-            function qn(n, s) {
-                1 & n && (t.TgZ(0, "span"), t._UZ(1, "br")(2, "br")(3, "br")(4, "mat-progress-bar", 2), t.qZA())
+            function Hn(a, s) {
+                1 & a && (t.TgZ(0, "span"), t._UZ(1, "br")(2, "br")(3, "br")(4, "mat-progress-bar", 2), t.qZA())
             }
-            let Hn = (() => {
-                class n {
-                    constructor(e, a, i) {
-                        this.ds = e, this.callService = a, this._snackBar = i, this.myFiles = [], this.show = !1
+            let Gn = (() => {
+                class a {
+                    constructor(e, n, i) {
+                        this.ds = e, this.callService = n, this._snackBar = i, this.myFiles = [], this.show = !1
                     }
-                    reactiveity(e, a = "") {
+                    reactiveity(e, n = "") {
                         let i = new b;
-                        i.page = this.ds.dataLookup(!1), i.key = this.ds.all_input.get(this.url)?.button_data?.name + "_" + e, i.value = "" === a ? this.ds.makeid(2) : a, i.url = this.url + "_" + e, this.ds.data_setter.emit(i)
+                        i.page = this.ds.dataLookup(!1), i.key = this.ds.all_input.get(this.url)?.button_data?.name + "_" + e, i.value = "" === n ? this.ds.makeid(2) : n, i.url = this.url + "_" + e, this.ds.data_setter.emit(i)
                     }
                     ngOnInit() {
                         this.data = this.ds.all_input.get(this.url)?.button_data
                     }
                     trigger() {
                         if (this.reactiveity("triggered"), this.data.redirect) return console.log(this.data.url), void window.open(this.data.url, "_black");
                         void 0 !== this.second_call && this.second_call.unsubscribe();
                         let e = this.callService.second_call_response(this.data.url, this.data.name, "");
-                        this.second_call = e.subscribe(a => {
+                        this.second_call = e.subscribe(n => {
                             try {
-                                var i = a;
+                                var i = n;
                                 this.reactiveity("result", i.button_result), this._snackBar.openFromComponent(F, {
                                     duration: 1e3 * i.display?.duration,
                                     data: {
                                         message: i.display?.message,
                                         status: i.display?.status
                                     }
                                 }), this.reactiveity("success"), this.show = !1
@@ -2773,88 +2804,88 @@
                                     duration: 5e3,
                                     data: {
                                         message: "backend failed",
                                         status: "error"
                                     }
                                 })
                             }
-                        }, a => {
+                        }, n => {
                             this.show = !1, this.reactiveity("failed"), this._snackBar.openFromComponent(F, {
                                 duration: 5e3,
                                 data: {
                                     message: "API called Failed",
                                     status: "error"
                                 }
                             })
                         })
                     }
                 }
-                return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(f.D), t.Y36(D), t.Y36(E.ux))
-                }, n.\u0275cmp = t.Xpm({
-                    type: n,
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.Y36(f.D), t.Y36(D), t.Y36(N.ux))
+                }, a.\u0275cmp = t.Xpm({
+                    type: a,
                     selectors: [
                         ["app-button"]
                     ],
                     inputs: {
                         url: "url"
                     },
                     decls: 3,
                     vars: 2,
                     consts: [
                         ["mat-raised-button", "", "color", "primary", 2, "display", "inline-block", "position", "relative", 3, "click"],
                         [4, "ngIf"],
                         ["mode", "indeterminate"]
                     ],
-                    template: function(e, a) {
+                    template: function(e, n) {
                         1 & e && (t.TgZ(0, "button", 0), t.NdJ("click", function() {
-                            return a.trigger()
-                        }), t._uU(1), t.qZA(), t.YNc(2, qn, 5, 0, "span", 1)), 2 & e && (t.xp6(1), t.Oqu(a.data.name), t.xp6(1), t.Q6J("ngIf", a.show))
+                            return n.trigger()
+                        }), t._uU(1), t.qZA(), t.YNc(2, Hn, 5, 0, "span", 1)), 2 & e && (t.xp6(1), t.Oqu(n.data.name), t.xp6(1), t.Q6J("ngIf", n.show))
                     },
                     dependencies: [L.lW, B.pW, g.O5]
-                }), n
+                }), a
             })();
             var Zt = p(31308),
                 rt = p(14984),
                 Ft = p(89181);
 
-            function Gn(n, s) {
-                1 & n && (t.TgZ(0, "mat-option", 6), t._UZ(1, "mat-spinner", 7), t.qZA())
+            function jn(a, s) {
+                1 & a && (t.TgZ(0, "mat-option", 6), t._UZ(1, "mat-spinner", 7), t.qZA())
             }
 
-            function jn(n, s) {
-                if (1 & n && (t.TgZ(0, "mat-option", 9), t._uU(1), t.qZA()), 2 & n) {
+            function Bn(a, s) {
+                if (1 & a && (t.TgZ(0, "mat-option", 9), t._uU(1), t.qZA()), 2 & a) {
                     const e = s.$implicit;
                     t.Q6J("value", e), t.xp6(1), t.hij(" ", e, " ")
                 }
             }
 
-            function Bn(n, s) {
-                if (1 & n && (t.ynx(0), t.YNc(1, jn, 2, 2, "mat-option", 8), t.BQk()), 2 & n) {
+            function zn(a, s) {
+                if (1 & a && (t.ynx(0), t.YNc(1, Bn, 2, 2, "mat-option", 8), t.BQk()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("ngForOf", e.options)
                 }
             }
-            let zn = (() => {
-                class n extends Zt.mL {
-                    constructor(e, a) {
-                        super(a), this.callService = e, this.url = "", this.name = "", this.current_value = "", this.fetchSuggestions = i => this.callService.second_call_response(this.url, this.name, i), this.isLoading = !1
+            let Kn = (() => {
+                class a extends Zt.mL {
+                    constructor(e, n) {
+                        super(n), this.callService = e, this.url = "", this.name = "", this.current_value = "", this.fetchSuggestions = i => this.callService.second_call_response(this.url, this.name, i), this.isLoading = !1
                     }
                     ngOnInit() {
                         super.ngOnInit(), this.url = this.scopedSchema.url, this.name = this.scopedSchema.search_name, this.form.valueChanges.subscribe(e => {
-                            e !== this.current_value && (this.current_value = e, this.fetchSuggestions(e).subscribe(a => {
-                                this.options = a.simple_fitler_data
+                            e !== this.current_value && (this.current_value = e, this.fetchSuggestions(e).subscribe(n => {
+                                this.options = n.simple_fitler_data
                             }))
                         })
                     }
                 }
-                return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(D), t.Y36(Ft.KT))
-                }, n.\u0275cmp = t.Xpm({
-                    type: n,
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.Y36(D), t.Y36(Ft.KT))
+                }, a.\u0275cmp = t.Xpm({
+                    type: a,
                     selectors: [
                         ["app-json-forms-server-side"]
                     ],
                     features: [t.qOj],
                     decls: 10,
                     vars: 8,
                     consts: [
@@ -2865,63 +2896,63 @@
                         ["class", "is-loading", 4, "ngIf"],
                         [4, "ngIf"],
                         [1, "is-loading"],
                         ["diameter", "30"],
                         [3, "value", 4, "ngFor", "ngForOf"],
                         [3, "value"]
                     ],
-                    template: function(e, a) {
+                    template: function(e, n) {
                         if (1 & e && (t.TgZ(0, "mat-form-field", 0)(1, "mat-label"), t._uU(2), t.qZA(), t.TgZ(3, "input", 1), t.NdJ("input", function(o) {
-                                return a.onChange(o)
+                                return n.onChange(o)
                             }), t.qZA(), t.TgZ(4, "mat-autocomplete", 2, 3), t.NdJ("optionSelected", function(o) {
-                                return a.onSelect(o)
-                            }), t.YNc(6, Gn, 2, 0, "mat-option", 4), t.YNc(7, Bn, 2, 1, "ng-container", 5), t.qZA(), t.TgZ(8, "mat-error"), t._uU(9), t.qZA()()), 2 & e) {
+                                return n.onSelect(o)
+                            }), t.YNc(6, jn, 2, 0, "mat-option", 4), t.YNc(7, zn, 2, 1, "ng-container", 5), t.qZA(), t.TgZ(8, "mat-error"), t._uU(9), t.qZA()()), 2 & e) {
                             const i = t.MAs(5);
-                            t.xp6(2), t.Oqu(a.label), t.xp6(1), t.s9C("placeholder", a.description), t.Q6J("id", a.id)("formControl", a.form)("matAutocomplete", i), t.xp6(3), t.Q6J("ngIf", a.isLoading), t.xp6(1), t.Q6J("ngIf", !a.isLoading), t.xp6(2), t.Oqu(a.error)
+                            t.xp6(2), t.Oqu(n.label), t.xp6(1), t.s9C("placeholder", n.description), t.Q6J("id", n.id)("formControl", n.form)("matAutocomplete", i), t.xp6(3), t.Q6J("ngIf", n.isLoading), t.xp6(1), t.Q6J("ngIf", !n.isLoading), t.xp6(2), t.Oqu(n.error)
                         }
                     },
-                    dependencies: [Z.yH, m.Fj, m.JJ, m.oH, bt.XC, bt.ZL, S.ey, x.TO, x.KE, x.hX, j.Nt, Yt.Ou, g.sg, g.O5]
-                }), n
+                    dependencies: [Z.yH, m.Fj, m.JJ, m.oH, bt.XC, bt.ZL, S.ey, x.TO, x.KE, x.hX, j.Nt, Qt.Ou, g.sg, g.O5]
+                }), a
             })();
 
-            function Kn(n, s) {
-                1 & n && (t.TgZ(0, "span"), t._UZ(1, "br")(2, "br")(3, "br")(4, "mat-progress-bar", 3), t.qZA())
+            function Xn(a, s) {
+                1 & a && (t.TgZ(0, "span"), t._UZ(1, "br")(2, "br")(3, "br")(4, "mat-progress-bar", 3), t.qZA())
             }
-            const Xn = (0, rt.xDy)((0, rt.TDq)("string"), (0, rt.wcO)(n => n.hasOwnProperty("url")));
-            let Wn = (() => {
-                class n {
-                    constructor(e, a, i) {
-                        this.ds = e, this.callService = a, this._snackBar = i, this.show = !1, this.renderers = [...Zt.x, {
-                            tester: (0, rt.yMz)(5, Xn),
-                            renderer: zn
+            const Wn = (0, rt.xDy)((0, rt.TDq)("string"), (0, rt.wcO)(a => a.hasOwnProperty("url")));
+            let $n = (() => {
+                class a {
+                    constructor(e, n, i) {
+                        this.ds = e, this.callService = n, this._snackBar = i, this.show = !1, this.renderers = [...Zt.x, {
+                            tester: (0, rt.yMz)(5, Wn),
+                            renderer: Kn
                         }]
                     }
                     ngOnInit() {
                         this.data = this.ds.all_input.get(this.url)?.form_data, this.formData = this.data.data
                     }
                     reactiveity(e) {
-                        let a = new b;
-                        a.page = this.ds.dataLookup(!1), a.key = this.ds.all_input.get(this.url)?.form_data?.name + "_" + e, a.value = this.ds.makeid(2), a.url = this.url + "_" + e, this.ds.data_setter.emit(a)
+                        let n = new b;
+                        n.page = this.ds.dataLookup(!1), n.key = this.ds.all_input.get(this.url)?.form_data?.name + "_" + e, n.value = this.ds.makeid(2), n.url = this.url + "_" + e, this.ds.data_setter.emit(n)
                     }
                     trigger() {
                         let e = new b;
                         e.page = this.ds.dataLookup(!1), e.url = this.url, e.key = this.data.name, e.value = this.formData, this.show = !0, this.ds.data_setter.emit(e), this.reactiveity("triggered");
-                        let a = this.callService.second_call_response(this.data.submit_info.url, void 0, void 0);
-                        this.call = a.subscribe(i => {
+                        let n = this.callService.second_call_response(this.data.submit_info.url, void 0, void 0);
+                        this.call = n.subscribe(i => {
                             console.log(i);
                             let o = i;
                             this.reactiveity("success");
                             let l = o.display?.duration,
-                                d = "API called Sucessfully ";
-                            null != o.display?.message && (d = o.display?.message);
+                                c = "API called Sucessfully ";
+                            null != o.display?.message && (c = o.display?.message);
                             let _ = o.display?.status;
                             this._snackBar.openFromComponent(F, {
                                 duration: 1e3 * l,
                                 data: {
-                                    message: d,
+                                    message: c,
                                     status: _
                                 }
                             }), this.show = !1
                         }, i => {
                             this.reactiveity("failed");
                             let o = i.error.display?.duration;
                             void 0 === o && (o = 5);
@@ -2931,136 +2962,136 @@
                                     message: "API called Failed",
                                     status: "error"
                                 }
                             })
                         })
                     }
                 }
-                return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(f.D), t.Y36(D), t.Y36(E.ux))
-                }, n.\u0275cmp = t.Xpm({
-                    type: n,
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.Y36(f.D), t.Y36(D), t.Y36(N.ux))
+                }, a.\u0275cmp = t.Xpm({
+                    type: a,
                     selectors: [
                         ["app-form"]
                     ],
                     inputs: {
                         url: "url"
                     },
                     decls: 7,
                     vars: 6,
                     consts: [
                         [3, "data", "schema", "uischema", "renderers", "dataChange"],
                         ["mat-raised-button", "", "color", "primary", 2, "position", "absolute", "left", "50%", 3, "click"],
                         [4, "ngIf"],
                         ["mode", "indeterminate"]
                     ],
-                    template: function(e, a) {
+                    template: function(e, n) {
                         1 & e && (t.TgZ(0, "jsonforms", 0), t.NdJ("dataChange", function(o) {
-                            return a.formData = o
+                            return n.formData = o
                         }), t.qZA(), t.TgZ(1, "button", 1), t.NdJ("click", function() {
-                            return a.trigger()
-                        }), t._uU(2), t.qZA(), t._UZ(3, "br")(4, "br")(5, "br"), t.YNc(6, Kn, 5, 0, "span", 2)), 2 & e && (t.Q6J("data", a.formData)("schema", a.data.form_schema)("uischema", a.data.ui_schema)("renderers", a.renderers), t.xp6(2), t.Oqu(a.data.submit_info.name), t.xp6(4), t.Q6J("ngIf", a.show))
+                            return n.trigger()
+                        }), t._uU(2), t.qZA(), t._UZ(3, "br")(4, "br")(5, "br"), t.YNc(6, Xn, 5, 0, "span", 2)), 2 & e && (t.Q6J("data", n.formData)("schema", n.data.form_schema)("uischema", n.data.ui_schema)("renderers", n.renderers), t.xp6(2), t.Oqu(n.data.submit_info.name), t.xp6(4), t.Q6J("ngIf", n.show))
                     },
                     dependencies: [L.lW, B.pW, g.O5, Ft.C]
-                }), n
+                }), a
             })();
 
-            function $n(n, s) {
-                if (1 & n && (t.TgZ(0, "span"), t._UZ(1, "app-box", 3), t.qZA()), 2 & n) {
+            function Vn(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-box", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function Vn(n, s) {
-                if (1 & n && (t.TgZ(0, "span"), t._UZ(1, "app-datetime", 4), t.qZA()), 2 & n) {
+            function ta(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-datetime", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function ta(n, s) {
-                if (1 & n && (t.TgZ(0, "span"), t._UZ(1, "app-table", 3), t.qZA()), 2 & n) {
+            function ea(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-table", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function ea(n, s) {
-                if (1 & n && (t.TgZ(0, "span"), t._UZ(1, "app-plot", 3), t.qZA()), 2 & n) {
+            function na(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-plot", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function na(n, s) {
-                if (1 & n && (t.TgZ(0, "span", 5), t._UZ(1, "app-checkbox", 3), t.qZA()), 2 & n) {
+            function aa(a, s) {
+                if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-checkbox", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function aa(n, s) {
-                if (1 & n && (t.TgZ(0, "span", 5), t._UZ(1, "app-radio", 4), t.qZA()), 2 & n) {
+            function ia(a, s) {
+                if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-radio", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function ia(n, s) {
-                if (1 & n && (t.TgZ(0, "span", 5), t._UZ(1, "app-slider", 4), t.qZA()), 2 & n) {
+            function sa(a, s) {
+                if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-slider", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function sa(n, s) {
-                if (1 & n && (t.TgZ(0, "span", 5), t._UZ(1, "app-button-toggle", 4), t.qZA()), 2 & n) {
+            function oa(a, s) {
+                if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-button-toggle", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function oa(n, s) {
-                if (1 & n && (t.TgZ(0, "span", 5), t._UZ(1, "app-toggle", 4), t.qZA()), 2 & n) {
+            function la(a, s) {
+                if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-toggle", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function la(n, s) {
-                if (1 & n) {
+            function ra(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "span")(1, "app-entry-point", 7), t.NdJ("fx", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(2);
                         return t.KtG(r.setFlex(l.url, i))
                     })("rd", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(2);
                         return t.KtG(r.setReactivity(l.url, i))
                     }), t.qZA(), t._UZ(2, "br"), t.qZA()
                 }
-                if (2 & n) {
+                if (2 & a) {
                     const e = s.$implicit,
-                        a = t.oxw(2);
-                    let i, o, l, r, d;
-                    t.xp6(1), t.Q6J("hidden", null == (i = a.reactivityData.get(e.url)) ? null : i.hidden)("url", e.url)("isSidebar", a.isSidebar)("fxFlex", (null == (o = a.flexData.get(e.url)) ? null : o.fxFlex) || "100%%")("fxFlex.md", (null == (l = a.flexData.get(e.url)) ? null : l.fxFlex_md) || "100%")("fxFlex.sm", (null == (r = a.flexData.get(e.url)) ? null : r.fxFlex_sm) || "100%")("fxFlex.xs", (null == (d = a.flexData.get(e.url)) ? null : d.fxFlex_sm) || "100%")
+                        n = t.oxw(2);
+                    let i, o, l, r, c;
+                    t.xp6(1), t.Q6J("hidden", null == (i = n.reactivityData.get(e.url)) ? null : i.hidden)("url", e.url)("isSidebar", n.isSidebar)("fxFlex", (null == (o = n.flexData.get(e.url)) ? null : o.fxFlex) || "100%%")("fxFlex.md", (null == (l = n.flexData.get(e.url)) ? null : l.fxFlex_md) || "100%")("fxFlex.sm", (null == (r = n.flexData.get(e.url)) ? null : r.fxFlex_sm) || "100%")("fxFlex.xs", (null == (c = n.flexData.get(e.url)) ? null : c.fxFlex_sm) || "100%")
                 }
             }
 
-            function ra(n, s) {
-                if (1 & n && (t.TgZ(0, "span"), t.YNc(1, la, 3, 7, "span", 6), t.qZA()), 2 & n) {
+            function pa(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t.YNc(1, ra, 3, 7, "span", 6), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("ngForOf", e.getURLs())
                 }
             }
 
-            function pa(n, s) {
-                if (1 & n) {
+            function ca(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "mat-tab", 9), t._UZ(1, "br"), t.TgZ(2, "app-sub-entry-point", 10), t.NdJ("rd", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(2);
                         return t.KtG(r.setReactivity(l.url, i))
                     })("rd", function(i) {
                         const l = t.CHM(e).$implicit,
@@ -3068,171 +3099,171 @@
                         return t.KtG(r.setReactivity(l.url, i))
                     })("fd", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(2);
                         return t.KtG(r.setFlex(l.url, i))
                     }), t.qZA()()
                 }
-                if (2 & n) {
+                if (2 & a) {
                     const e = s.$implicit,
-                        a = t.oxw(2);
-                    let i, o, l, r, d;
-                    t.Q6J("label", e.name || ""), t.xp6(2), t.Q6J("hidden", null == (i = a.reactivityData.get(e.url)) ? null : i.hidden)("url", e.url)("isSidebar", a.isSidebar)("fxFlex", (null == (o = a.flexData.get(e.url)) ? null : o.fxFlex) || "100%")("fxFlex.md", (null == (l = a.flexData.get(e.url)) ? null : l.fxFlex_md) || "100%")("fxFlex.sm", (null == (r = a.flexData.get(e.url)) ? null : r.fxFlex_sm) || "100%")("fxFlex.xs", (null == (d = a.flexData.get(e.url)) ? null : d.fxFlex_sm) || "100%")
+                        n = t.oxw(2);
+                    let i, o, l, r, c;
+                    t.Q6J("label", e.name || ""), t.xp6(2), t.Q6J("hidden", null == (i = n.reactivityData.get(e.url)) ? null : i.hidden)("url", e.url)("isSidebar", n.isSidebar)("fxFlex", (null == (o = n.flexData.get(e.url)) ? null : o.fxFlex) || "100%")("fxFlex.md", (null == (l = n.flexData.get(e.url)) ? null : l.fxFlex_md) || "100%")("fxFlex.sm", (null == (r = n.flexData.get(e.url)) ? null : r.fxFlex_sm) || "100%")("fxFlex.xs", (null == (c = n.flexData.get(e.url)) ? null : c.fxFlex_sm) || "100%")
                 }
             }
 
-            function ca(n, s) {
-                if (1 & n && (t.TgZ(0, "span")(1, "mat-tab-group"), t.YNc(2, pa, 3, 8, "mat-tab", 8), t.qZA()()), 2 & n) {
+            function da(a, s) {
+                if (1 & a && (t.TgZ(0, "span")(1, "mat-tab-group"), t.YNc(2, ca, 3, 8, "mat-tab", 8), t.qZA()()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(2), t.Q6J("ngForOf", e.getURLs())
                 }
             }
 
-            function da(n, s) {
-                if (1 & n) {
+            function ua(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "span")(1, "mat-expansion-panel")(2, "mat-expansion-panel-header")(3, "mat-panel-title"), t._uU(4), t.qZA()(), t._UZ(5, "br"), t.TgZ(6, "mat-panel-description", 5)(7, "app-sub-entry-point", 11), t.NdJ("rd", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(2);
                         return t.KtG(r.setReactivity(l.url, i))
                     })("fd", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(2);
                         return t.KtG(r.setFlex(l.url, i))
                     }), t.qZA()()()()
                 }
-                if (2 & n) {
+                if (2 & a) {
                     const e = s.$implicit,
-                        a = t.oxw(2);
-                    let i, o, l, r, d;
-                    t.xp6(4), t.hij(" ", e.name, " "), t.xp6(3), t.Q6J("url", e.url)("isSidebar", a.isSidebar)("hidden", null == (i = a.reactivityData.get(e.url)) ? null : i.hidden)("fxFlex", (null == (o = a.flexData.get(e.url)) ? null : o.fxFlex) || "100%")("fxFlex.md", (null == (l = a.flexData.get(e.url)) ? null : l.fxFlex_md) || "100%")("fxFlex.sm", (null == (r = a.flexData.get(e.url)) ? null : r.fxFlex_sm) || "50%")("fxFlex.xs", (null == (d = a.flexData.get(e.url)) ? null : d.fxFlex_sm) || "100%")
+                        n = t.oxw(2);
+                    let i, o, l, r, c;
+                    t.xp6(4), t.hij(" ", e.name, " "), t.xp6(3), t.Q6J("url", e.url)("isSidebar", n.isSidebar)("hidden", null == (i = n.reactivityData.get(e.url)) ? null : i.hidden)("fxFlex", (null == (o = n.flexData.get(e.url)) ? null : o.fxFlex) || "100%")("fxFlex.md", (null == (l = n.flexData.get(e.url)) ? null : l.fxFlex_md) || "100%")("fxFlex.sm", (null == (r = n.flexData.get(e.url)) ? null : r.fxFlex_sm) || "50%")("fxFlex.xs", (null == (c = n.flexData.get(e.url)) ? null : c.fxFlex_sm) || "100%")
                 }
             }
 
-            function ua(n, s) {
-                if (1 & n && (t.TgZ(0, "span")(1, "mat-accordion"), t._UZ(2, "br")(3, "br"), t.YNc(4, da, 8, 8, "span", 6), t.qZA()()), 2 & n) {
+            function _a(a, s) {
+                if (1 & a && (t.TgZ(0, "span")(1, "mat-accordion"), t._UZ(2, "br")(3, "br"), t.YNc(4, ua, 8, 8, "span", 6), t.qZA()()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(4), t.Q6J("ngForOf", e.getURLs())
                 }
             }
 
-            function _a(n, s) {
-                if (1 & n && (t.TgZ(0, "span", 5), t._UZ(1, "app-simple-filter", 4), t.qZA()), 2 & n) {
+            function ma(a, s) {
+                if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-simple-filter", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function ma(n, s) {
-                if (1 & n && (t.TgZ(0, "span", 5), t._UZ(1, "app-simple-server-filter", 4), t.qZA()), 2 & n) {
+            function ha(a, s) {
+                if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-simple-server-filter", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function ha(n, s) {
-                if (1 & n && (t.TgZ(0, "span", 5), t._UZ(1, "app-group-filter", 4), t.qZA()), 2 & n) {
+            function ga(a, s) {
+                if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-group-filter", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function ga(n, s) {
-                if (1 & n && (t.TgZ(0, "span", 5), t._UZ(1, "app-input", 4), t.qZA()), 2 & n) {
+            function fa(a, s) {
+                if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-input", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function fa(n, s) {
-                if (1 & n && (t.TgZ(0, "span", 5), t._UZ(1, "app-app-download", 3), t.qZA()), 2 & n) {
+            function xa(a, s) {
+                if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-app-download", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function xa(n, s) {
-                if (1 & n && (t.TgZ(0, "span", 5), t._UZ(1, "app-app-upload", 3), t.qZA()), 2 & n) {
+            function ba(a, s) {
+                if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-app-upload", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function ba(n, s) {
-                if (1 & n && (t.TgZ(0, "span"), t._UZ(1, "app-app-image", 3), t.qZA()), 2 & n) {
+            function Ca(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-app-image", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function Ca(n, s) {
-                if (1 & n && (t.TgZ(0, "span"), t._UZ(1, "app-highchart", 3), t.qZA()), 2 & n) {
+            function va(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-highchart", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function va(n, s) {
-                if (1 & n && (t.TgZ(0, "span"), t._UZ(1, "app-app-iframe", 3), t.qZA()), 2 & n) {
+            function ya(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-app-iframe", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function ya(n, s) {
-                if (1 & n && (t.TgZ(0, "span"), t._UZ(1, "app-custom-html", 3), t.qZA()), 2 & n) {
+            function Ta(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-custom-html", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.url)
                 }
             }
 
-            function Ta(n, s) {
-                if (1 & n && (t.TgZ(0, "span", 5), t._UZ(1, "app-button", 3), t.qZA()), 2 & n) {
+            function Sa(a, s) {
+                if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-button", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function Sa(n, s) {
-                if (1 & n && (t.TgZ(0, "span"), t._UZ(1, "app-form", 3), t.qZA()), 2 & n) {
+            function wa(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-form", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function wa(n, s) {
-                1 & n && (t.TgZ(0, "span"), t._UZ(1, "mat-progress-bar", 12), t.qZA())
+            function Za(a, s) {
+                1 & a && (t.TgZ(0, "span"), t._UZ(1, "mat-progress-bar", 12), t.qZA())
             }
 
-            function Za(n, s) {
-                if (1 & n) {
+            function Fa(a, s) {
+                if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "span")(1, "button", 13), t.NdJ("click", function() {
                         t.CHM(e);
                         const i = t.oxw();
                         return t.KtG(i.copy_error())
                     }), t.TgZ(2, "mat-icon"), t._uU(3, "content_copy"), t.qZA(), t.TgZ(4, "span"), t._uU(5, "Copy Error"), t.qZA()(), t.TgZ(6, "button", 13), t.NdJ("click", function() {
                         t.CHM(e);
                         const i = t.oxw();
                         return t.KtG(i.force_refresh())
                     }), t.TgZ(7, "mat-icon"), t._uU(8, "refresh"), t.qZA(), t.TgZ(9, "span"), t._uU(10, "Refresh Data"), t.qZA()()()
                 }
             }
-            let Fa = (() => {
-                class n {
-                    constructor(e, a, i, o) {
-                        this.ds = e, this.clipboard = a, this.dialog = i, this.api = o, this.rd = new t.vpe, this.fd = new t.vpe, this.reactivityData = new Map, this.flexData = new Map, this.reactive = new Gt, this.d = new Map, this.loading = !0, this.failed = !1
+            let Da = (() => {
+                class a {
+                    constructor(e, n, i, o) {
+                        this.ds = e, this.clipboard = n, this.dialog = i, this.api = o, this.rd = new t.vpe, this.fd = new t.vpe, this.reactivityData = new Map, this.flexData = new Map, this.reactive = new Gt, this.d = new Map, this.loading = !0, this.failed = !1
                     }
                     ngOnInit() {
-                        this.look_up = this.api.lookup(this.isSidebar, this.url), this.page = this.ds.get_page(), this.ds.input_emitter.subscribe(a => {
-                            if (a.lookup === this.look_up)
-                                if (void 0 !== a.message) this.loading = !0, this.failed = !0, this.error = a.message, this.tooltip_data = void 0, this.dialog_data = void 0, this.name = void 0, this.type = void 0;
-                                else if (a.calling) this.loading = !0, this.failed = !1, this.tooltip_data = void 0, this.dialog_data = void 0, this.name = void 0, this.type = void 0;
+                        this.look_up = this.api.lookup(this.isSidebar, this.url), this.page = this.ds.get_page(), this.ds.input_emitter.subscribe(n => {
+                            if (n.lookup === this.look_up)
+                                if (void 0 !== n.message) this.loading = !0, this.failed = !0, this.error = n.message, this.tooltip_data = void 0, this.dialog_data = void 0, this.name = void 0, this.type = void 0;
+                                else if (n.calling) this.loading = !0, this.failed = !1, this.tooltip_data = void 0, this.dialog_data = void 0, this.name = void 0, this.type = void 0;
                             else {
-                                let i = a.t;
+                                let i = n.t;
                                 this.loading = !1, this.failed = !1, this.tooltip_data = i?.tooltip_data, this.dialog_data = i?.dialog_data, this.reactive = i?.reactive, this.fd.emit(i.flex), this.rd.emit(this.reactive), this.name = this.api.set_name(i), this.type = i?.type, this.multi_url = this.api.get_multi_url(i)
                             }
                         });
                         let e = this.api.needToPull(this.isSidebar, this.url, this.page);
                         this.api.call_this.emit({
                             forced: e,
                             url: this.url,
@@ -3240,19 +3271,19 @@
                             page: this.page,
                             isSidebar: this.isSidebar
                         })
                     }
                     getURLs() {
                         return this.multi_url
                     }
-                    setFlex(e, a) {
-                        this.flexData.set(e, a)
+                    setFlex(e, n) {
+                        this.flexData.set(e, n)
                     }
-                    setReactivity(e, a) {
-                        this.reactivityData.set(e, a)
+                    setReactivity(e, n) {
+                        this.reactivityData.set(e, n)
                     }
                     copy_error() {
                         this.clipboard.copy(this.error)
                     }
                     force_refresh() {
                         this.api.getData(!0, this.url, this.look_up, this.page, this.isSidebar, "")
                     }
@@ -3260,18 +3291,18 @@
                         this.dialog_data && this.dialog.open(Re, {
                             height: this.dialog_data.height,
                             width: this.dialog_data.width,
                             data: this.dialog_data.url
                         })
                     }
                 }
-                return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(f.D), t.Y36(gt.TU), t.Y36(et.uw), t.Y36(Et))
-                }, n.\u0275cmp = t.Xpm({
-                    type: n,
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.Y36(f.D), t.Y36(gt.TU), t.Y36(et.uw), t.Y36(Nt))
+                }, a.\u0275cmp = t.Xpm({
+                    type: a,
                     selectors: [
                         ["app-sub-entry-point"]
                     ],
                     inputs: {
                         url: "url",
                         isSidebar: "isSidebar"
                     },
@@ -3293,80 +3324,80 @@
                         [3, "label", 4, "ngFor", "ngForOf"],
                         [3, "label"],
                         [3, "hidden", "url", "isSidebar", "fxFlex", "fxFlex.md", "fxFlex.sm", "fxFlex.xs", "rd", "fd"],
                         [3, "url", "isSidebar", "hidden", "fxFlex", "fxFlex.md", "fxFlex.sm", "fxFlex.xs", "rd", "fd"],
                         ["mode", "query"],
                         ["mat-menu-item", "", 3, "click"]
                     ],
-                    template: function(e, a) {
+                    template: function(e, n) {
                         if (1 & e && (t.TgZ(0, "span", 0), t.NdJ("click", function() {
-                                return a.openDialog()
-                            }), t.YNc(1, $n, 2, 1, "span", 1), t.YNc(2, Vn, 2, 2, "span", 1), t.YNc(3, ta, 2, 1, "span", 1), t.YNc(4, ea, 2, 1, "span", 1), t.YNc(5, na, 2, 1, "span", 2), t.YNc(6, aa, 2, 2, "span", 2), t.YNc(7, ia, 2, 2, "span", 2), t.YNc(8, sa, 2, 2, "span", 2), t.YNc(9, oa, 2, 2, "span", 2), t.YNc(10, ra, 2, 1, "span", 1), t.YNc(11, ca, 3, 1, "span", 1), t.YNc(12, ua, 5, 1, "span", 1), t.YNc(13, _a, 2, 2, "span", 2), t.YNc(14, ma, 2, 2, "span", 2), t.YNc(15, ha, 2, 2, "span", 2), t.YNc(16, ga, 2, 2, "span", 2), t.YNc(17, fa, 2, 1, "span", 2), t.YNc(18, xa, 2, 1, "span", 2), t.YNc(19, ba, 2, 1, "span", 1), t.YNc(20, Ca, 2, 1, "span", 1), t.YNc(21, va, 2, 1, "span", 1), t.YNc(22, ya, 2, 1, "span", 1), t.YNc(23, Ta, 2, 1, "span", 2), t.YNc(24, Sa, 2, 1, "span", 1), t.YNc(25, wa, 2, 0, "span", 1), t._UZ(26, "br"), t.YNc(27, Za, 11, 0, "span", 1), t.qZA()), 2 & e) {
+                                return n.openDialog()
+                            }), t.YNc(1, Vn, 2, 1, "span", 1), t.YNc(2, ta, 2, 2, "span", 1), t.YNc(3, ea, 2, 1, "span", 1), t.YNc(4, na, 2, 1, "span", 1), t.YNc(5, aa, 2, 1, "span", 2), t.YNc(6, ia, 2, 2, "span", 2), t.YNc(7, sa, 2, 2, "span", 2), t.YNc(8, oa, 2, 2, "span", 2), t.YNc(9, la, 2, 2, "span", 2), t.YNc(10, pa, 2, 1, "span", 1), t.YNc(11, da, 3, 1, "span", 1), t.YNc(12, _a, 5, 1, "span", 1), t.YNc(13, ma, 2, 2, "span", 2), t.YNc(14, ha, 2, 2, "span", 2), t.YNc(15, ga, 2, 2, "span", 2), t.YNc(16, fa, 2, 2, "span", 2), t.YNc(17, xa, 2, 1, "span", 2), t.YNc(18, ba, 2, 1, "span", 2), t.YNc(19, Ca, 2, 1, "span", 1), t.YNc(20, va, 2, 1, "span", 1), t.YNc(21, ya, 2, 1, "span", 1), t.YNc(22, Ta, 2, 1, "span", 1), t.YNc(23, Sa, 2, 1, "span", 2), t.YNc(24, wa, 2, 1, "span", 1), t.YNc(25, Za, 2, 0, "span", 1), t._UZ(26, "br"), t.YNc(27, Fa, 11, 0, "span", 1), t.qZA()), 2 & e) {
                             let i;
-                            t.Q6J("matTooltip", null !== (i = null == a.tooltip_data ? null : a.tooltip_data.label) && void 0 !== i ? i : "")("matTooltipDisabled", void 0 === a.tooltip_data), t.xp6(1), t.Q6J("ngIf", "box" === a.type), t.xp6(1), t.Q6J("ngIf", "date" === a.type), t.xp6(1), t.Q6J("ngIf", "table" === a.type), t.xp6(1), t.Q6J("ngIf", "chart" === a.type), t.xp6(1), t.Q6J("ngIf", "checkbox" === a.type), t.xp6(1), t.Q6J("ngIf", "radio" === a.type), t.xp6(1), t.Q6J("ngIf", "slider" === a.type), t.xp6(1), t.Q6J("ngIf", "button_toggle" === a.type), t.xp6(1), t.Q6J("ngIf", "toggle" === a.type), t.xp6(1), t.Q6J("ngIf", "multi_list" === a.type), t.xp6(1), t.Q6J("ngIf", "multi_tabs" === a.type), t.xp6(1), t.Q6J("ngIf", "multi_expand" === a.type), t.xp6(1), t.Q6J("ngIf", "simple_filter" == a.type), t.xp6(1), t.Q6J("ngIf", "simple_server_filter" == a.type), t.xp6(1), t.Q6J("ngIf", "group_filter" == a.type), t.xp6(1), t.Q6J("ngIf", "input" == a.type), t.xp6(1), t.Q6J("ngIf", "download" == a.type), t.xp6(1), t.Q6J("ngIf", "upload" == a.type), t.xp6(1), t.Q6J("ngIf", "image" == a.type), t.xp6(1), t.Q6J("ngIf", "highchart" == a.type), t.xp6(1), t.Q6J("ngIf", "iframe" == a.type), t.xp6(1), t.Q6J("ngIf", "custom_html" == a.type), t.xp6(1), t.Q6J("ngIf", "button" == a.type), t.xp6(1), t.Q6J("ngIf", "form" == a.type), t.xp6(1), t.Q6J("ngIf", a.loading), t.xp6(2), t.Q6J("ngIf", a.failed)
+                            t.Q6J("matTooltip", null !== (i = null == n.tooltip_data ? null : n.tooltip_data.label) && void 0 !== i ? i : "")("matTooltipDisabled", void 0 === n.tooltip_data), t.xp6(1), t.Q6J("ngIf", "box" === n.type), t.xp6(1), t.Q6J("ngIf", "date" === n.type), t.xp6(1), t.Q6J("ngIf", "table" === n.type), t.xp6(1), t.Q6J("ngIf", "chart" === n.type), t.xp6(1), t.Q6J("ngIf", "checkbox" === n.type), t.xp6(1), t.Q6J("ngIf", "radio" === n.type), t.xp6(1), t.Q6J("ngIf", "slider" === n.type), t.xp6(1), t.Q6J("ngIf", "button_toggle" === n.type), t.xp6(1), t.Q6J("ngIf", "toggle" === n.type), t.xp6(1), t.Q6J("ngIf", "multi_list" === n.type), t.xp6(1), t.Q6J("ngIf", "multi_tabs" === n.type), t.xp6(1), t.Q6J("ngIf", "multi_expand" === n.type), t.xp6(1), t.Q6J("ngIf", "simple_filter" == n.type), t.xp6(1), t.Q6J("ngIf", "simple_server_filter" == n.type), t.xp6(1), t.Q6J("ngIf", "group_filter" == n.type), t.xp6(1), t.Q6J("ngIf", "input" == n.type), t.xp6(1), t.Q6J("ngIf", "download" == n.type), t.xp6(1), t.Q6J("ngIf", "upload" == n.type), t.xp6(1), t.Q6J("ngIf", "image" == n.type), t.xp6(1), t.Q6J("ngIf", "highchart" == n.type), t.xp6(1), t.Q6J("ngIf", "iframe" == n.type), t.xp6(1), t.Q6J("ngIf", "custom_html" == n.type), t.xp6(1), t.Q6J("ngIf", "button" == n.type), t.xp6(1), t.Q6J("ngIf", "form" == n.type), t.xp6(1), t.Q6J("ngIf", n.loading), t.xp6(2), t.Q6J("ngIf", n.failed)
                         }
                     },
-                    dependencies: [Z.yH, R.pp, R.ib, R.yz, R.yK, R.u4, H.Hw, V.OP, B.pW, Tt.SP, Tt.uX, Ut.gM, g.sg, g.O5, He, Be, an, sn, cn, hn, tt, gn, xn, bn, yn, Zn, n, Dn, An, On, Mn, In.q, En, Rn, qt, Hn, Wn],
+                    dependencies: [Z.yH, R.pp, R.ib, R.yz, R.yK, R.u4, H.Hw, V.OP, B.pW, Tt.SP, Tt.uX, Ut.gM, g.sg, g.O5, He, Be, an, sn, cn, hn, tt, gn, xn, bn, yn, Zn, a, kn, Jn, Mn, In, Pn.q, Ln, qn, qt, Gn, $n],
                     styles: [".center[_ngcontent-%COMP%]{display:flex;justify-content:center;align-items:center}.full[_ngcontent-%COMP%]{width:100%;display:flex;justify-content:center;align-items:center}"]
-                }), n
+                }), a
             })();
-            var Da = p(44740),
-                ka = p(83787);
-            let Aa = (() => {
-                    class n {
-                        constructor(e, a) {
-                            this.cookie = e, this.data = a
-                        }
-                        intercept(e, a) {
-                            return "POST" === e.method ? a.handle(e).pipe((0, at.K)(i => (401 === i.status && (this.cookie.deleteCookie("auth_token"), this.data.reset_data()), (0, ka._)(i)))) : a.handle(e)
-                        }
-                    }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.LFG(Ht), t.LFG(f.D))
-                    }, n.\u0275prov = t.Yz7({
-                        token: n,
-                        factory: n.\u0275fac
-                    }), n
+            var ka = p(44740),
+                Aa = p(83787);
+            let Ja = (() => {
+                    class a {
+                        constructor(e, n) {
+                            this.cookie = e, this.data = n
+                        }
+                        intercept(e, n) {
+                            return "POST" === e.method ? n.handle(e).pipe((0, at.K)(i => (401 === i.status && (this.cookie.deleteCookie("auth_token"), this.data.reset_data()), (0, Aa._)(i)))) : n.handle(e)
+                        }
+                    }
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.LFG(Ht), t.LFG(f.D))
+                    }, a.\u0275prov = t.Yz7({
+                        token: a,
+                        factory: a.\u0275fac
+                    }), a
                 })(),
                 Ht = (() => {
-                    class n {
+                    class a {
                         constructor(e) {
                             this.document = e
                         }
                         deleteCookie(e) {
                             this.document.cookie = `${e}=; expires=Thu, 01 Jan 1970 00:00:00 UTC; path=/;`
                         }
                     }
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)(t.LFG(g.K0))
-                    }, n.\u0275prov = t.Yz7({
-                        token: n,
-                        factory: n.\u0275fac
-                    }), n
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)(t.LFG(g.K0))
+                    }, a.\u0275prov = t.Yz7({
+                        token: a,
+                        factory: a.\u0275fac
+                    }), a
                 })(),
-                Ja = (() => {
-                    class n {}
-                    return n.\u0275fac = function(e) {
-                        return new(e || n)
-                    }, n.\u0275mod = t.oAB({
-                        type: n,
+                Oa = (() => {
+                    class a {}
+                    return a.\u0275fac = function(e) {
+                        return new(e || a)
+                    }, a.\u0275mod = t.oAB({
+                        type: a,
                         bootstrap: [fe]
-                    }), n.\u0275inj = t.cJS({
+                    }), a.\u0275inj = t.cJS({
                         providers: [At.N, {
-                            provide: Y.TP,
-                            useClass: Aa,
+                            provide: Q.TP,
+                            useClass: Ja,
                             multi: !0
                         }, Ht],
-                        imports: [Ue.o9, m.u5, m.UX, we.rt, Ze.XD, gt.Iq, Ae.U5, xt.HT, Je.nZ, Fe._t, bt.Bb, Oe.g, Me._r, L.ot, Ct.vV, A.QW, Pt.p9, Ie.Hi, Pe.T5, q.FA, et.Is, Mt.t, R.To, nt.N6, H.Ps, j.c, G.ie, V.Tx, S.XK, vt.TU, B.Cv, Yt.Cq, yt.Fk, S.si, st.LD, it.SJ, Qt.KP, ft.rP, E.ZX, ot.JX, M.p0, Tt.Nh, Ot.g0, Ut.AV, Ye.dp, Qe.U8, De.eL, ke.Cl, T.b2, Y.JF, Te, J.Bz, Se.PW, Dt.xu, Nt.Ns.forRoot({
+                        imports: [Ue.o9, m.u5, m.UX, we.rt, Ze.XD, gt.Iq, Ae.U5, xt.HT, Je.nZ, Fe._t, bt.Bb, Oe.g, Me._r, L.ot, Ct.vV, A.QW, Pt.p9, Ie.Hi, Pe.T5, q.FA, et.Is, Mt.t, R.To, nt.N6, H.Ps, j.c, G.ie, V.Tx, S.XK, vt.TU, B.Cv, Qt.Cq, yt.Fk, S.si, st.LD, it.SJ, Yt.KP, ft.rP, N.ZX, ot.JX, M.p0, Tt.Nh, Ot.g0, Ut.AV, Qe.dp, Ye.U8, De.eL, ke.Cl, T.b2, Q.JF, Te, J.Bz, Se.PW, Dt.xu, Et.Ns.forRoot({
                             echarts: () => p.e(275).then(p.bind(p, 36275))
-                        }), lt.Co, Rt.pL, Da.SD, Ft.R2, Zt.D]
-                    }), n
+                        }), lt.Co, Rt.pL, ka.SD, Ft.R2, Zt.D]
+                    }), a
                 })();
             t.B6R(tt, function() {
-                return [A.a8, A.dk, A.dn, A.rt, g.O5, Fa, qt]
-            }, []), (0, t.G48)(), T.q6().bootstrapModule(Ja).catch(n => console.error(n)), console.info("Angular CDK version", pt.q.full), console.info("Angular Material version", S.q4.full)
+                return [A.a8, A.dk, A.dn, A.rt, g.O5, Da, qt]
+            }, []), (0, t.G48)(), T.q6().bootstrapModule(Oa).catch(a => console.error(a)), console.info("Angular CDK version", pt.q.full), console.info("Angular Material version", S.q4.full)
         }
     },
     O => {
         O.O(0, [736], () => O(O.s = 24269)), O.O()
     }
 ]);
```

### Comparing `zen_dash-0.6.1/zen_dash/static/polyfills.0a8881ff36766b1e.js` & `zen_dash-0.6.2/zen_dash/static/polyfills.0a8881ff36766b1e.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/static/runtime.6a9b461ae5a72237.js` & `zen_dash-0.6.2/zen_dash/static/runtime.6a9b461ae5a72237.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/static/styles.362a8260c32d36d9.css` & `zen_dash-0.6.2/zen_dash/static/styles.362a8260c32d36d9.css`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/static/vendor.3c67e76b6e4a9ca3.js` & `zen_dash-0.6.2/zen_dash/static/vendor.3c67e76b6e4a9ca3.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/support/__init__.py` & `zen_dash-0.6.2/zen_dash/support/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/tag/__init__.py` & `zen_dash-0.6.2/zen_dash/tag/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/zen_dash/websocket/__init__.py` & `zen_dash-0.6.2/zen_dash/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.1/PKG-INFO` & `zen_dash-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zen-dash
-Version: 0.6.1
+Version: 0.6.2
 Summary: Simple yet scable and production ready python dashboard that is better than shiny application for business.
 Home-page: https://zen-reportz.github.io/zen_dash/index.html
 License: MIT
 Author: Zen
 Author-email: zenreportz@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

