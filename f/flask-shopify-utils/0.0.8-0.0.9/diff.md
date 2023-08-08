# Comparing `tmp/flask_shopify_utils-0.0.8.tar.gz` & `tmp/flask_shopify_utils-0.0.9.tar.gz`

## Comparing `flask_shopify_utils-0.0.8.tar` & `flask_shopify_utils-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    32330 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/src/flask_shopify_utils/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/src/flask_shopify_utils/model.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/src/flask_shopify_utils/utils.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/tests/conftest.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/tests/test_admin_routes.py
--rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/tests/test_default_routes.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/tests/test_gdpr_routes.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/tests/test_graphql_cli.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/tests/test_init.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/LICENSE
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/README.md
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    32843 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.9/src/flask_shopify_utils/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.9/src/flask_shopify_utils/model.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.9/src/flask_shopify_utils/utils.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.9/tests/conftest.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.9/tests/test_admin_routes.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.9/tests/test_default_routes.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.9/tests/test_gdpr_routes.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.9/tests/test_graphql_cli.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.9/tests/test_init.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.9/README.md
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.9/PKG-INFO
```

### Comparing `flask_shopify_utils-0.0.8/src/flask_shopify_utils/__init__.py` & `flask_shopify_utils-0.0.9/src/flask_shopify_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     make_response, url_for
 from jinja2 import TemplateNotFound
 from jwt import encode as jwt_encode, decode as jwt_decode, ExpiredSignatureError
 from cerberus.validator import Validator
 from pytz import timezone
 from flask_shopify_utils.utils import get_version, GraphQLClient
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 JWT_DATA = TypeVar('JWT_DATA', dict, Response)
 current_time_func = None
 sqlalchemy_instance = None
 
 
 class ShopifyUtil:
