# Comparing `tmp/basic_type_operations-0.0.2.tar.gz` & `tmp/basic_type_operations-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic_type_operations-0.0.2.tar", last modified: Thu Jul 20 10:07:18 2023, max compression
+gzip compressed data, was "basic_type_operations-0.0.3.tar", last modified: Tue Aug  8 08:12:17 2023, max compression
```

## Comparing `basic_type_operations-0.0.2.tar` & `basic_type_operations-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 10:07:18.228008 basic_type_operations-0.0.2/
--rw-rw-rw-   0        0        0        0 2023-07-20 09:08:51.000000 basic_type_operations-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      735 2023-07-20 10:07:18.228008 basic_type_operations-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-20 09:09:08.000000 basic_type_operations-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 10:07:18.223008 basic_type_operations-0.0.2/basic_type_operations/
--rw-rw-rw-   0        0        0      343 2023-07-20 10:02:38.000000 basic_type_operations-0.0.2/basic_type_operations/__init__.py
--rw-rw-rw-   0        0        0    25674 2023-06-12 02:45:32.000000 basic_type_operations-0.0.2/basic_type_operations/date_operation.py
--rw-rw-rw-   0        0        0     2561 2023-07-20 09:11:50.000000 basic_type_operations-0.0.2/basic_type_operations/dict_operation.py
--rw-rw-rw-   0        0        0    16546 2023-07-20 09:11:50.000000 basic_type_operations-0.0.2/basic_type_operations/list_operation.py
--rw-rw-rw-   0        0        0     8379 2023-07-20 09:11:50.000000 basic_type_operations-0.0.2/basic_type_operations/number_operation.py
--rw-rw-rw-   0        0        0    14819 2023-07-07 02:49:08.000000 basic_type_operations-0.0.2/basic_type_operations/str_operation.py
--rw-rw-rw-   0        0        0      608 2023-06-07 05:58:42.000000 basic_type_operations-0.0.2/basic_type_operations/tuple_operation.py
-drwxrwxrwx   0        0        0        0 2023-07-20 10:07:18.227011 basic_type_operations-0.0.2/basic_type_operations.egg-info/
--rw-rw-rw-   0        0        0      735 2023-07-20 10:07:18.000000 basic_type_operations-0.0.2/basic_type_operations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      540 2023-07-20 10:07:18.000000 basic_type_operations-0.0.2/basic_type_operations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 10:07:18.000000 basic_type_operations-0.0.2/basic_type_operations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-20 10:07:18.000000 basic_type_operations-0.0.2/basic_type_operations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-20 10:07:18.000000 basic_type_operations-0.0.2/basic_type_operations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-20 10:07:18.229008 basic_type_operations-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1333 2023-07-20 10:06:57.000000 basic_type_operations-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 08:12:17.455427 basic_type_operations-0.0.3/
+-rw-rw-rw-   0        0        0        0 2023-07-20 09:08:51.000000 basic_type_operations-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      734 2023-08-08 08:12:17.455427 basic_type_operations-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-20 09:09:08.000000 basic_type_operations-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 08:12:17.451350 basic_type_operations-0.0.3/basic_type_operations/
+-rw-rw-rw-   0        0        0      343 2023-08-08 07:14:11.000000 basic_type_operations-0.0.3/basic_type_operations/__init__.py
+-rw-rw-rw-   0        0        0    24470 2023-08-08 07:12:10.000000 basic_type_operations-0.0.3/basic_type_operations/date_operation.py
+-rw-rw-rw-   0        0        0     2020 2023-08-08 07:12:10.000000 basic_type_operations-0.0.3/basic_type_operations/dict_operation.py
+-rw-rw-rw-   0        0        0    14833 2023-08-08 07:12:10.000000 basic_type_operations-0.0.3/basic_type_operations/list_operation.py
+-rw-rw-rw-   0        0        0     7844 2023-08-08 07:12:10.000000 basic_type_operations-0.0.3/basic_type_operations/number_operation.py
+-rw-rw-rw-   0        0        0    17148 2023-08-08 07:14:11.000000 basic_type_operations-0.0.3/basic_type_operations/str_operation.py
+-rw-rw-rw-   0        0        0      608 2023-06-07 05:58:42.000000 basic_type_operations-0.0.3/basic_type_operations/tuple_operation.py
+drwxrwxrwx   0        0        0        0 2023-08-08 08:12:17.454422 basic_type_operations-0.0.3/basic_type_operations.egg-info/
+-rw-rw-rw-   0        0        0      734 2023-08-08 08:12:17.000000 basic_type_operations-0.0.3/basic_type_operations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2023-08-08 08:12:17.000000 basic_type_operations-0.0.3/basic_type_operations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 08:12:17.000000 basic_type_operations-0.0.3/basic_type_operations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-08-08 08:12:17.000000 basic_type_operations-0.0.3/basic_type_operations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-08-08 08:12:17.000000 basic_type_operations-0.0.3/basic_type_operations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-08 08:12:17.455427 basic_type_operations-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1392 2023-08-08 08:12:13.000000 basic_type_operations-0.0.3/setup.py
```

### Comparing `basic_type_operations-0.0.2/PKG-INFO` & `basic_type_operations-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: basic_type_operations
-Version: 0.0.2
+Version: 0.0.3
 Summary: Short description
