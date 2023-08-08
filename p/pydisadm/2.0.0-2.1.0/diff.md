# Comparing `tmp/pydisadm-2.0.0.tar.gz` & `tmp/pydisadm-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisadm-2.0.0.tar", max compression
+gzip compressed data, was "pydisadm-2.1.0.tar", max compression
```

## Comparing `pydisadm-2.0.0.tar` & `pydisadm-2.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     3763 2023-08-07 04:45:06.181514 pydisadm-2.0.0/README.md
--rw-r--r--   0        0        0      142 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/__init__.py
--rw-r--r--   0        0        0     1232 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/__main__.py
--rw-r--r--   0        0        0        0 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/bot/__init__.py
--rw-r--r--   0        0        0     1546 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/bot/adm_bot.py
--rw-r--r--   0        0        0     7747 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/bot/adm_cog.py
--rw-r--r--   0        0        0     2649 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/bot/update_adm_modal.py
--rw-r--r--   0        0        0      702 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/bot/utils.py
--rw-r--r--   0        0        0     2388 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/configuration.py
--rw-r--r--   0        0        0        0 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/controller/__init__.py
--rw-r--r--   0        0        0     8071 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/controller/adm_controller.py
--rw-r--r--   0        0        0        0 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/data/__init__.py
--rw-r--r--   0        0        0   368313 2023-08-07 04:45:06.185514 pydisadm-2.0.0/pydisadm/data/mapConstellations.csv
--rw-r--r--   0        0        0    34613 2023-08-07 04:45:06.185514 pydisadm-2.0.0/pydisadm/data/mapRegions.csv
--rw-r--r--   0        0        0  3277768 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/data/mapSolarSystems.csv
--rw-r--r--   0        0        0        0 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/loader/__init__.py
--rw-r--r--   0        0        0      607 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/loader/datasets.py
--rw-r--r--   0        0        0     1085 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/loader/static_data.py
--rw-r--r--   0        0        0        0 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/runnable/__init__.py
--rw-r--r--   0        0        0     1330 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/runnable/runnable_refresh.py
--rw-r--r--   0        0        0        0 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/services/__init__.py
--rw-r--r--   0        0        0      896 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/services/common.py
--rw-r--r--   0        0        0     1137 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/services/database.py
--rw-r--r--   0        0        0     3520 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/services/database_mysql.py
--rw-r--r--   0        0        0     3152 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/services/database_sqlite.py
--rw-r--r--   0        0        0     1543 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/services/esi.py
--rw-r--r--   0        0        0      580 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/services/factory.py
--rw-r--r--   0        0        0        0 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/utils/__init__.py
--rw-r--r--   0        0        0      484 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/utils/adm_utils.py
--rw-r--r--   0        0        0      472 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/utils/datetime_utils.py
--rw-r--r--   0        0        0      623 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/utils/plot_utils.py
--rw-r--r--   0        0        0      193 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/utils/thread_utils.py
--rw-r--r--   0        0        0      999 2023-08-07 04:45:37.409736 pydisadm-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     4757 1970-01-01 00:00:00.000000 pydisadm-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3849 2023-08-08 21:53:50.850070 pydisadm-2.1.0/README.md
+-rw-r--r--   0        0        0      142 2023-08-08 21:53:50.850070 pydisadm-2.1.0/pydisadm/__init__.py
+-rw-r--r--   0        0        0     1232 2023-08-08 21:53:50.850070 pydisadm-2.1.0/pydisadm/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:53:50.850070 pydisadm-2.1.0/pydisadm/bot/__init__.py
+-rw-r--r--   0        0        0     1546 2023-08-08 21:53:50.850070 pydisadm-2.1.0/pydisadm/bot/adm_bot.py
+-rw-r--r--   0        0        0     7747 2023-08-08 21:53:50.850070 pydisadm-2.1.0/pydisadm/bot/adm_cog.py
+-rw-r--r--   0        0        0     2649 2023-08-08 21:53:50.850070 pydisadm-2.1.0/pydisadm/bot/update_adm_modal.py
+-rw-r--r--   0        0        0      702 2023-08-08 21:53:50.850070 pydisadm-2.1.0/pydisadm/bot/utils.py
+-rw-r--r--   0        0        0     2517 2023-08-08 21:53:50.850070 pydisadm-2.1.0/pydisadm/configuration.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:53:50.850070 pydisadm-2.1.0/pydisadm/controller/__init__.py
+-rw-r--r--   0        0        0     8296 2023-08-08 21:53:50.850070 pydisadm-2.1.0/pydisadm/controller/adm_controller.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:53:50.850070 pydisadm-2.1.0/pydisadm/data/__init__.py
+-rw-r--r--   0        0        0   368313 2023-08-08 21:53:50.854070 pydisadm-2.1.0/pydisadm/data/mapConstellations.csv
+-rw-r--r--   0        0        0    34613 2023-08-08 21:53:50.854070 pydisadm-2.1.0/pydisadm/data/mapRegions.csv
+-rw-r--r--   0        0        0  3277768 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/data/mapSolarSystems.csv
+-rw-r--r--   0        0        0        0 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/loader/__init__.py
+-rw-r--r--   0        0        0      607 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/loader/datasets.py
+-rw-r--r--   0        0        0     1085 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/loader/static_data.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/runnable/__init__.py
+-rw-r--r--   0        0        0     1330 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/runnable/runnable_refresh.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/services/__init__.py
+-rw-r--r--   0        0        0      896 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/services/common.py
+-rw-r--r--   0        0        0     1137 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/services/database.py
+-rw-r--r--   0        0        0     3520 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/services/database_mysql.py
+-rw-r--r--   0        0        0     3238 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/services/database_sqlite.py
+-rw-r--r--   0        0        0     1543 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/services/esi.py
+-rw-r--r--   0        0        0      580 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/services/factory.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/utils/__init__.py
+-rw-r--r--   0        0        0      484 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/utils/adm_utils.py
+-rw-r--r--   0        0        0      472 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/utils/datetime_utils.py
+-rw-r--r--   0        0        0      623 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/utils/plot_utils.py
+-rw-r--r--   0        0        0      193 2023-08-08 21:53:50.870070 pydisadm-2.1.0/pydisadm/utils/thread_utils.py
+-rw-r--r--   0        0        0      999 2023-08-08 21:54:23.790307 pydisadm-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4843 1970-01-01 00:00:00.000000 pydisadm-2.1.0/PKG-INFO
```

### Comparing `pydisadm-2.0.0/README.md` & `pydisadm-2.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 Configuration is done using environment variables or `dotenv`. See `.env.example` for example configuration.
 
 - `DISCORD_TOKEN` - the token bot should use when communicating with discord.
 - `DISCORD_CHANNEL` - the channel name bot should listen too, if this is empty the bot will listen to all channels.
 - `DISCORD_GUILD_ID` - the discord server bot should be part of
 - `DISCORD_APP_ID` - the bot application ID
 - `ALLIANCE_ID` - the alliance ID for collecting ADM values, only systems owned by this alliance will be collected.
