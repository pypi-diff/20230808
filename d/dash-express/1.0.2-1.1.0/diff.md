# Comparing `tmp/dash_express-1.0.2.tar.gz` & `tmp/dash_express-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_express-1.0.2.tar", last modified: Mon Jul 31 13:36:37 2023, max compression
+gzip compressed data, was "dash_express-1.1.0.tar", last modified: Tue Aug  8 06:19:35 2023, max compression
```

## Comparing `dash_express-1.0.2.tar` & `dash_express-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-31 13:36:37.484001 dash_express-1.0.2/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1071 2023-07-26 08:37:30.000000 dash_express-1.0.2/LICENSE
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     6089 2023-07-31 13:36:37.484001 dash_express-1.0.2/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     5606 2023-07-28 14:45:31.000000 dash_express-1.0.2/README.md
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-31 13:36:37.480001 dash_express-1.0.2/dash_express/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)    38275 2023-07-31 13:35:07.000000 dash_express-1.0.2/dash_express/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)    16540 2023-07-29 14:46:24.000000 dash_express-1.0.2/dash_express/_app_shell.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-31 13:36:37.484001 dash_express-1.0.2/dash_express/filters/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       88 2023-07-26 08:21:26.000000 dash_express-1.0.2/dash_express/filters/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     3374 2023-07-26 08:21:26.000000 dash_express-1.0.2/dash_express/filters/autofilter.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      482 2023-07-31 13:29:47.000000 dash_express-1.0.2/dash_express/filters/filterfunc.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-31 13:36:37.484001 dash_express-1.0.2/dash_express/kpi/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     2086 2023-07-31 13:17:41.000000 dash_express-1.0.2/dash_express/kpi/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     2360 2023-07-26 08:27:32.000000 dash_express-1.0.2/dash_express/preview_chart.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       11 2023-07-31 13:34:49.000000 dash_express-1.0.2/dash_express/version.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-31 13:36:37.480001 dash_express-1.0.2/dash_express.egg-info/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     6089 2023-07-31 13:36:37.000000 dash_express-1.0.2/dash_express.egg-info/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      443 2023-07-31 13:36:37.000000 dash_express-1.0.2/dash_express.egg-info/SOURCES.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-07-31 13:36:37.000000 dash_express-1.0.2/dash_express.egg-info/dependency_links.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      135 2023-07-31 13:36:37.000000 dash_express-1.0.2/dash_express.egg-info/requires.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       13 2023-07-31 13:36:37.000000 dash_express-1.0.2/dash_express.egg-info/top_level.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-07-31 13:36:37.484001 dash_express-1.0.2/setup.cfg
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1090 2023-07-31 13:35:26.000000 dash_express-1.0.2/setup.py
+drwxr-xr-x   0 kirill    (1000) kirill    (1000)        0 2023-08-08 06:19:35.835596 dash_express-1.1.0/
+-rw-r--r--   0 kirill    (1000) kirill    (1000)     1071 2023-08-02 02:51:58.000000 dash_express-1.1.0/LICENSE
+-rw-r--r--   0 kirill    (1000) kirill    (1000)     6053 2023-08-08 06:19:35.835596 dash_express-1.1.0/PKG-INFO
+-rw-r--r--   0 kirill    (1000) kirill    (1000)     5606 2023-08-02 02:51:58.000000 dash_express-1.1.0/README.md
+drwxr-xr-x   0 kirill    (1000) kirill    (1000)        0 2023-08-08 06:19:35.831596 dash_express-1.1.0/dash_express/
+-rw-r--r--   0 kirill    (1000) kirill    (1000)    38277 2023-08-08 06:06:10.000000 dash_express-1.1.0/dash_express/__init__.py
+-rw-r--r--   0 kirill    (1000) kirill    (1000)    19459 2023-08-08 06:03:22.000000 dash_express-1.1.0/dash_express/_app_shell.py
+drwxr-xr-x   0 kirill    (1000) kirill    (1000)        0 2023-08-08 06:19:35.834596 dash_express-1.1.0/dash_express/filters/
+-rw-r--r--   0 kirill    (1000) kirill    (1000)       88 2023-08-02 02:51:58.000000 dash_express-1.1.0/dash_express/filters/__init__.py
+-rw-r--r--   0 kirill    (1000) kirill    (1000)     3374 2023-08-02 02:51:58.000000 dash_express-1.1.0/dash_express/filters/autofilter.py
+-rw-r--r--   0 kirill    (1000) kirill    (1000)      482 2023-08-02 02:51:58.000000 dash_express-1.1.0/dash_express/filters/filterfunc.py
+drwxr-xr-x   0 kirill    (1000) kirill    (1000)        0 2023-08-08 06:19:35.834596 dash_express-1.1.0/dash_express/kpi/
+-rw-r--r--   0 kirill    (1000) kirill    (1000)     2086 2023-08-02 02:51:58.000000 dash_express-1.1.0/dash_express/kpi/__init__.py
+-rw-r--r--   0 kirill    (1000) kirill    (1000)     2360 2023-08-02 02:51:58.000000 dash_express-1.1.0/dash_express/preview_chart.py
+-rw-r--r--   0 kirill    (1000) kirill    (1000)       11 2023-08-02 02:51:58.000000 dash_express-1.1.0/dash_express/version.py
+drwxr-xr-x   0 kirill    (1000) kirill    (1000)        0 2023-08-08 06:19:35.833596 dash_express-1.1.0/dash_express.egg-info/
+-rw-r--r--   0 kirill    (1000) kirill    (1000)     6053 2023-08-08 06:19:35.000000 dash_express-1.1.0/dash_express.egg-info/PKG-INFO
+-rw-r--r--   0 kirill    (1000) kirill    (1000)      443 2023-08-08 06:19:35.000000 dash_express-1.1.0/dash_express.egg-info/SOURCES.txt
+-rw-r--r--   0 kirill    (1000) kirill    (1000)        1 2023-08-08 06:19:35.000000 dash_express-1.1.0/dash_express.egg-info/dependency_links.txt
+-rw-r--r--   0 kirill    (1000) kirill    (1000)      135 2023-08-08 06:19:35.000000 dash_express-1.1.0/dash_express.egg-info/requires.txt
+-rw-r--r--   0 kirill    (1000) kirill    (1000)       13 2023-08-08 06:19:35.000000 dash_express-1.1.0/dash_express.egg-info/top_level.txt
+-rw-r--r--   0 kirill    (1000) kirill    (1000)       38 2023-08-08 06:19:35.835596 dash_express-1.1.0/setup.cfg
+-rw-r--r--   0 kirill    (1000) kirill    (1000)     1090 2023-08-08 06:17:55.000000 dash_express-1.1.0/setup.py
```

### Comparing `dash_express-1.0.2/LICENSE` & `dash_express-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dash_express-1.0.2/PKG-INFO` & `dash_express-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: dash_express
-Version: 1.0.2
+Version: 1.1.0
 Summary: A tool for faster application development Plotly Dash
 Home-page: https://github.com/stpnvkirill/dash-express
 Author: Kirill Stepanov
 Author-email: stpnv.kirill.o@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Fast analytical web application with DashExpress
