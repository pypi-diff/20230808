# Comparing `tmp/Scrapset-6.9.5.tar.gz` & `tmp/Scrapset-7.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scrapset-6.9.5.tar", last modified: Mon Aug  7 17:11:56 2023, max compression
+gzip compressed data, was "Scrapset-7.0.5.tar", last modified: Mon Aug  7 18:24:41 2023, max compression
```

## Comparing `Scrapset-6.9.5.tar` & `Scrapset-7.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 17:11:56.819665 Scrapset-6.9.5/
--rw-rw-rw-   0        0        0     8276 2023-08-07 17:11:56.820662 Scrapset-6.9.5/PKG-INFO
--rw-rw-rw-   0        0        0     8045 2023-08-07 16:27:51.000000 Scrapset-6.9.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 17:11:56.786642 Scrapset-6.9.5/Scrapset/
--rw-rw-rw-   0        0        0    12999 2023-08-07 17:09:52.000000 Scrapset-6.9.5/Scrapset/Scrapset.py
--rw-rw-rw-   0        0        0       81 2023-08-07 15:52:26.000000 Scrapset-6.9.5/Scrapset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 17:11:56.818665 Scrapset-6.9.5/Scrapset.egg-info/
--rw-rw-rw-   0        0        0     8276 2023-08-07 17:11:56.000000 Scrapset-6.9.5/Scrapset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-08-07 17:11:56.000000 Scrapset-6.9.5/Scrapset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 17:11:56.000000 Scrapset-6.9.5/Scrapset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-07 17:11:56.000000 Scrapset-6.9.5/Scrapset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-08-07 17:11:56.000000 Scrapset-6.9.5/Scrapset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-07 17:11:56.000000 Scrapset-6.9.5/Scrapset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2023-07-30 04:41:08.000000 Scrapset-6.9.5/licence.txt
--rw-rw-rw-   0        0        0      158 2023-08-07 17:11:56.823188 Scrapset-6.9.5/setup.cfg
--rw-rw-rw-   0        0        0      499 2023-08-07 17:11:41.000000 Scrapset-6.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 18:24:41.008847 Scrapset-7.0.5/
+-rw-rw-rw-   0        0        0     8276 2023-08-07 18:24:41.010147 Scrapset-7.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8045 2023-08-07 16:27:51.000000 Scrapset-7.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 18:24:40.987837 Scrapset-7.0.5/Scrapset/
+-rw-rw-rw-   0        0        0    13000 2023-08-07 18:24:31.000000 Scrapset-7.0.5/Scrapset/Scrapset.py
+-rw-rw-rw-   0        0        0       81 2023-08-07 15:52:26.000000 Scrapset-7.0.5/Scrapset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 18:24:41.007841 Scrapset-7.0.5/Scrapset.egg-info/
+-rw-rw-rw-   0        0        0     8276 2023-08-07 18:24:40.000000 Scrapset-7.0.5/Scrapset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-08-07 18:24:40.000000 Scrapset-7.0.5/Scrapset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 18:24:40.000000 Scrapset-7.0.5/Scrapset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-07 18:24:40.000000 Scrapset-7.0.5/Scrapset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-08-07 18:24:40.000000 Scrapset-7.0.5/Scrapset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-07 18:24:40.000000 Scrapset-7.0.5/Scrapset.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2023-07-30 04:41:08.000000 Scrapset-7.0.5/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-08-07 18:24:41.011144 Scrapset-7.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      499 2023-08-07 18:20:07.000000 Scrapset-7.0.5/setup.py
```

### Comparing `Scrapset-6.9.5/PKG-INFO` & `Scrapset-7.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 6.9.5
+Version: 7.0.5
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-6.9.5/README.md` & `Scrapset-7.0.5/README.md`

 * *Files identical despite different names*

### Comparing `Scrapset-6.9.5/Scrapset/Scrapset.py` & `Scrapset-7.0.5/Scrapset/Scrapset.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
             driver.quit()
             logging.error('Invalid Url')
     def vessel_location(self,url):
         try:
             driver=webdriver.Chrome()
             c=1
             text=list()
-            while c<=10:
+            while c<=293:
                 driver.get(url+f'/ports?page={c}')
                 time.sleep(0.4)
                 cards=driver.find_elements(By.XPATH,'/html/body/div[1]/div/main/div[1]/table/tbody/tr')
                 for card in cards:
                     text.append(card.text+'<>')
                 c=c+1
             driver.quit()
```

### Comparing `Scrapset-6.9.5/Scrapset.egg-info/PKG-INFO` & `Scrapset-7.0.5/Scrapset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 6.9.5
+Version: 7.0.5
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-6.9.5/licence.txt` & `Scrapset-7.0.5/licence.txt`

 * *Files identical despite different names*

