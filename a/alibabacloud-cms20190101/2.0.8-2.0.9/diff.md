# Comparing `tmp/alibabacloud_cms20190101-2.0.8.tar.gz` & `tmp/alibabacloud_cms20190101-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cms20190101-2.0.8.tar", last modified: Fri Jul 28 05:32:44 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cms20190101-2.0.9.tar", last modified: Tue Aug  8 01:38:13 2023, max compression
```

## Comparing `alibabacloud_cms20190101-2.0.8.tar` & `alibabacloud_cms20190101-2.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/
--rw-r--r--   0 root         (0) root         (0)      508 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2338 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   668027 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101/client.py
--rw-r--r--   0 root         (0) root         (0)  1808781 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2338 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2621 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 01:38:13.000000 alibabacloud_cms20190101-2.0.9/
+-rw-r--r--   0 root         (0) root         (0)      565 2023-08-08 01:38:12.000000 alibabacloud_cms20190101-2.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-08 01:38:12.000000 alibabacloud_cms20190101-2.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-08 01:38:12.000000 alibabacloud_cms20190101-2.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2338 2023-08-08 01:38:13.000000 alibabacloud_cms20190101-2.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-08-08 01:38:12.000000 alibabacloud_cms20190101-2.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-08-08 01:38:12.000000 alibabacloud_cms20190101-2.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 01:38:13.000000 alibabacloud_cms20190101-2.0.9/alibabacloud_cms20190101/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-08 01:38:12.000000 alibabacloud_cms20190101-2.0.9/alibabacloud_cms20190101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   668519 2023-08-08 01:38:12.000000 alibabacloud_cms20190101-2.0.9/alibabacloud_cms20190101/client.py
+-rw-r--r--   0 root         (0) root         (0)  1812113 2023-08-08 01:38:12.000000 alibabacloud_cms20190101-2.0.9/alibabacloud_cms20190101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 01:38:13.000000 alibabacloud_cms20190101-2.0.9/alibabacloud_cms20190101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2338 2023-08-08 01:38:12.000000 alibabacloud_cms20190101-2.0.9/alibabacloud_cms20190101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-08-08 01:38:12.000000 alibabacloud_cms20190101-2.0.9/alibabacloud_cms20190101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 01:38:12.000000 alibabacloud_cms20190101-2.0.9/alibabacloud_cms20190101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-08 01:38:12.000000 alibabacloud_cms20190101-2.0.9/alibabacloud_cms20190101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-08-08 01:38:12.000000 alibabacloud_cms20190101-2.0.9/alibabacloud_cms20190101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-08 01:38:13.000000 alibabacloud_cms20190101-2.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2621 2023-08-08 01:38:12.000000 alibabacloud_cms20190101-2.0.9/setup.py
```

### Comparing `alibabacloud_cms20190101-2.0.8/LICENSE` & `alibabacloud_cms20190101-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cms20190101-2.0.8/PKG-INFO` & `alibabacloud_cms20190101-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cms20190101
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud Cloud Monitor (20190101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cms20190101-2.0.8/README-CN.md` & `alibabacloud_cms20190101-2.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cms20190101-2.0.8/README.md` & `alibabacloud_cms20190101-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101/client.py` & `alibabacloud_cms20190101-2.0.9/alibabacloud_cms20190101/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2703,14 +2703,16 @@
         """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.address):
             query['Address'] = request.address
         if not UtilClient.is_unset(request.alert_ids):
             query['AlertIds'] = request.alert_ids
+        if not UtilClient.is_unset(request.custom_schedule):
+            query['CustomSchedule'] = request.custom_schedule
         if not UtilClient.is_unset(request.interval):
             query['Interval'] = request.interval
         if not UtilClient.is_unset(request.isp_cities):
             query['IspCities'] = request.isp_cities
         if not UtilClient.is_unset(request.options_json):
             query['OptionsJson'] = request.options_json
         if not UtilClient.is_unset(request.task_name):
@@ -2752,14 +2754,16 @@
         """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.address):
             query['Address'] = request.address
         if not UtilClient.is_unset(request.alert_ids):
             query['AlertIds'] = request.alert_ids
