# Comparing `tmp/PyNINA-0.3.1.tar.gz` & `tmp/PyNINA-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNINA-0.3.1.tar", last modified: Sun Jul 16 11:25:38 2023, max compression
+gzip compressed data, was "PyNINA-0.3.2.tar", last modified: Tue Aug  8 19:48:17 2023, max compression
```

## Comparing `PyNINA-0.3.1.tar` & `PyNINA-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-07-16 11:25:38.861994 PyNINA-0.3.1/
--rwxrwxrwx   0 user      (1000) user      (1000)     1087 2021-08-31 18:45:53.000000 PyNINA-0.3.1/LICENSE
--rwxrwxrwx   0 user      (1000) user      (1000)     2061 2023-07-16 11:25:38.859426 PyNINA-0.3.1/PKG-INFO
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-07-16 11:25:38.760341 PyNINA-0.3.1/PyNINA.egg-info/
--rwxrwxrwx   0 user      (1000) user      (1000)     2061 2023-07-16 11:25:38.000000 PyNINA-0.3.1/PyNINA.egg-info/PKG-INFO
--rwxrwxrwx   0 user      (1000) user      (1000)      285 2023-07-16 11:25:38.000000 PyNINA-0.3.1/PyNINA.egg-info/SOURCES.txt
--rwxrwxrwx   0 user      (1000) user      (1000)        1 2023-07-16 11:25:38.000000 PyNINA-0.3.1/PyNINA.egg-info/dependency_links.txt
--rwxrwxrwx   0 user      (1000) user      (1000)       15 2023-07-16 11:25:38.000000 PyNINA-0.3.1/PyNINA.egg-info/requires.txt
--rwxrwxrwx   0 user      (1000) user      (1000)        7 2023-07-16 11:25:38.000000 PyNINA-0.3.1/PyNINA.egg-info/top_level.txt
--rwxrwxrwx   0 user      (1000) user      (1000)      552 2021-09-11 21:30:24.000000 PyNINA-0.3.1/README.md
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-07-16 11:25:38.843569 PyNINA-0.3.1/pynina/
--rwxrwxrwx   0 user      (1000) user      (1000)      138 2023-07-16 11:20:13.000000 PyNINA-0.3.1/pynina/__init__.py
--rwxrwxrwx   0 user      (1000) user      (1000)     1431 2023-04-30 11:34:43.000000 PyNINA-0.3.1/pynina/baseApi.py
--rwxrwxrwx   0 user      (1000) user      (1000)    15135 2023-04-30 11:32:16.000000 PyNINA-0.3.1/pynina/const.py
--rwxrwxrwx   0 user      (1000) user      (1000)      696 2022-12-08 20:25:43.000000 PyNINA-0.3.1/pynina/label_matcher.py
--rwxrwxrwx   0 user      (1000) user      (1000)     2143 2022-12-08 20:25:43.000000 PyNINA-0.3.1/pynina/nina.py
--rwxrwxrwx   0 user      (1000) user      (1000)     2596 2023-07-16 11:19:44.000000 PyNINA-0.3.1/pynina/warning.py
--rwxrwxrwx   0 user      (1000) user      (1000)       38 2023-07-16 11:25:38.862535 PyNINA-0.3.1/setup.cfg
--rwxrwxrwx   0 user      (1000) user      (1000)      585 2023-07-16 11:20:13.000000 PyNINA-0.3.1/setup.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-08-08 19:48:17.076236 PyNINA-0.3.2/
+-rwxrwxrwx   0 user      (1000) user      (1000)     1087 2021-08-31 18:45:53.000000 PyNINA-0.3.2/LICENSE
+-rwxrwxrwx   0 user      (1000) user      (1000)     2061 2023-08-08 19:48:17.071380 PyNINA-0.3.2/PKG-INFO
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-08-08 19:48:16.771998 PyNINA-0.3.2/PyNINA.egg-info/
+-rwxrwxrwx   0 user      (1000) user      (1000)     2061 2023-08-08 19:48:16.000000 PyNINA-0.3.2/PyNINA.egg-info/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)      285 2023-08-08 19:48:16.000000 PyNINA-0.3.2/PyNINA.egg-info/SOURCES.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        1 2023-08-08 19:48:16.000000 PyNINA-0.3.2/PyNINA.egg-info/dependency_links.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)       15 2023-08-08 19:48:16.000000 PyNINA-0.3.2/PyNINA.egg-info/requires.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        7 2023-08-08 19:48:16.000000 PyNINA-0.3.2/PyNINA.egg-info/top_level.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)      552 2021-09-11 21:30:24.000000 PyNINA-0.3.2/README.md
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-08-08 19:48:17.034625 PyNINA-0.3.2/pynina/
+-rwxrwxrwx   0 user      (1000) user      (1000)      138 2023-08-08 19:45:10.000000 PyNINA-0.3.2/pynina/__init__.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1509 2023-08-08 19:35:57.000000 PyNINA-0.3.2/pynina/baseApi.py
+-rwxrwxrwx   0 user      (1000) user      (1000)    14085 2023-08-08 19:31:54.000000 PyNINA-0.3.2/pynina/const.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      696 2022-12-08 20:25:43.000000 PyNINA-0.3.2/pynina/label_matcher.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2297 2023-08-08 19:37:03.000000 PyNINA-0.3.2/pynina/nina.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2685 2023-08-08 19:37:12.000000 PyNINA-0.3.2/pynina/warning.py
+-rwxrwxrwx   0 user      (1000) user      (1000)       38 2023-08-08 19:48:17.077919 PyNINA-0.3.2/setup.cfg
+-rwxrwxrwx   0 user      (1000) user      (1000)      587 2023-08-08 19:45:10.000000 PyNINA-0.3.2/setup.py
```

### Comparing `PyNINA-0.3.1/LICENSE` & `PyNINA-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNINA-0.3.1/PKG-INFO` & `PyNINA-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNINA
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python API wrapper to retrieve warnings from the german NINA app.
 Home-page: https://gitlab.com/DeerMaximum/pynina
 Author: DeerMaximum
 Author-email: git983456@parabelmail.de
 License: MIT License
         
         Copyright (c) 2021 DeerMaximum
```

### Comparing `PyNINA-0.3.1/PyNINA.egg-info/PKG-INFO` & `PyNINA-0.3.2/PyNINA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNINA
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python API wrapper to retrieve warnings from the german NINA app.
 Home-page: https://gitlab.com/DeerMaximum/pynina
 Author: DeerMaximum
 Author-email: git983456@parabelmail.de
 License: MIT License
         
         Copyright (c) 2021 DeerMaximum