@@ -219,23 +219,25 @@
             @utils.check_hmac
             def index():
                 pass
         """
 
         @wraps(func)
         def decorator(*args, **kwargs):
-            # check timestamp
-            timestamp1 = int(request.args.get('timestamp', '0'))
-            timestamp2 = int(time()) - 86400
-            if timestamp1 < timestamp2:
-                return jsonify(dict(message='The request has expired', status=401))
             params = request.args
             if len([x for x in params.keys() if x in ['shop', 'hmac', 'host', 'timestamp', 'session']]) < 4:
                 # Redirect to the Docs page
                 return redirect(url_for('docs_default.index'))
+            # Check timestamp
+            timestamp1 = int(request.args.get('timestamp', '0'))
+            timestamp2 = int(time()) - 86400
+            if timestamp1 < timestamp2:
+                resp = self.proxy_response(401, 'The request has expired')
+                resp.status_code = 401
+                return resp
             # Check Hmac
             if not compare_digest(
                     self.validate_hmac(params),
                     request.args.get('hmac', '')
             ):
                 resp = self.proxy_response(401, 'Invalid HMAC')
                 resp.status_code = 401
@@ -552,15 +554,15 @@
             'docs_default',
             'docs_routes',
             url_prefix='/docs',
             static_folder=static_folder,
             template_folder=static_folder,
         )
 
-        @doc_routes.route('/', methods=['GET'])
+        @doc_routes.route('', methods=['GET'])
         def index() -> Response:
             """
             Show the docs for default message
             """
             try:
                 return make_response(render_template('index.html'))
             except TemplateNotFound:
@@ -570,19 +572,17 @@
         default_routes = Blueprint(
             'shopify_default',
             'shopify_default_routes',
             static_folder=static_folder,
             template_folder=static_folder,
         )
 
-        # Register the `admin` route
-        @default_routes.route('/', methods=['GET'], endpoint='index')
+        @default_routes.route('/admin', methods=['GET'], endpoint='admin')
         @self.check_hmac
-        def index() -> Response:
-            """ Show Embedded App or Docs page """
+        def admin() -> Response:
             # check database
             bypass = self.config.get('BYPASS_VALIDATE', 0)
             if bypass != 0:
                 g.store_id = bypass
             else:
                 store = self.db.query(Store).filter_by(key=g.store_key).first()
                 if not store:
@@ -601,14 +601,24 @@
                     host=g.host,
                     jwtToken=self.create_admin_jwt_token()
                 )
             except TemplateNotFound:
                 return self.proxy_response(0, 'Oops... The `index.html` is gone!')
             return make_response(code)
 
+        # Index Route -> redirect to Docs or Admin
+        @default_routes.route('/', methods=['GET'], endpoint='index')
+        def index() -> Response:
+            """ Show Embedded App or Docs page """
+            params = request.args
+            if len([x for x in params.keys() if x in ['shop', 'hmac', 'host', 'timestamp', 'session']]) < 4:
+                # Redirect to the Docs page
+                return redirect(url_for('docs_default.index'))
+            return redirect(url_for('shopify_default.admin'))
+
         # Register the `callback` route
         @default_routes.route('/callback', methods=['GET'], endpoint='callback')
         @self.check_callback
         def callback():
             url = 'https://{}/admin/oauth/access_token'.format(g.store_key)
             res = post_request(url, json=dict(
                 client_id=self.config.get('SHOPIFY_API_KEY'),
@@ -737,15 +747,16 @@
             """ Check the granted scopes is update to date or not """
             if action not in ['reinstall', 'status']:
                 return self.admin_response()
             record = Store.query.filter_by(id=g.store_id).first()
             if not record:
                 return self.admin_response(400, 'Store[{}] does not exist!'.format(g.store_id))
             if action == 'reinstall':
-                return self.admin_response(data=url_for('shopify_default.install', shop=record.key, _external=True, _scheme='https'))
+                return self.admin_response(
+                    data=url_for('shopify_default.install', shop=record.key, _external=True, _scheme='https'))
             current_scopes = record.scopes.lower().split(',')
             scopes = self.config.get('SCOPES').lower().split(',')
             removes = [v for v in current_scopes if v not in scopes]
             adds = [v for v in scopes if v not in current_scopes]
             return self.admin_response(data=dict(
                 removes=removes,
                 adds=adds,
```

### Comparing `flask_shopify_utils-0.0.8/src/flask_shopify_utils/model.py` & `flask_shopify_utils-0.0.9/src/flask_shopify_utils/model.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.8/src/flask_shopify_utils/utils.py` & `flask_shopify_utils-0.0.9/src/flask_shopify_utils/utils.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.8/tests/conftest.py` & `flask_shopify_utils-0.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.8/tests/test_admin_routes.py` & `flask_shopify_utils-0.0.9/tests/test_admin_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.8/tests/test_default_routes.py` & `flask_shopify_utils-0.0.9/tests/test_default_routes.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 
 def test_default_routes_enroll(utils):
     utils.enroll_default_route()
 
     rules = []
     for val in utils.app.url_map.iter_rules():
-        if val.rule in ['/', '/install', '/callback']:
+        if val.rule in ['/', '/install', '/callback', '/admin']:
             rules.append(val.rule)
-    assert 3 == len(rules)
+    assert 4 == len(rules)
 
 
 def test_install_route(utils):
     utils.enroll_default_route()
     client = utils.app.test_client()
     # Success
     params = dict(shop='test.myshopify.com')
@@ -89,46 +89,65 @@
     assert result.get('status') == 500
     assert result.get('message') == 'Something went wrong while doing the OAuth!'
 
 
 def test_index_route(utils):
     utils.enroll_default_route()
     client = utils.app.test_client()
-    # Error - docs page error
+    # none parameters -> docs page
     res = client.get('/')
-    assert res.status_code == 200
-    # Error - timestamp expired
+    assert res.status_code == 302
+    assert res.headers.get('Location', '') == '/docs'
+    params = dict(
+        timestamp=int(time()),
+        host='host_token_for_app_bridge',
+        shop='test.myshopify.com',
+        session='shopify_session_token',
+        hmac='test'
+    )
+    res = client.get('/?{}'.format(urlencode(params)))
+    assert res.status_code == 302
+    assert res.headers.get('Location', '') == '/admin'
+
+
+def test_admin_index_route(utils):
+    utils.enroll_default_route()
+    client = utils.app.test_client()
+    # none parameters -> docs page
+    res = client.get('/admin')
+    assert res.status_code == 302
+    assert res.headers.get('Location', '') == '/docs'
+    # Error - Invalid Timestamp
     timestamp = int(time()) - 86400 - 1
     params = dict(
         timestamp=timestamp,
         host='host_token_for_app_bridge',
         shop='test.myshopify.com',
         session='shopify_session_token',
         hmac='test'
     )
-    res = client.get('/?{}'.format(urlencode(params)))
-    assert res.status_code == 200
+    res = client.get('/admin?{}'.format(urlencode(params)))
+    assert res.status_code == 401
     result = res.get_json()
     assert result.get('status') == 401
     assert result.get('message') == "The request has expired"
     # Error - Invalid Hmac
     params['timestamp'] = int(time())
-    res = client.get('/?{}'.format(urlencode(params)))
+    res = client.get('/admin?{}'.format(urlencode(params)))
     assert res.status_code == 401
     result = res.get_json()
     assert result.get('status') == 401
     assert result.get('message') == "Invalid HMAC"
-    # pass
+    # Error - No Database Record
     del params['hmac']
     params['hmac'] = utils.validate_hmac(params)
-    res = client.get('/?{}'.format(urlencode(params)))
-    # Success -> no record in database
-    assert res.status_code == 404
+    res = client.get('/admin?{}'.format(urlencode(params)))
     result = res.get_json()
     assert result.get('status') == 404
+    assert 'not found in database!' in result.get('message')
+    # Bypass - pass
     utils.config['BYPASS_VALIDATE'] = 1
-    res = client.get('/?{}'.format(urlencode(params)))
+    res = client.get('/admin?{}'.format(urlencode(params)))
     assert res.status_code == 200
     result = res.get_json()
     assert 0 == result.get('status')
     assert 'Oops... The `index.html` is gone!' == result.get('message')
-
```

### Comparing `flask_shopify_utils-0.0.8/tests/test_gdpr_routes.py` & `flask_shopify_utils-0.0.9/tests/test_gdpr_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.8/LICENSE` & `flask_shopify_utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.8/README.md` & `flask_shopify_utils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.8/pyproject.toml` & `flask_shopify_utils-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.8/PKG-INFO` & `flask_shopify_utils-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-shopify-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Flask extension for Shopify app development
 Project-URL: Homepage, https://github.com/leocxy/flask-shopify-utils
 Project-URL: Bug Tracker, https://github.com/leocxy/flask-shopify-utils/issues
 Author: Leo Chen
 Author-email: leo.cxy88@gmail.com
 Maintainer: Leo Chen
 Maintainer-email: leo.cxy88@gmail.com
```

