# Comparing `tmp/rug-0.8.4.tar.gz` & `tmp/rug-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rug-0.8.4.tar", max compression
+gzip compressed data, was "rug-0.8.5.tar", max compression
```

## Comparing `rug-0.8.4.tar` & `rug-0.8.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      762 2023-06-16 06:42:16.417052 rug-0.8.4/README.md
--rw-r--r--   0        0        0      853 2023-08-05 08:06:24.171775 rug-0.8.4/pyproject.toml
--rw-r--r--   0        0        0      263 2023-08-04 16:20:35.385529 rug-0.8.4/rug/__init__.py
--rw-r--r--   0        0        0     4266 2022-10-10 19:45:59.707606 rug-0.8.4/rug/alphaquery.py
--rw-r--r--   0        0        0     2688 2022-08-11 07:37:52.820634 rug-0.8.4/rug/barchart.py
--rw-r--r--   0        0        0     4997 2023-06-16 06:35:11.344249 rug-0.8.4/rug/base.py
--rw-r--r--   0        0        0     4150 2022-12-23 18:09:17.774153 rug-0.8.4/rug/etfdb.py
--rw-r--r--   0        0        0      683 2022-07-27 20:03:36.438856 rug-0.8.4/rug/exceptions.py
--rw-r--r--   0        0        0     3038 2023-06-16 06:33:17.358960 rug-0.8.4/rug/finviz.py
--rw-r--r--   0        0        0     5276 2023-08-05 08:02:40.481001 rug-0.8.4/rug/stockanalysis.py
--rw-r--r--   0        0        0     1947 2022-08-11 08:42:20.047418 rug-0.8.4/rug/stocktwits.py
--rw-r--r--   0        0        0     6910 2023-05-05 06:58:34.815386 rug-0.8.4/rug/tipranks.py
--rw-r--r--   0        0        0     1764 1970-01-01 00:00:00.000000 rug-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0      762 2023-06-16 06:42:16.417052 rug-0.8.5/README.md
+-rw-r--r--   0        0        0      853 2023-08-08 09:26:55.156717 rug-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-08-06 16:18:57.666687 rug-0.8.5/rug/__init__.py
+-rw-r--r--   0        0        0     4266 2022-10-10 19:45:59.707606 rug-0.8.5/rug/alphaquery.py
+-rw-r--r--   0        0        0     2688 2022-08-11 07:37:52.820634 rug-0.8.5/rug/barchart.py
+-rw-r--r--   0        0        0     4997 2023-06-16 06:35:11.344249 rug-0.8.5/rug/base.py
+-rw-r--r--   0        0        0     4150 2022-12-23 18:09:17.774153 rug-0.8.5/rug/etfdb.py
+-rw-r--r--   0        0        0      683 2022-07-27 20:03:36.438856 rug-0.8.5/rug/exceptions.py
+-rw-r--r--   0        0        0     3038 2023-06-16 06:33:17.358960 rug-0.8.5/rug/finviz.py
+-rw-r--r--   0        0        0     5626 2023-08-08 09:17:29.797599 rug-0.8.5/rug/stockanalysis.py
+-rw-r--r--   0        0        0     1947 2022-08-11 08:42:20.047418 rug-0.8.5/rug/stocktwits.py
+-rw-r--r--   0        0        0     6910 2023-05-05 06:58:34.815386 rug-0.8.5/rug/tipranks.py
+-rw-r--r--   0        0        0     4548 2023-08-08 09:15:35.160159 rug-0.8.5/rug/yahoo.py
+-rw-r--r--   0        0        0     1764 1970-01-01 00:00:00.000000 rug-0.8.5/PKG-INFO
```

### Comparing `rug-0.8.4/README.md` & `rug-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `rug-0.8.4/pyproject.toml` & `rug-0.8.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rug"
-version = "0.8.4"
+version = "0.8.5"
 description = "Library for fetching various stock data from the internet (official and unofficial APIs)."
 authors = ["Pavel Hrdina"]
 classifiers = [
     "Programming Language :: Python :: 3.6",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Intended Audience :: Developers",
```

