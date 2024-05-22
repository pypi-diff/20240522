# Comparing `tmp/txdpy-7.7.1.tar.gz` & `tmp/txdpy-7.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\86186\Desktop\?????\txdpy\txdpy\dist\.tmp-yb2on2wa\txdpy-7.7.1.tar", last modified: Fri May 10 08:33:56 2024, max compression
+gzip compressed data, was "C:\Users\86186\Desktop\?????\txdpy\txdpy\dist\.tmp-3jjz0bka\txdpy-7.7.2.tar", last modified: Wed May 22 10:14:54 2024, max compression
```

## Comparing `txdpy-7.7.1.tar` & `txdpy-7.7.2.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 08:33:56.000000 txdpy-7.7.1/
--rw-rw-rw-   0        0        0       71 2024-05-10 08:33:56.000000 txdpy-7.7.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-10 08:33:56.000000 txdpy-7.7.1/setup.cfg
--rw-rw-rw-   0        0        0      378 2024-05-10 08:33:26.000000 txdpy-7.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:33:56.000000 txdpy-7.7.1/txdpy/
--rw-rw-rw-   0        0        0    39935 2024-03-21 05:24:55.000000 txdpy-7.7.1/txdpy/URLjoin.py
--rw-rw-rw-   0        0        0     2881 2024-05-10 08:31:02.000000 txdpy-7.7.1/txdpy/__init__.py
--rw-rw-rw-   0        0        0    28642 2024-05-10 07:26:22.000000 txdpy-7.7.1/txdpy/bk_179.py
--rw-rw-rw-   0        0        0     3855 2024-04-30 03:54:19.000000 txdpy-7.7.1/txdpy/easyreq.py
--rw-rw-rw-   0        0        0     2403 2024-05-08 01:15:10.000000 txdpy-7.7.1/txdpy/excel_easy.py
--rw-rw-rw-   0        0        0     2472 2024-04-10 04:32:34.000000 txdpy-7.7.1/txdpy/get_key.py
--rw-rw-rw-   0        0        0     1715 2024-03-21 05:24:55.000000 txdpy-7.7.1/txdpy/list_processing.py
--rw-rw-rw-   0        0        0     1515 2024-03-21 05:24:55.000000 txdpy-7.7.1/txdpy/lookup.py
--rw-rw-rw-   0        0        0     2850 2024-03-22 06:06:06.000000 txdpy-7.7.1/txdpy/progress_display.py
--rw-rw-rw-   0        0        0     9985 2024-05-10 08:32:05.000000 txdpy-7.7.1/txdpy/pytmysql.py
--rw-rw-rw-   0        0        0    11855 2024-04-07 07:33:20.000000 txdpy-7.7.1/txdpy/read_data.py
--rw-rw-rw-   0        0        0     3049 2024-04-16 09:49:08.000000 txdpy-7.7.1/txdpy/requests_operation.py
--rw-rw-rw-   0        0        0     2031 2024-03-21 05:24:55.000000 txdpy-7.7.1/txdpy/selenium_Firefox.py
--rw-rw-rw-   0        0        0      933 2024-03-21 05:24:55.000000 txdpy-7.7.1/txdpy/str_category.py
--rw-rw-rw-   0        0        0     1042 2024-04-03 08:33:24.000000 txdpy-7.7.1/txdpy/text_similar.py
--rw-rw-rw-   0        0        0      623 2024-03-21 05:24:55.000000 txdpy-7.7.1/txdpy/translate.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:33:56.000000 txdpy-7.7.1/txdpy.egg-info/
--rw-rw-rw-   0        0        0       71 2024-05-10 08:33:56.000000 txdpy-7.7.1/txdpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2024-05-10 08:33:56.000000 txdpy-7.7.1/txdpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 08:33:56.000000 txdpy-7.7.1/txdpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-05-10 08:33:56.000000 txdpy-7.7.1/txdpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-10 08:33:56.000000 txdpy-7.7.1/txdpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 10:14:54.000000 txdpy-7.7.2/
+-rw-rw-rw-   0        0        0       71 2024-05-22 10:14:54.000000 txdpy-7.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-22 10:14:54.000000 txdpy-7.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      378 2024-05-22 10:14:08.000000 txdpy-7.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:14:54.000000 txdpy-7.7.2/txdpy/
+-rw-rw-rw-   0        0        0    39935 2024-03-21 05:24:55.000000 txdpy-7.7.2/txdpy/URLjoin.py
+-rw-rw-rw-   0        0        0     3208 2024-05-18 04:17:35.000000 txdpy-7.7.2/txdpy/__init__.py
+-rw-rw-rw-   0        0        0    29120 2024-05-22 04:14:09.000000 txdpy-7.7.2/txdpy/bk_179.py
+-rw-rw-rw-   0        0        0     3856 2024-05-15 07:29:14.000000 txdpy-7.7.2/txdpy/easyreq.py
+-rw-rw-rw-   0        0        0     2744 2024-05-22 08:33:27.000000 txdpy-7.7.2/txdpy/excel_easy.py
+-rw-rw-rw-   0        0        0     2472 2024-04-10 04:32:34.000000 txdpy-7.7.2/txdpy/get_key.py
+-rw-rw-rw-   0        0        0     1715 2024-03-21 05:24:55.000000 txdpy-7.7.2/txdpy/list_processing.py
+-rw-rw-rw-   0        0        0     1641 2024-05-11 06:16:59.000000 txdpy-7.7.2/txdpy/lookup.py
+-rw-rw-rw-   0        0        0     2850 2024-03-22 06:06:06.000000 txdpy-7.7.2/txdpy/progress_display.py
+-rw-rw-rw-   0        0        0     9986 2024-05-20 11:16:51.000000 txdpy-7.7.2/txdpy/pytmysql.py
+-rw-rw-rw-   0        0        0    13194 2024-05-22 06:32:12.000000 txdpy-7.7.2/txdpy/read_data.py
+-rw-rw-rw-   0        0        0     3049 2024-04-16 09:49:08.000000 txdpy-7.7.2/txdpy/requests_operation.py
+-rw-rw-rw-   0        0        0     2031 2024-03-21 05:24:55.000000 txdpy-7.7.2/txdpy/selenium_Firefox.py
+-rw-rw-rw-   0        0        0      932 2024-05-15 05:12:12.000000 txdpy-7.7.2/txdpy/str_category.py
+-rw-rw-rw-   0        0        0     1042 2024-04-03 08:33:24.000000 txdpy-7.7.2/txdpy/text_similar.py
+-rw-rw-rw-   0        0        0      623 2024-03-21 05:24:55.000000 txdpy-7.7.2/txdpy/translate.py
+-rw-rw-rw-   0        0        0     5184 2024-05-18 03:29:16.000000 txdpy-7.7.2/txdpy/文本括号及引号不匹配检查.py
+-rw-rw-rw-   0        0        0     1976 2024-05-22 01:10:29.000000 txdpy-7.7.2/txdpy/文本错别字检查.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:14:54.000000 txdpy-7.7.2/txdpy.egg-info/
+-rw-rw-rw-   0        0        0       71 2024-05-22 10:14:54.000000 txdpy-7.7.2/txdpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2024-05-22 10:14:54.000000 txdpy-7.7.2/txdpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 10:14:54.000000 txdpy-7.7.2/txdpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-05-22 10:14:54.000000 txdpy-7.7.2/txdpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-22 10:14:54.000000 txdpy-7.7.2/txdpy.egg-info/top_level.txt
```

### Comparing `txdpy-7.7.1/txdpy/URLjoin.py` & `txdpy-7.7.2/txdpy/URLjoin.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.1/txdpy/__init__.py` & `txdpy-7.7.2/txdpy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
            'is_num', 'is_Sletter', 'is_Bletter', 'is_letter', 'is_num_letter', 'is_chinese',
            'get_chinese', 'get_letter', 'get_Bletter', 'get_Sletter', 'get_Sletter', 'get_num', 'get_middle',
            'get_num_letter', 'webptablesl', 'req', 'dow_file', 'list_dupl', 'selenium_firefox', 'get_ssq','is_ssq',
            'prurar_code', 'convert_pc', 'convert_kl', 'delete_flase_empty', 'txdavg', 'txdmin',
            'txdperc', 'QueryScoreRank', 'timer', 'exenla', 'getexcelth', 'prvadepl', 'read_excel',
            'ExtractEnrollmentLabels', 'sortedlbys', 'UpdateName', 'optstr','progbar','text_similar'
            'Recognit_Data_Process','gen_excel','translate','ReadData','get_major_name','GetSchoolName',
