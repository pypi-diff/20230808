# Comparing `tmp/gtfs_functions-2.0.4.tar.gz` & `tmp/gtfs_functions-2.0.5.tar.gz`

## Comparing `gtfs_functions-2.0.4.tar` & `gtfs_functions-2.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/build.sh
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/gtfs_functions/__init__.py
--rw-r--r--   0        0        0    12840 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/gtfs_functions/aux_functions.py
--rw-r--r--   0        0        0    25785 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/gtfs_functions/gtfs_functions.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/gtfs_functions/gtfs_plots.py
--rw-r--r--   0        0        0    51256 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/images/bus_segments.jpg
--rw-r--r--   0        0        0    40486 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/images/fancy_speed_per_hour.jpg
--rw-r--r--   0        0        0   139815 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/images/heatmap.jpg
--rw-r--r--   0        0        0    29542 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/images/histogram.jpg
--rw-r--r--   0        0        0    83883 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/images/kepler_seg_freq.jpg
--rw-r--r--   0        0        0    89459 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/images/kepler_speeds.jpg
--rw-r--r--   0        0        0    74232 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/images/line_frequencies.jpg
--rw-r--r--   0        0        0   138097 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/images/map_line_freq.jpg
--rw-r--r--   0        0        0   153724 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/images/map_stop_freq.jpg
--rw-r--r--   0        0        0    31273 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/images/routes.jpg
--rw-r--r--   0        0        0    16267 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/images/shapes.jpg
--rw-r--r--   0        0        0    28295 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/images/speed_hour.jpg
--rw-r--r--   0        0        0    42723 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/images/stop_times.jpg
--rw-r--r--   0        0        0    24980 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/images/stops.jpg
--rw-r--r--   0        0        0   114837 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/images/stops_freq_output.jpg
--rw-r--r--   0        0        0    13998 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/images/trips.jpg
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/LICENSE.txt
--rw-r--r--   0        0        0    18462 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/pyproject.toml
--rw-r--r--   0        0        0    19348 2020-02-02 00:00:00.000000 gtfs_functions-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/build.sh
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/gtfs_functions/__init__.py
+-rw-r--r--   0        0        0    13104 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/gtfs_functions/aux_functions.py
+-rw-r--r--   0        0        0    35009 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/gtfs_functions/gtfs_functions.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/gtfs_functions/gtfs_plots.py
+-rw-r--r--   0        0        0    51256 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/images/bus_segments.jpg
+-rw-r--r--   0        0        0    40486 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/images/fancy_speed_per_hour.jpg
+-rw-r--r--   0        0        0   139815 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/images/heatmap.jpg
+-rw-r--r--   0        0        0    29542 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/images/histogram.jpg
+-rw-r--r--   0        0        0    83883 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/images/kepler_seg_freq.jpg
+-rw-r--r--   0        0        0    89459 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/images/kepler_speeds.jpg
+-rw-r--r--   0        0        0    74232 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/images/line_frequencies.jpg
+-rw-r--r--   0        0        0   138097 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/images/map_line_freq.jpg
+-rw-r--r--   0        0        0   153724 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/images/map_stop_freq.jpg
+-rw-r--r--   0        0        0    31273 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/images/routes.jpg
+-rw-r--r--   0        0        0    16267 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/images/shapes.jpg
+-rw-r--r--   0        0        0    28295 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/images/speed_hour.jpg
+-rw-r--r--   0        0        0    42723 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/images/stop_times.jpg
+-rw-r--r--   0        0        0    24980 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/images/stops.jpg
+-rw-r--r--   0        0        0   114837 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/images/stops_freq_output.jpg
+-rw-r--r--   0        0        0    13998 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/images/trips.jpg
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/LICENSE.txt
+-rw-r--r--   0        0        0    18597 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0    19483 2020-02-02 00:00:00.000000 gtfs_functions-2.0.5/PKG-INFO
```

### Comparing `gtfs_functions-2.0.4/gtfs_functions/aux_functions.py` & `gtfs_functions-2.0.5/gtfs_functions/aux_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 import numpy as np
 
 
 def add_runtime(st):
     # Get the runtime between stops
     logging.info('adding runtime')
