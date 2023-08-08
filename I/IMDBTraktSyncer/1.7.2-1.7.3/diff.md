# Comparing `tmp/IMDBTraktSyncer-1.7.2.tar.gz` & `tmp/IMDBTraktSyncer-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.7.2.tar", last modified: Wed Aug  2 07:07:56 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.7.3.tar", last modified: Tue Aug  8 20:43:45 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.7.2.tar` & `IMDBTraktSyncer-1.7.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 07:07:56.036050 IMDBTraktSyncer-1.7.2/
-drwxrwxrwx   0        0        0        0 2023-08-02 07:07:56.003039 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    41616 2023-08-02 07:06:39.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4624 2023-07-31 01:18:20.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4317 2023-07-31 01:18:20.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     6946 2023-08-02 06:46:34.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     1669 2023-07-31 01:18:20.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/errorLogger.py
--rw-rw-rw-   0        0        0    11546 2023-08-02 05:50:14.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0    10572 2023-07-31 01:18:20.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0    12192 2023-07-31 01:18:20.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:07:56.033041 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    12719 2023-08-02 07:07:55.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-08-02 07:07:55.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 07:07:55.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-08-02 07:07:55.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-08-02 07:07:55.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-02 07:07:55.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.7.2/LICENSE
--rw-rw-rw-   0        0        0    12719 2023-08-02 07:07:56.035040 IMDBTraktSyncer-1.7.2/PKG-INFO
--rw-rw-rw-   0        0        0    11972 2023-08-02 07:07:19.000000 IMDBTraktSyncer-1.7.2/README.md
--rw-rw-rw-   0        0        0       42 2023-08-02 07:07:56.036050 IMDBTraktSyncer-1.7.2/setup.cfg
--rw-rw-rw-   0        0        0     1377 2023-08-02 07:00:53.000000 IMDBTraktSyncer-1.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:43:45.911128 IMDBTraktSyncer-1.7.3/
+drwxrwxrwx   0        0        0        0 2023-08-08 20:43:45.881129 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    41616 2023-08-02 07:06:39.000000 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4624 2023-08-02 08:19:49.000000 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4317 2023-08-08 20:41:50.000000 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     6946 2023-08-02 06:46:34.000000 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1669 2023-07-31 01:18:20.000000 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0    11546 2023-08-02 05:50:14.000000 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0    10572 2023-07-31 01:18:20.000000 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0    12192 2023-07-31 01:18:20.000000 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:43:45.908128 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    12733 2023-08-08 20:43:45.000000 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-08-08 20:43:45.000000 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 20:43:45.000000 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-08-08 20:43:45.000000 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-08-08 20:43:45.000000 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-08 20:43:45.000000 IMDBTraktSyncer-1.7.3/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.7.3/LICENSE
+-rw-rw-rw-   0        0        0    12733 2023-08-08 20:43:45.910128 IMDBTraktSyncer-1.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11986 2023-08-08 20:42:31.000000 IMDBTraktSyncer-1.7.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-08 20:43:45.911128 IMDBTraktSyncer-1.7.3/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2023-08-08 20:42:08.000000 IMDBTraktSyncer-1.7.3/setup.py
```

### Comparing `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/authTrakt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import requests
 import time
 try:
     from IMDBTraktSyncer import errorLogger as EL
 except ImportError:
     import errorLogger as EL
 
-def make_trakt_request(url, headers=None, params=None, payload=None, max_retries=3):
-    retry_delay = 5  # seconds between retries
+def make_trakt_request(url, headers=None, params=None, payload=None, max_retries=5):
+    retry_delay = 1  # seconds between retries
     retry_attempts = 0
 
     while retry_attempts < max_retries:
         response = None
         try:
             response = requests.post(url, headers=headers, json=payload)
```

### Comparing `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/checkChromedriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     subprocess.run([sys.executable, '-m', 'pip', 'install', '--no-cache-dir', f'chromedriver-py=={version}'])
 
 def install_chromedriver_fallback_method():
     print("Using install chromedriver-py fallback method")
     # Install the chromedriver-py package using the Python interpreter
     feed = feedparser.parse('https://pypi.org/rss/project/chromedriver-py/releases.xml')
     # Get the second latest release version
