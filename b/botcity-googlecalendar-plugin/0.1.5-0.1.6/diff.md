# Comparing `tmp/botcity-googlecalendar-plugin-0.1.5.tar.gz` & `tmp/botcity-googlecalendar-plugin-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/bot-googlecalendar-plugin/bot-googlecalendar-plugin/dist/.tmp-ldbyvyfl/botcity-googlecalendar-plugin-0.1.5.ta", last modified: Wed Feb  8 12:54:53 2023, max compression
+gzip compressed data, was "/home/runner/work/bot-googlecalendar-plugin/bot-googlecalendar-plugin/dist/.tmp-6pif4vjt/botcity-googlecalendar-plugin-0.1.6.ta", last modified: Tue Aug  8 14:12:27 2023, max compression
```

## Comparing `botcity-googlecalendar-plugin-0.1.5.tar` & `botcity-googlecalendar-plugin-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 12:54:53.000000 botcity-googlecalendar-plugin-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-08 12:54:40.000000 botcity-googlecalendar-plugin-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-02-08 12:54:53.000000 botcity-googlecalendar-plugin-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-02-08 12:54:40.000000 botcity-googlecalendar-plugin-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 12:54:53.000000 botcity-googlecalendar-plugin-0.1.5/botcity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 12:54:53.000000 botcity-googlecalendar-plugin-0.1.5/botcity/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 12:54:53.000000 botcity-googlecalendar-plugin-0.1.5/botcity/plugins/googlecalendar/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-08 12:54:40.000000 botcity-googlecalendar-plugin-0.1.5/botcity/plugins/googlecalendar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-08 12:54:53.000000 botcity-googlecalendar-plugin-0.1.5/botcity/plugins/googlecalendar/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-02-08 12:54:40.000000 botcity-googlecalendar-plugin-0.1.5/botcity/plugins/googlecalendar/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 12:54:53.000000 botcity-googlecalendar-plugin-0.1.5/botcity_googlecalendar_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-02-08 12:54:53.000000 botcity-googlecalendar-plugin-0.1.5/botcity_googlecalendar_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-02-08 12:54:53.000000 botcity-googlecalendar-plugin-0.1.5/botcity_googlecalendar_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 12:54:53.000000 botcity-googlecalendar-plugin-0.1.5/botcity_googlecalendar_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-08 12:54:53.000000 botcity-googlecalendar-plugin-0.1.5/botcity_googlecalendar_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-08 12:54:53.000000 botcity-googlecalendar-plugin-0.1.5/botcity_googlecalendar_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-08 12:54:40.000000 botcity-googlecalendar-plugin-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-08 12:54:53.000000 botcity-googlecalendar-plugin-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-08 12:54:40.000000 botcity-googlecalendar-plugin-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 12:54:53.000000 botcity-googlecalendar-plugin-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-08 12:54:40.000000 botcity-googlecalendar-plugin-0.1.5/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-02-08 12:54:40.000000 botcity-googlecalendar-plugin-0.1.5/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-02-08 12:54:40.000000 botcity-googlecalendar-plugin-0.1.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:12:27.000000 botcity-googlecalendar-plugin-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 14:12:13.000000 botcity-googlecalendar-plugin-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-08-08 14:12:27.000000 botcity-googlecalendar-plugin-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-08-08 14:12:13.000000 botcity-googlecalendar-plugin-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:12:27.000000 botcity-googlecalendar-plugin-0.1.6/botcity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:12:27.000000 botcity-googlecalendar-plugin-0.1.6/botcity/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:12:27.000000 botcity-googlecalendar-plugin-0.1.6/botcity/plugins/googlecalendar/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-08 14:12:13.000000 botcity-googlecalendar-plugin-0.1.6/botcity/plugins/googlecalendar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-08 14:12:27.000000 botcity-googlecalendar-plugin-0.1.6/botcity/plugins/googlecalendar/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-08-08 14:12:13.000000 botcity-googlecalendar-plugin-0.1.6/botcity/plugins/googlecalendar/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:12:27.000000 botcity-googlecalendar-plugin-0.1.6/botcity_googlecalendar_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-08-08 14:12:27.000000 botcity-googlecalendar-plugin-0.1.6/botcity_googlecalendar_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-08 14:12:27.000000 botcity-googlecalendar-plugin-0.1.6/botcity_googlecalendar_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:12:27.000000 botcity-googlecalendar-plugin-0.1.6/botcity_googlecalendar_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-08 14:12:27.000000 botcity-googlecalendar-plugin-0.1.6/botcity_googlecalendar_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 14:12:27.000000 botcity-googlecalendar-plugin-0.1.6/botcity_googlecalendar_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-08 14:12:13.000000 botcity-googlecalendar-plugin-0.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-08 14:12:27.000000 botcity-googlecalendar-plugin-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-08 14:12:13.000000 botcity-googlecalendar-plugin-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:12:27.000000 botcity-googlecalendar-plugin-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-08 14:12:13.000000 botcity-googlecalendar-plugin-0.1.6/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-08-08 14:12:13.000000 botcity-googlecalendar-plugin-0.1.6/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-08-08 14:12:13.000000 botcity-googlecalendar-plugin-0.1.6/versioneer.py
```

### Comparing `botcity-googlecalendar-plugin-0.1.5/PKG-INFO` & `botcity-googlecalendar-plugin-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botcity-googlecalendar-plugin
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://bitbucket.org/botcitydev/bot-googlecalendar-plugin-python.git
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # BotCity Google Calendar Plugin - Python
 
 ## 🤖 Computer-vision based UI Automation