+    st.sort_values(by=['trip_id', 'stop_sequence'], inplace=True, ascending=True)
     c = st.trip_id == st.trip_id.shift(-1)
     st.loc[c, 'runtime_sec'] = st.arrival_time.shift(-1)[c] - st.arrival_time[c]
     st['end_stop_id'] = st.stop_id.shift(-1)
 
     return st
 
 
@@ -364,15 +365,14 @@
     elif check_null('route_long_name'):
         routes['route_name'] = routes.route_short_name
     else:
         routes['route_name'] =\
             routes.route_short_name.astype(str)\
                 + ' ' + routes.route_long_name.astype(str)
 
-
     data = pd.merge(
         data, routes[['route_id', 'route_name']],
         left_on='route_id', right_on='route_id', how='left')
 
     return data
 
 
@@ -386,7 +386,17 @@
     #The EPSG code is 32600+zone for positive latitudes and 32700+zone for negatives.
     if lat_referece <0:
         epsg_code = 32700 + zone[2]
     else:
         epsg_code = 32600 + zone[2]
         
     return epsg_code
+
+
+def num_to_letters(num):
+    result = ""
+    while num > 0:
+        num -= 1
+        digit = num % 26
+        result = chr(digit + 65) + result
+        num //= 26
+    return result
```

### Comparing `gtfs_functions-2.0.4/gtfs_functions/gtfs_functions.py` & `gtfs_functions-2.0.5/gtfs_functions/gtfs_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,40 +2,48 @@
 import pandas as pd
 from zipfile import ZipFile
 import os
 import logging
 import geopandas as gpd
 import logging
 import requests, io
-import pendulum
+import pendulum as pl
 import hashlib
 from shapely.geometry import LineString, MultiPoint
 from gtfs_functions.aux_functions import *
+import sys
+
+if not sys.warnoptions:
+    import warnings
+    warnings.simplefilter("ignore")
 
 logging.basicConfig(level=logging.INFO)
 
 
 class Feed:
     def __init__(
             self,
             gtfs_path: str,
             time_windows: list = [0, 6, 9, 15, 19, 22, 24],
             busiest_date: bool = True,
             geo: bool = True,
-            patterns: bool = True
+            patterns: bool = True,
+            dates: list = []
             ):
 
         self._gtfs_path = gtfs_path
         self._time_windows = time_windows
         self._busiest_date = busiest_date
         self._geo = geo
         self._patterns = patterns
+        self._dates = dates
         self._routes_patterns = None
         self._trips_patterns = None
         self._files = None
+        self._bbox = None
         self._busiest_service_id = None
         self._agency = None
         self._calendar = None
         self._calendar_dates = None
         self._trips = None
         self._routes = None
         self._stops = None
@@ -43,16 +51,16 @@
         self._shapes = None
         self._stops_freq = None
         self._lines_freq = None
         self._segments = None
         self._segments_freq = None
         self._speeds = None
         self._avg_speeds = None
-        
-    
+        self._dates_service_id = None
+
     @property
     def gtfs_path(self):
         return self._gtfs_path
     
     @property
     def time_windows(self):
         return self._time_windows
@@ -69,14 +77,24 @@
     def files(self):
         if self._files is None:
             self._files = self.get_files()
     
         return self._files
 
     @property
+    def bbox(self):
+        if self._bbox is None:
+            self._bbox = self.get_bbox()
+        return self._bbox
+
+    @property
+    def dates(self):
+        return self._dates
+
+    @property
     def routes_patterns(self):
         """
         Return the patterns of each route and the number of trips defined
         for each pattern.
         """
         if self._routes_patterns is None:
             (trips_patterns, routes_patterns) = self.get_routes_patterns(self.trips)