-Home-page: https://github.com/SkyOceanchen/basic_type_operations.git
+Home-page: https://gitee.com/SkyOceanchen/basic_type_operations.git
 Author: SkyOceanChen
 Author-email: skyoceanchen@foxmail.com
 License: MIT
 Keywords: basic_type,python,str,list,numpy,number,datetime,time,calendar
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `basic_type_operations-0.0.2/basic_type_operations/date_operation.py` & `basic_type_operations-0.0.3/basic_type_operations/date_operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,24 +209,14 @@
         if not date:
             date = datetime.date.today()
         # 获取当月第一天的星期和当月的总天数
         month = date.month
         year = date.year
         firstDayWeekDay, monthRange = calendar.monthrange(year, month)
         return monthRange
-        # month = date.month
-        # if month == 12:
-        #     year = date.year
-        #     date2 = datetime.date.today().replace(year=year + 1, month=1, day=1) - datetime.timedelta(days=1)
-        # else:
-        #     date2 = datetime.date.today().replace(month=month + 1, day=1) - datetime.timedelta(days=1)
-        # data_start = datetime.datetime.strptime(str(date), '%Y-%m-%d')
-        # data_end = datetime.datetime.strptime(str(date2), '%Y-%m-%d')
-        # return data_end.day - data_start.day + 1
-
     # </editor-fold>
     # <editor-fold desc="开始和结束相差的天数">
     @staticmethod
     def two_time_days(start_time, end_time):
         days = (end_time - start_time).days
         return days
 
@@ -258,24 +248,21 @@
     @staticmethod
     def determine_leap_year(year):
         '''
         输入年份，判断是否是闰年。闰年判断方法：能被4整除，但不能被100整除；或者能被 400 整除。需要用到算术运算符和逻辑运算符
         :param year:
         :return:
         '''
-        # year = int(input('输入年份: '))
         is_leap = year % 4 == 0 and year % 100 != 0 or year % 400 == 0
         return is_leap
-        # print(is_leap)
 
     # </editor-fold>
     # <editor-fold desc="间隔相同天数时间">
     @staticmethod
     def datetime_interval_same_day(start_time, days):
-        # start_time = datetime.datetime(year=2020, month=12, day=15)
         now_time = datetime.datetime.now()
         return now_time - datetime.timedelta(days=(now_time - start_time).days % days)
 
     # </editor-fold>
     # <editor-fold desc="距离 某时 多少分钟前">
     @staticmethod
     def how_minutes_before_to_now(date=None, minutes=10):
@@ -546,16 +533,14 @@
     # <editor-fold desc="2021-02-01 10:10:10">
     @staticmethod
     def string_year_second(date_str):
         # print("2.把字符串转成datetime: ", datetime.strptime(st, "%Y:%m:%d %H:%M:%S"))
         if isinstance(date_str, datetime.datetime):
             return date_str
         else:
-            #         data = timezone.datetime.strptime(date, '%Y-%m-%d %H:%M:%S').replace(
-            #             tzinfo=None)
             return datetime.datetime.strptime(date_str, "%Y-%m-%d %H:%M:%S")
 
     # </editor-fold>
     # <editor-fold desc="接受的格式为2021-02-03">
     @staticmethod
     def string_year_days(date_str, params=True):
         if isinstance(date_str, datetime.datetime):
@@ -596,23 +581,14 @@
         :param xldate:
         :param datemode:
         :return:
         """
         epoch_1904 = datetime.datetime(1904, 1, 1)
         epoch_1900 = datetime.datetime(1899, 12, 31)
         epoch_1900_minus_1 = datetime.datetime(1899, 12, 30)
-        """
-        Convert an Excel date/time number into a :class:`datetime.datetime` object.
-
-        :param xldate: The Excel number
-        :param datemode: 0: 1900-based, 1: 1904-based.
-
-        :returns: A :class:`datetime.datetime` object.
-        """
-
         # Set the epoch based on the 1900/1904 datemode.
         if datemode:
             epoch = epoch_1904
         else:
             if xldate < 60:
                 epoch = epoch_1900
             else:
@@ -666,22 +642,18 @@
         # utc_date =(utcnow-) .isoformat()
         return utcnow.strftime('%Y-%m-%dT%H:%M:%S%z')
 
     # </editor-fold>
     # <editor-fold desc="UTC 2021-12-23T11:13:24+0000 -转换成 2021-12-23T11:13:24 ">
     @staticmethod
     def utc_local_date(utc_data1):
-        # utc_data1 = '2021-12-23T11:13:24+0000'
-        # utc_data1 = '2021-11-01T20:17:00.000+0000'
-        # utc_data1 = s
         t = utc_data1[:19]
         utc_date2 = datetime.datetime.strptime(t, "%Y-%m-%dT%H:%M:%S")
         local_date = utc_date2 + datetime.timedelta(hours=8)
         return local_date
-
     # </editor-fold>
     # </editor-fold>
     # <editor-fold desc="把时间戳转化为时间: 1479264792 to 2016-11-16 10:53:12'">
     @staticmethod
     def TimeStampToTime(timestamp):
         timeStruct = time.localtime(timestamp)
         return time.strftime('%Y-%m-%d %H:%M:%S', timeStruct)
```