```

### Comparing `PyNINA-0.3.1/README.md` & `PyNINA-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `PyNINA-0.3.1/pynina/baseApi.py` & `PyNINA-0.3.2/pynina/baseApi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import asyncio
 from typing import Any, Dict
 
 from aiohttp import ClientSession, ClientConnectionError, ClientTimeout
 
+from .const import _LOGGER
+
 
 class BaseAPI:
     """Class to perform CMI API requests"""
 
     def __init__(self, session: ClientSession = None):
         """Constructor for BaseAPI."""
         self.session = session
@@ -14,14 +16,16 @@
     async def _makeRequest(self, url: str):
         """Retrieve data from API."""
         internalSession: bool = False
         if self.session is None:
             internalSession = True
             self.session = ClientSession()
 
+        _LOGGER.debug(f"Try to fetch {url}")
+
         try:
             async with self.session.get(url, timeout=ClientTimeout(total=9)) as res:
                 if res.status != 200:
                     raise ApiError(f"Invalid response: {res.status}")
 
                 json: Dict[str, Any] = await res.json()
                 if internalSession:
```

### Comparing `PyNINA-0.3.1/pynina/const.py` & `PyNINA-0.3.2/pynina/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,311 +1,315 @@
+from logging import Logger, getLogger, NullHandler
+
 ENDPOINT_REGIONAL_CODE: str = "https://www.xrepository.de/api/xrepository/urn:de:bund:destatis:bevoelkerungsstatistik:schluessel:rs_2021-07-31/download/Regionalschl_ssel_2021-07-31.json"
 ENDPOINT_NINA_BASE: str = "https://warnung.bund.de/api31/dashboard/"
 ENDPOINT_WARNING_DETAIL: str = "https://warnung.bund.de/api31/warnings/"
-ENDPOINT_DE_LABELS: str = "https://warnung.bund.de/api/appdata/gsb/labels/de_labels.json"
+ENDPOINT_DE_LABELS: str = (
+    "https://warnung.bund.de/api/appdata/gsb/labels/de_labels.json"
+)
+
+_LOGGER: Logger = getLogger(__package__)
+_LOGGER.addHandler(NullHandler())
 