@@ -176,8 +174,7 @@
 * <a href="https://pandas.pydata.org/" class="external-link" target="_blank">Pandas DataFrame</a> for the data store & compute measure.
 * <a href="https://www.dash-mantine-components.com/" class="external-link" target="_blank">Dash Mantine Components</a> for the create pretty UI
 * <a href="https://dash-leaflet.herokuapp.com/" class="external-link" target="_blank">Dash Leaflet</a> for the create maps
 
 ## License
 
 This project is licensed under the terms of the MIT license.
-
```

### Comparing `dash_express-1.0.2/README.md` & `dash_express-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dash_express-1.0.2/dash_express/__init__.py` & `dash_express-1.1.0/dash_express/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     :param cache: flask_caching.Cache instance, dict or True (default: True)
     :type cache: flask_caching.Cache instance, dict or True
 
     :param default_cache_timeout: flask_caching.Cache timeout in seconds (default: 3600)
     :type default_cache_timeout: int
 
     :param app_shell: Appshell class for customization UI your app
-    :type app_shell: BaseAppShell instance
+    :type app_shell: AppShell instance
     
     -------------------------------
 
     :param name: The name Flask should use for your app. Even if you provide
         your own ``server``, ``name`` will be used to help find assets.
         Typically ``__name__`` (the magic global var, not a string) is the
         best value to use. Default ``'__main__'``, env: ``DASH_APP_NAME``