-    version = feed.entries[1].title.split()[-1]
+    version = feed.entries[0].title.split()[-1]
     # Install the chromedriver-py package using pip
     subprocess.run([sys.executable, '-m', 'pip', 'install', '--no-cache-dir', f'chromedriver-py=={version}'])
 
 # Check if chromedriver-py is already installed
 try:
     dist = pkg_resources.get_distribution('chromedriver-py')
     installed_version = dist.version.split('.')[0]  # Retrieve only the prefix
```

### Comparing `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/errorLogger.py` & `IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/errorLogger.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/imdbData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.7.3/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.7.3/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.7.2
+Version: 1.7.3
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 
 # IMDB-Trakt-Syncer
 This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Existing items will not be overwritten. Ratings, watchlist and comment/review sync are all optional. The user will be prompted to enter their settings and credentials on first run.
 
 The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux and Mac). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/IMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During installation, tick the box for adding Python to your PATH variable. _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During Python installation, tick the box for adding Python to your PATH variable. _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## Installing the Script:
@@ -51,15 +51,15 @@
 ## Installing a Specific Version:
 ```
 python -m pip install IMDBTraktSyncer==VERSION_NUMBER
 ```
 _Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) (e.g. 1.1.6) and run in your operating system's native command line._
 
 ## Alternative Manual Installation Method (without pip install)
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During installation, tick the box for adding Python to your PATH variable.  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During Python installation, tick the box for adding Python to your PATH variable.  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run `IMDBTraktSyncer.py` or open the terminal and navigate to the folder where `IMDBTraktSyncer.py` is located. Run `IMDBTraktSyncer.py` in the terminal.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## For Setting Up Automation See the Following Wiki Pages:
```

### Comparing `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.7.3/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.2/LICENSE` & `IMDBTraktSyncer-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.2/PKG-INFO` & `IMDBTraktSyncer-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.7.2
+Version: 1.7.3
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 
 # IMDB-Trakt-Syncer
 This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Existing items will not be overwritten. Ratings, watchlist and comment/review sync are all optional. The user will be prompted to enter their settings and credentials on first run.
 
 The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux and Mac). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/IMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During installation, tick the box for adding Python to your PATH variable. _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During Python installation, tick the box for adding Python to your PATH variable. _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## Installing the Script:
@@ -51,15 +51,15 @@
 ## Installing a Specific Version:
 ```
 python -m pip install IMDBTraktSyncer==VERSION_NUMBER
 ```
 _Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) (e.g. 1.1.6) and run in your operating system's native command line._
 
 ## Alternative Manual Installation Method (without pip install)
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During installation, tick the box for adding Python to your PATH variable.  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During Python installation, tick the box for adding Python to your PATH variable.  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run `IMDBTraktSyncer.py` or open the terminal and navigate to the folder where `IMDBTraktSyncer.py` is located. Run `IMDBTraktSyncer.py` in the terminal.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## For Setting Up Automation See the Following Wiki Pages:
```

### Comparing `IMDBTraktSyncer-1.7.2/README.md` & `IMDBTraktSyncer-1.7.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # IMDB-Trakt-Syncer
 This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Existing items will not be overwritten. Ratings, watchlist and comment/review sync are all optional. The user will be prompted to enter their settings and credentials on first run.
 
 The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux and Mac). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/IMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During installation, tick the box for adding Python to your PATH variable. _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During Python installation, tick the box for adding Python to your PATH variable. _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## Installing the Script:
@@ -35,15 +35,15 @@
 ## Installing a Specific Version:
 ```
 python -m pip install IMDBTraktSyncer==VERSION_NUMBER
 ```
 _Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) (e.g. 1.1.6) and run in your operating system's native command line._
 
 ## Alternative Manual Installation Method (without pip install)
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During installation, tick the box for adding Python to your PATH variable.  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During Python installation, tick the box for adding Python to your PATH variable.  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run `IMDBTraktSyncer.py` or open the terminal and navigate to the folder where `IMDBTraktSyncer.py` is located. Run `IMDBTraktSyncer.py` in the terminal.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## For Setting Up Automation See the Following Wiki Pages:
```

### Comparing `IMDBTraktSyncer-1.7.2/setup.py` & `IMDBTraktSyncer-1.7.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.7.2'
+VERSION = '1.7.3'
 DESCRIPTION = 'A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