-CITY_STATES_CODE = [
-    "02",
-    "11"
-]
+CITY_STATES_CODE = ["02", "11"]
 
 COUNTIES = {
-        "01051": "Dithmarschen - Schleswig-Holstein",
-        "01053": "Herzogtum Lauenburg - Schleswig-Holstein",
-        "01054": "Nordfriesland - Schleswig-Holstein",
-        "01055": "Ostholstein - Schleswig-Holstein",
-        "01056": "Pinneberg - Schleswig-Holstein",
-        "01057": "Plön - Schleswig-Holstein",
-        "01058": "Rendsburg-Eckernförde - Schleswig-Holstein",
-        "01059": "Schleswig-Flensburg - Schleswig-Holstein",
-        "01060": "Segeberg - Schleswig-Holstein",
-        "01061": "Steinburg - Schleswig-Holstein",
-        "01062": "Stormarn - Schleswig-Holstein",
-        "03151": "Gifhorn - Niedersachsen",
-        "03153": "Goslar - Niedersachsen",
-        "03154": "Helmstedt - Niedersachsen",
-        "03155": "Northeim - Niedersachsen",
-        "03157": "Peine - Niedersachsen",
-        "03158": "Wolfenbüttel - Niedersachsen",
-        "03159": "Göttingen - Niedersachsen",
-        "03241": "Hannover, Region - Niedersachsen",
-        "03251": "Diepholz - Niedersachsen",
-        "03252": "Hameln-Pyrmont - Niedersachsen",
-        "03254": "Hildesheim - Niedersachsen",
-        "03255": "Holzminden - Niedersachsen",
-        "03256": "Nienburg/Weser - Niedersachsen",
-        "03257": "Schaumburg - Niedersachsen",
-        "03351": "Celle - Niedersachsen",
-        "03352": "Cuxhaven - Niedersachsen",
-        "03353": "Harburg - Niedersachsen",
-        "03354": "Lüchow-Dannenberg - Niedersachsen",
-        "03355": "Lüneburg - Niedersachsen",
-        "03356": "Osterholz - Niedersachsen",
-        "03357": "Rotenburg (Wümme) - Niedersachsen",
-        "03358": "Heidekreis - Niedersachsen",
-        "03359": "Stade - Niedersachsen",
-        "03360": "Uelzen - Niedersachsen",
-        "03361": "Verden - Niedersachsen",
-        "03451": "Ammerland - Niedersachsen",
-        "03452": "Aurich - Niedersachsen",
-        "03453": "Cloppenburg - Niedersachsen",
-        "03454": "Emsland - Niedersachsen",
-        "03455": "Friesland - Niedersachsen",
-        "03456": "Grafschaft Bentheim - Niedersachsen",
-        "03457": "Leer - Niedersachsen",
-        "03458": "Oldenburg - Niedersachsen",
-        "03459": "Osnabrück - Niedersachsen",
-        "03460": "Vechta - Niedersachsen",
-        "03461": "Wesermarsch - Niedersachsen",
-        "03462": "Wittmund - Niedersachsen",
-        "05154": "Kleve - Nordrhein-Westfalen",
-        "05158": "Mettmann - Nordrhein-Westfalen",
-        "05162": "Rhein-Kreis Neuss - Nordrhein-Westfalen",
-        "05166": "Viersen - Nordrhein-Westfalen",
-        "05170": "Wesel - Nordrhein-Westfalen",
-        "05334": "Aachen, Städteregion - Nordrhein-Westfalen",
-        "05358": "Düren - Nordrhein-Westfalen",
-        "05362": "Rhein-Erft-Kreis - Nordrhein-Westfalen",
-        "05366": "Euskirchen - Nordrhein-Westfalen",
-        "05370": "Heinsberg - Nordrhein-Westfalen",
-        "05374": "Oberbergischer Kreis - Nordrhein-Westfalen",
-        "05378": "Rheinisch-Bergischer Kreis - Nordrhein-Westfalen",
-        "05382": "Rhein-Sieg-Kreis - Nordrhein-Westfalen",
-        "05554": "Borken - Nordrhein-Westfalen",
-        "05558": "Coesfeld - Nordrhein-Westfalen",
-        "05562": "Recklinghausen - Nordrhein-Westfalen",
-        "05566": "Steinfurt - Nordrhein-Westfalen",
-        "05570": "Warendorf - Nordrhein-Westfalen",
-        "05754": "Gütersloh - Nordrhein-Westfalen",
-        "05758": "Herford - Nordrhein-Westfalen",
-        "05762": "Höxter - Nordrhein-Westfalen",
-        "05766": "Lippe - Nordrhein-Westfalen",
-        "05770": "Minden-Lübbecke - Nordrhein-Westfalen",
-        "05774": "Paderborn - Nordrhein-Westfalen",
-        "05954": "Ennepe-Ruhr-Kreis - Nordrhein-Westfalen",
-        "05958": "Hochsauerlandkreis - Nordrhein-Westfalen",
-        "05962": "Märkischer Kreis - Nordrhein-Westfalen",
-        "05966": "Olpe - Nordrhein-Westfalen",
-        "05970": "Siegen-Wittgenstein - Nordrhein-Westfalen",
-        "05974": "Soest - Nordrhein-Westfalen",
-        "05978": "Unna - Nordrhein-Westfalen",
-        "06431": "Bergstraße - Hessen",
-        "06432": "Darmstadt-Dieburg - Hessen",
-        "06433": "Groß-Gerau - Hessen",
-        "06434": "Hochtaunuskreis - Hessen",
-        "06435": "Main-Kinzig-Kreis - Hessen",
-        "06436": "Main-Taunus-Kreis - Hessen",
-        "06437": "Odenwaldkreis - Hessen",
-        "06438": "Offenbach - Hessen",
-        "06439": "Rheingau-Taunus-Kreis - Hessen",
-        "06440": "Wetteraukreis - Hessen",
-        "06531": "Gießen - Hessen",
-        "06532": "Lahn-Dill-Kreis - Hessen",
-        "06533": "Limburg-Weilburg - Hessen",
-        "06534": "Marburg-Biedenkopf - Hessen",
-        "06535": "Vogelsbergkreis - Hessen",
-        "06631": "Fulda - Hessen",
-        "06632": "Hersfeld-Rotenburg - Hessen",
-        "06633": "Kassel - Hessen",
-        "06634": "Schwalm-Eder-Kreis - Hessen",
-        "06635": "Waldeck-Frankenberg - Hessen",
-        "06636": "Werra-Meißner-Kreis - Hessen",
-        "07131": "Ahrweiler - Rheinland-Pfalz",
-        "07132": "Altenkirchen (Westerwald) - Rheinland-Pfalz",
-        "07133": "Bad Kreuznach - Rheinland-Pfalz",
-        "07134": "Birkenfeld - Rheinland-Pfalz",
-        "07135": "Cochem-Zell - Rheinland-Pfalz",
-        "07137": "Mayen-Koblenz - Rheinland-Pfalz",
-        "07138": "Neuwied - Rheinland-Pfalz",
-        "07140": "Rhein-Hunsrück-Kreis - Rheinland-Pfalz",
-        "07141": "Rhein-Lahn-Kreis - Rheinland-Pfalz",
-        "07143": "Westerwaldkreis - Rheinland-Pfalz",
-        "07231": "Bernkastel-Wittlich - Rheinland-Pfalz",
-        "07232": "Eifelkreis Bitburg-Prüm - Rheinland-Pfalz",
-        "07233": "Vulkaneifel - Rheinland-Pfalz",
-        "07235": "Trier-Saarburg - Rheinland-Pfalz",
-        "07331": "Alzey-Worms - Rheinland-Pfalz",
-        "07332": "Bad Dürkheim - Rheinland-Pfalz",
-        "07333": "Donnersbergkreis - Rheinland-Pfalz",
-        "07334": "Germersheim - Rheinland-Pfalz",
-        "07335": "Kaiserslautern - Rheinland-Pfalz",
-        "07336": "Kusel - Rheinland-Pfalz",
-        "07337": "Südliche Weinstraße - Rheinland-Pfalz",
-        "07338": "Rhein-Pfalz-Kreis - Rheinland-Pfalz",
-        "07339": "Mainz-Bingen - Rheinland-Pfalz",
-        "07340": "Südwestpfalz - Rheinland-Pfalz",
-        "08115": "Böblingen - Baden-Württemberg",
-        "08116": "Esslingen - Baden-Württemberg",
-        "08117": "Göppingen - Baden-Württemberg",
-        "08118": "Ludwigsburg - Baden-Württemberg",
-        "08119": "Rems-Murr-Kreis - Baden-Württemberg",
-        "08125": "Heilbronn - Baden-Württemberg",
-        "08126": "Hohenlohekreis - Baden-Württemberg",
-        "08127": "Schwäbisch Hall - Baden-Württemberg",
-        "08128": "Main-Tauber-Kreis - Baden-Württemberg",
-        "08135": "Heidenheim - Baden-Württemberg",
-        "08136": "Ostalbkreis - Baden-Württemberg",
-        "08215": "Karlsruhe - Baden-Württemberg",
-        "08216": "Rastatt - Baden-Württemberg",
-        "08225": "Neckar-Odenwald-Kreis - Baden-Württemberg",
-        "08226": "Rhein-Neckar-Kreis - Baden-Württemberg",
-        "08235": "Calw - Baden-Württemberg",
-        "08236": "Enzkreis - Baden-Württemberg",
-        "08237": "Freudenstadt - Baden-Württemberg",
-        "08315": "Breisgau-Hochschwarzwald - Baden-Württemberg",
-        "08316": "Emmendingen - Baden-Württemberg",
-        "08317": "Ortenaukreis - Baden-Württemberg",
-        "08325": "Rottweil - Baden-Württemberg",
-        "08326": "Schwarzwald-Baar-Kreis - Baden-Württemberg",
-        "08327": "Tuttlingen - Baden-Württemberg",
-        "08335": "Konstanz - Baden-Württemberg",
-        "08336": "Lörrach - Baden-Württemberg",
-        "08337": "Waldshut - Baden-Württemberg",
-        "08415": "Reutlingen - Baden-Württemberg",
-        "08416": "Tübingen - Baden-Württemberg",
-        "08417": "Zollernalbkreis - Baden-Württemberg",
-        "08425": "Alb-Donau-Kreis - Baden-Württemberg",
-        "08426": "Biberach - Baden-Württemberg",
-        "08435": "Bodenseekreis - Baden-Württemberg",
-        "08436": "Ravensburg - Baden-Württemberg",
-        "08437": "Sigmaringen - Baden-Württemberg",
-        "09171": "Altötting - Bayern",
-        "09172": "Berchtesgadener Land - Bayern",
-        "09173": "Bad Tölz-Wolfratshausen - Bayern",
-        "09174": "Dachau - Bayern",
-        "09175": "Ebersberg - Bayern",
-        "09176": "Eichstätt - Bayern",
-        "09177": "Erding - Bayern",
-        "09178": "Freising - Bayern",
-        "09179": "Fürstenfeldbruck - Bayern",
-        "09180": "Garmisch-Partenkirchen - Bayern",
-        "09181": "Landsberg am Lech - Bayern",
-        "09182": "Miesbach - Bayern",
-        "09183": "Mühldorf am Inn - Bayern",
-        "09184": "München - Bayern",
-        "09185": "Neuburg-Schrobenhausen - Bayern",
-        "09186": "Pfaffenhofen an der Ilm - Bayern",
-        "09187": "Rosenheim - Bayern",
-        "09188": "Starnberg - Bayern",
-        "09189": "Traunstein - Bayern",
-        "09190": "Weilheim-Schongau - Bayern",
-        "09271": "Deggendorf - Bayern",
-        "09272": "Freyung-Grafenau - Bayern",
-        "09273": "Kelheim - Bayern",
-        "09274": "Landshut - Bayern",
-        "09275": "Passau - Bayern",
-        "09276": "Regen - Bayern",
-        "09277": "Rottal-Inn - Bayern",
-        "09278": "Straubing-Bogen - Bayern",
-        "09279": "Dingolfing-Landau - Bayern",
-        "09371": "Amberg-Sulzbach - Bayern",
-        "09372": "Cham - Bayern",
-        "09373": "Neumarkt in der Oberpfalz - Bayern",
-        "09374": "Neustadt an der Waldnaab - Bayern",
-        "09375": "Regensburg - Bayern",
-        "09376": "Schwandorf - Bayern",
-        "09377": "Tirschenreuth - Bayern",
-        "09471": "Bamberg - Bayern",
-        "09472": "Bayreuth - Bayern",
-        "09473": "Coburg - Bayern",
-        "09474": "Forchheim - Bayern",
-        "09475": "Hof - Bayern",
-        "09476": "Kronach - Bayern",
-        "09477": "Kulmbach - Bayern",
-        "09478": "Lichtenfels - Bayern",
-        "09479": "Wunsiedel im Fichtelgebirge - Bayern",
-        "09571": "Ansbach - Bayern",
-        "09572": "Erlangen-Höchstadt - Bayern",
-        "09573": "Fürth - Bayern",
-        "09574": "Nürnberger Land - Bayern",
-        "09575": "Neustadt an der Aisch-Bad Windsheim - Bayern",
-        "09576": "Roth - Bayern",
-        "09577": "Weißenburg-Gunzenhausen - Bayern",
-        "09671": "Aschaffenburg - Bayern",
-        "09672": "Bad Kissingen - Bayern",
-        "09673": "Rhön-Grabfeld - Bayern",
-        "09674": "Haßberge - Bayern",
-        "09675": "Kitzingen - Bayern",
-        "09676": "Miltenberg - Bayern",
-        "09677": "Main-Spessart - Bayern",
-        "09678": "Schweinfurt - Bayern",
-        "09679": "Würzburg - Bayern",
-        "09771": "Aichach-Friedberg - Bayern",
-        "09772": "Augsburg - Bayern",
-        "09773": "Dillingen an der Donau - Bayern",
-        "09774": "Günzburg - Bayern",
-        "09775": "Neu-Ulm - Bayern",
-        "09776": "Lindau (Bodensee) - Bayern",
-        "09777": "Ostallgäu - Bayern",
-        "09778": "Unterallgäu - Bayern",
-        "09779": "Donau-Ries - Bayern",
-        "09780": "Oberallgäu - Bayern",
-        "10041": "Saarbrücken, Regionalverband - Saarland",
-        "10042": "Merzig-Wadern - Saarland",
-        "10043": "Neunkirchen - Saarland",
-        "10044": "Saarlouis - Saarland",
-        "10045": "Saarpfalz-Kreis - Saarland",
-        "10046": "Sachsen-Anhalt. Wendel - Saarland",
-        "12060": "Barnim - Brandenburg",
-        "12061": "Dahme-Spreewald - Brandenburg",
-        "12062": "Elbe-Elster - Brandenburg",
-        "12063": "Havelland - Brandenburg",
-        "12064": "Märkisch-Oderland - Brandenburg",
-        "12065": "Oberhavel - Brandenburg",
-        "12066": "Oberspreewald-Lausitz - Brandenburg",
-        "12067": "Oder-Spree - Brandenburg",
-        "12068": "Ostprignitz-Ruppin - Brandenburg",
-        "12069": "Potsdam-Mittelmark - Brandenburg",
-        "12070": "Prignitz - Brandenburg",
-        "12071": "Spree-Neiße - Brandenburg",
-        "12072": "Teltow-Fläming - Brandenburg",
-        "12073": "Uckermark - Brandenburg",
-        "13071": "Mecklenburgische Seenplatte - Mecklenburg-Vorpommern",
-        "13072": "Rostock - Mecklenburg-Vorpommern",
-        "13073": "Vorpommern-Rügen - Mecklenburg-Vorpommern",
-        "13074": "Nordwestmecklenburg - Mecklenburg-Vorpommern",
-        "13075": "Vorpommern-Greifswald - Mecklenburg-Vorpommern",
-        "13076": "Ludwigslust-Parchim - Mecklenburg-Vorpommern",
-        "14521": "Erzgebirgskreis - Sachsen",
-        "14522": "Mittelsachsen - Sachsen",
-        "14523": "Vogtlandkreis - Sachsen",
-        "14524": "Zwickau - Sachsen",
-        "14625": "Bautzen - Sachsen",
-        "14626": "Görlitz - Sachsen",
-        "14627": "Meißen - Sachsen",
-        "14628": "Sächsische Schweiz-Osterzgebirge - Sachsen",
-        "14729": "Leipzig - Sachsen",
-        "14730": "Nordsachsen - Sachsen",
-        "15081": "Altmarkkreis Salzwedel - Sachsen-Anhalt",
-        "15082": "Anhalt-Bitterfeld - Sachsen-Anhalt",
-        "15083": "Börde - Sachsen-Anhalt",
-        "15084": "Burgenlandkreis - Sachsen-Anhalt",
-        "15085": "Harz - Sachsen-Anhalt",
-        "15086": "Jerichower Land - Sachsen-Anhalt",
-        "15087": "Mansfeld-Südharz - Sachsen-Anhalt",
-        "15088": "Saalekreis - Sachsen-Anhalt",
-        "15089": "Salzlandkreis - Sachsen-Anhalt",
-        "15090": "Stendal - Sachsen-Anhalt",
-        "15091": "Wittenberg - Sachsen-Anhalt",
-        "16061": "Eichsfeld - Thüringen",
-        "16062": "Nordhausen - Thüringen",
-        "16063": "Wartburgkreis - Thüringen",
-        "16064": "Unstrut-Hainich-Kreis - Thüringen",
-        "16065": "Kyffhäuserkreis - Thüringen",
-        "16066": "Schmalkalden-Meiningen - Thüringen",
-        "16067": "Gotha - Thüringen",
-        "16068": "Sömmerda - Thüringen",
-        "16069": "Hildburghausen - Thüringen",
-        "16070": "Ilm-Kreis - Thüringen",
-        "16071": "Weimarer Land - Thüringen",
-        "16072": "Sonneberg - Thüringen",
-        "16073": "Saalfeld-Rudolstadt - Thüringen",
-        "16074": "Saale-Holzland-Kreis - Thüringen",
-        "16075": "Saale-Orla-Kreis - Thüringen",
-        "16076": "Greiz - Thüringen",
-        "16077": "Altenburger Land - Thüringen",
-    }
+    "01051": "Dithmarschen - Schleswig-Holstein",
+    "01053": "Herzogtum Lauenburg - Schleswig-Holstein",
+    "01054": "Nordfriesland - Schleswig-Holstein",
+    "01055": "Ostholstein - Schleswig-Holstein",
+    "01056": "Pinneberg - Schleswig-Holstein",
+    "01057": "Plön - Schleswig-Holstein",
+    "01058": "Rendsburg-Eckernförde - Schleswig-Holstein",
+    "01059": "Schleswig-Flensburg - Schleswig-Holstein",
+    "01060": "Segeberg - Schleswig-Holstein",
+    "01061": "Steinburg - Schleswig-Holstein",
+    "01062": "Stormarn - Schleswig-Holstein",
+    "03151": "Gifhorn - Niedersachsen",
+    "03153": "Goslar - Niedersachsen",
+    "03154": "Helmstedt - Niedersachsen",
+    "03155": "Northeim - Niedersachsen",
+    "03157": "Peine - Niedersachsen",
+    "03158": "Wolfenbüttel - Niedersachsen",
+    "03159": "Göttingen - Niedersachsen",
+    "03241": "Hannover, Region - Niedersachsen",
+    "03251": "Diepholz - Niedersachsen",
+    "03252": "Hameln-Pyrmont - Niedersachsen",
+    "03254": "Hildesheim - Niedersachsen",
+    "03255": "Holzminden - Niedersachsen",
+    "03256": "Nienburg/Weser - Niedersachsen",
+    "03257": "Schaumburg - Niedersachsen",
+    "03351": "Celle - Niedersachsen",
+    "03352": "Cuxhaven - Niedersachsen",
+    "03353": "Harburg - Niedersachsen",
+    "03354": "Lüchow-Dannenberg - Niedersachsen",
+    "03355": "Lüneburg - Niedersachsen",
+    "03356": "Osterholz - Niedersachsen",
+    "03357": "Rotenburg (Wümme) - Niedersachsen",
+    "03358": "Heidekreis - Niedersachsen",
+    "03359": "Stade - Niedersachsen",
+    "03360": "Uelzen - Niedersachsen",
+    "03361": "Verden - Niedersachsen",
+    "03451": "Ammerland - Niedersachsen",
+    "03452": "Aurich - Niedersachsen",
+    "03453": "Cloppenburg - Niedersachsen",
+    "03454": "Emsland - Niedersachsen",
+    "03455": "Friesland - Niedersachsen",
+    "03456": "Grafschaft Bentheim - Niedersachsen",
+    "03457": "Leer - Niedersachsen",
+    "03458": "Oldenburg - Niedersachsen",
+    "03459": "Osnabrück - Niedersachsen",
+    "03460": "Vechta - Niedersachsen",
+    "03461": "Wesermarsch - Niedersachsen",
+    "03462": "Wittmund - Niedersachsen",
+    "05154": "Kleve - Nordrhein-Westfalen",
+    "05158": "Mettmann - Nordrhein-Westfalen",
+    "05162": "Rhein-Kreis Neuss - Nordrhein-Westfalen",
+    "05166": "Viersen - Nordrhein-Westfalen",
+    "05170": "Wesel - Nordrhein-Westfalen",
+    "05334": "Aachen, Städteregion - Nordrhein-Westfalen",
+    "05358": "Düren - Nordrhein-Westfalen",
+    "05362": "Rhein-Erft-Kreis - Nordrhein-Westfalen",
+    "05366": "Euskirchen - Nordrhein-Westfalen",
+    "05370": "Heinsberg - Nordrhein-Westfalen",
+    "05374": "Oberbergischer Kreis - Nordrhein-Westfalen",
+    "05378": "Rheinisch-Bergischer Kreis - Nordrhein-Westfalen",
+    "05382": "Rhein-Sieg-Kreis - Nordrhein-Westfalen",
+    "05554": "Borken - Nordrhein-Westfalen",
+    "05558": "Coesfeld - Nordrhein-Westfalen",
+    "05562": "Recklinghausen - Nordrhein-Westfalen",
+    "05566": "Steinfurt - Nordrhein-Westfalen",
+    "05570": "Warendorf - Nordrhein-Westfalen",
+    "05754": "Gütersloh - Nordrhein-Westfalen",
+    "05758": "Herford - Nordrhein-Westfalen",
+    "05762": "Höxter - Nordrhein-Westfalen",
+    "05766": "Lippe - Nordrhein-Westfalen",
+    "05770": "Minden-Lübbecke - Nordrhein-Westfalen",
+    "05774": "Paderborn - Nordrhein-Westfalen",
+    "05954": "Ennepe-Ruhr-Kreis - Nordrhein-Westfalen",
+    "05958": "Hochsauerlandkreis - Nordrhein-Westfalen",
+    "05962": "Märkischer Kreis - Nordrhein-Westfalen",
+    "05966": "Olpe - Nordrhein-Westfalen",
+    "05970": "Siegen-Wittgenstein - Nordrhein-Westfalen",
+    "05974": "Soest - Nordrhein-Westfalen",
+    "05978": "Unna - Nordrhein-Westfalen",
+    "06431": "Bergstraße - Hessen",
+    "06432": "Darmstadt-Dieburg - Hessen",
+    "06433": "Groß-Gerau - Hessen",
+    "06434": "Hochtaunuskreis - Hessen",
+    "06435": "Main-Kinzig-Kreis - Hessen",
+    "06436": "Main-Taunus-Kreis - Hessen",
+    "06437": "Odenwaldkreis - Hessen",
+    "06438": "Offenbach - Hessen",
+    "06439": "Rheingau-Taunus-Kreis - Hessen",
+    "06440": "Wetteraukreis - Hessen",
+    "06531": "Gießen - Hessen",
+    "06532": "Lahn-Dill-Kreis - Hessen",
+    "06533": "Limburg-Weilburg - Hessen",
+    "06534": "Marburg-Biedenkopf - Hessen",
+    "06535": "Vogelsbergkreis - Hessen",
+    "06631": "Fulda - Hessen",
+    "06632": "Hersfeld-Rotenburg - Hessen",
+    "06633": "Kassel - Hessen",
+    "06634": "Schwalm-Eder-Kreis - Hessen",
+    "06635": "Waldeck-Frankenberg - Hessen",
+    "06636": "Werra-Meißner-Kreis - Hessen",
+    "07131": "Ahrweiler - Rheinland-Pfalz",
+    "07132": "Altenkirchen (Westerwald) - Rheinland-Pfalz",
+    "07133": "Bad Kreuznach - Rheinland-Pfalz",
+    "07134": "Birkenfeld - Rheinland-Pfalz",
+    "07135": "Cochem-Zell - Rheinland-Pfalz",
+    "07137": "Mayen-Koblenz - Rheinland-Pfalz",
+    "07138": "Neuwied - Rheinland-Pfalz",
+    "07140": "Rhein-Hunsrück-Kreis - Rheinland-Pfalz",
+    "07141": "Rhein-Lahn-Kreis - Rheinland-Pfalz",
+    "07143": "Westerwaldkreis - Rheinland-Pfalz",
+    "07231": "Bernkastel-Wittlich - Rheinland-Pfalz",
+    "07232": "Eifelkreis Bitburg-Prüm - Rheinland-Pfalz",
+    "07233": "Vulkaneifel - Rheinland-Pfalz",
+    "07235": "Trier-Saarburg - Rheinland-Pfalz",
+    "07331": "Alzey-Worms - Rheinland-Pfalz",
+    "07332": "Bad Dürkheim - Rheinland-Pfalz",
+    "07333": "Donnersbergkreis - Rheinland-Pfalz",
+    "07334": "Germersheim - Rheinland-Pfalz",
+    "07335": "Kaiserslautern - Rheinland-Pfalz",
+    "07336": "Kusel - Rheinland-Pfalz",
+    "07337": "Südliche Weinstraße - Rheinland-Pfalz",
+    "07338": "Rhein-Pfalz-Kreis - Rheinland-Pfalz",
+    "07339": "Mainz-Bingen - Rheinland-Pfalz",
+    "07340": "Südwestpfalz - Rheinland-Pfalz",
+    "08115": "Böblingen - Baden-Württemberg",
+    "08116": "Esslingen - Baden-Württemberg",
+    "08117": "Göppingen - Baden-Württemberg",
+    "08118": "Ludwigsburg - Baden-Württemberg",
+    "08119": "Rems-Murr-Kreis - Baden-Württemberg",
+    "08125": "Heilbronn - Baden-Württemberg",
+    "08126": "Hohenlohekreis - Baden-Württemberg",
+    "08127": "Schwäbisch Hall - Baden-Württemberg",
+    "08128": "Main-Tauber-Kreis - Baden-Württemberg",
+    "08135": "Heidenheim - Baden-Württemberg",
+    "08136": "Ostalbkreis - Baden-Württemberg",
+    "08215": "Karlsruhe - Baden-Württemberg",
+    "08216": "Rastatt - Baden-Württemberg",
+    "08225": "Neckar-Odenwald-Kreis - Baden-Württemberg",
+    "08226": "Rhein-Neckar-Kreis - Baden-Württemberg",
+    "08235": "Calw - Baden-Württemberg",
+    "08236": "Enzkreis - Baden-Württemberg",
+    "08237": "Freudenstadt - Baden-Württemberg",
+    "08315": "Breisgau-Hochschwarzwald - Baden-Württemberg",
+    "08316": "Emmendingen - Baden-Württemberg",
+    "08317": "Ortenaukreis - Baden-Württemberg",
+    "08325": "Rottweil - Baden-Württemberg",
+    "08326": "Schwarzwald-Baar-Kreis - Baden-Württemberg",
+    "08327": "Tuttlingen - Baden-Württemberg",
+    "08335": "Konstanz - Baden-Württemberg",
+    "08336": "Lörrach - Baden-Württemberg",
+    "08337": "Waldshut - Baden-Württemberg",
+    "08415": "Reutlingen - Baden-Württemberg",
+    "08416": "Tübingen - Baden-Württemberg",
+    "08417": "Zollernalbkreis - Baden-Württemberg",
+    "08425": "Alb-Donau-Kreis - Baden-Württemberg",
+    "08426": "Biberach - Baden-Württemberg",
+    "08435": "Bodenseekreis - Baden-Württemberg",
+    "08436": "Ravensburg - Baden-Württemberg",
+    "08437": "Sigmaringen - Baden-Württemberg",
+    "09171": "Altötting - Bayern",
+    "09172": "Berchtesgadener Land - Bayern",
+    "09173": "Bad Tölz-Wolfratshausen - Bayern",
+    "09174": "Dachau - Bayern",
+    "09175": "Ebersberg - Bayern",
+    "09176": "Eichstätt - Bayern",
+    "09177": "Erding - Bayern",
+    "09178": "Freising - Bayern",
+    "09179": "Fürstenfeldbruck - Bayern",
+    "09180": "Garmisch-Partenkirchen - Bayern",
+    "09181": "Landsberg am Lech - Bayern",
+    "09182": "Miesbach - Bayern",
+    "09183": "Mühldorf am Inn - Bayern",
+    "09184": "München - Bayern",
+    "09185": "Neuburg-Schrobenhausen - Bayern",
+    "09186": "Pfaffenhofen an der Ilm - Bayern",
+    "09187": "Rosenheim - Bayern",
+    "09188": "Starnberg - Bayern",
+    "09189": "Traunstein - Bayern",
+    "09190": "Weilheim-Schongau - Bayern",
+    "09271": "Deggendorf - Bayern",
+    "09272": "Freyung-Grafenau - Bayern",
+    "09273": "Kelheim - Bayern",
+    "09274": "Landshut - Bayern",
+    "09275": "Passau - Bayern",
+    "09276": "Regen - Bayern",
+    "09277": "Rottal-Inn - Bayern",
+    "09278": "Straubing-Bogen - Bayern",
+    "09279": "Dingolfing-Landau - Bayern",
+    "09371": "Amberg-Sulzbach - Bayern",
+    "09372": "Cham - Bayern",
+    "09373": "Neumarkt in der Oberpfalz - Bayern",
+    "09374": "Neustadt an der Waldnaab - Bayern",
+    "09375": "Regensburg - Bayern",
+    "09376": "Schwandorf - Bayern",
+    "09377": "Tirschenreuth - Bayern",
+    "09471": "Bamberg - Bayern",
+    "09472": "Bayreuth - Bayern",
+    "09473": "Coburg - Bayern",
+    "09474": "Forchheim - Bayern",
+    "09475": "Hof - Bayern",
+    "09476": "Kronach - Bayern",
+    "09477": "Kulmbach - Bayern",
+    "09478": "Lichtenfels - Bayern",
+    "09479": "Wunsiedel im Fichtelgebirge - Bayern",
+    "09571": "Ansbach - Bayern",
+    "09572": "Erlangen-Höchstadt - Bayern",
+    "09573": "Fürth - Bayern",
+    "09574": "Nürnberger Land - Bayern",
+    "09575": "Neustadt an der Aisch-Bad Windsheim - Bayern",
+    "09576": "Roth - Bayern",
+    "09577": "Weißenburg-Gunzenhausen - Bayern",
+    "09671": "Aschaffenburg - Bayern",
+    "09672": "Bad Kissingen - Bayern",
+    "09673": "Rhön-Grabfeld - Bayern",
+    "09674": "Haßberge - Bayern",
+    "09675": "Kitzingen - Bayern",
+    "09676": "Miltenberg - Bayern",
+    "09677": "Main-Spessart - Bayern",
+    "09678": "Schweinfurt - Bayern",
+    "09679": "Würzburg - Bayern",
+    "09771": "Aichach-Friedberg - Bayern",
+    "09772": "Augsburg - Bayern",
+    "09773": "Dillingen an der Donau - Bayern",
+    "09774": "Günzburg - Bayern",
+    "09775": "Neu-Ulm - Bayern",
+    "09776": "Lindau (Bodensee) - Bayern",
+    "09777": "Ostallgäu - Bayern",
+    "09778": "Unterallgäu - Bayern",
+    "09779": "Donau-Ries - Bayern",
+    "09780": "Oberallgäu - Bayern",
+    "10041": "Saarbrücken, Regionalverband - Saarland",
+    "10042": "Merzig-Wadern - Saarland",
+    "10043": "Neunkirchen - Saarland",
+    "10044": "Saarlouis - Saarland",
+    "10045": "Saarpfalz-Kreis - Saarland",
+    "10046": "Sachsen-Anhalt. Wendel - Saarland",
+    "12060": "Barnim - Brandenburg",
+    "12061": "Dahme-Spreewald - Brandenburg",
+    "12062": "Elbe-Elster - Brandenburg",
+    "12063": "Havelland - Brandenburg",
+    "12064": "Märkisch-Oderland - Brandenburg",
+    "12065": "Oberhavel - Brandenburg",
+    "12066": "Oberspreewald-Lausitz - Brandenburg",
+    "12067": "Oder-Spree - Brandenburg",
+    "12068": "Ostprignitz-Ruppin - Brandenburg",
+    "12069": "Potsdam-Mittelmark - Brandenburg",
+    "12070": "Prignitz - Brandenburg",
+    "12071": "Spree-Neiße - Brandenburg",
+    "12072": "Teltow-Fläming - Brandenburg",
+    "12073": "Uckermark - Brandenburg",
+    "13071": "Mecklenburgische Seenplatte - Mecklenburg-Vorpommern",
+    "13072": "Rostock - Mecklenburg-Vorpommern",
+    "13073": "Vorpommern-Rügen - Mecklenburg-Vorpommern",
+    "13074": "Nordwestmecklenburg - Mecklenburg-Vorpommern",
+    "13075": "Vorpommern-Greifswald - Mecklenburg-Vorpommern",
+    "13076": "Ludwigslust-Parchim - Mecklenburg-Vorpommern",
+    "14521": "Erzgebirgskreis - Sachsen",
+    "14522": "Mittelsachsen - Sachsen",
+    "14523": "Vogtlandkreis - Sachsen",
+    "14524": "Zwickau - Sachsen",
+    "14625": "Bautzen - Sachsen",
+    "14626": "Görlitz - Sachsen",
+    "14627": "Meißen - Sachsen",
+    "14628": "Sächsische Schweiz-Osterzgebirge - Sachsen",
+    "14729": "Leipzig - Sachsen",
+    "14730": "Nordsachsen - Sachsen",
+    "15081": "Altmarkkreis Salzwedel - Sachsen-Anhalt",
+    "15082": "Anhalt-Bitterfeld - Sachsen-Anhalt",
+    "15083": "Börde - Sachsen-Anhalt",
+    "15084": "Burgenlandkreis - Sachsen-Anhalt",
+    "15085": "Harz - Sachsen-Anhalt",
+    "15086": "Jerichower Land - Sachsen-Anhalt",
+    "15087": "Mansfeld-Südharz - Sachsen-Anhalt",
+    "15088": "Saalekreis - Sachsen-Anhalt",
+    "15089": "Salzlandkreis - Sachsen-Anhalt",
+    "15090": "Stendal - Sachsen-Anhalt",
+    "15091": "Wittenberg - Sachsen-Anhalt",
+    "16061": "Eichsfeld - Thüringen",
+    "16062": "Nordhausen - Thüringen",
+    "16063": "Wartburgkreis - Thüringen",
+    "16064": "Unstrut-Hainich-Kreis - Thüringen",
+    "16065": "Kyffhäuserkreis - Thüringen",
+    "16066": "Schmalkalden-Meiningen - Thüringen",
+    "16067": "Gotha - Thüringen",
+    "16068": "Sömmerda - Thüringen",
+    "16069": "Hildburghausen - Thüringen",
+    "16070": "Ilm-Kreis - Thüringen",
+    "16071": "Weimarer Land - Thüringen",
+    "16072": "Sonneberg - Thüringen",
+    "16073": "Saalfeld-Rudolstadt - Thüringen",
+    "16074": "Saale-Holzland-Kreis - Thüringen",
+    "16075": "Saale-Orla-Kreis - Thüringen",
+    "16076": "Greiz - Thüringen",
+    "16077": "Altenburger Land - Thüringen",
+}
 
 
 class ReadOnlyClass(type):
     def __setattr__(self, name, value):
         raise ValueError(name)
