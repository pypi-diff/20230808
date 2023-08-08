# Comparing `tmp/wedne-0.1.1.tar.gz` & `tmp/wedne-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wedne-0.1.1.tar", max compression
+gzip compressed data, was "wedne-1.0.0.tar", max compression
```

## Comparing `wedne-0.1.1.tar` & `wedne-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     2590 2023-08-08 14:45:44.084132 wedne-0.1.1/README.md
--rw-r--r--   0        0        0      950 2023-08-08 14:45:31.748614 wedne-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-08 13:10:56.356160 wedne-0.1.1/wedne/__init__.py
--rw-r--r--   0        0        0        0 2023-08-08 13:10:56.360160 wedne-0.1.1/wedne/client/__init__.py
--rw-r--r--   0        0        0     1203 2023-08-08 13:10:56.368161 wedne-0.1.1/wedne/client/__main__.py
--rw-r--r--   0        0        0      338 2023-08-08 13:10:56.376161 wedne-0.1.1/wedne/client/consts.py
--rw-r--r--   0        0        0      533 2023-08-08 13:10:56.380161 wedne-0.1.1/wedne/client/shared_commands.py
--rw-r--r--   0        0        0     2802 2023-08-08 13:10:56.384162 wedne-0.1.1/wedne/client/telegram.py
--rw-r--r--   0        0        0     1801 2023-08-08 13:10:56.392162 wedne-0.1.1/wedne/client/watcher.py
--rw-r--r--   0        0        0      399 2023-08-08 13:10:56.396162 wedne-0.1.1/wedne/commands.py
--rw-r--r--   0        0        0        0 2023-08-08 13:10:56.404163 wedne-0.1.1/wedne/server/__init__.py
--rw-r--r--   0        0        0     1178 2023-08-08 13:10:56.408163 wedne-0.1.1/wedne/server/__main__.py
--rw-r--r--   0        0        0      186 2023-08-08 13:10:56.416164 wedne-0.1.1/wedne/server/api/__init__.py
--rw-r--r--   0        0        0      759 2023-08-08 13:10:56.420164 wedne-0.1.1/wedne/server/api/stats.py
--rw-r--r--   0        0        0      999 2023-08-08 14:44:51.556007 wedne-0.1.1/wedne/server/api/visits.py
--rw-r--r--   0        0        0     2259 2023-08-08 13:10:56.432165 wedne-0.1.1/wedne/server/db.py
--rw-r--r--   0        0        0      428 2023-08-08 13:10:56.436165 wedne-0.1.1/wedne/server/settings.py
--rw-r--r--   0        0        0     1542 2023-08-08 13:10:56.440165 wedne-0.1.1/wedne/server/tasks.py
--rw-r--r--   0        0        0      288 2023-08-08 13:10:56.448166 wedne-0.1.1/wedne/utils.py
--rw-r--r--   0        0        0     3146 1970-01-01 00:00:00.000000 wedne-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1463 2023-08-08 17:39:59.372075 wedne-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     4499 2023-08-08 17:45:10.592681 wedne-1.0.0/README.md
+-rw-r--r--   0        0        0     1085 2023-08-08 17:45:41.389165 wedne-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-08 13:10:56.356160 wedne-1.0.0/wedne/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:10:56.360160 wedne-1.0.0/wedne/client/__init__.py
+-rw-r--r--   0        0        0     1203 2023-08-08 13:10:56.368161 wedne-1.0.0/wedne/client/__main__.py
+-rw-r--r--   0        0        0      338 2023-08-08 13:10:56.376161 wedne-1.0.0/wedne/client/consts.py
+-rw-r--r--   0        0        0      533 2023-08-08 13:10:56.380161 wedne-1.0.0/wedne/client/shared_commands.py
+-rw-r--r--   0        0        0     2802 2023-08-08 13:10:56.384162 wedne-1.0.0/wedne/client/telegram.py
+-rw-r--r--   0        0        0     1801 2023-08-08 13:10:56.392162 wedne-1.0.0/wedne/client/watcher.py
+-rw-r--r--   0        0        0      399 2023-08-08 13:10:56.396162 wedne-1.0.0/wedne/commands.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:10:56.404163 wedne-1.0.0/wedne/server/__init__.py
+-rw-r--r--   0        0        0     1178 2023-08-08 13:10:56.408163 wedne-1.0.0/wedne/server/__main__.py
+-rw-r--r--   0        0        0      186 2023-08-08 13:10:56.416164 wedne-1.0.0/wedne/server/api/__init__.py
+-rw-r--r--   0        0        0      759 2023-08-08 13:10:56.420164 wedne-1.0.0/wedne/server/api/stats.py
+-rw-r--r--   0        0        0      999 2023-08-08 14:44:51.556007 wedne-1.0.0/wedne/server/api/visits.py
+-rw-r--r--   0        0        0     2259 2023-08-08 13:10:56.432165 wedne-1.0.0/wedne/server/db.py
+-rw-r--r--   0        0        0      428 2023-08-08 13:10:56.436165 wedne-1.0.0/wedne/server/settings.py
+-rw-r--r--   0        0        0     1542 2023-08-08 13:10:56.440165 wedne-1.0.0/wedne/server/tasks.py
+-rw-r--r--   0        0        0      288 2023-08-08 13:10:56.448166 wedne-1.0.0/wedne/utils.py
+-rw-r--r--   0        0        0     5292 1970-01-01 00:00:00.000000 wedne-1.0.0/PKG-INFO
```

### Comparing `wedne-0.1.1/README.md` & `wedne-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # wedne: координируем строительство башни
 