+- `ALLIANCE_IGNORE_TCU` - set to any value to ignore TCU's when collecting ADM values
 - `DB_SERVICE` - which database to use, can be: sqlite or mysql
 - `DB_CONNECTION_STRING` - the connection string
 - `DB_KEEP_ADM_DAYS` - how many days adm history should be kept in database (default 7).
 
 ### DB_CONNECTION_STRING examples
 - `sqlite` - `adm-data.sqlite` a file name
 - `mysql` - `root:root@127.0.0.1:3600/pydisadm` - a connection string (user:password@host:port/database). See [mysqlclient](https://docs.sqlalchemy.org/en/20/dialects/mysql.html#module-sqlalchemy.dialects.mysql.mysqldb) for more information
```

### Comparing `pydisadm-2.0.0/pydisadm/__main__.py` & `pydisadm-2.1.0/pydisadm/__main__.py`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pydisadm/bot/adm_bot.py` & `pydisadm-2.1.0/pydisadm/bot/adm_bot.py`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pydisadm/bot/adm_cog.py` & `pydisadm-2.1.0/pydisadm/bot/adm_cog.py`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pydisadm/bot/update_adm_modal.py` & `pydisadm-2.1.0/pydisadm/bot/update_adm_modal.py`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pydisadm/bot/utils.py` & `pydisadm-2.1.0/pydisadm/bot/utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pydisadm/configuration.py` & `pydisadm-2.1.0/pydisadm/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 
         if self.database['service'] not in Configuration.DB_SERVICES:
             raise ValueError(
                 f'[configuration] unsupported `DB_SERVICE`: {self.database["service"]}'
             )
 
         self.alliance = {
-            'id': os.getenv('ALLIANCE_ID')
+            'id': os.getenv('ALLIANCE_ID'),
+            'ignore_tcu': os.getenv('ALLIANCE_IGNORE_TCU')
         }
 
         keep_adm_days = self.database['keep_adm_days']
         if keep_adm_days is not None:
             try:
                 keep_adm_days = int(keep_adm_days)
             except ValueError as error:
@@ -57,13 +58,14 @@
         """Create printable string from configuration"""
         return (f'{self.__class__.__name__}' +
             f'(discord_token={self.discord["token"]}, ' +
             f'discord_channel={self.discord["channel"]}, ' +
             f'discord_app_id={self.discord["app_id"]}, ' +
             f'discord_guild_id={self.discord["guild_id"]}, ' +
             f'alliance_id={self.alliance["id"]}, ' +
+            f'alliance_ignore_tcu={self.alliance["ignore_tcu"]}, ' +
             f'db_keep_adm_days={self.database["keep_adm_days"]}, ' +
             f'db_service={self.database["service"]}, ' +
             f'db_connection_string={self.database["connection_string"]})')
 
     def __str__(self):
         return self.pretty_print()
```

### Comparing `pydisadm-2.0.0/pydisadm/controller/adm_controller.py` & `pydisadm-2.1.0/pydisadm/controller/adm_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,18 +123,21 @@
         system_adm['system_id'] = system['solarSystemID']
         system_adm['adm'] = [adm]
 
         self.tier_list(system_adm)
 
         return system_adm
 
-    def get_alliance_structures(self, structures, alliance_id):
+    def get_alliance_structures(self, structures, alliance_id, ignore_tcu):
         """Retrieve a list of alliance sovreignty structures"""
         structure_data = pd.DataFrame.from_dict(structures)
 
+        if ignore_tcu:
+            structure_data = structure_data[structure_data['structure_type_id'] != 32226]
+
         drop_columns = [
             'structure_id',
             'structure_type_id',
             'vulnerable_end_time',
             'vulnerable_start_time',
         ]
 
@@ -169,18 +172,18 @@
         insert_systems = self.create_system_adm_from_index(
             system, military, industrial, strategic)
 
         self.database.insert_systems(insert_systems)
 
         return (True, insert_systems['adm'][0])
 
-    def get_system_adms(self, alliance_id):
+    def get_system_adms(self, alliance_id, ignore_tcu):
         """Retrieve ADM for systems controlled by alliance"""
         structures = sovereignty_structures()
-        system_adms = self.get_alliance_structures(structures, alliance_id)
+        system_adms = self.get_alliance_structures(structures, alliance_id, ignore_tcu)
 
         system_adms.drop_duplicates(inplace=True)
 
         drop_columns = ['alliance_id']
         system_adms.drop(columns=drop_columns, inplace=True)
 
         rename_columns = {'solar_system_id': 'system_id',
@@ -197,15 +200,16 @@
         systems.sort_values(by='adm', inplace=True, ascending=True)
 
         return systems.iloc[0]
 
     def update_adm_data(self):
         """Update ADM data"""
         alliance_id = self.configuration.alliance['id']
-        system_adms = self.get_system_adms(alliance_id)
+        ignore_tcu = self.configuration.alliance['ignore_tcu']
+        system_adms = self.get_system_adms(alliance_id, ignore_tcu)
 
         self.database.insert_systems(system_adms)
 
     def purge_adm_records(self, days_old: int):
         """Purge adm records more than days_old days old"""
 
         self.database.delete_system_rows(days_old)
```

### Comparing `pydisadm-2.0.0/pydisadm/data/mapConstellations.csv` & `pydisadm-2.1.0/pydisadm/data/mapConstellations.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pydisadm/data/mapRegions.csv` & `pydisadm-2.1.0/pydisadm/data/mapRegions.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pydisadm/data/mapSolarSystems.csv` & `pydisadm-2.1.0/pydisadm/data/mapSolarSystems.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pydisadm/loader/datasets.py` & `pydisadm-2.1.0/pydisadm/loader/datasets.py`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pydisadm/loader/static_data.py` & `pydisadm-2.1.0/pydisadm/loader/static_data.py`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pydisadm/runnable/runnable_refresh.py` & `pydisadm-2.1.0/pydisadm/runnable/runnable_refresh.py`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pydisadm/services/common.py` & `pydisadm-2.1.0/pydisadm/services/common.py`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pydisadm/services/database.py` & `pydisadm-2.1.0/pydisadm/services/database.py`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pydisadm/services/database_mysql.py` & `pydisadm-2.1.0/pydisadm/services/database_mysql.py`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pydisadm/services/database_sqlite.py` & `pydisadm-2.1.0/pydisadm/services/database_sqlite.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
         self.conn = sqlite3.connect(conn_string)
         self.setup()
 
     def setup(self):
         """Setup database schema"""
         cur = self.conn.cursor()
-        cur.execute(CREATE_TABLE_ADM)
-        cur.execute(CREATE_TABLE_MAP)
+        cur.execute(CREATE_TABLE_ADM.replace('AUTO_INCREMENT', 'AUTOINCREMENT'))
+        cur.execute(CREATE_TABLE_MAP.replace('AUTO_INCREMENT', 'AUTOINCREMENT'))
         self.conn.commit()
 
     def insert_systems(self, systems):
         """Insert system ADM records"""
         systems.to_sql('adm', self.conn, index=False, if_exists='append')
 
         self.conn.commit()
```

### Comparing `pydisadm-2.0.0/pydisadm/services/esi.py` & `pydisadm-2.1.0/pydisadm/services/esi.py`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pydisadm/services/factory.py` & `pydisadm-2.1.0/pydisadm/services/factory.py`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pydisadm/utils/plot_utils.py` & `pydisadm-2.1.0/pydisadm/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-2.0.0/pyproject.toml` & `pydisadm-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydisadm"
-version = "2.0.0"
+version = "2.1.0"
 description = "A Discord bot providing ADM summaries."
 repository = "https://github.com/agelito/adm-bot"
 authors = ["Axel Wettervik"]
 license = "MIT"
 readme = "README.md"
 include = ["data/*.csv"]
```

### Comparing `pydisadm-2.0.0/PKG-INFO` & `pydisadm-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydisadm
-Version: 2.0.0
+Version: 2.1.0
 Summary: A Discord bot providing ADM summaries.
 Home-page: https://github.com/agelito/adm-bot
 License: MIT
 Author: Axel Wettervik
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -91,14 +91,15 @@
 Configuration is done using environment variables or `dotenv`. See `.env.example` for example configuration.
 
 - `DISCORD_TOKEN` - the token bot should use when communicating with discord.
 - `DISCORD_CHANNEL` - the channel name bot should listen too, if this is empty the bot will listen to all channels.
 - `DISCORD_GUILD_ID` - the discord server bot should be part of
 - `DISCORD_APP_ID` - the bot application ID
 - `ALLIANCE_ID` - the alliance ID for collecting ADM values, only systems owned by this alliance will be collected.
+- `ALLIANCE_IGNORE_TCU` - set to any value to ignore TCU's when collecting ADM values
 - `DB_SERVICE` - which database to use, can be: sqlite or mysql
 - `DB_CONNECTION_STRING` - the connection string
 - `DB_KEEP_ADM_DAYS` - how many days adm history should be kept in database (default 7).
 
 ### DB_CONNECTION_STRING examples
 - `sqlite` - `adm-data.sqlite` a file name
 - `mysql` - `root:root@127.0.0.1:3600/pydisadm` - a connection string (user:password@host:port/database). See [mysqlclient](https://docs.sqlalchemy.org/en/20/dialects/mysql.html#module-sqlalchemy.dialects.mysql.mysqldb) for more information
```