### Comparing `basic_type_operations-0.0.2/basic_type_operations/dict_operation.py` & `basic_type_operations-0.0.3/basic_type_operations/dict_operation.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,67 +2,50 @@
 """
 @Time : 2023/3/29
 @Author : skyoceanchen
 @TEL: 18916403796
 @File : dict_operation.py 
 @PRODUCT_NAME : PyCharm 
 """
+from collections import Counter
 
 
 # <editor-fold desc="字典类工具">
 class DictOperation(object):
     @staticmethod
     def twodictadd(dict1, dict2):
-        # 方法2
-        for m, n in dict2.items():
-            if m in dict1:
-                dict1[m] += n
-            else:
-                dict1.setdefault(m, n)
-        return dict1
-        # 方法1
-        # dict1 = {'torch': 6, 'gold coin': 42}
-        # dict2 = {'rope': 1, 'gold': 20}
-        # print(dict1, dict2)
-        # dict_new = dict(Counter(dict1) + Counter(dict2))
-        # print(dict_new)
-        # return dict_new
+        dict_new = dict(Counter(dict1) + Counter(dict2))
+        return dict_new
 
     # <editor-fold desc="取出列表内所有字典的value值">
     @staticmethod
     def list_dict_value(lis):
         """
-        for item in list:
-           for key in item:
-              print(item[key])
         :param lis:
         :return:
         """
         res = [item[key] for item in lis for key in item]
         return res
 
     # </editor-fold>
     # <editor-fold desc="取出列表内所有字典的keys值">
     @staticmethod
     def list_dict_keys(lis):
         """
-        for item in list:
-           for key in item:
-              print(item[key])
         :param lis:
         :return:
         """
         res = [key for item in lis for key in item]
         return res
 
     # </editor-fold>
     # <editor-fold desc="字典组成的数组怎么进行去重">
     @staticmethod
     def dic_duplicate_remove(data):  # 适用一般情况
-        # data = reduce(lambda x, y: x + [y] if y not in x else x, [[], ] + data)#可能会被打死在工位上
+        # data = reduce(lambda x, y: x + [y] if y not in x else x, [[], ] + data)#
         data = [dict(t) for t in set([tuple(d.items()) for d in data])]
         return data
 
     @staticmethod
     def delete_duplicate_str(data):  # 适用这种情况如： data2 = [{"a": {"b": "c"}}, {"a": {"b": "c"}}]
         immutable_dict = set([str(item) for item in data])
         data = [eval(i) for i in immutable_dict]
```

### Comparing `basic_type_operations-0.0.2/basic_type_operations/list_operation.py` & `basic_type_operations-0.0.3/basic_type_operations/list_operation.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,21 +110,14 @@
             return None
 
     # </editor-fold>
     # <editor-fold desc="相同长度的二维数组的转置">
     @staticmethod
     def dimensional_list_two_same(data_lis):
         try:
