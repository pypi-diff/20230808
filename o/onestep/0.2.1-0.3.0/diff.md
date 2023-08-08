# Comparing `tmp/onestep-0.2.1.tar.gz` & `tmp/onestep-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onestep-0.2.1.tar", max compression
+gzip compressed data, was "onestep-0.3.0.tar", max compression
```

## Comparing `onestep-0.2.1.tar` & `onestep-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1362 2023-08-04 08:03:15.312882 onestep-0.2.1/README.md
--rw-r--r--   0        0        0      636 2023-08-04 08:03:15.312882 onestep-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1390 2023-08-04 08:03:15.312882 onestep-0.2.1/src/onestep/__init__.py
--rw-r--r--   0        0        0      414 2023-08-04 08:03:15.312882 onestep-0.2.1/src/onestep/_utils.py
--rw-r--r--   0        0        0      221 2023-08-04 08:03:15.312882 onestep-0.2.1/src/onestep/broker/__init__.py
--rw-r--r--   0        0        0     4543 2023-08-04 08:03:15.312882 onestep-0.2.1/src/onestep/broker/base.py
--rw-r--r--   0        0        0      957 2023-08-04 08:03:15.312882 onestep-0.2.1/src/onestep/broker/cron.py
--rw-r--r--   0        0        0      151 2023-08-04 08:03:15.312882 onestep-0.2.1/src/onestep/broker/memory.py
--rw-r--r--   0        0        0     2291 2023-08-04 08:03:15.312882 onestep-0.2.1/src/onestep/broker/rabbitmq.py
--rw-r--r--   0        0        0     2144 2023-08-04 08:03:15.312882 onestep-0.2.1/src/onestep/broker/webhook.py
--rw-r--r--   0        0        0      610 2023-08-04 08:03:15.312882 onestep-0.2.1/src/onestep/exception.py
--rw-r--r--   0        0        0     4543 2023-08-04 08:03:15.312882 onestep-0.2.1/src/onestep/message.py
--rw-r--r--   0        0        0      286 2023-08-04 08:03:15.312882 onestep-0.2.1/src/onestep/middleware/__init__.py
--rw-r--r--   0        0        0      521 2023-08-04 08:03:15.316882 onestep-0.2.1/src/onestep/middleware/base.py
--rw-r--r--   0        0        0     2438 2023-08-04 08:03:15.316882 onestep-0.2.1/src/onestep/middleware/config.py
--rw-r--r--   0        0        0     6350 2023-08-04 08:03:15.316882 onestep-0.2.1/src/onestep/onestep.py
--rw-r--r--   0        0        0     2699 2023-08-04 08:03:15.316882 onestep-0.2.1/src/onestep/retry.py
--rw-r--r--   0        0        0      293 2023-08-04 08:03:15.316882 onestep-0.2.1/src/onestep/signal.py
--rw-r--r--   0        0        0      618 2023-08-04 08:03:15.316882 onestep-0.2.1/src/onestep/state.py
--rw-r--r--   0        0        0     3516 2023-08-04 08:03:15.316882 onestep-0.2.1/src/onestep/worker.py
--rw-r--r--   0        0        0     1956 1970-01-01 00:00:00.000000 onestep-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1362 2023-08-08 15:18:34.516024 onestep-0.3.0/README.md
+-rw-r--r--   0        0        0      666 2023-08-08 15:18:34.520024 onestep-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1390 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/__init__.py
+-rw-r--r--   0        0        0      414 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/_utils.py
+-rw-r--r--   0        0        0      258 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/broker/__init__.py
+-rw-r--r--   0        0        0     4543 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/broker/base.py
+-rw-r--r--   0        0        0      957 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/broker/cron.py
+-rw-r--r--   0        0        0      151 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/broker/memory.py
+-rw-r--r--   0        0        0     2291 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/broker/rabbitmq.py
+-rw-r--r--   0        0        0     2291 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/broker/redis.py
+-rw-r--r--   0        0        0     2144 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/broker/webhook.py
+-rw-r--r--   0        0        0      610 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/exception.py
+-rw-r--r--   0        0        0     3897 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/message.py
+-rw-r--r--   0        0        0      286 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/middleware/__init__.py
+-rw-r--r--   0        0        0      521 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/middleware/base.py
+-rw-r--r--   0        0        0     2438 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/middleware/config.py
+-rw-r--r--   0        0        0     6610 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/onestep.py
+-rw-r--r--   0        0        0     2740 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/retry.py
+-rw-r--r--   0        0        0      293 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/signal.py
+-rw-r--r--   0        0        0      618 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/state.py
+-rw-r--r--   0        0        0     3863 2023-08-08 15:18:34.520024 onestep-0.3.0/src/onestep/worker.py
+-rw-r--r--   0        0        0     2007 1970-01-01 00:00:00.000000 onestep-0.3.0/PKG-INFO
```

### Comparing `onestep-0.2.1/README.md` & `onestep-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ## Brokers
 
 - [x] MemoryBroker
 - [x] CronBroker
 - [x] WebHookBroker
 - [x] RabbitMQBroker