@@ -210,119 +228,329 @@
     @property
     def avg_speeds(self):
         if self._avg_speeds is None:
             self._avg_speeds = self.get_avg_speeds()
 
         return self._avg_speeds
     
+    @property
+    def dates_service_id(self):
+        if self._dates_service_id is None:
+            self._dates_service_id = self.get_dates_service_id()
+        return self._dates_service_id
+    
+    @trips.setter
+    def trips(self, value):
+        self._trips = value
+
+    @stop_times.setter
+    def stop_times(self, value):
+        self._stop_times = value
+
+    @stops.setter
+    def stops(self, value):
+        self._stops = value
+
+    @routes.setter
+    def routes(self, value):
+        self._routes = value
+
+    @dates_service_id.setter
+    def dates_service_id(self, value):
+        self._dates_service_id = value
 
     def get_files(self):
         try:
             with ZipFile(self.gtfs_path) as myzip:
                 return myzip.namelist()    
         # Try as a URL if the file is not in local
         except FileNotFoundError as e:
             
             r = requests.get(self.gtfs_path)
 
             with ZipFile(io.BytesIO(r.content)) as myzip:
                 return myzip.namelist()
 
-    
+    def get_bbox(self):
+        logging.info('Getting the bounding box.')
+        stops = extract_file('stops', self)
+
+        max_x = stops.stop_lon.max()
+        min_x = stops.stop_lon.min()
+        max_y = stops.stop_lat.max()
+        min_y = stops.stop_lat.min()
+
+        geo = {
+            'type': 'Polygon',
+            'coordinates': [
+                [
+                    [max_x, max_y],
+                    [max_x, min_y],
+                    [min_x, min_y],
+                    [min_x, max_y],
+                    [max_x, max_y]
+                ]
+            ]
+        }
+
+        return geo
+
+
     def get_routes_patterns(self, trips):
         """
         Compute the different patterns of each route.
         returns (trips_patterns, routes_patterns)
         """
         stop_times = self.stop_times
         logging.info('computing patterns')