-            # max_len = len(data_lis[0])
-            # b = [[] for _ in range(max_len)]  # 转置后列表
-            # if len(data_lis) > 0:
-            #     for i in range(max_len):  # 行数
-            #         for ls in data_lis:
-            #             b[i].append(ls[i])
-            #     return b
             li = np.array(data_lis)
             li = li.T
             li = li.tolist()
             return li
             # return None
         except:
             return None
@@ -205,20 +198,14 @@
         for index in range(num_len):
             res = None
             if float(lis2[index]) == 0:
                 res = 0
             else:
                 res = round(float(lis1[index]) / float(lis2[index]), 2)
             lst3.append(res)
-            # for i in lis2:
-            #     if i == '0':
-            #         rs = 0
-            #     else:
-            #         rs = round(float(item) / float(i), 2)
-            #     lst3.append(rs)
         return lst3
 
     # </editor-fold>
     # <editor-fold desc="列表保留n位小数">
     @staticmethod
     def list_Keep_place(data, decimal=0):
         if decimal == 0:
@@ -228,17 +215,15 @@
                 else:
                     data[i] = NumberOperation.round_up(data[i])
         else:
             for i in range(len(data)):
                 if isinstance(data[i], str):
                     continue
                 else:
-                    # data[i] = float('%.%f' % (data[i], decimal))
                     data[i] = NumberOperation.round_up(data[i], decimal)
-                # print(data[i], type(data[i]))
 
         return data
 
     # </editor-fold>
     # <editor-fold desc="二维数组求平均值">
     @staticmethod
     def two_dimensional_avgList(lis, keep_decimal=2, integer=False):
@@ -276,38 +261,22 @@
             return round(value, keep_decimal)
         return value
 
     # </editor-fold>
     # <editor-fold desc="不同长度的二维数组合并一维数组">
     @staticmethod
     def dimensional_list_two_marge(two_list):
-        # alist = [[3, 4, 5], [6, 7, 22], [35, 46, 78], [100]]
-        # print(list(itertools.chain(alist[0], alist[1])))
         len_a = len(two_list)
         new_list = []
         for i in range(len_a):
             new_list = list(itertools.chain(new_list, two_list[i]))
         return new_list
 
     # </editor-fold>
     # <editor-fold desc="数组分成相同长度的二维数组">
-    # def lst_trans0(test_list, n):
-    #     """n: split list into `n` groups
-    #     """
-    #     len_list = len(test_list)
-    #     m = math.ceil(len_list / float(n))
-    #     alist = []
-    #     group_m = -1
-    #     for i in range(len_list):
-    #         if i % m == 0:
-    #             group_m += 1
-    #             alist.append([test_list[i]])
-    #         else:
-    #             alist[group_m].append(test_list[i])
-    #     return alist
     @staticmethod
     def lst_trans0(test_list, n):
         """n: 一组多少条数据
         """
         len_list = len(test_list)
         n = math.ceil(len_list / float(n))
         m = math.ceil(len_list / float(n))
@@ -437,23 +406,18 @@
         for i in range(l):
             for j in range(n):
                 if section[j][0] <= lis[i] <= section[j][1]:
                     divided_list[j].append(lis1[i])
         y_section = []
         dic = {}
         for index, value in enumerate(divided_list):
-            # y_section.append(value.__len__())
-            # y_section.append(value)
             dic[x_section[index]] = round(len(value) / len(lis1), 2)
-            # dic[x_section[index]] = value.__len__()
-        # return y_section, x_section, dic
         return dic
 
     # </editor-fold>
-
     # <editor-fold desc="二维数据中，各个数据所占的百分比">
     @staticmethod
     def all_np_fen(arr_list):
         # 拼接数组函数
         List = list(itertools.chain.from_iterable(arr_list))
         arr = np.array(List)
         # print(arr.shape, type(arr.shape[0]))  # 二维元素的个数
@@ -464,22 +428,12 @@
             arr_new = arr[mask]
             v = arr_new.size
             result[k] = v
         key_list = list(result.keys())
         num_count = arr.shape[0]
         return_result = {}
         for keys in key_list:
-            # print(result[keys] / num_count, type(result[keys] / num_count))
             dat = result[keys] / num_count
             return_result[str(keys)] = NumberOperation.decimalToPercentageFuncTwo(dat)
-
-        # {1: 2, 2: 3, 3: 3, 4: 1, 5: 3}
         return return_result