-           'get_code_name','unify_keys','school_ljdm','MysqlConn'
+           'get_code_name','unify_keys','school_ljdm','MysqlConn','文本括号及引号不匹配检查','文本错别字检查方法一','文本错别字检查方法二'
            # 'PyBloomFilter'
            ]
 
 from .URLjoin import urljoin
 from .requests_operation import headers_dict
 from .requests_operation import param_dict
 from .requests_operation import webptablesl
@@ -62,8 +62,11 @@
 from .bk_179 import unify_keys
 from .bk_179 import school_ljdm
 from .excel_easy import read_excel
 from .excel_easy import gen_excel
 from .translate import translate
 from .read_data import ReadData
 from .progress_display import progbar
-from .text_similar import text_similar
+from .text_similar import text_similar
+from .文本括号及引号不匹配检查 import 文本括号及引号不匹配检查
+from .文本错别字检查 import 文本错别字检查方法一
+from .文本错别字检查 import 文本错别字检查方法二
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `txdpy-7.7.1/txdpy/bk_179.py` & `txdpy-7.7.2/txdpy/bk_179.py`

 * *Files 2% similar despite different names*

```diff
@@ -408,22 +408,22 @@
         :param major:专业名称
         :param batch:批次
         :param school_name:学校名称，学校名称中有“职业”关键字优先在职业本科查找专业名称信息
         :return:专业名称、专业名称逻辑代码、二级大类、二级大类逻辑代码、一级大类、一级大类逻辑代码
         """
         major_name = get_major_name(major)[0]
         if '专科' in batch:
-            return self.data.get('专科' + '_' + major_name, [None] * 6)
+            return self.data.get('专科' + '_' + major_name, [major_name]+[None] * 7)
         else:
             major_name = '本科预科班' if '预科' in major_name else major_name
             mana = self.data.get('本科' + '_' + major_name)
             if mana:
                 return mana
             if '职业' in school_name:
-                return self.data.get('职业本科' + '_' + major_name, [None] * 6)
+                return self.data.get('职业本科' + '_' + major_name, [major_name]+[None] * 7)
         return [None] * 6
 
 #对列表中的多个列表以第某个元素进行排序
 def sortedlbys(lists,i,reverse=False):
     """
     :param lists:数据列表
     :param i:一维数据中基准索引
@@ -516,15 +516,20 @@
     """
     def __init__(self):
         self.schools=sorted([x[0] for x in ReadData('院校名称').data[1:]], key=lambda x: len(x), reverse=True)
     def __call__(self,school):
         school=optstr(school)
         for school_name in self.schools:
             if school.startswith(school_name):
-                return [school_name,school.replace(school_name,'',1)]
+                院校备注 = school.replace(school_name,'',1) or None
+                if 院校备注:
+                    if 院校备注.startswith('('):
+                        院校备注 = 院校备注.strip('(').strip(')')
+                return [school_name,院校备注]
+        raise ValueError('院校名称和备注提取失败，院校名称未被添加到院校名称库')
 
 def get_code_name(s):
     """
     提取院校代码和名称或专业代码和名称
     """
     code = re.search('(^[0-9A-Za-z]+)', optstr(s)).group(1)
     name = optstr(s.lstrip(code))
@@ -551,19 +556,21 @@
                 if y==k1:
                     ks[i]=k2
                     break
     return ks
 
 def school_ljdm():
     """
-    返回院校逻辑代码
+    :return: 返回院校逻辑代码字典
     """
     schools = [x[0] for x in ReadData('院校名称').data[1:]]
     school_dict = {}
     for x in ReadData('院校库', ['院校逻辑代码', '院校名称']).data[1:]:
         school_name = optstr(x[1])
         x_0_re = re.search('\((.+?)\)', school_name)
         if x_0_re:
-            if x_0_re.group(1).strip('原') in schools:
-                school_name = school_name.replace(f'({x_0_re.group(1)})', '')
+            old_school_name = x_0_re.group(1)
+            if old_school_name.strip('原') in schools:
+                school_name = school_name.replace(f'({old_school_name})', '')
+                school_dict[old_school_name.strip('原')] = x[0]
         school_dict[school_name] = x[0]
     return school_dict
```