@@ -265,15 +265,15 @@
         @self.callback(Output("layout-store", 'data'),
                     Input("layout-store", 'data'))
         def send_layout(d):
             dict1 = {k: v.render()
                     for k, v in self.PAGES.items() if v.is_accessible()}
             dict2 = {k: v.preview()for k, v in self.PAGES.items()
                     if not v.is_accessible() and v.access_mode == 'view'}
-            dict3 = {'#error': [None, self.app_shell.ERROR_PAGE]}
+            dict3 = {'#error': [None, self.app_shell.error_page(self)]}
 
             meta = {k:v.metatags() for k, v in self.PAGES.items()}
 
             return {'content':{**dict1, **dict2, **dict3}, 'navs': self.app_shell._build_navs(self), 'meta':meta}
 
         # Render Chart
         @self.callback([Output({'type': 'graph', 'id': ALL}, 'figure'),
@@ -439,14 +439,15 @@
         self.clientside_callback(
             """ function(layout) {                        
                 return [layout['navs']] } """,
             [Output("nav-content", 'children')],
             Input("layout-store", 'data'))
         
         self.app_shell.app_shell_clientside(self)
+        self.app_shell.base_clientside(self)
 
     def compile_layout(self):
         """Compile layout and callback functions"""
         self._app_shell()
         self.DOWNLOAD_OPPORTUNITY = np.any([page.download_opportunity for page in self.PAGES.values()])
         self.register_clientside_callback()
         self.register_server_callback()
@@ -533,23 +534,23 @@
         return True
 
     def render(self):
         filters = [
             dmc.CardSection(
                 dmc.Group(
                     children=[
-                        dmc.Title('Фильтры', order=3),
+                        dmc.Title('Filters', order=3),
                         dmc.LoadingOverlay(
                             dmc.Tooltip(
                                 multiline=True,
                                 width=220,
                                 withArrow=True,
                                 transition="fade",
                                 transitionDuration=200,
-                                label="Скачать данные в виде таблицы",
+                                label="Download data",
                                 children=[dmc.ActionIcon(
                                     DashIconify(
                                         icon="line-md:download-loop", height=25),
                                     color="gray",
                                     id={'type': 'download-frame-action',
                                         'page': self.URL},
                                     variant="transparent",
@@ -590,15 +591,15 @@
                 mt=15),
         ]
         page_content = self.get_prewiew_layout()
         return [filters, page_content]
     
     def metatags(self):
         return {'title':self.title, 'description':self.description}
-
+   
     def register_frame(self, get_df):
         @self.app.cache.cached(timeout = self.app.default_cache_timeout, key_prefix=str(self) + '/')
         def get_df_func():
             df = get_df()
             return df  
                 
         self.get_df_func = get_df_func
```

### Comparing `dash_express-1.0.2/dash_express/_app_shell.py` & `dash_express-1.1.0/dash_express/_app_shell.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,28 +13,26 @@
 DARK_PLOTLY_TEMPLATES['layout']['margin'] = margin
 
 LIGHT_PLOTLY_TEMPLATES = pio.templates["plotly_white"]
 LIGHT_PLOTLY_TEMPLATES['layout']['paper_bgcolor'] = 'rgba(0,0,0,0)'
 LIGHT_PLOTLY_TEMPLATES['layout']['plot_bgcolor'] = 'rgba(0,0,0,0)'
 LIGHT_PLOTLY_TEMPLATES['layout']['margin'] = margin
 
-
-class BaseAppShell(object):
+class AppShell(object):
     def __init__(self, 
                 primary_colors='indigo',
                 theme=None,
                 default_colorscheme='light',
                 light_plotly_templates=None,
                 dark_plotly_templates=None,
                 dark_leaflet_tile=None,
                 light_leaflet_tile=None,
                 autocolorway=True,
                 theme_icon_dark="line-md:moon-filled-alt-to-sunny-filled-loop-transition", 
-                theme_icon_light="line-md:sunny-filled-loop-to-moon-filled-loop-transition",
-                error_page = None):
+                theme_icon_light="line-md:sunny-filled-loop-to-moon-filled-loop-transition"):
         self.PRIMARY_COLORS = primary_colors
         self.THEME = theme or {}
         self.THEME["primaryColor"] = self.PRIMARY_COLORS
         self.DEFAULT_THEME = default_colorscheme
         self.NAV_BUTTON_KWARGS = dict(color='primary',
                                 p=3, miw=50, variant='subtle')
         self.THEME_ICON = {'dark': theme_icon_dark,"light": theme_icon_light}
@@ -42,97 +40,151 @@
                             "light": "yellow"}
         
         self.LIGHT_PLOTLY_TEMPLATES = light_plotly_templates or LIGHT_PLOTLY_TEMPLATES
         self.DARK_PLOTLY_TEMPLATES = dark_plotly_templates or DARK_PLOTLY_TEMPLATES
         self.DARK_LEAFLET_TILE = dark_leaflet_tile or 'https://tiles.stadiamaps.com/tiles/alidade_smooth_dark/{z}/{x}/{y}{r}.png'
         self.LIGHT_LEAFLET_TILE = light_leaflet_tile or 'https://{s}.basemaps.cartocdn.com/light_all/{z}/{x}/{y}{r}.png'
 
-        self.ERROR_PAGE = error_page or dmc.Stack(
-                    align="center",
-                    children=[
-                        dmc.Text(
-                            [
-                                "If you think this page should exist, create an issue ",
-                                dmc.Anchor(
-                                    "here",
-                                    underline=False,
-                                    href="https://github.com/thedirtyfew/dash-extensions/issues/new",
-                                ),
-                                ".",
-                            ]
-                        ),
-                        dmc.Anchor("Go back to home ->",
-                                href="/", underline=False),
-                    ],
-                )
                 
         if autocolorway:
             self.autocolorway()
 
+    def autocolorway(self):
+        """Create a color path based on the primary color"""
+        primarycolors = self.PRIMARY_COLORS
+        lst = [[k, v[-1]] for k, v in dmc.theme.DEFAULT_COLORS.items()]
+        colorway = list(sorted(lst, key = lambda x: '#zzzz' if (x[0] == primarycolors) else x[1], reverse=True))
+        colorway = [i[1].upper() for i in colorway][:10]
+        self.LIGHT_PLOTLY_TEMPLATES['layout']['colorway'] = colorway
+        self.DARK_PLOTLY_TEMPLATES['layout']['colorway']  = colorway
+
     def build_nav_name(self, name, access):
+        """Get the name of the navigation button"""
         name = [name, dmc.Group(DashIconify(icon="majesticons:lock"), ml=3)
                 ] if not access else name
-
         return name
 
     def _build_nav(self, page):
+        """Get the navigation button"""
         nav_name = self.build_nav_name(page.name, page.is_accessible())
         nav = dmc.Button(nav_name, **self.NAV_BUTTON_KWARGS)
         nav.id = dict(type='nav-link', href=str(page.URL))
         return dmc.Anchor(nav, href=page.URL, pt=4)
 
     def _build_navs(self, app):
-
+        """Get a list of all available navigation buttons"""
         navs = [self._build_nav(page) for page in app.PAGES.values() if page.is_accessible(
         ) or page.access_mode == 'view']
 
         def filters(e):
             if e != None:
                 return True
             else:
                 return False
 
         out_filter = list(filter(filters, navs))
         return out_filter
-
+    
     def logo_container(self, app):
+        """Get a logo for the navigation bar
+        
+        :param app: DashExpress app
+
+        Example:
+        ```python
+        dmc.Header(
+            height=60, children=[self.logo_container(app),]
+        )
+        ```
+        """
         return dmc.Anchor(
             dmc.Image(height=45, id='logo-img') if isinstance(self.LOGO, dict) else self.LOGO,
             weight=550,
             size=30,
-            href=app.config.get('url_base_pathname') or '/',
+            href=self.url_base(app),
             underline=False,
             pr='xl',
         ) if self.LOGO else html.Div()
-
+    
     def color_scheme_toggle(self, icon, **kwargs):
+        """Get a color scheme switch
+        
+        :param icon: icon for dmc.ActionIcon
+        :type icon: DashIconify
+
+        Example:
+        ```python
+        dmc.MediaQuery(
+            self.color_scheme_toggle(
+                icon=DashIconify(
+                    icon="", width=22                                        
+                ),
+                variant="outline",
+                radius='sm',
+                size='lg',
+            ),
+            smallerThan="lg",
+            styles={"display": "none"},
+
+        )
+        ```
+        """
+        icon.id = 'color-scheme-icon'
         action_icon = dmc.ActionIcon(icon, **kwargs)
         action_icon.id = "color-scheme-toggle"
         return action_icon
 
     def filter_wrapper_toggle(self, icon, **kwargs):
+        """Get a filter wrapper switch
+        
+        :param icon: icon for dmc.ActionIcon
+        :type icon: DashIconify
+
+        Example:
+        ```python
+       dmc.MediaQuery(
+            self.filter_wrapper_toggle(
+                DashIconify(
+                    icon="", width=22,
+                    id='filter-wrapper-icon'
+                ),
+                variant="outline",
+                radius='sm',
+                size='lg',
+                color='indigo',
+            ),
+            smallerThan="lg",
+            styles={"display": "none"},
+        )
+        ```
+        """
         action_icon = dmc.ActionIcon(icon, **kwargs)
         action_icon.id = "filter-wrapper-toggle"
         return action_icon
-
+ 
     def filter_wrapper(self):
-        return html.Div(id="sidebar-filter")
-
+        """Get a container with filters"""
+        return html.Div([html.Div(id="sidebar-filter"), 
+                dcc.Store(id='filter-wrapper-store')])
+ 
     def dashboard_wrapper(self):
+        """Get a container with dashboard"""
         return html.Div(id='page_layout')
 
     def _build_menulink(self, page):
+        """Get a button for the mobile menu"""
         icon = 'tabler:shield-lock' if not page.is_accessible() else 'tabler:arrow-big-right-lines'
         return dmc.MenuItem(
             page.name,
             id=dict(type='nav-link-menu', href=page.URL),
             icon=DashIconify(icon=icon), href=page.URL, py=5
         )
 
     def _build_menulinks(self, app):
+        """Get a drop-down list for the mobile menu"""
         navs = [self._build_menulink(page) for page in app.PAGES.values() if page.is_accessible(
         ) or page.access_mode == 'view']
 
         def filters(e):
             if e != None:
                 return True
             else:
@@ -142,24 +194,115 @@
         return dmc.MenuDropdown(
             [
                 dmc.MenuLabel("Application", miw=200, py=5),
                 dmc.MenuItem("Filters", icon=DashIconify(icon="tabler:filter"),
                              id="filter-wrapper-dropdown", py=5,),
                 dmc.MenuItem("Color", icon=DashIconify(
                     icon="tabler:sun"), id="color-scheme-toggle-dropdown", py=5),
-                dmc.MenuItem("Account", icon=DashIconify(
-                    icon="tabler:user"), href='/profile', py=5),
                 dmc.MenuDivider(),
                 dmc.MenuLabel("Pages", miw=200, py=5),
             ] + out_filter,
             miw=200,
             style={'z-index': '30000'}
         )
 
+    def _app_provider(self, app):
+        """get the primary downloadable component
+
+        !Do not change"""
+        return dmc.MantineProvider(
+            dmc.MantineProvider(
+                theme=self.THEME,
+                inherit=True,
+                children=[
+                    dcc.Store(id="theme-store", storage_type="local"),
+                    dcc.Store(id="layout-store", storage_type="local"),
+                    dcc.Store(id="filter-store", storage_type="local"),
+                    dcc.Store(id="page-store"),
+                    dcc.Store(id='contentfilter-store'),
+                    dcc.Location(id='url-store'),
+                    self.render(app)
+                ]
+            ),
+            theme={"colorScheme": self.DEFAULT_THEME},
+            id="mantine-docs-theme-provider",
+            withGlobalStyles=True,
+            withNormalizeCSS=True,
+        )
+    
+    def base_clientside(self, app):
+        """Basic callback functions on the client side"""
+        # Theme addition
+        app.clientside_callback(
+            """ function(data) {  
+                const icon = data["colorScheme"] == "dark" ? "%(dark_icon)s" : "%(light_icon)s";
+                const color = data["colorScheme"] != "dark" ? "%(dark_color)s" : "%(light_color)s";
+                return [icon, color]                
+              } """ % dict(
+                dark_icon=self.THEME_ICON.get('dark'),
+                light_icon=self.THEME_ICON.get('light'),
+                dark_color=self.THEME_ICON_COLOR.get('dark'),
+                light_color=self.THEME_ICON_COLOR.get('light')
+
+            ),
+            Output("color-scheme-icon", "icon"),
+            Output("color-scheme-toggle", "color"),
+            Input("theme-store", "data"),
+        )
+        # Nav-link variant
+        app.clientside_callback(
+            """ function(url, href) { 
+                const res = [];  
+                const res2 = []        
+                for (var i = 0; i < href.length; i++) {
+                    res[i] = href[i]["href"] == url ? 'light':'subtle'
+                };
+                for (var i = 0; i < href.length; i++) {
+                    res2[i] = href[i]["href"] == url ? 'indigo':undefined
+                };            
+                return [res, res2] } """,
+            [Output({'type': 'nav-link', 'href': ALL}, 'variant'),
+             Output({'type': 'nav-link-menu', 'href': ALL}, 'color')],
+            Input("url-store", 'pathname'),
+            State({'type': 'nav-link', 'href': ALL}, 'id'))
+
+    def nav_items_container(self, orientation='h'):
+        """Get navigation buttons"""
+        if orientation=='h':
+            return dmc.Group(
+                            id='nav-content',
+                            spacing=3,
+                        )
+        else:
+             return dmc.Stack(
+                            id='nav-content',
+                            spacing=3,
+                        )
+
+    def url_base(self, app):
+        """Get a link to the home page"""
+        return app.config.get('_pathname') or '/'
+
+    def error_page(self, app):
+        """Get the error page"""
+        return dmc.Stack(
+                    align="center",
+                    children=[
+                        dmc.Text(
+                            [
+                                "404 Not Found",
+                            ]
+                        ),
+                        dmc.Anchor("Go back to home ->",
+                                href=self.url_base(app), underline=False),
+                    ],
+                )
+
     def mobile_menu(self, app):
+        """Get a menu for mobile devices"""
         return dmc.Menu(
             [
                 dmc.MenuTarget(
                     dmc.ActionIcon(
                         DashIconify(
                             icon="line-md:close-to-menu-alt-transition",
                             width=18,
@@ -169,27 +312,28 @@
                         size='lg',
                     )),
                 self._build_menulinks(app),
             ],
             position="bottom-end",
             offset=5
         )
-
+    
+class BaseAppShell(AppShell):
     def nav_content(self, app):
         nav_cont = dmc.Grid(
             justify="center",
             style={"height": 60},
             children=[
                 dmc.Col(
                     dmc.Group([
                         self.logo_container(app),
-                        dmc.MediaQuery(dmc.Group(
-                            id='nav-content',
-                            spacing=3,
-                        ), smallerThan="lg", styles={"display": "none"}, ),
+                        dmc.MediaQuery(
+                            self.nav_items_container(orientation='h'), 
+                            smallerThan="lg", 
+                            styles={"display": "none"}, ),
                     ]),
                     pt=7,
                     span="content",
                 ),
                 dmc.Col(
                     span="auto",
                     children=dmc.Group(
@@ -210,16 +354,15 @@
                                 ),
                                 smallerThan="lg",
                                 styles={"display": "none"},
                             ),
                             dmc.MediaQuery(
                                 self.color_scheme_toggle(
                                     icon=DashIconify(
-                                        icon="", width=22,
-                                        id='color-scheme-icon'
+                                        icon="", width=22                                        
                                     ),
                                     variant="outline",
                                     radius='sm',
                                     size='lg',
                                 ),
                                 smallerThan="lg",
                                 styles={"display": "none"},
@@ -234,24 +377,22 @@
                     ),
                 ),
             ],
         )
         return nav_cont
 
     def navbar(self, app):
+        """Create a navigation panel layout"""
         navbar = dmc.Card(self.nav_content(app), radius='md',
-                          withBorder=True, mt=15, m=0, p=8, style={'position': 'block', 'overflow': 'inherit'})
+                          withBorder=True, mt=15, m=0, style={'position': 'block', 'overflow': 'inherit'})
         return navbar
 
-    def render(self, app):
-        container = dmc.Container(
-            [
-                self.navbar(app),
-                dcc.Store(id='filter-wrapper-store'),
-                dmc.Grid([
+    def content_wrapper(self):
+        """Create a layout of the main content"""
+        return dmc.Grid([
                     dmc.Col(
                         dmc.MediaQuery(
                             dmc.Card(
                                 self.filter_wrapper(),
                                 mt=15,
                                 mb=0,
                                 withBorder=True,
@@ -279,35 +420,25 @@
                                 w='100%'
                             ),
                             innerBoxStyle={'width': '100%'},
                             largerThan='md',
                             styles={'height': 'calc(100vh - 135px)'}),
                         span='auto')
                 ])
+
+    def render(self, app):
+        container = dmc.Container(
+            [
+                self.navbar(app),
+                self.content_wrapper()
             ], size='xxl')
         return container
 
     def app_shell_clientside(self, app):
-        # Theme addition
-        app.clientside_callback(
-            """ function(data) {  
-                const icon = data["colorScheme"] == "dark" ? "%(dark_icon)s" : "%(light_icon)s";
-                const color = data["colorScheme"] != "dark" ? "%(dark_color)s" : "%(light_color)s";
-                return [icon, color]                
-              } """ % dict(
-                dark_icon=self.THEME_ICON.get('dark'),
-                light_icon=self.THEME_ICON.get('light'),
-                dark_color=self.THEME_ICON_COLOR.get('dark'),
-                light_color=self.THEME_ICON_COLOR.get('light')
-
-            ),
-            Output("color-scheme-icon", "icon"),
-            Output("color-scheme-toggle", "color"),
-            Input("theme-store", "data"),
-        )
+        """Add additional callbacks on the client side"""
         # Hide filters
         app.clientside_callback(
             """ function(data) {  return data["display"]  } """,
             Output("grid-provider", "display"),
             Input("filter-wrapper-store", "data"),
         )
         app.clientside_callback(
@@ -323,107 +454,66 @@
                 }
             }""",
             Output("filter-wrapper-store", "data"),
             Input("filter-wrapper-toggle", "n_clicks"),
             Input("filter-wrapper-dropdown", "n_clicks"),
             State("filter-wrapper-store", "data"),
         )
-        # Nav-link variant
-        app.clientside_callback(
-            """ function(url, href) { 
-                const res = [];  
-                const res2 = []        
-                for (var i = 0; i < href.length; i++) {
-                    res[i] = href[i]["href"] == url ? 'light':'subtle'
-                };
-                for (var i = 0; i < href.length; i++) {
-                    res2[i] = href[i]["href"] == url ? 'indigo':undefined
-                };            
-                return [res, res2] } """,
-            [Output({'type': 'nav-link', 'href': ALL}, 'variant'),
-             Output({'type': 'nav-link-menu', 'href': ALL}, 'color')],
-            Input("url-store", 'pathname'),
-            State({'type': 'nav-link', 'href': ALL}, 'id'))
-
+        
     def app_shell_serverside(self, app):
+        """Add additional server-side callbacks"""
         ...
 
-    def _app_provider(self, app):
-        return dmc.MantineProvider(
-            dmc.MantineProvider(
-                theme=self.THEME,
-                inherit=True,
-                children=[
-                    dcc.Store(id="theme-store", storage_type="local"),
-                    dcc.Store(id="layout-store", storage_type="local"),
-                    dcc.Store(id="filter-store", storage_type="local"),
-                    dcc.Store(id="page-store"),
-                    dcc.Store(id='contentfilter-store'),
-                    dcc.Location(id='url-store'),
-                    self.render(app)
-                ]
-            ),
-            theme={"colorScheme": self.DEFAULT_THEME},
-            id="mantine-docs-theme-provider",
-            withGlobalStyles=True,
-            withNormalizeCSS=True,
-        )
-
-    def autocolorway(self):
-        primarycolors = self.PRIMARY_COLORS
-        lst = [[k, v[-1]] for k, v in dmc.theme.DEFAULT_COLORS.items()]
-        colorway = list(sorted(lst, key = lambda x: '#zzzz' if (x[0] == primarycolors) else x[1], reverse=True))
-        colorway = [i[1].upper() for i in colorway][:10]
-        self.LIGHT_PLOTLY_TEMPLATES['layout']['colorway'] = colorway
-        self.DARK_PLOTLY_TEMPLATES['layout']['colorway']  = colorway
-
-
 class AsideAppShell(BaseAppShell):
     def navbar(self, app):
-        navbar = dmc.Header(
-            self.nav_content(app),
-            mt=5, m=0, p=8,
-            height=60,
-            fixed=True,
-            px=25)
+        """Create a navigation panel layout"""
+        navbar = dmc.Header(self.nav_content(app), height=60, m=0, p=10, style={'position': 'block', 'overflow': 'inherit'})
         return navbar
     
-    def filter_wrapper(self):
-        return dmc.Navbar(
-        fixed=True,
-        id="components-navbar",
-        position={"top": 60},
-        width={"base": 240},
-        children=[
-            dmc.ScrollArea(
-                html.Div(id="sidebar-filter"),
-                offsetScrollbars=True,
-                type="scroll",
-                mt=20
-            )
-        ],
-    )
-
-    
-    def render(self, app):
-        container = dmc.Container(
-            [
-                self.navbar(app),
-                dcc.Store(id='filter-wrapper-store'),
-                self.filter_wrapper(),
-                dmc.Grid([
+    def content_wrapper(self):
+        """Create a layout of the main content"""
+        return dmc.Grid([
                     dmc.Col(
                         dmc.MediaQuery(
                             dmc.ScrollArea(
                                 self.dashboard_wrapper(),
                                 mt=15,
                                 h='100%',
                                 w='100%'
                             ),
                             innerBoxStyle={'width': '100%'},
                             largerThan='md',
-                            styles={'height': 'calc(100vh - 100px)'}),
+                            styles={'height': 'calc(100vh - 135px)'}),
                         span='auto')
-                ], ml=250)
-            ], size='xxl', mt=60)
-        return container
-
+                ])
+    
+    def render(self, app):
+        container = dmc.Container(
+            [
+                self.navbar(app),
+                self.content_wrapper()
+            ], size=1500)
+        navbar = dmc.Drawer(
+                padding="md",
+                # fixed=True,
+                size=250,
+                # opened=True,
+                overlayOpacity=0.55,
+                overlayBlur=3,
+                zIndex=9,
+                id='drawer',
+                # height='calc(100vh-60px)',
+                children=self.filter_wrapper(),
+            )
+        return html.Div([navbar, container])
+    
+    def app_shell_clientside(self, app):
+       # Hide filters
+        app.clientside_callback(
+            """ function(n,n2, opened) {  
+                if (n || n2) {return opened != true } 
+                return dash_clientside.no_update} """,
+            Output("drawer", "opened"),
+            Input("filter-wrapper-toggle", "n_clicks"),
+            Input("filter-wrapper-dropdown", "n_clicks"),
+            State("drawer", "opened"),
+        )
```

### Comparing `dash_express-1.0.2/dash_express/filters/autofilter.py` & `dash_express-1.1.0/dash_express/filters/autofilter.py`

 * *Files identical despite different names*

### Comparing `dash_express-1.0.2/dash_express/kpi/__init__.py` & `dash_express-1.1.0/dash_express/kpi/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_express-1.0.2/dash_express/preview_chart.py` & `dash_express-1.1.0/dash_express/preview_chart.py`

 * *Files identical despite different names*

### Comparing `dash_express-1.0.2/dash_express.egg-info/PKG-INFO` & `dash_express-1.1.0/dash_express.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: dash-express
-Version: 1.0.2
+Version: 1.1.0
 Summary: A tool for faster application development Plotly Dash
 Home-page: https://github.com/stpnvkirill/dash-express
 Author: Kirill Stepanov
 Author-email: stpnv.kirill.o@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Fast analytical web application with DashExpress
@@ -176,8 +174,7 @@
 * <a href="https://pandas.pydata.org/" class="external-link" target="_blank">Pandas DataFrame</a> for the data store & compute measure.
 * <a href="https://www.dash-mantine-components.com/" class="external-link" target="_blank">Dash Mantine Components</a> for the create pretty UI
 * <a href="https://dash-leaflet.herokuapp.com/" class="external-link" target="_blank">Dash Leaflet</a> for the create maps
 
 ## License
 
 This project is licensed under the terms of the MIT license.
-
```

### Comparing `dash_express-1.0.2/setup.py` & `dash_express-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dash_express",
-    version="1.0.2",                     
+    version="1.1.0",                     
     author="Kirill Stepanov",
     author_email="stpnv.kirill.o@gmail.com",
     description="A tool for faster application development Plotly Dash",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[                      
         "dash>=2.11.1",
```