-
-    # def tuokonglv():
-    #     dic = all_np_fen([[1, 1, 3, 2, 2, 2, 2, 2, 2, 2, 3], [3, 2, 1], [4, 5, 6]])
-    #     print(dic)
-
-    # tuokonglv()
-
     # </editor-fold>
 # </editor-fold>
```

### Comparing `basic_type_operations-0.0.2/basic_type_operations/number_operation.py` & `basic_type_operations-0.0.3/basic_type_operations/number_operation.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 @Time : 2023/3/29
 @Author : skyoceanchen
 @TEL: 18916403796
 @File : number_operation.py 
 @PRODUCT_NAME : PyCharm 
 """
 import random
+
+
 # <editor-fold desc="数值类工具">
 class NumberOperation(object):
     # <editor-fold desc="判断是否为数字">
     @staticmethod
     def is_number(s):
         try:
             float(s)
@@ -152,17 +154,14 @@
     # </editor-fold>
     # <editor-fold desc="是否构成三角形">
     @staticmethod
     def triangle_true(a, b, c):
         """
         是否构成三角形
         """
-        # a = float(input('输入三角形三条边：\n a = '))
-        # b = float(input(' b = '))
-        # c = float(input(' c = '))
         if a + b > c and a + c > b and b + c > a:
             return True
         else:
             return False
 
     # </editor-fold>
     # <editor-fold desc="是否是素数">
@@ -171,16 +170,15 @@
         """
             是否是素数
         输入一个正整数，判断是否是素数。素数定义：大于1的自然数中，只能被1和它本身整除的自然数。如：3、5、7
 
         判断是否是素数
         """
 
-        # num = int(input('请输入一个正整数: '))
-        end = int(num // 2) + 1  # 只判断前半部分是否能整除即可，前半部分没有能整除的因此，后半部分肯定也没有
+        end = int(num // 2) + 1  #
 
         is_prime = True
         for x in range(2, end):
             if num % x == 0:
                 is_prime = False
                 break
         if is_prime and num != 1:
@@ -201,21 +199,14 @@
         low = num % 10
         mid = num // 10 % 10
         high = num // 100
         if num == low ** 3 + mid ** 3 + high ** 3:
             return True
         else:
             return False
-        # for num in range(100, 1000):
-        #     low = num % 10
-        #     mid = num // 10 % 10
-        #     high = num // 100
-        #     if num == low ** 3 + mid ** 3 + high ** 3:
-        #         print(num)
-
     # </editor-fold>
     # <editor-fold desc="阿拉伯数字转换成中文">
     # 12 -->  一二
     @staticmethod
     def num_to_char(num):
         """数字转中文"""
         num = str(num)
@@ -256,9 +247,8 @@
         :param decimal_num: 小数保留位数
         :return:
         """
         return round(random.uniform(start, end), decimal_num)
 
     # </editor-fold>
 