-- [ ] RedisBroker
+- [x] RedisBroker
 - [ ] KafkaBroker
 
 ## example
 
 ```python
 from onestep import step, WebHookBroker
```

### Comparing `onestep-0.2.1/pyproject.toml` & `onestep-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "onestep"
-version = "0.2.1"
+version = "0.3.0"
 description = ""
 authors = ["miclon <jcnd@163.com>"]
 readme = "README.md"
 packages = [
     { include = 'onestep', from = 'src' }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 asgiref = "^3.6.0"
 blinker = "^1.5"
 croniter = "^1.3.8"
 usepy-plugin-rabbitmq = "^0.1.0"
+usepy-plugin-redis = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 nacos-sdk-python = "^0.1.12"
 redis = "^4.5.1"
 autopep8 = "^2.0.2"
 loguru = "^0.6.0"
```

### Comparing `onestep-0.2.1/src/onestep/__init__.py` & `onestep-0.3.0/src/onestep/__init__.py`

 * *Files identical despite different names*

### Comparing `onestep-0.2.1/src/onestep/broker/base.py` & `onestep-0.3.0/src/onestep/broker/base.py`

 * *Files identical despite different names*

### Comparing `onestep-0.2.1/src/onestep/broker/cron.py` & `onestep-0.3.0/src/onestep/broker/cron.py`

 * *Files identical despite different names*

### Comparing `onestep-0.2.1/src/onestep/broker/rabbitmq.py` & `onestep-0.3.0/src/onestep/broker/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `onestep-0.2.1/src/onestep/broker/webhook.py` & `onestep-0.3.0/src/onestep/broker/webhook.py`

 * *Files identical despite different names*

### Comparing `onestep-0.2.1/src/onestep/exception.py` & `onestep-0.3.0/src/onestep/exception.py`

 * *Files identical despite different names*

### Comparing `onestep-0.2.1/src/onestep/message.py` & `onestep-0.3.0/src/onestep/message.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,149 +1,138 @@
 import json
 import sys
 import time
 import uuid
-from traceback import format_exception, TracebackException
+from traceback import TracebackException
 from typing import Optional, Any, Union
 
 from onestep._utils import catch_error
 
 
+class MessageTracebackException(TracebackException):
+    def __init__(self, exc_type, exc_value, exc_traceback, **kwargs):
+        super().__init__(exc_type, exc_value, exc_traceback, **kwargs)
+        self.exc_value = exc_value
+
+
 class Extra:
     def __init__(self, task_id=None, publish_time=None, failure_count=0):
         self.task_id = task_id or str(uuid.uuid4())
         self.publish_time = publish_time or round(time.time(), 3)
         self.failure_count = failure_count
-    
+
     def to_dict(self):
         return {
             'task_id': self.task_id,
             'publish_time': self.publish_time,
             'failure_count': self.failure_count,
         }
-    
+
     def __str__(self):
         return str(self.to_dict())
-    
+
     def __repr__(self):
         return f"{self.__class__.__name__}({self.task_id}, {self.publish_time}, {self.failure_count})"
 
 
 class Message:
-    
+
     def __init__(
             self,
             body: Optional[Union[dict, Any]] = None,
             extra: Optional[Union[dict, Extra]] = None,
             msg: Optional[Any] = None,
             broker=None
     ):
         self.body = body
         self.extra = self._set_extra(extra)
         self.msg = msg
-        
+
         self.broker = broker
         self._exception = None
-    
+
     @staticmethod
     def _set_extra(extra):
         if isinstance(extra, Extra):
             return extra
         elif isinstance(extra, dict):
             return Extra(**extra)
         else:
             return Extra()
-    
-    def set_exception(self, exception: Optional[Union[TracebackException, Exception, Any]] = None):
-        """设置异常信息 一般不用自己传入exception，会自动获取"""
-        self.exception = exception if exception else TracebackException(*sys.exc_info())
+
+    def set_exception(self):
+        """设置异常信息，会自动获取"""
+        self._exception = MessageTracebackException(*sys.exc_info())
         self.failure_count = self.failure_count + 1
-    
+
     @property
-    def exception(self):
+    def exception(self) -> Optional[MessageTracebackException]:
         return self._exception
-    
-    @exception.setter
-    def exception(self, value):
-        self._exception = value
-    
+
     @property
     def fail(self):
         return self.exception is not None
-    
+
     @property
     def failure_count(self):
         return self.extra.failure_count
-    
+
     @failure_count.setter
     def failure_count(self, value):
         self.extra.failure_count = value
-    
+
     def replace(self, **kwargs):
         """替换当前message的属性"""
         for key, value in kwargs.items():
             if not hasattr(self, key):
                 continue
             if key == 'extra':
                 value = self._set_extra(value)
             setattr(self, key, value)
         return self
-    
+
     def to_dict(self, include_exception=False) -> dict:
         data = {'body': self.body, 'extra': self.extra.to_dict()}
         if include_exception and self.exception:
-            if isinstance(self.exception, TracebackException):
-                data['exception'] = "".join(self.exception.format(chain=True))  # noqa
-            elif isinstance(self.exception, Exception):
-                data['exception'] = "".join(
-                    format_exception(
-                        self.exception.__class__, self.exception,
-                        self.exception.__getattr__('__traceback__', None)
-                    )
-                )
-            else:
-                try:
-                    data['exception'] = json.dumps(self.exception)
-                except Exception:
-                    data['exception'] = str(self.exception)
-        
+            data['exception'] = "".join(self.exception.format(chain=True))  # noqa
+
         return data
-    
+
     def to_json(self, include_exception=False) -> str:
         return json.dumps(self.to_dict(include_exception))
-    
+
     @catch_error()
     def confirm(self):
         """确认消息"""
         self.broker.confirm(self)
-    
+
     @catch_error()
     def reject(self):
         """拒绝消息"""
         self.broker.reject(self)
-    
+
     @catch_error()
     def requeue(self, is_source=False):
         """
         重发消息：先拒绝 再 重入
         
         :param is_source: 是否是源消息，True: 使用消息的最新数据重入当前队列，False: 使用消息的最新数据重入当前队列
         """
         self.broker.requeue(self, is_source=is_source)
-    
+
     def __getattr__(self, item):
         return None
-    
+
     def __delattr__(self, item):
         if hasattr(self, item):
             setattr(self, item, None)
-    
+
     def __str__(self):
         return str(self.to_dict())
-    
+
     def __repr__(self):
         return f"<{self.__class__.__name__} {self.body}>"
 
 
 if __name__ == '__main__':
     msg = Message()
     msg.x = 1
```

### Comparing `onestep-0.2.1/src/onestep/middleware/base.py` & `onestep-0.3.0/src/onestep/middleware/base.py`

 * *Files identical despite different names*

### Comparing `onestep-0.2.1/src/onestep/middleware/config.py` & `onestep-0.3.0/src/onestep/middleware/config.py`

 * *Files identical despite different names*

### Comparing `onestep-0.2.1/src/onestep/onestep.py` & `onestep-0.3.0/src/onestep/onestep.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,24 @@
 
 class BaseOneStep:
     consumers: Dict[str, List[WorkerThread]] = collections.defaultdict(list)
     state = State()  # 全局状态
 
     def __init__(self, fn,
                  group: str = "OneStep",
+                 name: str = None,
                  from_broker: Union[BaseBroker, List[BaseBroker], None] = None,
                  to_broker: Union[BaseBroker, List[BaseBroker], None] = None,
                  workers: Optional[int] = None,
                  middlewares: Optional[List[Any]] = None,
                  retry: Union[Callable, object] = NeverRetry(),
                  error_callback: Optional[Union[Callable, object]] = None):
         self.group = group
         self.fn = fn
+        self.name = name or fn.__name__
         self.workers = workers or DEFAULT_WORKERS
         self.middlewares = middlewares or []
 
         self.from_brokers = self._init_broker(from_broker)
         self.to_brokers = self._init_broker(to_broker)
         self.retry = retry
         self.error_callback = error_callback
@@ -68,38 +70,42 @@
             consumers = [c for v in cls.consumers.values() for c in v]
         else:
             consumers = cls.consumers[group]
         return consumers
 
     @classmethod
     def start(cls, group: Optional[str] = None):
+        logger.debug(f"start: {group=}")
         for consumer in cls._find_consumers(group):
             consumer.start()
+            logger.debug(f"started: {consumer=}")
 
     @classmethod
     def stop(cls, group: Optional[str] = None):
+        logger.debug(f"stop: {group=}")
         for consumer in cls._find_consumers(group):
             consumer.shutdown()
+            logger.debug(f"stopped: {consumer=}")
 
     def wraps(self, func):
         @functools.wraps(func)
         def wrapped_f(*args, **kwargs):
             return self(*args, **kwargs)  # noqa
 
         return wrapped_f
 
     def send(self, result, broker=None):
         """将返回的内容交给broker发送"""
         if result is None:
-            logger.debug("send(result): body is empty")
+            logger.warning("send(result): body is empty")
             return
 
         brokers = self._init_broker(broker) or self.to_brokers
         if not brokers:
-            logger.debug("send(result): broker is empty")
+            logger.warning("send(result): broker is empty")
             return
 
         # 如果是Message类型，就不再封装
         message = result if isinstance(result, Message) else Message(body=result)
 
         self.before_emit("send", message=message)
         for broker in brokers:
```

### Comparing `onestep-0.2.1/src/onestep/retry.py` & `onestep-0.3.0/src/onestep/retry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import ABC, abstractmethod
 from typing import Optional, Tuple, Union, Type
+
 from .exception import RetryViaLocal, RetryViaQueue
 from .message import Message
 
 
 class BaseRetry(ABC):
     
     @abstractmethod
@@ -35,15 +36,15 @@
 
 class RetryIfException(BaseRetry):
     
     def __init__(self, exceptions: Optional[Tuple[Union[Exception, Type]]] = Exception):
         self.exceptions = exceptions
     
     def __call__(self, message) -> Optional[bool]:
-        return isinstance(message.exception, self.exceptions)  # noqa
+        return isinstance(message.exception.exc_value, self.exceptions)  # noqa
 
 
 class AdvancedRetry(TimesRetry):
     """高级重试策略
     
     1. 本地重试：如果异常是 RetryViaLocal 或 指定异常，且重试次数未达到上限，则本地重试，不回调
     2. 队列重试：如果异常是 RetryViaQueue，且重试次数未达到上限，则入队重试，不回调
@@ -51,18 +52,18 @@
     注：待重试的异常若继承自 RetryException，则可单独指定重试次数，否则默认为 3 次
     """
     def __init__(self, times: int = 3, exceptions: Optional[Tuple[Union[Exception, Type]]] = None):
         super().__init__(times=times)
         self.exceptions = (RetryViaLocal, RetryViaQueue) + (exceptions or ())
     
     def __call__(self, message: Message) -> Optional[bool]:
-        if isinstance(message.exception, self.exceptions):
-            max_retry_times = getattr(message.exception, "times", None) or self.times
+        if isinstance(message.exception.exc_value, self.exceptions):
+            max_retry_times = getattr(message.exception.exc_value, "times", None) or self.times
             if message.failure_count < max_retry_times:
-                if isinstance(message.exception, RetryViaQueue):
+                if isinstance(message.exception.exc_value, RetryViaQueue):
                     return None  # 入队重试，不回调
                 return True  # 本地重试，不回调
             else:
                 return False  # 不重试了，回调
         else:
             return False  # 其他异常，回调
```

### Comparing `onestep-0.2.1/src/onestep/state.py` & `onestep-0.3.0/src/onestep/state.py`

 * *Files identical despite different names*

### Comparing `onestep-0.2.1/src/onestep/worker.py` & `onestep-0.3.0/src/onestep/worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 """
 将指定的函数放入线程中运行
 """
+try:
+    from collections import Iterable
+except ImportError:
+    from collections.abc import Iterable
 import logging
 import threading
 from asyncio import iscoroutinefunction
 from inspect import isasyncgenfunction
 
 from asgiref.sync import async_to_sync
 
@@ -41,23 +45,29 @@
         """
         self.__shutdown_event.clear()
 
         while not self.__shutdown:
             if self.__shutdown:
                 break
             # TODO：consume应当传入一些配置参数
-            for message in self.broker.consume():
-                if message is None:
+            for result in self.broker.consume():
+                if result is None:
                     continue
-                message.broker = message.broker or self.broker
-                logger.debug(f"receive message<{message}>")
-                message_received.send(self, message=message)
-                self.instance.before_emit("receive", message=message)
-                self._run_instance(message)
-                self.instance.after_emit("receive", message=message)
+                messages = (
+                    result
+                    if isinstance(result, Iterable)
+                    else [result]
+                )
+                for message in messages:
+                    message.broker = message.broker or self.broker
+                    logger.debug(f"{self.instance.name} receive message<{message}> from {self.broker!r}")
+                    message_received.send(self, message=message)
+                    self.instance.before_emit("receive", message=message)
+                    self._run_instance(message)
+                    self.instance.after_emit("receive", message=message)
 
     def shutdown(self):
         self.__shutdown = True
         self.__shutdown_event.wait()
 
     def _run_instance(self, message):
         while True:
@@ -66,22 +76,22 @@
                     async_to_sync(self.instance)(message, *self.args, **self.kwargs)
                 else:
                     self.instance(message, *self.args, **self.kwargs)
                 message_consumed.send(self, message=message)
                 return message.confirm()
             except DropMessage as e:
                 message_drop.send(self, message=message, reason=e)
-                logger.warning(f"{self.instance.fn.__name__} dropped <{type(e).__name__}: {str(e)}>")
+                logger.warning(f"{self.instance.name} dropped <{type(e).__name__}: {str(e)}>")
                 return message.reject()
             except Exception as e:
                 message_error.send(self, message=message, error=e)
                 if self.instance.state.debug:
-                    logger.exception(f"{self.instance.fn.__name__} run error <{type(e).__name__}: {str(e)}>")
+                    logger.exception(f"{self.instance.name} run error <{type(e).__name__}: {str(e)}>")
                 else:
-                    logger.error(f"{self.instance.fn.__name__} run error <{type(e).__name__}: {str(e)}>")
+                    logger.error(f"{self.instance.name} run error <{type(e).__name__}: {str(e)}>")
                 message.set_exception()
 
                 retry_state = self.retry(message)
                 if retry_state:  # True=继续（执行重试）
                     continue
                 elif retry_state is False:  # False=结束（执行回调）
                     if self.error_callback:
```

### Comparing `onestep-0.2.1/PKG-INFO` & `onestep-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: onestep
-Version: 0.2.1
+Version: 0.3.0
 Summary: 
 Author: miclon
 Author-email: jcnd@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asgiref (>=3.6.0,<4.0.0)
 Requires-Dist: blinker (>=1.5,<2.0)
 Requires-Dist: croniter (>=1.3.8,<2.0.0)
 Requires-Dist: usepy-plugin-rabbitmq (>=0.1.0,<0.2.0)
+Requires-Dist: usepy-plugin-redis (>=0.1.0,<0.2.0)
 Description-Content-Type: text/markdown
 
 # OneStep
 
 <a href="https://github.com/mic1on/onestep/actions/workflows/test.yml?query=event%3Apush+branch%3Amain" target="_blank">
     <img src="https://github.com/mic1on/onestep/workflows/test%20suite/badge.svg?branch=main&event=push" alt="Test">
 </a>
@@ -34,15 +35,15 @@
 
 ## Brokers
 
 - [x] MemoryBroker
 - [x] CronBroker
 - [x] WebHookBroker
 - [x] RabbitMQBroker
-- [ ] RedisBroker
+- [x] RedisBroker
 - [ ] KafkaBroker
 
 ## example
 
 ```python
 from onestep import step, WebHookBroker
```