+![PyPI](https://img.shields.io/pypi/v/wedne)
+![PyPI - License](https://img.shields.io/pypi/l/wedne)
+
 _This project was built for a Russian-speaking community. There's no English version of
-README._
+the README._
 
-В vas3k.club чатах любят строить башни. Башни --- это однобуквенные сообщения от
-участников, из которых может составиться слово. Самый важный башенный день --- среда. В
+В чатах "Вастрик Клуба" любят строить башни. Башни — это однобуквенные сообщения от
+участников, из которых может составиться слово. Самый важный башенный день — среда. В
 среду принято строить "ITSWEDNESDAYMYDUDES" и отправлять лягушек. Это непросто: постоянно
 кто-то хочет отправить сообщение между буквами. Клубчанин не может быть посередине,
 приходится выбирать между созиданием и разрушением.
 
 wedne состоит из двух частей: `wedne.server` и `wedne.client`. Клиенты регистрируются в
 общем сервере и получают команды: отправить такую-то букву в такое-то время.
 
 ## Инструкции
 
 ### Как строить башни?
 
 Не обязательно быть программистом. Прочтите эту секцию и узнайте, как поучаствовать в
 строительстве.
 
-1. Скачайте на компьютер [установщик Python](py),
+1. Скачайте на компьютер [установщик Python][py],
 2. Пройдите установку (если спросят, отметьте "Add python.exe to PATH"),
 3. Откройте приложение "Терминал" или "Командную строку",
-4. Введите туда `python -m pip install wedne` --- теперь вы установили wedne,
+4. Введите туда `python -m pip install wedne` — теперь вы установили wedne,
 5. Наконец введите `python -m wedne.client` и залогиньтесь как в телеграме.
 
 Теперь у вас работает клиент. Он подключится к серверу и начнет ждать команду. Когда
 придет время, в чат от вашего имени отправится буква.
 
 Можете закрывать инструкцию.
 
@@ -40,10 +43,46 @@
 
 Проще всего склонировать и запустить с помощью Docker Compose:
 
 ```sh
 docker compose up
 ```
 
+Без докера надо запустить API и обработчик задач:
+
+```sh
+python -m wedne.server run_api
+
+python -m wedne.server consume_tasks
+```
+
+## FAQ
+
+### Почему я должен входить в телеграм? Это безопасно?
+
+wedne должен отправить букву в чат от какого-то аккаунта. При входе как раз подключается
+такой аккаунт. Исходный код открыт, можно проверить самому, как используются данные
+телеграма.
+
+### Без телеграма можно?
+
+Нельзя.
+
+### Какие команды могут прийти с сервера?
+
+Только команда из трех переменных: какую букву отправлять, когда отправлять и после кого
+отправлять. Сервер не может скомандовать отправить слово или предложение — клиент такое не
+примет. Сервер не может направить клиентов на другой чат — ID чата хранится на клиентах
+локально. Схема команды: `wedne/commands.py`
+
+### Не могу запустить, помогите?
+
+Спросите помощи в [чате "Бар"][chat].
+
+### Ничего не понимаю, что за башни и что за клуб?
 
+Кажется, вы не знаете про ["Вастрик Клуб"][club]. Этот проект написан для него. Если вы не
+участник, вам wedne будет бесполезен.
 
 [py]: https://www.python.org/downloads/
+[chat]: https://vas3k.club/room/bar/chat/
+[club]: https://vas3k.club/
```

### Comparing `wedne-0.1.1/pyproject.toml` & `wedne-1.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 [tool.poetry]
 name = "wedne"
-version = "0.1.1"
-description = ""
+version = "1.0.0"
+description = "Координируем строительство башни"
 authors = ["Oskar Sharipov"]
 readme = "README.md"
+license = "BSD-3-Clause"
+repository = "https://github.com/igoose1/wedne"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = {extras = ["dotenv"], version = "^1.10.9"}
 fire = "^0.5.0"
 httpx = "^0.24.1"
 telethon = "^1.28.5"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wedne-0.1.1/wedne/client/__main__.py` & `wedne-1.0.0/wedne/client/__main__.py`

 * *Files identical despite different names*

### Comparing `wedne-0.1.1/wedne/client/shared_commands.py` & `wedne-1.0.0/wedne/client/shared_commands.py`

 * *Files identical despite different names*

### Comparing `wedne-0.1.1/wedne/client/telegram.py` & `wedne-1.0.0/wedne/client/telegram.py`

 * *Files identical despite different names*

### Comparing `wedne-0.1.1/wedne/client/watcher.py` & `wedne-1.0.0/wedne/client/watcher.py`

 * *Files identical despite different names*

### Comparing `wedne-0.1.1/wedne/server/__main__.py` & `wedne-1.0.0/wedne/server/__main__.py`

 * *Files identical despite different names*

### Comparing `wedne-0.1.1/wedne/server/api/stats.py` & `wedne-1.0.0/wedne/server/api/stats.py`

 * *Files identical despite different names*

### Comparing `wedne-0.1.1/wedne/server/api/visits.py` & `wedne-1.0.0/wedne/server/api/visits.py`

 * *Files identical despite different names*

### Comparing `wedne-0.1.1/wedne/server/db.py` & `wedne-1.0.0/wedne/server/db.py`

 * *Files identical despite different names*

### Comparing `wedne-0.1.1/wedne/server/tasks.py` & `wedne-1.0.0/wedne/server/tasks.py`

 * *Files identical despite different names*