+        if not UtilClient.is_unset(request.custom_schedule):
+            query['CustomSchedule'] = request.custom_schedule
         if not UtilClient.is_unset(request.interval):
             query['Interval'] = request.interval
         if not UtilClient.is_unset(request.isp_cities):
             query['IspCities'] = request.isp_cities
         if not UtilClient.is_unset(request.options_json):
             query['OptionsJson'] = request.options_json
         if not UtilClient.is_unset(request.task_name):
@@ -13639,14 +13643,16 @@
         """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.address):
             query['Address'] = request.address
         if not UtilClient.is_unset(request.alert_ids):
             query['AlertIds'] = request.alert_ids
+        if not UtilClient.is_unset(request.custom_schedule):
+            query['CustomSchedule'] = request.custom_schedule
         if not UtilClient.is_unset(request.interval):
             query['Interval'] = request.interval
         if not UtilClient.is_unset(request.interval_unit):
             query['IntervalUnit'] = request.interval_unit
         if not UtilClient.is_unset(request.isp_cities):
             query['IspCities'] = request.isp_cities
         if not UtilClient.is_unset(request.options_json):
@@ -13688,14 +13694,16 @@
         """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.address):
             query['Address'] = request.address
         if not UtilClient.is_unset(request.alert_ids):
             query['AlertIds'] = request.alert_ids
+        if not UtilClient.is_unset(request.custom_schedule):
+            query['CustomSchedule'] = request.custom_schedule
         if not UtilClient.is_unset(request.interval):
             query['Interval'] = request.interval
         if not UtilClient.is_unset(request.interval_unit):
             query['IntervalUnit'] = request.interval_unit
         if not UtilClient.is_unset(request.isp_cities):
             query['IspCities'] = request.isp_cities
         if not UtilClient.is_unset(request.options_json):
```

### Comparing `alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101/models.py` & `alibabacloud_cms20190101-2.0.9/alibabacloud_cms20190101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7946,14 +7946,15 @@
 
 
 class CreateSiteMonitorRequest(TeaModel):
     def __init__(
         self,
         address: str = None,
         alert_ids: str = None,
+        custom_schedule: str = None,
         interval: str = None,
         isp_cities: str = None,
         options_json: str = None,
         region_id: str = None,
         task_name: str = None,
         task_type: str = None,
     ):
@@ -7962,14 +7963,15 @@
         # The name must be 4 to 100 characters in length, and can contain letters, digits, and underscores (\_).
         self.address = address
         # Indicates whether the existing alert rule was associated with the site monitoring task. Valid values:
         # 
         # *   true
         # *   false
         self.alert_ids = alert_ids
+        self.custom_schedule = custom_schedule
         # The operation that you want to perform. Set the value to **CreateSiteMonitor**.
         self.interval = interval
         # The information of the detection points. If you leave this parameter empty, the system randomly selects three detection points.
         # 
         # The value is a JSON array. Example: `[{"city":"546","isp":"465"},{"city":"572","isp":"465"},{"city":"738","isp":"465"}]`. The values of the city field indicate Beijing, Hangzhou, and Qingdao.
         # 
         # For information about how to obtain detection points, see [DescribeSiteMonitorISPCityList](~~115045~~).
@@ -7995,14 +7997,16 @@
             return _map
 
         result = dict()
         if self.address is not None:
             result['Address'] = self.address
         if self.alert_ids is not None:
             result['AlertIds'] = self.alert_ids
+        if self.custom_schedule is not None:
+            result['CustomSchedule'] = self.custom_schedule
         if self.interval is not None:
             result['Interval'] = self.interval
         if self.isp_cities is not None:
             result['IspCities'] = self.isp_cities
         if self.options_json is not None:
             result['OptionsJson'] = self.options_json
         if self.region_id is not None:
@@ -8015,14 +8019,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Address') is not None:
             self.address = m.get('Address')
         if m.get('AlertIds') is not None:
             self.alert_ids = m.get('AlertIds')