```

### Comparing `PyNINA-0.3.1/pynina/label_matcher.py` & `PyNINA-0.3.2/pynina/label_matcher.py`

 * *Files identical despite different names*

### Comparing `PyNINA-0.3.1/pynina/nina.py` & `PyNINA-0.3.2/pynina/nina.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 from typing import Dict, Any
 
 from aiohttp import ClientSession
 
-from .const import ReadOnlyClass, ENDPOINT_REGIONAL_CODE, ENDPOINT_NINA_BASE, CITY_STATES_CODE, COUNTIES
+from .const import (
+    ReadOnlyClass,
+    ENDPOINT_REGIONAL_CODE,
+    ENDPOINT_NINA_BASE,
+    CITY_STATES_CODE,
+    COUNTIES,
+    _LOGGER,
+)
 from .baseApi import BaseAPI
 from .warning import Warning
 from .label_matcher import LabelMatcher
 
 
 class Nina(BaseAPI, metaclass=ReadOnlyClass):
     """Main class to interact with the NINA API"""
@@ -27,37 +34,39 @@
         """Update the warnings."""
         if not len(self.matcher.labels):
             await self.matcher.update()
 
         self.warnings.clear()
 
         for regionCode in self.regions:
+            _LOGGER.debug(f"Update region: {regionCode}")
             url: str = ENDPOINT_NINA_BASE + regionCode + ".json"
             data = await self._makeRequest(url)
 
             self.warnings[regionCode] = []
 
             for warn in data:
                 warning: Warning = Warning(warn)
                 await warning.getDetails(self.matcher)
                 self.warnings[regionCode].append(warning)
 
     async def getAllRegionalCodes(self) -> Dict[str, str]:
         """Fetch all regional codes."""