```

### Comparing `botcity-googlecalendar-plugin-0.1.5/README.md` & `botcity-googlecalendar-plugin-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `botcity-googlecalendar-plugin-0.1.5/botcity/plugins/googlecalendar/plugin.py` & `botcity-googlecalendar-plugin-0.1.6/botcity/plugins/googlecalendar/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from datetime import datetime
 from enum import Enum
 from typing import List, Union
 
 from gcsa.calendar import Calendar
 from gcsa.event import Event
 from gcsa.google_calendar import GoogleCalendar
-# from gcsa.recurrence import *
-from gcsa.recurrence import (DAILY, FR, HOURLY, MO, MONTHLY, SA, SU, TH, TU,
-                             WE, WEEKLY, Recurrence)
+from gcsa.recurrence import (DAILY, FR, MO, MONTHLY, SA, SU, TH, TU, WE,
+                             WEEKLY, Recurrence)
+from google.auth.transport.requests import Request
 from google.oauth2.credentials import Credentials
+from google_auth_oauthlib.flow import InstalledAppFlow
 
 
 class EventRecurrence(Enum):
-    HOURLY = HOURLY
     DAILY = DAILY
     WEEKLY = WEEKLY
     MONTHLY = MONTHLY
 
 
 class EventDays(Enum):
     MONDAY = MO
@@ -26,108 +26,115 @@
     THURSDAY = TH
     FRIDAY = FR
     SATURDAY = SA
     SUNDAY = SU
 
 
 class BotGoogleCalendarPlugin:
-    def __init__(self, credentials_file_path: str, token_file_path: str, calendar: str = "primary") -> None:
+    def __init__(self, credentials_file_path: str, calendar: str = "primary") -> None:
         """
-        Init BotGoogleCalendarPlugin.
+        BotGoogleCalendarPlugin.
 
         Args:
             credentials_file_path (str): The path of the credentials json file obtained at Google Cloud Platform.
-            token_file_path (str): The path of the token json file.
-            calendar (str): The id of the calendar that will be used. Defaults to "primary".
+            calendar (str, optional): The id of the calendar that will be used. Defaults to "primary".
+                To see the id of a calendar, go to the Integrate Calendar tab in the calendar settings.
         """
+        creds = None
+        scopes = ['https://www.googleapis.com/auth/calendar']
+
+        # The file token_calendar.json stores the user's access and refresh tokens, and is
+        # created automatically when the authorization flow completes for the first
+        # time.
+        credentials_dir = os.path.abspath(os.path.dirname(credentials_file_path))
+
+        if os.path.exists(os.path.join(credentials_dir, 'token_calendar.json')):
+            creds = Credentials.from_authorized_user_file(
+                os.path.join(credentials_dir, 'token_calendar.json'), scopes)
+        # If there are no (valid) credentials available, let the user log in.
+        if not creds or not creds.valid:
+            if creds and creds.expired and creds.refresh_token:
+                creds.refresh(Request())
+            else:
+                flow = InstalledAppFlow.from_client_secrets_file(
+                    os.path.abspath(credentials_file_path), scopes)
+                creds = flow.run_local_server(port=0)
+            # Save the credentials for the next run
+            with open(os.path.join(credentials_dir, 'token_calendar.json'), 'w') as token:
+                token.write(creds.to_json())
+
         self._calendar_service = GoogleCalendar(
-            credentials_path=credentials_file_path,
-            credentials=self.__get_credentials(token_file_path=token_file_path),
-            token_path=token_file_path,
+            credentials=creds,
             default_calendar=calendar
         )
 
-    @staticmethod
-    def __get_credentials(token_file_path: str):
-        """
-        Get credential google by token file.
-
-        Args:
-            token_file_path (str): The path of the token json file.
-
-        Returns:
-            Credentials: Class credentials google
-        """
-        scopes = ['https://www.googleapis.com/auth/calendar']
-        if not os.path.exists(token_file_path):
-            raise RuntimeError("Não foi encontrado o token file.")
-        return Credentials.from_authorized_user_file(token_file_path, scopes)
+    @property
+    def calendar_service(self) -> GoogleCalendar:
+        """The Google Calendar account service."""
+        return self._calendar_service
 
     def get_events(self, date_min: datetime = None, date_max: datetime = None) -> List[Event]:
         """
-        Get all calendar events that haven't happened yet.
+        Get all calendar events.
 
         Args:
             date_min (datetime, optional): Events date is within or later than the specified date.
                 Set this value if you want to return events that have already happened.
             date_max (datetime, optional): Events date is earlier or equal than the specified date.
 
         Returns:
             List[Event]: The list containing all the calendar events.
         """
-        return list(self._calendar_service.get_events(time_min=date_min, time_max=date_max))
+        return list(self.calendar_service.get_events(time_min=date_min, time_max=date_max))
 
-    def create_calendar(self, title: str, description: str = None, calendar_id: str = None):
+    def create_calendar(self, title: str, description: str = None) -> None:
         """
-         Create a new calendar.
+        Create a new secondary calendar.
 
         Args:
             title (str): Title of the calendar.
-            description (str, optional): Identifier of the calendar.
-            calendar_id (str, optional): Description of the calendar.
-
-        Returns:
-            dict: The dict object with ID.
+            description (str, optional): Description of the calendar.
         """
         calendar = Calendar(
-            description=description,
             summary=title,
-            calendar_id=calendar_id,
+            description=description
         )
-        return self._calendar_service.add_calendar(calendar=calendar)
+        self.calendar_service.add_calendar(calendar=calendar)
 
-    def get_calendar(self, calendar_id: str = None):
+    def get_calendar(self, calendar_id: str = None) -> Calendar:
         """
         Return the calendar with the corresponding calendar_id.
 
         Args:
             calendar_id (str, optional): Calendar identifier.
+                To see the id of a calendar, go to the Integrate Calendar tab in the calendar settings.
 
         Returns:
-            Calendar: Object calendar.
+            Calendar: The Calendar object.
         """
-        return self._calendar_service.get_calendar(calendar_id=calendar_id)
+        return self.calendar_service.get_calendar(calendar_id=calendar_id)
 
-    def get_calendars(self):
+    def get_calendars(self) -> List[Calendar]:
         """
-        Return the calendars.
+        Return the calendars on the user's calendar list.
 
         Returns:
-            List[Calendar]: Object calendar.
+            List[Calendar]: The list containing all the Calendar objects.
         """
-        return list(self._calendar_service.get_calendar_list())
+        return list(self.calendar_service.get_calendar_list())
 
-    def delete_calendar(self, calendar: Union[Calendar, str]):
+    def delete_calendar(self, calendar: Union[Calendar, str]) -> None:
         """
-        Delete calendar.
+        Delete a secondary calendar.
 
         Args:
-            calendar (Union[Calendar, str], optional): Calendar identifier.
+            calendar (Calendar | str): The calendar identifier or the Calendar object.
+                To see the id of a calendar, go to the Integrate Calendar tab in the calendar settings.
         """
-        self._calendar_service.delete_calendar(calendar=calendar)
+        self.calendar_service.delete_calendar(calendar=calendar)
 
     def create_event(self, title: str, description: str, start_date: datetime,
                      end_date: datetime = None, attendees: List[str] = None) -> None:
         """
         Create a new event on the calendar.
 
         Args:
@@ -140,15 +147,15 @@
         event = Event(
             summary=title,
             description=description,
             start=start_date,
             end=end_date,
             attendees=attendees
         )
-        self._calendar_service.add_event(event)
+        self.calendar_service.add_event(event)
 
     def create_recurring_event(
             self,
             title: str,
             description: str,
             start_date: datetime,
             end_date: datetime = None,
@@ -185,28 +192,28 @@
             summary=title,
             description=description,
             start=start_date,
             end=end_date,
             attendees=attendees,
             recurrence=recurrence_rule
         )
-        self._calendar_service.add_event(event)
+        self.calendar_service.add_event(event)
 
     def move_event(self, event: Event, destination_calendar: str) -> None:
         """
         Move a event from the calendar to another calendar.
 
         Args:
             event (Event): The event to be moved.
             destination_calendar (str): The id of the destination calendar.
                 To see the id of a calendar, go to the Integrate Calendar tab in the calendar settings.
         """
-        self._calendar_service.move_event(event, destination_calendar)
+        self.calendar_service.move_event(event, destination_calendar)
 
     def delete_event(self, event: Event) -> None:
         """
         Delete a event from the calendar.
 
         Args:
             event (Event): The event to be deleted.
         """
-        self._calendar_service.delete_event(event)
+        self.calendar_service.delete_event(event)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `botcity-googlecalendar-plugin-0.1.5/botcity_googlecalendar_plugin.egg-info/PKG-INFO` & `botcity-googlecalendar-plugin-0.1.6/botcity_googlecalendar_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botcity-googlecalendar-plugin
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://bitbucket.org/botcitydev/bot-googlecalendar-plugin-python.git
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # BotCity Google Calendar Plugin - Python
 
 ## 🤖 Computer-vision based UI Automation