### Comparing `txdpy-7.7.1/txdpy/easyreq.py` & `txdpy-7.7.2/txdpy/easyreq.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         logger.info(f'\t地址：{url}\t\t状态码：' + Fore.YELLOW + str(res.status_code))
 
     return res
 
 def dow_file(path_name,href,add_suffix=True):
     """
     :param path_name: 下载路径及文件名，c:/a.pdf
-    :param src: 下载链接
+    :param href: 下载链接
     :return:
     """
     name = path_name.split('/')[-1]
     if add_suffix:
         path_name += '.'+href.split('.')[-1]
     print('开始下载：', name, href)
     res = requests.get(href, stream=True,verify=False)
```

### Comparing `txdpy-7.7.1/txdpy/excel_easy.py` & `txdpy-7.7.2/txdpy/excel_easy.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,18 +14,20 @@
     if header:
         data = list(data)
         data.insert(0,header)
     workbook = xlsxwriter.Workbook(save_path if save_path.endswith('.xlsx') else f'{save_path}.xlsx')
     sheet = workbook.add_worksheet()
     for row_num, row_data in enumerate(tqdm(data,desc=f'{os.path.basename(save_path)}')):
         for col_num, col_value in enumerate(row_data):
-            if is_optstr:
-                sheet.write(row_num, col_num, optstr(col_value if col_value is None else str(col_value)))
-            else:
-                sheet.write(row_num, col_num, col_value)
+            if col_value:
+                if is_optstr:
+                    col_value = optstr(col_value)
+            if type(col_value) not in [int, float] and col_value is not None:
+                col_value = str(col_value)
+            sheet.write(row_num, col_num, col_value)
     workbook.close()
 
 #读取execl数据
 def read_excel(file_path,sheet_index=0):
     """
     :param file_path:文件路径或路径下第一个文件
     :param sheet_index:工作表索引默认第一个
@@ -45,15 +47,26 @@
             workbook = load_workbook(filename=file_path,read_only=True)
             worksheet = workbook.worksheets[sheet_index]
             for row in worksheet.iter_rows():
                 datas.append([prvadepl(cell.value) if isinstance(cell.value, float) else cell.value for cell in row])
         except zipfile.BadZipFile:
             from txdpy import webptablesl
             with open(file_path, 'r', encoding='utf-8') as f:
-                return webptablesl(f.read(), '//table')
+                datas = webptablesl(f.read(), '//table')
     elif file_path.endswith('.xls'):
         import xlrd
         workbook = xlrd.open_workbook(file_path)
         sheet_by_index = workbook.sheet_by_index(sheet_index)
         for row_idx in range(sheet_by_index.nrows):
             datas.append([prvadepl(cell) if isinstance(cell, float) else cell for cell in sheet_by_index.row_values(row_idx)])
-    return datas
+
+    i = [i for i, l in enumerate(datas[0]) if not l and datas[0][i - 1]]
+
+    data = []
+    if i:
+        i = i[-1]
+        for l in datas:
+            if any(l): data.append(l[:i])
+    else:
+        for l in datas:
+            if any(l): data.append(l)
+    return data
```

### Comparing `txdpy-7.7.1/txdpy/get_key.py` & `txdpy-7.7.2/txdpy/get_key.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.1/txdpy/list_processing.py` & `txdpy-7.7.2/txdpy/list_processing.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.1/txdpy/lookup.py` & `txdpy-7.7.2/txdpy/lookup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 import re
 
 #提取汉字
 def get_chinese(s:str):
-    """
+    """提取汉字
     :param s: 提取的字符串
     :return: 返回提取结果列表
     """
     return re.findall('([\u4e00-\u9fa5]+)',s)
 
 #提取字母
 def get_letter(s:str):