+        _LOGGER.debug("Get all regional codes")
         rawCodeData: Dict[str, Any] = await self._makeRequest(ENDPOINT_REGIONAL_CODE)
 
         regionalCodes: Dict[str, str] = {}
         for dataBlock in rawCodeData["daten"]:
             id: str = dataBlock[0]
             name: str = dataBlock[1]
 
             if id[:5] in COUNTIES:
                 name = f"{name} ({COUNTIES[id[:5]]})"
 
             if id[:2] not in CITY_STATES_CODE:
-                id = id[:len(id) - 7] + "0000000"
+                id = id[: len(id) - 7] + "0000000"
                 regionalCodes[name] = id
 
             if id[:2] in CITY_STATES_CODE and id[:2] + "0" * 10 == id:
                 regionalCodes[name] = id
 
         return regionalCodes
```

### Comparing `PyNINA-0.3.1/pynina/warning.py` & `PyNINA-0.3.2/pynina/warning.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import datetime
 from typing import Dict, Any, Optional
 
 from aiohttp import ClientSession
 
 from .baseApi import BaseAPI
-from .const import ReadOnlyClass, ENDPOINT_WARNING_DETAIL
+from .const import ReadOnlyClass, ENDPOINT_WARNING_DETAIL, _LOGGER
 from .label_matcher import LabelMatcher
 
 
 class Warning(BaseAPI, metaclass=ReadOnlyClass):
     """Class to reflect a warning."""