+        if m.get('CustomSchedule') is not None:
+            self.custom_schedule = m.get('CustomSchedule')
         if m.get('Interval') is not None:
             self.interval = m.get('Interval')
         if m.get('IspCities') is not None:
             self.isp_cities = m.get('IspCities')
         if m.get('OptionsJson') is not None:
             self.options_json = m.get('OptionsJson')
         if m.get('RegionId') is not None:
@@ -34075,14 +34081,88 @@
         if m.get('MetricRule') is not None:
             for k in m.get('MetricRule'):
                 temp_model = DescribeSiteMonitorAttributeResponseBodyMetricRulesMetricRule()
                 self.metric_rule.append(temp_model.from_map(k))
         return self
 
 
+class DescribeSiteMonitorAttributeResponseBodySiteMonitorsCustomScheduleDays(TeaModel):
+    def __init__(
+        self,
+        days: List[int] = None,
+    ):
+        self.days = days
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.days is not None:
+            result['days'] = self.days
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('days') is not None:
+            self.days = m.get('days')
+        return self
+
+
+class DescribeSiteMonitorAttributeResponseBodySiteMonitorsCustomSchedule(TeaModel):
+    def __init__(
+        self,
+        days: DescribeSiteMonitorAttributeResponseBodySiteMonitorsCustomScheduleDays = None,
+        end_hour: int = None,
+        start_hour: int = None,
+        time_zone: str = None,
+    ):
+        self.days = days
+        self.end_hour = end_hour
+        self.start_hour = start_hour
+        self.time_zone = time_zone
+
+    def validate(self):
+        if self.days:
+            self.days.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.days is not None:
+            result['days'] = self.days.to_map()
+        if self.end_hour is not None:
+            result['end_hour'] = self.end_hour
+        if self.start_hour is not None:
+            result['start_hour'] = self.start_hour
+        if self.time_zone is not None:
+            result['time_zone'] = self.time_zone
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('days') is not None:
+            temp_model = DescribeSiteMonitorAttributeResponseBodySiteMonitorsCustomScheduleDays()
+            self.days = temp_model.from_map(m['days'])
+        if m.get('end_hour') is not None:
+            self.end_hour = m.get('end_hour')
+        if m.get('start_hour') is not None:
+            self.start_hour = m.get('start_hour')
+        if m.get('time_zone') is not None:
+            self.time_zone = m.get('time_zone')
+        return self
+
+
 class DescribeSiteMonitorAttributeResponseBodySiteMonitorsIspCitiesIspCity(TeaModel):
     def __init__(
         self,
         city: str = None,
         city_name: str = None,
         isp: str = None,
         isp_name: str = None,
@@ -34435,25 +34515,27 @@
 
 
 class DescribeSiteMonitorAttributeResponseBodySiteMonitors(TeaModel):
     def __init__(
         self,
         address: str = None,
         agent_group: str = None,
+        custom_schedule: DescribeSiteMonitorAttributeResponseBodySiteMonitorsCustomSchedule = None,
         interval: str = None,
         isp_cities: DescribeSiteMonitorAttributeResponseBodySiteMonitorsIspCities = None,
         option_json: DescribeSiteMonitorAttributeResponseBodySiteMonitorsOptionJson = None,
         task_id: str = None,
         task_name: str = None,
         task_state: str = None,
         task_type: str = None,
     ):
         # The information of detection points. The information includes the carriers that provide the detection points and the cities where the detection points reside.
         self.address = address
         self.agent_group = agent_group
+        self.custom_schedule = custom_schedule
         # The name of the site monitoring task.
         self.interval = interval
         # The name of the carrier.
         self.isp_cities = isp_cities
         self.option_json = option_json
         # The ID of the city.
         self.task_id = task_id
@@ -34464,14 +34546,16 @@
         # The status of the site monitoring task. Valid values:
         # 
         # *   1: The task is enabled.
         # *   2: The task is disabled.
         self.task_type = task_type
 
     def validate(self):
+        if self.custom_schedule:
+            self.custom_schedule.validate()
         if self.isp_cities:
             self.isp_cities.validate()
         if self.option_json:
             self.option_json.validate()
 
     def to_map(self):
         _map = super().to_map()
@@ -34479,14 +34563,16 @@
             return _map
 
         result = dict()
         if self.address is not None:
             result['Address'] = self.address
         if self.agent_group is not None:
             result['AgentGroup'] = self.agent_group
+        if self.custom_schedule is not None:
+            result['CustomSchedule'] = self.custom_schedule.to_map()
         if self.interval is not None:
             result['Interval'] = self.interval
         if self.isp_cities is not None:
             result['IspCities'] = self.isp_cities.to_map()
         if self.option_json is not None:
             result['OptionJson'] = self.option_json.to_map()
         if self.task_id is not None:
@@ -34501,14 +34587,17 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Address') is not None:
             self.address = m.get('Address')
         if m.get('AgentGroup') is not None:
             self.agent_group = m.get('AgentGroup')
+        if m.get('CustomSchedule') is not None:
+            temp_model = DescribeSiteMonitorAttributeResponseBodySiteMonitorsCustomSchedule()
+            self.custom_schedule = temp_model.from_map(m['CustomSchedule'])
         if m.get('Interval') is not None:
             self.interval = m.get('Interval')
         if m.get('IspCities') is not None:
             temp_model = DescribeSiteMonitorAttributeResponseBodySiteMonitorsIspCities()
             self.isp_cities = temp_model.from_map(m['IspCities'])
         if m.get('OptionJson') is not None:
             temp_model = DescribeSiteMonitorAttributeResponseBodySiteMonitorsOptionJson()
@@ -43100,26 +43189,28 @@
 
 
 class ModifySiteMonitorRequest(TeaModel):
     def __init__(
         self,
         address: str = None,
         alert_ids: str = None,
+        custom_schedule: str = None,
         interval: str = None,
         interval_unit: str = None,
         isp_cities: str = None,
         options_json: str = None,
         region_id: str = None,
         task_id: str = None,
         task_name: str = None,
     ):
         # The ID of the site monitoring task.
         self.address = address
         # The returned message.
         self.alert_ids = alert_ids
+        self.custom_schedule = custom_schedule
         # The HTTP status code.
         # 
         # >  The status code 200 indicates that the call was successful.
         self.interval = interval
         # The extended options of the protocol that is used by the site monitoring task. The options vary based on the protocol.
         self.interval_unit = interval_unit
         # The operation that you want to perform. Set the value to ModifySiteMonitor.
@@ -43143,14 +43234,16 @@
             return _map
 
         result = dict()
         if self.address is not None:
             result['Address'] = self.address
         if self.alert_ids is not None:
             result['AlertIds'] = self.alert_ids
+        if self.custom_schedule is not None:
+            result['CustomSchedule'] = self.custom_schedule
         if self.interval is not None:
             result['Interval'] = self.interval
         if self.interval_unit is not None:
             result['IntervalUnit'] = self.interval_unit
         if self.isp_cities is not None:
             result['IspCities'] = self.isp_cities
         if self.options_json is not None:
@@ -43165,14 +43258,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Address') is not None:
             self.address = m.get('Address')
         if m.get('AlertIds') is not None:
             self.alert_ids = m.get('AlertIds')
+        if m.get('CustomSchedule') is not None:
+            self.custom_schedule = m.get('CustomSchedule')
         if m.get('Interval') is not None:
             self.interval = m.get('Interval')
         if m.get('IntervalUnit') is not None:
             self.interval_unit = m.get('IntervalUnit')
         if m.get('IspCities') is not None:
             self.isp_cities = m.get('IspCities')
         if m.get('OptionsJson') is not None:
```

### Comparing `alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101.egg-info/PKG-INFO` & `alibabacloud_cms20190101-2.0.9/alibabacloud_cms20190101.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cms20190101
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud Cloud Monitor (20190101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cms20190101-2.0.8/setup.py` & `alibabacloud_cms20190101-2.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cms20190101.
 
-Created on 28/07/2023
+Created on 08/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cms20190101"
 NAME = "alibabacloud_cms20190101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Cloud Monitor (20190101) SDK Library for Python"
```