-    """
+    """提取字母
     :param s: 提取的字符串
     :return: 返回提取结果列表
     """
     return re.findall('([a-zA-Z]+)',s)
 
 #提取大写字母
 def get_Bletter(s:str):
-    """
+    """提取大写字母
     :param s: 提取的字符串
     :return: 返回提取结果列表
     """
     return re.findall('([A-Z]+)',s)
 
 #提取小写字母
 def get_Sletter(s:str):
-    """
+    """提取小写字母
     :param s: 提取的字符串
     :return: 返回提取结果列表
     """
     return re.findall('([a-z]+)',s)
 
 #提取数字
 def get_num(s:str):
-    """
+    """提取数字
     :param s: 提取的字符串
     :return: 返回提取结果列表
     """
     return re.findall('([0-9]+)',s)
 
 #提取数字或字母或数字和字母
 def get_num_letter(s:str):
-    """
+    """提取数字或字母或数字和字母
     :param s: 提取的字符串
     :return: 返回提取结果列表
     """
     return re.findall('([0-9a-zA-Z]+)',s)
 
 #自定义提取
 def get_middle(s:str,front:str,after:str,contain=True):
-    """
+    """自定义提取
     :param front: 开头字符串
     :param after: 结尾字符串
     :param s: 查找字符串
     :param contain: 是否包含开头和末尾的字符串
     :return: 返回提取结果列表
     """
     if contain:
