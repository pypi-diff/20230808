# Comparing `tmp/alibabacloud_cms20190101_py2-1.0.2.tar.gz` & `tmp/alibabacloud_cms20190101_py2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cms20190101_py2-1.0.2.tar", last modified: Fri Jul 28 05:32:56 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cms20190101_py2-1.0.3.tar", last modified: Tue Aug  8 01:35:53 2023, max compression
```

## Comparing `alibabacloud_cms20190101_py2-1.0.2.tar` & `alibabacloud_cms20190101_py2-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2482 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   282025 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101/client.py
--rw-r--r--   0 root         (0) root         (0)  1828595 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2482 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2913 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      163 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/alibabacloud_cms20190101/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/alibabacloud_cms20190101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   282271 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/alibabacloud_cms20190101/client.py
+-rw-r--r--   0 root         (0) root         (0)  1832013 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/alibabacloud_cms20190101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/alibabacloud_cms20190101_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/alibabacloud_cms20190101_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/alibabacloud_cms20190101_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/alibabacloud_cms20190101_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/alibabacloud_cms20190101_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/alibabacloud_cms20190101_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2913 2023-08-08 01:35:53.000000 alibabacloud_cms20190101_py2-1.0.3/setup.py
```

### Comparing `alibabacloud_cms20190101_py2-1.0.2/LICENSE` & `alibabacloud_cms20190101_py2-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cms20190101_py2-1.0.2/PKG-INFO` & `alibabacloud_cms20190101_py2-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cms20190101_py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud Cloud Monitor (20190101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cms20190101_py2-1.0.2/README-CN.md` & `alibabacloud_cms20190101_py2-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cms20190101_py2-1.0.2/README.md` & `alibabacloud_cms20190101_py2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101/client.py` & `alibabacloud_cms20190101_py2-1.0.3/alibabacloud_cms20190101/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1273,14 +1273,16 @@
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
@@ -6151,14 +6153,16 @@
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

### Comparing `alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101/models.py` & `alibabacloud_cms20190101_py2-1.0.3/alibabacloud_cms20190101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7043,25 +7043,26 @@
         if m.get('body') is not None:
             temp_model = CreateMonitoringAgentProcessResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateSiteMonitorRequest(TeaModel):
-    def __init__(self, address=None, alert_ids=None, interval=None, isp_cities=None, options_json=None,
-                 region_id=None, task_name=None, task_type=None):
+    def __init__(self, address=None, alert_ids=None, custom_schedule=None, interval=None, isp_cities=None,
+                 options_json=None, region_id=None, task_name=None, task_type=None):
         # The name of the site monitoring task.
         # 
         # The name must be 4 to 100 characters in length, and can contain letters, digits, and underscores (\_).
         self.address = address  # type: str
         # Indicates whether the existing alert rule was associated with the site monitoring task. Valid values:
         # 
         # *   true
         # *   false
         self.alert_ids = alert_ids  # type: str
+        self.custom_schedule = custom_schedule  # type: str
         # The operation that you want to perform. Set the value to **CreateSiteMonitor**.
         self.interval = interval  # type: str
         # The information of the detection points. If you leave this parameter empty, the system randomly selects three detection points.
         # 
         # The value is a JSON array. Example: `[{"city":"546","isp":"465"},{"city":"572","isp":"465"},{"city":"738","isp":"465"}]`. The values of the city field indicate Beijing, Hangzhou, and Qingdao.
         # 
         # For information about how to obtain detection points, see [DescribeSiteMonitorISPCityList](~~115045~~).
@@ -7087,14 +7088,16 @@
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
@@ -7107,14 +7110,16 @@
 
     def from_map(self, m=None):
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
@@ -30387,14 +30392,79 @@
         if m.get('MetricRule') is not None:
             for k in m.get('MetricRule'):
                 temp_model = DescribeSiteMonitorAttributeResponseBodyMetricRulesMetricRule()
                 self.metric_rule.append(temp_model.from_map(k))
         return self
 
 
+class DescribeSiteMonitorAttributeResponseBodySiteMonitorsCustomScheduleDays(TeaModel):
+    def __init__(self, days=None):
+        self.days = days  # type: list[int]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeSiteMonitorAttributeResponseBodySiteMonitorsCustomScheduleDays, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.days is not None:
+            result['days'] = self.days
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('days') is not None:
+            self.days = m.get('days')
+        return self
+
+
+class DescribeSiteMonitorAttributeResponseBodySiteMonitorsCustomSchedule(TeaModel):
+    def __init__(self, days=None, end_hour=None, start_hour=None, time_zone=None):
+        self.days = days  # type: DescribeSiteMonitorAttributeResponseBodySiteMonitorsCustomScheduleDays
+        self.end_hour = end_hour  # type: int
+        self.start_hour = start_hour  # type: int
+        self.time_zone = time_zone  # type: str
+
+    def validate(self):
+        if self.days:
+            self.days.validate()
+
+    def to_map(self):
+        _map = super(DescribeSiteMonitorAttributeResponseBodySiteMonitorsCustomSchedule, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, city=None, city_name=None, isp=None, isp_name=None):
         # The ID of the carrier.
         self.city = city  # type: str
         # The name of the metric.
         self.city_name = city_name  # type: str
         # The information of the alert rules that are configured for the site monitoring task.
@@ -30699,19 +30769,20 @@
             self.time_out = m.get('time_out')
         if m.get('username') is not None:
             self.username = m.get('username')
         return self
 
 
 class DescribeSiteMonitorAttributeResponseBodySiteMonitors(TeaModel):
-    def __init__(self, address=None, agent_group=None, interval=None, isp_cities=None, option_json=None,
-                 task_id=None, task_name=None, task_state=None, task_type=None):
+    def __init__(self, address=None, agent_group=None, custom_schedule=None, interval=None, isp_cities=None,
+                 option_json=None, task_id=None, task_name=None, task_state=None, task_type=None):
         # The information of detection points. The information includes the carriers that provide the detection points and the cities where the detection points reside.
         self.address = address  # type: str
         self.agent_group = agent_group  # type: str
+        self.custom_schedule = custom_schedule  # type: DescribeSiteMonitorAttributeResponseBodySiteMonitorsCustomSchedule
         # The name of the site monitoring task.
         self.interval = interval  # type: str
         # The name of the carrier.
         self.isp_cities = isp_cities  # type: DescribeSiteMonitorAttributeResponseBodySiteMonitorsIspCities
         self.option_json = option_json  # type: DescribeSiteMonitorAttributeResponseBodySiteMonitorsOptionJson
         # The ID of the city.
         self.task_id = task_id  # type: str
@@ -30722,14 +30793,16 @@
         # The status of the site monitoring task. Valid values:
         # 
         # *   1: The task is enabled.
         # *   2: The task is disabled.
         self.task_type = task_type  # type: str
 
     def validate(self):
+        if self.custom_schedule:
+            self.custom_schedule.validate()
         if self.isp_cities:
             self.isp_cities.validate()
         if self.option_json:
             self.option_json.validate()
 
     def to_map(self):
         _map = super(DescribeSiteMonitorAttributeResponseBodySiteMonitors, self).to_map()
@@ -30737,14 +30810,16 @@
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
@@ -30759,14 +30834,17 @@
 
     def from_map(self, m=None):
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
@@ -38430,20 +38508,21 @@
         if m.get('body') is not None:
             temp_model = ModifyMonitorGroupInstancesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifySiteMonitorRequest(TeaModel):
-    def __init__(self, address=None, alert_ids=None, interval=None, interval_unit=None, isp_cities=None,
-                 options_json=None, region_id=None, task_id=None, task_name=None):
+    def __init__(self, address=None, alert_ids=None, custom_schedule=None, interval=None, interval_unit=None,
+                 isp_cities=None, options_json=None, region_id=None, task_id=None, task_name=None):
         # The ID of the site monitoring task.
         self.address = address  # type: str
         # The returned message.
         self.alert_ids = alert_ids  # type: str
+        self.custom_schedule = custom_schedule  # type: str
         # The HTTP status code.
         # 
         # >  The status code 200 indicates that the call was successful.
         self.interval = interval  # type: str
         # The extended options of the protocol that is used by the site monitoring task. The options vary based on the protocol.
         self.interval_unit = interval_unit  # type: str
         # The operation that you want to perform. Set the value to ModifySiteMonitor.
@@ -38467,14 +38546,16 @@
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
@@ -38489,14 +38570,16 @@
 
     def from_map(self, m=None):
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

### Comparing `alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101_py2.egg-info/PKG-INFO` & `alibabacloud_cms20190101_py2-1.0.3/alibabacloud_cms20190101_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cms20190101-py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud Cloud Monitor (20190101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cms20190101_py2-1.0.2/setup.py` & `alibabacloud_cms20190101_py2-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cms20190101_py2.
 
-Created on 28/07/2023
+Created on 08/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cms20190101"
 NAME = "alibabacloud_cms20190101_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Cloud Monitor (20190101) SDK Library for Python2"
```