```

### Comparing `botcity-googlecalendar-plugin-0.1.5/setup.py` & `botcity-googlecalendar-plugin-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `botcity-googlecalendar-plugin-0.1.5/tests/test_plugin.py` & `botcity-googlecalendar-plugin-0.1.6/tests/test_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,27 +15,14 @@
         title=f"{title}_recurring_daily",
         start_date=now,
         description="testing recurring daily",
         recurrence=EventRecurrence.DAILY
     )
 
 
-@pytest.mark.xfail(reason="API Google return code 400")
-def test_create_recurring_hourly_event(bot: BotGoogleCalendarPlugin, title: str, now: datetime.datetime):
-    now = now + datetime.timedelta(hours=2)
-    end_date = now + datetime.timedelta(hours=5)
-    bot.create_recurring_event(
-        title=f"{title}_recurring_hourly",
-        start_date=now,
-        description="testing recurring hourly",
-        recurrence=EventRecurrence.HOURLY,
-        end_date=end_date
-    )
-
-
 def test_create_recurring_weekly_event(bot: BotGoogleCalendarPlugin, title: str, now: datetime.datetime):
     now = now + datetime.timedelta(hours=3)
     bot.create_recurring_event(
         title=f"{title}_recurring_weekly",
         start_date=now,
         description="testing recurring weekly",
         recurrence=EventRecurrence.WEEKLY
```

### Comparing `botcity-googlecalendar-plugin-0.1.5/versioneer.py` & `botcity-googlecalendar-plugin-0.1.6/versioneer.py`

 * *Files identical despite different names*