### Comparing `rug-0.8.4/rug/alphaquery.py` & `rug-0.8.5/rug/alphaquery.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.4/rug/barchart.py` & `rug-0.8.5/rug/barchart.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.4/rug/base.py` & `rug-0.8.5/rug/base.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.4/rug/etfdb.py` & `rug-0.8.5/rug/etfdb.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.4/rug/exceptions.py` & `rug-0.8.5/rug/exceptions.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.4/rug/finviz.py` & `rug-0.8.5/rug/finviz.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.4/rug/stockanalysis.py` & `rug-0.8.5/rug/stockanalysis.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,155 +38,155 @@
         # improperly parsed  - "%" has it's own column and the
         # last "shares" column is then not parsed.
         parser.feed(finds[0])
         parser.data[:6] = ("No.", "Symbol", "Name", "% Weight", "Shares")
 
         return parser.get_data()
 
-    def get_current_price_change(self):
-        """
-        Fetches current market price inc. pre/post market
-        prices/percent/value changes. Also returns current
-        market state (pre-market, open, post-market, closed).
-
-        Fetched stucture has following fields:
-
-        - state (pre-market, open, post-market, closed)
-        - pre_market
-            - change
-                - percents
-                - value
-            - value
-        - current_market
-            - change
-                - percents
-                - value
-            - value
-        - post_market
-            - change
-                - percents
-                - value
-            - value
-
-        Returned dict looks like:
-
-        .. code-block:: python
-
-            {
-                "state": "open",
-                "pre_market": {
-                    "change": {
-                        "percents": -1.32476,
-                        "value": -1.42001
-                    },
-                    "value": 105.77
-                },
-                "current_market": {
-                    "change": {
-                        "percents": -1.6046284000000002,
-                        "value": -1.7200012
-                    },
-                    "value": 105.47
-                },
-                "post_market": {
-                    "change": {
-                        "percents": 0.0,
-                        "value": 0.0
-                    },
-                    "value": 0.0
-                }
-            }
-
-        :return: Current/Pre/Post market numbers (all are floats).
-        :rtype: dict
-        """
-
-        def get_state(data):
-            """
-            Returns one of following market states:
-
-            - open
-            - closed
-            - pre-market
-            - post-market
-            """
-
-            # Is state "extended" (meaning closed)?
-            if not data["e"]:
-                return data["ms"].lower()
-            else:
-                # Converts "After-hours" to "post-market".
-                if "after-hours" == data["es"].lower():
-                    return "post-market"
-
-                return data["es"].lower()
-
-        try:
-            response = self._get(
-                f"https://stockanalysis.com/api/quotes/s/{self.symbol.lower()}"
-            )
-        except Exception as e:
-            raise SymbolNotFound from e
-
-        data = response.json()["data"]
-        state = get_state(data)
-        to_return = {
-            "state": state,
-        }
-
-        # Pre-market data.
-        if "pre-market" == state:
-            to_return["pre_market"] = {
-                "change": {
-                    "percents": data["ecp"],
-                    "value": data["ec"],
-                },
-                "value": data["ep"],
-            }
-        else:
-            to_return["pre_market"] = {
-                "change": {
-                    "percents": 0,
-                    "value": 0,
-                },
-                "value": 0,
-            }
-
-        # Market to_return.
-        if "open" == data["ms"]:
-            to_return["current_market"] = {
-                "change": {
-                    "percents": data["cp"],
-                    "value": data["c"],
-                },
-                "value": data["p"],
-            }
-
-        else:
-            to_return["current_market"] = {
-                "change": {
-                    "percents": 0,
-                    "value": 0,
-                },
-                "value": 0,
-            }
-
-        # Post-market data.
-        if "post-market" == state:
-            to_return["post_market"] = {
-                "change": {
-                    "percents": data["ecp"],
-                    "value": data["ec"],
-                },
-                "value": data["ep"],
-            }
-
-        else:
-            to_return["post_market"] = {
-                "change": {
-                    "percents": 0,
-                    "value": 0,
-                },
-                "value": 0,
-            }
-
-        return to_return
+    # def get_current_price_change(self):
+    #     """
+    #     Fetches current market price inc. pre/post market
+    #     prices/percent/value changes. Also returns current
+    #     market state (pre-market, open, post-market, closed).
+    #
+    #     Fetched stucture has following fields:
+    #
+    #     - state (pre-market, open, post-market, closed)
+    #     - pre_market
+    #         - change
+    #             - percents
+    #             - value
+    #         - value
+    #     - current_market
+    #         - change
+    #             - percents
+    #             - value
+    #         - value
+    #     - post_market
+    #         - change
+    #             - percents
+    #             - value
+    #         - value
+    #
+    #     Returned dict looks like:
+    #
+    #     .. code-block:: python
+    #
+    #         {
+    #             "state": "open",
+    #             "pre_market": {
+    #                 "change": {
+    #                     "percents": -1.32476,
+    #                     "value": -1.42001
+    #                 },
+    #                 "value": 105.77
+    #             },
+    #             "current_market": {
+    #                 "change": {
+    #                     "percents": -1.6046284000000002,
+    #                     "value": -1.7200012
+    #                 },
+    #                 "value": 105.47
+    #             },
+    #             "post_market": {
+    #                 "change": {
+    #                     "percents": 0.0,
+    #                     "value": 0.0
+    #                 },
+    #                 "value": 0.0
+    #             }
+    #         }
+    #
+    #     :return: Current/Pre/Post market numbers (all are floats).
+    #     :rtype: dict
+    #     """
+    #
+    #     def get_state(data):
+    #         """
+    #         Returns one of following market states:
+    #
+    #         - open
+    #         - closed
+    #         - pre-market
+    #         - post-market
+    #         """
+    #
+    #         # Is state "extended" (meaning closed)?
+    #         if not data["e"]:
+    #             return data["ms"].lower()
+    #         else:
+    #             # Converts "After-hours" to "post-market".
+    #             if "after-hours" == data["es"].lower():
+    #                 return "post-market"
+    #
+    #             return data["es"].lower()
+    #
+    #     try:
+    #         response = self._get(
+    #             f"https://stockanalysis.com/api/quotes/s/{self.symbol.lower()}"
+    #         )
+    #     except Exception as e:
+    #         raise SymbolNotFound from e
+    #
+    #     data = response.json()["data"]
+    #     state = get_state(data)
+    #     to_return = {
+    #         "state": state,
+    #     }
+    #
+    #     # Pre-market data.
+    #     if "pre-market" == state:
+    #         to_return["pre_market"] = {
+    #             "change": {
+    #                 "percents": data["ecp"],
+    #                 "value": data["ec"],
+    #             },
+    #             "value": data["ep"],
+    #         }
+    #     else:
+    #         to_return["pre_market"] = {
+    #             "change": {
+    #                 "percents": 0,
+    #                 "value": 0,
+    #             },
+    #             "value": 0,
+    #         }
+    #
+    #     # Market to_return.
+    #     if "open" == data["ms"]:
+    #         to_return["current_market"] = {
+    #             "change": {
+    #                 "percents": data["cp"],
+    #                 "value": data["c"],
+    #             },
+    #             "value": data["p"],
+    #         }
+    #
+    #     else:
+    #         to_return["current_market"] = {
+    #             "change": {
+    #                 "percents": 0,
+    #                 "value": 0,
+    #             },
+    #             "value": 0,
+    #         }
+    #
+    #     # Post-market data.
+    #     if "post-market" == state:
+    #         to_return["post_market"] = {
+    #             "change": {
+    #                 "percents": data["ecp"],
+    #                 "value": data["ec"],
+    #             },
+    #             "value": data["ep"],
+    #         }
+    #
+    #     else:
+    #         to_return["post_market"] = {
+    #             "change": {
+    #                 "percents": 0,
+    #                 "value": 0,
+    #             },
+    #             "value": 0,
+    #         }
+    #
+    #     return to_return
```

### Comparing `rug-0.8.4/rug/stocktwits.py` & `rug-0.8.5/rug/stocktwits.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.4/rug/tipranks.py` & `rug-0.8.5/rug/tipranks.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.4/PKG-INFO` & `rug-0.8.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rug
-Version: 0.8.4
+Version: 0.8.5
 Summary: Library for fetching various stock data from the internet (official and unofficial APIs).
 Home-page: https://github.com/im-n1/rug
 License: MIT
 Author: Pavel Hrdina
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