-        trip_stops = stop_times.copy()
-
-        trip_stops = trip_stops[
-            ['route_id', 'direction_id', 'shape_id',
+        trip_stops = stop_times[
+            ['route_id', 'route_name', 'direction_id', 'shape_id',
              'trip_id', 'stop_id', 'stop_sequence']]
         trip_stops['zipped_stops'] = list(
             zip(trip_stops.stop_id, trip_stops.stop_sequence))
 
-        trip_stops_zipped = trip_stops.groupby(
-            ['trip_id'])['zipped_stops'].apply(list)
+        trip_stops_zipped = trip_stops.pivot_table(
+            'zipped_stops',
+            index=['trip_id', 'route_id', 'route_name', 'direction_id', 'shape_id'],
+            aggfunc=list
+        ).reset_index()
         
-        def sort_stops(x):
-            return sorted(x, key=lambda x: x[1])
-
-        trip_stops_zipped_sorted = trip_stops_zipped.apply(sort_stops)
-        trip_stops_zipped_sorted = trip_stops_zipped.apply(str)
-        # trip_stops_zipped_sorted = trip_stops_zipped.apply(str)
-        trips_with_stops = trips.merge(
-            trip_stops_zipped_sorted, on='trip_id')
+        trips_with_stops = trips.merge(trip_stops_zipped)
 
         def version_hash(x):
             hash = hashlib.sha1(f"{x.route_id}{x.direction_id}{str(x.zipped_stops)}".encode("UTF-8")).hexdigest()
             return hash[:18]
-        trips_with_stops['pattern'] = trips_with_stops.apply(
+
+        trips_with_stops['pattern_id'] = trips_with_stops.apply(
             version_hash, axis=1)
 
+        # Count number of trips per pattern to identify the main one
+        route_patterns = trips_with_stops.pivot_table(
+            'trip_id',
+            index=[
+                'route_id', 'route_name', 'pattern_id', 'direction_id',
+                'shape_id', trips_with_stops.zipped_stops.astype(str)
+            ], aggfunc='count').reset_index()
+
+        route_patterns = route_patterns\
+            .rename({'trip_id': 'cnt_trips'}, axis=1)\
+                .sort_values(
+                    by=['route_name', 'direction_id', 'cnt_trips'],
+                    ascending=[True, True, False]
+                ).reset_index(drop=True)
+        
+        # Add simple names to patterns: A, B, C, etc.
+        n_patterns = route_patterns.pivot_table('cnt_trips', index=['route_name', 'direction_id'], aggfunc='count').reset_index()
+        n_patterns['route_pattern'] = n_patterns.cnt_trips.apply(lambda row: tuple(np.arange(1, row+1)))
+        n_patterns = n_patterns.explode('route_pattern').reset_index(drop=True)
+        n_patterns['route_pattern'] = n_patterns.route_pattern.apply(num_to_letters)
+        n_patterns['pattern_name'] = n_patterns.route_name + ' - ' + n_patterns.direction_id.astype(int).astype(str) + ' - ' + n_patterns.route_pattern
+        n_patterns.sort_values(by=['route_name', 'direction_id', 'route_pattern'], inplace=True)
+
+        route_patterns = route_patterns.merge(
+            n_patterns[['route_pattern', 'pattern_name']],
+            right_index=True, left_index=True, how='left')
+        
+        # Bring the pattern names to trips
+        trips_with_stops = trips_with_stops.merge(
+            route_patterns[['pattern_id', 'route_pattern', 'pattern_name']],
+            how='left')
         trips_with_patterns = trips_with_stops[[
-            'trip_id', 'route_id', 'pattern', 'route_name',
+            'trip_id', 'route_id', 'pattern_id', 'route_pattern', 'pattern_name','route_name',
             'service_id', 'direction_id', 'shape_id']]
 
-        
-        route_patterns = trips_with_stops.groupby(
-            ['route_id', 'pattern', 'direction_id',
-             'shape_id', 'zipped_stops']).count()[['trip_id']]
-        route_patterns = route_patterns.rename(
-            {'trip_id': 'cnt_trips'}, axis=1).reset_index()
-
         return trips_with_patterns.copy(), route_patterns.copy()
 
     
     def get_busiest_service_id(self):
         """
         Returns the service_id with most trips as a string.
         """
         trips = extract_file('trips', self)
         return trips.pivot_table(
             'trip_id', index='service_id', aggfunc='count')\
                 .sort_values(by='trip_id', ascending=False).index[0]
 
 
+    def get_dates_service_id(self):
+        dates_service_id = self.parse_calendar()
+        return dates_service_id.groupby('date').service_id.apply(list)
+
+
     def get_agency(self):
         return extract_file('agency', self)
 
 
     def get_calendar(self):
         return extract_file('calendar', self)
 
 
     def get_calendar_dates(self):
         return extract_file('calendar_dates', self)
 
 
+    def parse_calendar(self):
+        calendar = self.calendar
+        calendar_dates = self.calendar_dates
+        busiest_date = self.busiest_date
+
+        # Parse dates
+        calendar['start_date_dt'] = calendar.start_date.astype(str).apply(pl.parse)
+        calendar['end_date_dt'] = calendar.end_date.astype(str).apply(pl.parse) 
+
+        # Get all dates for a given service_id
+        calendar['all_dates'] = calendar.apply(
+            lambda x: np.array([
+                d for d in pl.period(x.start_date_dt, x.end_date_dt).range('days')
+                ]), axis=1
+            )
+        
+        # Boolean variables for day types
+        cols = [
+            'monday', 'tuesday', 'wednesday', 'thursday', 'friday',
+            'saturday', 'sunday']
+        
+        vf = np.vectorize(bool)
+        calendar[cols] = vf(calendar[cols].values)
+
+        # Hash weekdays to make it faster
+        def get_hash_weekdays(row):
+            return {
+                i: v
+                for i, v in enumerate(row[cols].values[0])
+            }
+
+        hash_weekdays = calendar.groupby('service_id').apply(get_hash_weekdays)
+
+        # Filter dates depending on the days of the week
+        calendar['filtered_dates'] = calendar.apply(lambda row: row.all_dates[
+            [
+                hash_weekdays[row.service_id][d.weekday()]
+                for d in row.all_dates
+            ]], axis=1)
+        
+        # Explode filtered_dates
+        t = calendar[['service_id', 'filtered_dates']].explode('filtered_dates')
+        t['filtered_dates'] = t.filtered_dates.dt.date.astype(str)
+
+        t = t.groupby('filtered_dates').service_id.apply(list)
+
+        # Create dictionary with dates as keys and service_id as items
+        date_hash = t.apply(lambda x: dict(zip(x, [True] * len(x)))).to_dict()
+        
+        # --- Do the same for calendar_dates ---
+        calendar_dates['date_str'] = calendar_dates.date.astype(str).apply(pl.parse)\
+            .dt.date.astype(str)
+        
+        cdates_hash = calendar_dates[calendar_dates.exception_type==1].groupby('date_str')\
+            .service_id.apply(list)\
+            .apply(lambda x: dict(zip(x, [True] * len(x)))).to_dict()
+        
+        
+        # Were dates provided or we're looking for the busiest_date?
+        if busiest_date:
+            # We need to look for the busiest date.
+            # To do enable that we need to return the complete
+            # list of dates to `get_trips()`
+            # Get max date and min date
+            dates = list(date_hash.keys()) + list(cdates_hash.keys())
+        else:
+            dates = self.dates
+
+            # Check if the dates have service in the calendars
+            remove_dates = []
+            for i, d in enumerate(dates):
+                if (d not in date_hash) & (d not in cdates_hash):
+                    print(f'The date "{d}" does not have service in this feed and will be removed from the analysis.')
+                    remove_dates.append(d)
+
+            for d in remove_dates:
+                dates.remove(d)
+
+        # Create dataframe with the service_id that applies to each date        
+        aux = pd.concat([pd.DataFrame(date_hash), pd.DataFrame(cdates_hash)]).T.reset_index()
+        dates_service_id = pd.melt(aux, id_vars='index', value_vars=aux.columns)
+        dates_service_id.columns=['date', 'service_id', 'keep']
+        
+        return dates_service_id[~dates_service_id.keep.isnull()]
+
+
     def get_trips(self):
         routes = self.routes
+        dates = self.dates
 
         trips = extract_file('trips', self)
         trips['trip_id'] = trips.trip_id.astype(str)
         trips['route_id'] = trips.route_id.astype(str)
 
         if 'shape_id' in trips.columns:
             trips['shape_id'] = trips.shape_id.astype(str)
-        
+
+        # If we were asked to only fetch the busiest date
+        # if self.busiest_date:
+            # trips = trips[trips.service_id==self.busiest_service_id]
+
+        # If we're looking for the busiest date or a specific list of
+        # dates we need to parse de calendar
+        if (self.busiest_date) | (dates!=[]):
+            """
+            In the case we have three possibilites:
+            1. busiest_date=True & dates==[]: in this case the user looks for the 
+                busiest date in the entire feed
+            2. busiest_date=True & dates!=[]: in this case the user looks for the
+                busiest date within the date range provided.
+            3. busiest_daet=False & dates!=[]: in this case the user looks for the
+                entire feed within the date range provided and we don't need to change
+                the "dates" variable at all.
+            """
+            dates_service_id = self.parse_calendar()
+
+            # If busiest_date=True, we have to count the number of trips
+            if self.busiest_date:
+                # Trip per date
+                date_ntrips = trips.merge(dates_service_id).groupby(['date']).\
+                        trip_id.count().sort_values(ascending=False)
+                
+            # If we are looking for the busiest date within our date period,
+            # we only keep the dates in that period of time.
+            if (self.busiest_date) & (dates!=[]):
+                dates_service_id = dates_service_id[dates_service_id.date.isin(dates)]
+                date_ntrips = date_ntrips[date_ntrips.index.isin(dates)]
+            
+            # Now that we've considered both cases we can just filter 
+            # with the busiest_date of the "dates" that made it this far
+            if self.busiest_date:
+                # In that case, if "dates" is empty we need to find the busiest date
+                busiest_date = list(date_ntrips[date_ntrips==date_ntrips.max()].index)
+                max_trips = date_ntrips[date_ntrips==date_ntrips.max()].values[0]
+
+                logging.info(f'The busiest date/s of this feed or your selected date range is/are:  {busiest_date} with {max_trips} trips.')
+                logging.info('In that more than one busiest date was found, the first one will be considered.')
+                logging.info(f'In this case is {busiest_date[0]}.')
+
+                # We need "dates" to be a list
+                dates = busiest_date[:1]
+            
+            # Keep only the trips that are relevant to the use case
+            trips = trips.set_index('service_id').join(
+                dates_service_id[dates_service_id.date.isin(dates)]\
+                    .set_index('service_id'),
+                how='inner'
+            ).reset_index(names='service_id').drop(['keep', 'date'], axis=1).drop_duplicates()
+
         # Get routes info in trips
         # The GTFS feed might be missing some of the keys, e.g. direction_id or shape_id.
         # To allow processing incomplete GTFS data, we must reindex instead:
         # https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#deprecate-loc-reindex-listlike
         # This will add NaN for any missing columns.
         cols = ['trip_id', 'route_id', 'route_name', 'service_id', 'direction_id', 'shape_id']
         trips = add_route_name(trips, routes).reindex(columns=cols)
         
-        # trips = trips[cols]    
-        # If we were asked to only fetch the busiest date
-        if self.busiest_date:
-            trips = trips[trips.service_id==self.busiest_service_id]
+        # Fill null values
+        trips['direction_id'] = trips.direction_id.fillna(0)
 
         return trips
 
 
     def get_routes(self):
         routes = extract_file('routes', self)
         routes['route_id'] = routes.route_id.astype(str)
@@ -350,25 +578,24 @@
         stops['stop_id'] = stops.stop_id.astype(str)
         stops['stop_name'] = stops.stop_name.astype(str)
 
         return stops
 
 
     def get_stop_times(self):
+        # Get trips, routes and stops info in stop_times
+        stop_times = extract_file('stop_times', self)
         if self._trips is not None: # prevents infinite loop
             logging.info('_trips is defined in stop_times')
             trips = self._trips
         else:
             logging.info('get trips in stop_times')
             trips = self.trips
         stops = self.stops
 
-        # Get trips, routes and stops info in stop_times
-        stop_times = extract_file('stop_times', self)
-        
         # Fix data types
         stop_times['trip_id'] = stop_times.trip_id.astype(str)
         stop_times['stop_id'] = stop_times.stop_id.astype(str)
         
         if 'route_id' in stop_times.columns:
             stop_times['route_id'] = stop_times.route_id.astype(str)
```

### Comparing `gtfs_functions-2.0.4/gtfs_functions/gtfs_plots.py` & `gtfs_functions-2.0.5/gtfs_functions/gtfs_plots.py`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/images/bus_segments.jpg` & `gtfs_functions-2.0.5/images/bus_segments.jpg`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/images/fancy_speed_per_hour.jpg` & `gtfs_functions-2.0.5/images/fancy_speed_per_hour.jpg`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/images/heatmap.jpg` & `gtfs_functions-2.0.5/images/heatmap.jpg`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/images/histogram.jpg` & `gtfs_functions-2.0.5/images/histogram.jpg`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/images/kepler_seg_freq.jpg` & `gtfs_functions-2.0.5/images/kepler_seg_freq.jpg`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/images/kepler_speeds.jpg` & `gtfs_functions-2.0.5/images/kepler_speeds.jpg`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/images/line_frequencies.jpg` & `gtfs_functions-2.0.5/images/line_frequencies.jpg`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/images/map_line_freq.jpg` & `gtfs_functions-2.0.5/images/map_line_freq.jpg`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/images/map_stop_freq.jpg` & `gtfs_functions-2.0.5/images/map_stop_freq.jpg`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/images/routes.jpg` & `gtfs_functions-2.0.5/images/routes.jpg`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/images/shapes.jpg` & `gtfs_functions-2.0.5/images/shapes.jpg`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/images/speed_hour.jpg` & `gtfs_functions-2.0.5/images/speed_hour.jpg`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/images/stop_times.jpg` & `gtfs_functions-2.0.5/images/stop_times.jpg`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/images/stops.jpg` & `gtfs_functions-2.0.5/images/stops.jpg`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/images/stops_freq_output.jpg` & `gtfs_functions-2.0.5/images/stops_freq_output.jpg`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/images/trips.jpg` & `gtfs_functions-2.0.5/images/trips.jpg`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/LICENSE.txt` & `gtfs_functions-2.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gtfs_functions-2.0.4/README.md` & `gtfs_functions-2.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # GTFS functions
 
 This package allows you to create various layers directly from the GTFS and visualize the results in the most straightforward way possible.
 
+## Update August 2023:
+* Possibility to parse the GTFS for a specific date.
+`feed = Feed(gtfs_path, dates=['2023-03-31, 2023-04-01])`
+
 ## Update March 2023:
 * Removed dependency with [partridge](https://github.com/remix/partridge). As much as we love this package and think it is absolutely great, removing a dependency gives us more control and keeps this package from failing whenever something changes in `partridge`.
 * We treat the GTFS as a class, where each file is a property. See examples below to find out how to work with it. We hope this simplifies your code.
 * Fixed and enhanced **segment cutting**. Shout out to [Mattijs De Paepe](https://github.com/mattijsdp)
 * Support to identify route patterns!! Check it out using `feed.routes_patterns`. Shout out to [Tobias Bartsch](https://github.com/tobiasbartsch)
 * The rest should stay the same.
```

### Comparing `gtfs_functions-2.0.4/pyproject.toml` & `gtfs_functions-2.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gtfs-functions"
-version = "2.0.4"
+version = "2.0.5"
 authors = [
   { name="Santiago Toso", email="santiagoa.toso@gmail.com" },
 ]
 description = "Package to easily wrangle GTFS files geospatially."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `gtfs_functions-2.0.4/PKG-INFO` & `gtfs_functions-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtfs-functions
-Version: 2.0.4
+Version: 2.0.5
 Summary: Package to easily wrangle GTFS files geospatially.
 Project-URL: Homepage, https://github.com/Bondify/gtfs_functions/tree/master
 Project-URL: Bug Tracker, https://github.com/Bondify/gtfs_functions/issues
 Author-email: Santiago Toso <santiagoa.toso@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,18 @@
 Requires-Dist: utm>=0.7.0
 Description-Content-Type: text/markdown
 
 # GTFS functions
 
 This package allows you to create various layers directly from the GTFS and visualize the results in the most straightforward way possible.
 
+## Update August 2023:
+* Possibility to parse the GTFS for a specific date.
+`feed = Feed(gtfs_path, dates=['2023-03-31, 2023-04-01])`
+
 ## Update March 2023:
 * Removed dependency with [partridge](https://github.com/remix/partridge). As much as we love this package and think it is absolutely great, removing a dependency gives us more control and keeps this package from failing whenever something changes in `partridge`.
 * We treat the GTFS as a class, where each file is a property. See examples below to find out how to work with it. We hope this simplifies your code.
 * Fixed and enhanced **segment cutting**. Shout out to [Mattijs De Paepe](https://github.com/mattijsdp)
 * Support to identify route patterns!! Check it out using `feed.routes_patterns`. Shout out to [Tobias Bartsch](https://github.com/tobiasbartsch)
 * The rest should stay the same.
```