```

### Comparing `txdpy-7.7.1/txdpy/progress_display.py` & `txdpy-7.7.2/txdpy/progress_display.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.1/txdpy/pytmysql.py` & `txdpy-7.7.2/txdpy/pytmysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,17 +64,17 @@
             self.db.close()
         if self.server:
             self.server.close()
         logger.info(f'已断开与MySQL数据库的连接')
 
     def insert(self, table_name, data_pass: Union[dict, List[dict]]):
         """  mysql插入数据
-       :param table_name 表名
-       :param data_pass 参数接收字典/列表[字典] 格式
-       """
+        :param table_name 表名
+        :param data_pass 参数接收字典/列表[字典] 格式
+        """
         if not data_pass or not self.cursor:
             logger.error(f'数据列表为空或连接未建立')
             return
         try:
             if isinstance(data_pass, list):
                 keys = set().union(*data_pass)
                 columns = ', '.join(keys) # 构建SQL语句中的列名部分
@@ -94,15 +94,14 @@
                     self.db.commit()
                 logger.success(f"{self.cursor.rowcount} 条记录插入成功")
 
         except Exception as e:
             logger.error(f"插入数据时发生错误: {translate(str(e))}")
 
 class PyMySQL:
-
     def __init__(self, host: str = 'localhost', port=3306, user: str = 'root', password: str = '', database: str = '',
                  auto_add_key=False):
         """
         :param host: 默认本地地址
         :param user: 默认root
         :param password: 数据库密码
         :param database: 数据库
```

### Comparing `txdpy-7.7.1/txdpy/read_data.py` & `txdpy-7.7.2/txdpy/read_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # coding:utf-8
 
 import json, pymysql, re, xlrd,xlsxwriter,os
 from typing import Union,List
 from loguru import logger
 from sshtunnel import SSHTunnelForwarder
 from tqdm import tqdm