+
     def __init__(self, data: Dict[str, Any], session: ClientSession = None):
         """Initialize."""
         super().__init__(session)
 
         self.id: str = data["payload"]["id"]
         self.headline: str = data["payload"]["data"]["headline"]
         self.severity: str = data["payload"]["data"]["severity"]
@@ -33,14 +34,16 @@
             currDate: datetime = datetime.datetime.now().timestamp()
             expiresDate = datetime.datetime.fromisoformat(self.expires).timestamp()
             return currDate < expiresDate
         return True
 
     async def getDetails(self, matcher: LabelMatcher = None):
         """Get the details of a warning."""
+        _LOGGER.debug(f"Fetch details for {self.id}")
+
         url: str = ENDPOINT_WARNING_DETAIL + self.id + ".json"
         data = await self._makeRequest(url)
 
         infos = data["info"][0]
 
         self.description = infos["description"]
 
@@ -60,9 +63,11 @@
             self.recommended_actions = [infos["instruction"].replace("<br/>", " ")]
 
         if matcher is not None and len(self.recommended_actions) == 0:
             for code in recommended_actions_raw:
                 self.recommended_actions.append(matcher.match(code))
 
     def __repr__(self) -> str:
-        return f"{self.id} ({self.sent}): [{self.sender}, {self.start} - " \
-               f"{self.expires} ({self.sent})] {self.headline}, {self.description}"
+        return (
+            f"{self.id} ({self.sent}): [{self.sender}, {self.start} - "
+            f"{self.expires} ({self.sent})] {self.headline}, {self.description}"
+        )
```

### Comparing `PyNINA-0.3.1/setup.py` & `PyNINA-0.3.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,18 +4,18 @@
     readme = f.read()
 
 with open("LICENSE", "r") as f:
     license = f.read()
 
 setup(
     name="PyNINA",
-    version="0.3.1",
+    version="0.3.2",
     description="A Python API wrapper to retrieve warnings from the german NINA app.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/DeerMaximum/pynina",
     author="DeerMaximum",
     author_email="git983456@parabelmail.de",
     license=license,
     packages=["pynina"],
     install_requires=["aiohttp>=3.7.4"],
-)
+)
```