-
-# </editor-fold>
+# </editor-fold>
```

### Comparing `basic_type_operations-0.0.2/basic_type_operations/str_operation.py` & `basic_type_operations-0.0.3/basic_type_operations/str_operation.py`

 * *Files 19% similar despite different names*

```diff
@@ -225,29 +225,93 @@
       lis = ["河南省", "郑州市", "湖北省", "武汉市"]
       process.extract("郑州", lis, limit=2)
       output:[('郑州市', 90), ('河南省', 0)]
       """
         return process.extract(str, lis, limit=limit)
 
     # </editor-fold>
-
     # <editor-fold desc="在列表中找最佳匹配的字符串和相似度">
     @staticmethod
     def extractOne(lis, str):
         """
         lis = ["河南省", "郑州市", "湖北省", "武汉市"]
         process.extractOne("郑州", lis)
         output:('郑州市', 90)
         process.extractOne("北京", lis)
         output:('湖北省', 45)
         """
         return process.extractOne(str, lis)
     # </editor-fold>
 
 
+# 引用 https://codeigo.com/python/printing-subscript-and-superscript/
+class StrUpperLower(object):
+    letter_big = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
+    letter_small = "abcdefghijklmnopqrstuvwxyz"
+    upper_num = "⁰¹²³⁴⁵⁶⁷⁸⁹"
+    lower_num = "₀₁₂₃₄₅₆₇₈₉"
+    upper_letter = "ⁱⁿ"
+    lower_letter = "ₐₑₒₓₕₖₗₘₙₚₛₜ"
+    other_upper_string = "⁺⁻⁼⁽⁾"
+    other_lower_string = "₊₋₌₍₎"
+    tem = '℃'
+    temF = '℉'
+    other1 = "^"
+    other2 = " ‰  ₔ._α β χ δ ε η γ ι κ λ μ ν ω ο φ πψ ρ σ τ θ υ ξ ζ"
+
+    # 字母 大写
+    def letter_big_to_small(self, msg):
+        # 创建字符映射表
+        maketrans = str.maketrans(StrUpperLower.letter_big, StrUpperLower.letter_small)
+        return msg.translate(maketrans)
+
+    def letter_small_to_big(self, msg):
+        # 创建字符映射表
+        maketrans = str.maketrans(StrUpperLower.letter_small, StrUpperLower.letter_big)
+        return msg.translate(maketrans)
+
+    def letter_lower(self, msg):
+        # 创建字符映射表
+        msg = msg.lower()
+        maketrans = str.maketrans("aeoxhklmnpst", StrUpperLower.lower_letter)
+        return msg.translate(maketrans)
+
+    def letter_upper(self, msg):
+        # 创建字符映射表
+        msg = msg.lower()
+        maketrans = str.maketrans("in", StrUpperLower.upper_letter)
+        return msg.translate(maketrans)
+
+    def num_lower(self, msg):
+        # 创建字符映射表
+        maketrans = str.maketrans(StrUpperLower.upper_num, StrUpperLower.lower_num)
+        return msg.translate(maketrans)
+
+    def num_upper(self, msg):
+        # 创建字符映射表
+        maketrans = str.maketrans(StrUpperLower.lower_num, StrUpperLower.upper_num)
+        return msg.translate(maketrans)
+    # def other_lower(self,msg):
+
+
+"""
+案例
+# 要转换的字符串
+formula = 'y=x3+2x2+3x+4'
+# 匹配出要转换的表示次幂的字符
+results = re.findall(r'x\d\+', formula)
+# 依次替换成上标的格式
+for s in results:
+    # s[:-1]的目的是让结尾的加号(+)不参与替换操作，因为“+”与通配符有冲突
+    formula = re.sub(s[:-1], s[:-1].translate(sup_map), formula)
+print(formula)  # 输出：y=x³+2x²+3x+4
+
+"""
+
+
 # 字符串判断
 class StringJudge(object):
     # <editor-fold desc="所有字符都是数字或者字母">
     @staticmethod
     def isalnum(str):
         """
         :param str: 字符串
```

### Comparing `basic_type_operations-0.0.2/basic_type_operations/tuple_operation.py` & `basic_type_operations-0.0.3/basic_type_operations/tuple_operation.py`

 * *Files identical despite different names*

### Comparing `basic_type_operations-0.0.2/basic_type_operations.egg-info/PKG-INFO` & `basic_type_operations-0.0.3/basic_type_operations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: basic-type-operations
-Version: 0.0.2
+Version: 0.0.3
 Summary: Short description
-Home-page: https://github.com/SkyOceanchen/basic_type_operations.git
+Home-page: https://gitee.com/SkyOceanchen/basic_type_operations.git
 Author: SkyOceanChen
 Author-email: skyoceanchen@foxmail.com
 License: MIT
 Keywords: basic_type,python,str,list,numpy,number,datetime,time,calendar
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `basic_type_operations-0.0.2/basic_type_operations.egg-info/SOURCES.txt` & `basic_type_operations-0.0.3/basic_type_operations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basic_type_operations-0.0.2/setup.py` & `basic_type_operations-0.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '0.0.2'  # Any format you want
+version = '0.0.3'  # Any format you want
 DESCRIPTION = 'Easily cut the basic type by basic_type_operations'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='basic_type_operations',
@@ -12,15 +12,15 @@
     version=version,
     license='MIT',
     description='Short description',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="SkyOceanChen",
     author_email="skyoceanchen@foxmail.com",
-    url='https://github.com/SkyOceanchen/basic_type_operations.git',
+    url='https://gitee.com/SkyOceanchen/basic_type_operations.git',
     keywords=['basic_type', 'python', "str", "list", "numpy", "number", "datetime", "time", 'calendar'],
     install_requires=[
         # All external pip packages you are importing
         'numpy',
         'fuzzywuzzy',
         'pinyin',
         'djangorestframework',
@@ -31,8 +31,12 @@
         'Operating System :: OS Independent',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.10',
     ],
 )
-# python setup.py bdist_wheel sdist
+"""
+python setup.py bdist_wheel sdist
+twine upload dist/*
+SkyOceanChen/CHNEziqing527#
+"""
```