+import zipfile
 
 class ReadData:
     """
     读取mysql和.xlsx文件数据，提供一些方便的方法
     """
     def __init__(self,xlsx_mysql_sql:Union[str,List[List]],needful_field:List[str]=None,select_sql=None,xlsx_sheet_index=0,replace_th=True):
         """
@@ -27,44 +28,48 @@
         data_info = xlsx_mysql_sql
         if type(data_info) == list:
             if all(isinstance(sub_lst, list) for sub_lst in data_info):
                 self.data = data_info
                 self.data[0] = [str(f) for f in self.data[0]]  # 数据第一行必须作为列索引且为字段名称类型字符串
             else:
                 raise ValueError('数据必须是二维列表')
-        elif data_info.endswith('.xlsx'):  # 判断是否为.xlsx文件读取数据
-            self.read_xlsx(data_info, xlsx_sheet_index)
+        elif data_info.endswith('.xlsx') or data_info.endswith('.xls'):  # 判断是否为.xlsx文件读取数据
+            self.read_excel(data_info, xlsx_sheet_index)
+
         else:
             self.read_mysql(data_info, select_sql)  # 当做查询数据库数据
 
         # 替换表头字段名称为中文
         self.data[0] = self.replace_th_name(self.data[0])
 
         if len(self.data) == 0:
             raise ValueError('表格数据为空，此类(ReadData)读取数据第一行必须用作为索引')
 
         self.column_index = {field: i for i, field in enumerate(self.data[0])}  # 创建列索引
 
         if needful_field:  # 判断是否有需要保留的字段，按保留的字段保留数据
             self.reserve_needful_field(needful_field)
 
-        self.abnormal_inspection(list(self.column_index.keys()))  # 异常数据检查
+        # self.abnormal_inspection(list(self.column_index.keys()))  # 异常数据检查
 
         for k, v in self.column_index.items():
-            exec(f'self.{k}={v}')
+            try:
+                exec(f'self.{k}={v}')
+            except:
+                pass
 
         self.len_row = len(self.data)  # 行数
         self.len_col = len(self.data[0])  # 列数
 
     def connect_mysql(self):
         self.db = pymysql.connect(host=self.mysql_config["1"]['host'], port=3306, user='root',
                                   password=self.mysql_config["1"]['password'],
                                   database=self.mysql_config["1"]['database'])
         self.cursor = self.db.cursor()
-        self.cursor.execute("""select * from 表名称对应关系""")
+        self.cursor.execute("""select * from 公司表名称对应关系""")
         self.table_dict = {k: v for k, v in (v[0].split(':') for v in self.cursor.fetchall())}
 
     def select_mysql_data(self, sql, table_name=None):
         if not table_name: table_name = extract_table_name(sql)
         if table_name in self.table_dict.values():
             if 'information_schema.COLUMNS' in sql:
                 sql = sql.replace('需要替换的数据库名称', self.mysql_config["2"]['db'])
@@ -95,18 +100,17 @@
         table_name = self.table_dict.get(table_name, table_name)
         table_header = self.select_mysql_data(f"""SELECT COLUMN_NAME   
                                 FROM information_schema.COLUMNS
                                 WHERE TABLE_SCHEMA = '需要替换的数据库名称' AND TABLE_NAME = '{table_name}'   
                                 ORDER BY ORDINAL_POSITION ASC;""", table_name)
         return [k[0] for k in table_header]
 
-    def replace_th_name(self, lit):  # 替换表头名称
+    def replace_th_name(self, lit): # 替换表头名称
         if not self.replace_th: return lit
-        th_dict = {k: v for k, v in
-                   (v[0].split(':') for v in self.select_mysql_data("""select * from 表头字段对应名称"""))}
+        th_dict = {k: v for k, v in (v[0].split(':') for v in self.select_mysql_data("""select * from 表头字段对应名称"""))}
         new_name = []
         for name in lit:
             new_name.append(th_dict.get(name, name))
         return new_name
 
     def read_mysql(self, name, select_sql):
         if name[:6].lower() == 'select':
@@ -126,42 +130,65 @@
             self.table_name = name
             table_name = self.table_dict.get(name, name)
             self.data.append(self.replace_th_name(self.get_th(table_name)))
             sql = f"""select * from `{table_name}`{' where ' + select_sql if select_sql else ''}"""
             logger.info(sql)
             self.data += [list(v) for v in self.select_mysql_data(sql)]
 
-    def read_xlsx(self, file_path, sheet_index):
+    # 读取execl数据
+    def read_excel(self, file_path, sheet_index=0):
         """
         :param file_path:文件路径或路径下第一个文件
         :param sheet_index:工作表索引默认第一个
