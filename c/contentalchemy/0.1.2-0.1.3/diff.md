# Comparing `tmp/contentalchemy-0.1.2.tar.gz` & `tmp/contentalchemy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contentalchemy-0.1.2.tar", max compression
+gzip compressed data, was "contentalchemy-0.1.3.tar", max compression
```

## Comparing `contentalchemy-0.1.2.tar` & `contentalchemy-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0        0 2023-07-27 02:40:10.435321 contentalchemy-0.1.2/README.md
--rw-r--r--   0        0        0      279 2023-07-27 06:01:38.764204 contentalchemy-0.1.2/contentalchemy/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 03:13:04.336291 contentalchemy-0.1.2/contentalchemy/images/__init__.py
--rw-r--r--   0        0        0      175 2023-07-27 04:45:27.477854 contentalchemy-0.1.2/contentalchemy/images/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2023-07-27 03:14:18.966030 contentalchemy-0.1.2/contentalchemy/images/sync_api/__init__.py
--rw-r--r--   0        0        0      184 2023-07-27 04:45:27.477854 contentalchemy-0.1.2/contentalchemy/images/sync_api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2182 2023-07-27 04:45:27.477854 contentalchemy-0.1.2/contentalchemy/images/sync_api/__pycache__/snapper.cpython-310.pyc
--rw-r--r--   0        0        0     2064 2023-07-27 04:05:29.541928 contentalchemy-0.1.2/contentalchemy/images/sync_api/snapper.py
--rwxr-xr-x   0        0        0    16864 2023-07-26 18:41:09.439633 contentalchemy-0.1.2/contentalchemy/images/sync_api/snapshot_template.html
--rw-r--r--   0        0        0      333 2023-07-27 06:02:04.726859 contentalchemy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 contentalchemy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      488 2023-07-27 06:35:50.067968 contentalchemy-0.1.3/README.md
+-rw-r--r--   0        0        0      463 2023-08-08 07:06:59.714839 contentalchemy-0.1.3/contentalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 11:11:59.790729 contentalchemy-0.1.3/contentalchemy/content_formatters/__init__.py
+-rw-r--r--   0        0        0     2937 2023-08-04 04:07:03.411369 contentalchemy-0.1.3/contentalchemy/content_formatters/base.py
+-rw-r--r--   0        0        0        0 2023-07-27 03:13:04.336291 contentalchemy-0.1.3/contentalchemy/images/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 03:14:18.966030 contentalchemy-0.1.3/contentalchemy/images/async_api/__init__.py
+-rw-r--r--   0        0        0     2336 2023-08-08 07:03:39.793960 contentalchemy-0.1.3/contentalchemy/images/async_api/snapper.py
+-rwxr-xr-x   0        0        0    16864 2023-07-26 18:41:09.439633 contentalchemy-0.1.3/contentalchemy/images/async_api/snapshot_template.html
+-rw-r--r--   0        0        0        0 2023-07-27 03:14:18.966030 contentalchemy-0.1.3/contentalchemy/images/sync_api/__init__.py
+-rw-r--r--   0        0        0     2137 2023-08-02 03:45:31.309802 contentalchemy-0.1.3/contentalchemy/images/sync_api/snapper.py
+-rwxr-xr-x   0        0        0    16864 2023-07-26 18:41:09.439633 contentalchemy-0.1.3/contentalchemy/images/sync_api/snapshot_template.html
+-rw-r--r--   0        0        0      448 2023-08-08 07:07:29.808437 contentalchemy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1270 1970-01-01 00:00:00.000000 contentalchemy-0.1.3/PKG-INFO
```

### Comparing `contentalchemy-0.1.2/contentalchemy/images/sync_api/snapper.py` & `contentalchemy-0.1.3/contentalchemy/images/sync_api/snapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         with sync_playwright() as playwright:
             chromium = playwright.chromium
             endpoint = self._browser_endpoint
             browser = chromium.connect_over_cdp(endpoint) if endpoint else chromium.launch()
             page = browser.new_page()
             page.set_content(content)
             page.locator('#MathInput').evaluate("(element, value) => element.value = value", html)
+            page.wait_for_function('typeof typesetInput === "function"')
             page.evaluate('typesetInput()')
             page.wait_for_load_state('domcontentloaded')
             page.wait_for_load_state('networkidle')
             page.wait_for_selector('#status')
             data = page.locator('#MathPreview').screenshot(scale='css')
             page.close()
             browser.close()
```

### Comparing `contentalchemy-0.1.2/contentalchemy/images/sync_api/snapshot_template.html` & `contentalchemy-0.1.3/contentalchemy/images/async_api/snapshot_template.html`

 * *Files identical despite different names*