+        return:表格数据
         """
-        # 打开Excel文件并获取工作表
-        workbook = xlrd.open_workbook(file_path)
-        worksheet = workbook.sheet_by_index(sheet_index)
-        # 遍历每一行数据
-        for i in range(worksheet.nrows):
-            self.data.append(worksheet.row_values(i))
-
+        if not file_path.endswith('.xlsx') and not file_path.endswith('.xls'):
+            file_paths = ls(file_path)
+            for path in file_paths:
+                if path.endswith('.xlsx') or path.endswith('.xls'):
+                    file_path = path
+                    break
+
+        datas = []
+        if file_path.endswith('.xlsx'):
+            from openpyxl import load_workbook
+            try:
+                workbook = load_workbook(filename=file_path, read_only=True)
+                worksheet = workbook.worksheets[sheet_index]
+                for row in worksheet.iter_rows():
+                    datas.append(
+                        [prvadepl(cell.value) if isinstance(cell.value, float) else cell.value for cell in row])
+            except zipfile.BadZipFile:
+                from txdpy import webptablesl
+                with open(file_path, 'r', encoding='utf-8') as f:
+                    datas = webptablesl(f.read(), '//table')
+        elif file_path.endswith('.xls'):
+            import xlrd
+            workbook = xlrd.open_workbook(file_path)
+            sheet_by_index = workbook.sheet_by_index(sheet_index)
+            for row_idx in range(sheet_by_index.nrows):
+                datas.append([prvadepl(cell) if isinstance(cell, float) else cell for cell in
+                              sheet_by_index.row_values(row_idx)])
+        self.data = [row for row in datas if any(row)]
         self.data[0] = [str(f) for f in self.data[0]]  # 数据第一行必须作为列索引且为字段名称类型字符串
 
-    def abnormal_inspection(self, header):
-        """
-        数据异常检查
-        """
-        if '' in header:
-            raise ValueError('表头存在空字符串')
-        for char in ',', '-', '、':
-            if char in ''.join(header):
-                raise ValueError(f'表头名称不允许出现“{char}”')
-        for v in header:
-            if is_num(v):
-                raise ValueError('表头名称不允许出现纯自然数')
-        if len(header) != len(set(header)):
-            raise ValueError('表头字段不允许出现出重复名称')
+    # def abnormal_inspection(self, header):
+    #     """
+    #     数据异常检查
+    #     """
+        # if '' in header:
+        #     raise ValueError('表头存在空字符串')
+        # for char in ',', '-', '、':
+        #     if char in ''.join(header):
+        #         raise ValueError(f'表头名称不允许出现“{char}”')
+        # for v in header:
+        #     if is_num(v):
+        #         raise ValueError('表头名称不允许出现纯自然数')
+        # if len(header) != len(set(header)):
+        #     raise ValueError('表头字段不允许出现出重复名称')
 
     def reserve_needful_field(self, needful_field):
         """
         保留数据所需字段
         """
         data = []
         for row in self.data:
```

### Comparing `txdpy-7.7.1/txdpy/requests_operation.py` & `txdpy-7.7.2/txdpy/requests_operation.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.1/txdpy/selenium_Firefox.py` & `txdpy-7.7.2/txdpy/selenium_Firefox.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.1/txdpy/str_category.py` & `txdpy-7.7.2/txdpy/str_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 #判断是否为纯数字和字母
 def is_num_letter(s):
     if type(s)==int:
         return True
     if type(s)!=str:
         return False
-    if re.search('^([0-9a-zA-Z]+)$',s):
+    if re.search('^([\da-zA-Z]+)$',s):
         return True
     return False
 
 #判断是否为纯汉字
 def is_chinese(s:str):
     if re.search('^([\u4e00-\u9fa5]+)$',s):
         return True
```

### Comparing `txdpy-7.7.1/txdpy/text_similar.py` & `txdpy-7.7.2/txdpy/text_similar.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.1/txdpy/translate.py` & `txdpy-7.7.2/txdpy/translate.py`

 * *Files identical despite different names*

