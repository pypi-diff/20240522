# Comparing `tmp/Fr1997v011-1.5.6.tar.gz` & `tmp/Fr1997v011-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.5.6.tar", last modified: Thu May 16 08:09:48 2024, max compression
+gzip compressed data, was "Fr1997v011-1.5.8.tar", last modified: Tue May 21 11:21:26 2024, max compression
```

## Comparing `Fr1997v011-1.5.6.tar` & `Fr1997v011-1.5.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 08:09:48.389280 Fr1997v011-1.5.6/
-drwxrwxrwx   0        0        0        0 2024-05-16 08:09:48.381280 Fr1997v011-1.5.6/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-05-16 08:09:48.000000 Fr1997v011-1.5.6/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-05-16 08:09:48.000000 Fr1997v011-1.5.6/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 08:09:48.000000 Fr1997v011-1.5.6/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-16 08:09:48.000000 Fr1997v011-1.5.6/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-05-16 08:09:48.000000 Fr1997v011-1.5.6/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.5.6/LICENSE
--rw-rw-rw-   0        0        0      182 2024-05-16 08:09:48.388291 Fr1997v011-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-05-16 08:09:46.000000 Fr1997v011-1.5.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 08:09:48.382280 Fr1997v011-1.5.6/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.5.6/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:09:48.385280 Fr1997v011-1.5.6/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.5.6/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   180774 2024-05-16 08:07:59.000000 Fr1997v011-1.5.6/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:09:48.387280 Fr1997v011-1.5.6/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.5.6/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-16 08:09:48.389280 Fr1997v011-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-05-16 08:08:41.000000 Fr1997v011-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:21:26.392385 Fr1997v011-1.5.8/
+drwxrwxrwx   0        0        0        0 2024-05-21 11:21:26.384378 Fr1997v011-1.5.8/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-05-21 11:21:26.000000 Fr1997v011-1.5.8/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-21 11:21:26.000000 Fr1997v011-1.5.8/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 11:21:26.000000 Fr1997v011-1.5.8/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-21 11:21:26.000000 Fr1997v011-1.5.8/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-05-21 11:21:26.000000 Fr1997v011-1.5.8/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.5.8/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-05-21 11:21:26.391384 Fr1997v011-1.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-05-17 03:42:08.000000 Fr1997v011-1.5.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 11:21:26.386389 Fr1997v011-1.5.8/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.5.8/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:21:26.388385 Fr1997v011-1.5.8/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.5.8/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   161603 2024-05-21 11:21:23.000000 Fr1997v011-1.5.8/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:21:26.390387 Fr1997v011-1.5.8/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.5.8/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-21 11:21:26.393384 Fr1997v011-1.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-05-21 11:21:23.000000 Fr1997v011-1.5.8/setup.py
```

### Comparing `Fr1997v011-1.5.6/LICENSE` & `Fr1997v011-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.5.6/README.md` & `Fr1997v011-1.5.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.5.6.tar.gz
+pip install dist/Fr1997v011-1.5.7.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.5.6/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.5.8/fr1997_mode/mode_func/all_func.py`

 * *Files 4% similar despite different names*

```diff
@@ -394,14 +394,15 @@
     def add_rate(v_new, v_old):
         if v_new == 0 or v_old == 0:
             rate = 0
         else:
             rate = round((v_new - v_old) / v_old * 100, 2)
         return rate
 
+
 # requests 封装
 class HttpJike(object):
 
     def __init__(self):
         self.status_code = 500
         self.msg = 'ok'
         self.text = None
@@ -1497,15 +1498,15 @@
         base_ret_data['play_num'] = 0
         base_ret_data['good_count'] = like_num
         base_ret_data['comment_count'] = comment_num
         base_ret_data['share_count'] = forward_num
         base_ret_data['collect_count'] = collect_count
         base_ret_data['user_id'] = user_id
 
-        base_ret_data['update_time'] = int(time.time()),
+        base_ret_data['update_time'] = int(time.time())
         base_ret_data['create_date'] = create_time
         base_ret_data['release_time'] = release_time
         base_ret_data['nickname'] = nickname
         base_ret_data['author_head'] = author_head
         base_ret_data['describe'] = describe
 
         base_ret_data['download_addr_url_list2'] = download_addr_url_list2
@@ -2114,15 +2115,15 @@
 
         base_ret_data['play_num'] = 0
         base_ret_data['good_count'] = like_num
         base_ret_data['comment_count'] = comment_num
         base_ret_data['share_count'] = forward_num
         base_ret_data['collect_count'] = collect_count
 
-        base_ret_data['update_time'] = int(time.time()),
+        base_ret_data['update_time'] = int(time.time())
         base_ret_data['create_date'] = create_time
         base_ret_data['release_time'] = release_time
         base_ret_data['nickname'] = nickname
         base_ret_data['describe'] = describe
 
         if tp == 'django_video_info':
             return {
@@ -2772,14 +2773,24 @@
                 elif method == 'select' or method == 's':
                     cursor.execute(sql)
                     return cursor.fetchall()
                 elif method == 'del_table' or method == 'dt':
                     sql_del = f'DROP TABLE {table}'
                     cursor.execute(sql_del)
                     conn.commit()
+                elif method == 'in':
+                    field = kwargs.get('field')
+                    by_id = kwargs.get('by_id')
+                    id_list = kwargs.get('id_list')
+                    if not id_list or not field or not by_id:
+                        return ()
+                    format_strings = ','.join(['%s'] * len(id_list))
+                    sql_in = f"SELECT {field} FROM {table} WHERE {by_id} IN ({format_strings})"
+                    cursor.execute(sql_in, id_list)
+                    return cursor.fetchall()
                 else:
                     cursor.execute(sql)
                     return cursor.fetchall()
         except Exception as e:
             print(f"数据库链接错误:{e}")
         finally:
             conn.close()
@@ -3980,495 +3991,14 @@
                 Method='GET',
             )
             return download_url
         except Exception as E:
             print('Fr包err cnd获取路径失败', E)
 
 
-# FastGpt
-class FastGptAuto:
-
-    def __init__(self, **kwargs):
-        self.run_path = int(kwargs.get('run_path', 2))  # 2测试 01正式
-        self.avatar = "/icon/logo.svg"
-
-        # 正式|测试
-        if self.run_path == 2:
-            self.conn_tp = 2
-            self.base_url = 'http://101.35.29.36:3020/api'
-            self.authorization = 'fastgpt-nE4z8uvJrrh5N1OvvdjDFG7Y055Rj9xVVXKeVSghM1cFAr1zXRUMdxm5v7a6pC'
-        else:
-            self.conn_tp = ModeFunc().path
-            self.base_url = 'https://aitest.dso100.com/api'
-            self.authorization = 'fastgpt-nE4z8uvJrrh5N1OvvdjDFG7Y055Rj9xVVXKeVSghM1cFAr1zXRUMdxm5v7a6pC'
-
-        self.user_text_table = 'cd_douyin_user_video_text'
-        self.es_user_text_table = 'douyin_user_video_text'
-        self.all_dataset_table = 'cd_fast_article_dataset'
-
-    # 通过后台生成的token https://aitest.dso100.com/account?currentTab=apikey
-    def get_header(self):
-        return {
-            'Authorization': f'Bearer {self.authorization}',
-            'user-agent': config_dict['base_ua'],
-        }
-
-    # 通过登录获取的token
-    def get_token_header(self, refresh=0):
-        key = 'fastgpt_token_v1'
-        token = cache_get(key)
-        if not token or refresh == 1:
-            url = f'{self.base_url}/support/user/account/loginByPassword'
-            data = {"username": "root", "password": "45d257ac8225ef3436843c66083736af23a24e7fd63a57f712e60e19c39248be"}
-            res = requests.post(url=url, json=data)
-            token = res.json()['data']['token']
-            cache_set(key, token, 3600)
-        return {
-            'cookie': f'token={token}',
-            'user-agent': config_dict['base_ua'],
-        }
-
-    # app list
-    def lit(self):
-        response = requests.get(f'{self.base_url}/core/app/list', headers=self.get_token_header())
-        print(response.json())
-
-    # 应用 创建
-    def app_create(self, member_id):
-        sql = 'SELECT name,json_data FROM `cd_python_json` where `name` = "fastgpt_app_create_json"'
-        all_data = mode_pro.mysql_db(method="s", table="cd_python_json", sql=sql)
-        for at in all_data:
-            fastgpt_app_create_json = json.loads(at[1])
-            time_data = time.strftime("%Y%m%d", time.localtime(int(time.time())))
-            fastgpt_app_create_json['avatar'] = "/icon/logo.svg"
-            fastgpt_app_create_json['name'] = f'{time_data}-{int(time.time())}-{str(member_id)}'
-            response = requests.post(f'{self.base_url}/core/app/create', headers=self.get_token_header(),
-                                     json=fastgpt_app_create_json)
-            if response.status_code == 200:
-                data_data = response.json()
-                code = data_data['code']
-                if code == 200:
-                    return data_data
-        return {'code': 500}
-
-    # 应用 创建key
-    def app_chat_key(self, member_id, appId):
-        data = {"name": member_id, "limit": {"maxUsagePoints": -1}, "appId": appId}
-        response = requests.post(f'{self.base_url}/support/openapi/create', headers=self.get_token_header(),
-                                 json=data)
-        if response.status_code == 200:
-            data_data = response.json()
-            code = data_data['code']
-            if code == 200:
-                return data_data
-        return {'code': 500}
-
-    # 应用 创建key
-    def app_log(self, member_id, appId):
-        url = f'{self.base_url}/core/chat/init?appId={appId}&chatId={member_id}&loadCustomFeedbacks=true'
-        params = (
-            ('appId', appId),
-            ('chatId', member_id),
-            ('loadCustomFeedbacks', 'true'),
-        )
-        response = requests.get(url, headers=self.get_token_header(), params=params)
-        if response.status_code == 200:
-            data_data = response.json()
-            code = data_data['code']
-            if code == 200:
-                return data_data
-        return {'code': 500}
-
-    # 应用 修改 【知识库】 【提示词】
-    def app_update(self, app_id, up_data):
-        response = requests.post(
-            f'{self.base_url}/core/app/update?appId={app_id}',
-            headers=self.get_token_header(),
-            json=up_data)
-        if response.status_code == 200:
-            data_data = response.json()
-            code = data_data['code']
-            if code == 200:
-                return data_data
-        return {'code': 500}
-
-    # 知识库 创建
-    def dataset_create(self, dataset_name):
-        data = {
-            "parentId": None,
-            "type": "dataset",
-            "name": dataset_name,
-            "intro": '',
-            "avatar": self.avatar,
-            "vectorModel": "text-embedding-ada-002",
-            "agentModel": 'gpt-3.5-turbo-1106'
-        }
-        response = requests.post(f'{self.base_url}/core/dataset/create', headers=self.get_header(), json=data)
-        if response.status_code == 200:
-            data_data = response.json()
-            code = data_data['code']
-            if code == 200:
-                return data_data['data']
-
-    # 知识库 全部
-    def dataset_look_all(self):
-        t = 'fastgpt-4HuWTuvo4niPmg5myRqxRAJWrGwXzShJ1DSJyjRfUnjyULmK5Zp2iL3'
-        response = requests.get(f'{self.base_url}/core/dataset/list?parentId=', headers=self.get_header())
-        return response.json()
-
-    # 知识库 详情
-    def dataset_look_info(self, dataset_id):
-        response = requests.get(f'{self.base_url}/core/dataset/detail?id={dataset_id}', headers=self.get_header())
-        return response.json()
-
-    # 知识库 删除
-    def dataset_del(self, dataset_id):
-        response = requests.get(f'{self.base_url}/core/dataset/delete?id={dataset_id}', headers=self.get_header())
-        return response.json()
-
-    # 集合 创建
-    def collection_create(self, dataset_name, collection_name='测试'):
-        data = {
-            "datasetId": dataset_name,
-            "parentId": None,
-            "name": collection_name,
-            "type": "virtual",
-            "metadata": {
-                "test": 111
-            }
-        }
-        response = requests.post(f'{self.base_url}/core/dataset/collection/create', headers=self.get_header(),
-                                 json=data)
-        if response.status_code == 200:
-            data_data = response.json()
-            print(data_data)
-            code = data_data['code']
-            if code == 200:
-                return data_data['data']
-
-    # 知识库 集合 列表
-    def dataset_collection_list(self, dataset_id):
-        data = {
-            "pageNum": 1,
-            "pageSize": 100,
-            "datasetId": dataset_id,
-            "parentId": "",
-            "searchText": ""
-        }
-        response = requests.get(f'{self.base_url}/core/dataset/collection/list', headers=self.get_header(), json=data)
-        return response.json()
-
-    # 集合 纯文本集合
-    def collection_create_txt(self, dataset_name):
-        data = {
-            "text": "我喜欢踢足球",
-            "datasetId": dataset_name,
-            "parentId": None,
-            "name": "足球",
-
-            "trainingType": "qa",
-            "chunkSize": 8000,
-            "chunkSplitter": "",
-            "qaPrompt": "11",
-
-            "metadata": {}
-        }
-        response = requests.post(f'{self.base_url}/core/dataset/collection/create/text', headers=self.get_header(),
-                                 json=data)
-        if response.status_code == 200:
-            data_data = response.json()
-            print(data_data)
-            code = data_data['code']
-            if code == 200:
-                return data_data['data']
-
-    # 集合 添加数据
-    def collection_push_data(self, collection_id, push_data):
-        """
-            [
-                {
-                    "q": "文本文本文本文本文本",
-                    "a": ""
-                },
-            ]
-        """
-        # 每次添加50个
-        err = 0
-        split_push_data = mode_data.list_avg_split(push_data, 50)
-        for each_push_data in split_push_data:
-            time.sleep(1)
-            data = {
-                "collectionId": collection_id,
-                "trainingMode": "chunk",
-                "prompt": "",
-                "billId": "",
-                "data": each_push_data
-            }
-            try:
-                response = requests.post(f'{self.base_url}/core/dataset/data/pushData', headers=self.get_header(),
-                                         json=data)
-                if response.status_code == 200:
-                    data_data = response.json()
-                    code = data_data['code']
-                    if code != 200:
-                        err = 1
-                else:
-                    err = 1
-            except:
-                err = 1
-
-        return err
-
-    # 时间转换
-    def time_frame_stamp(self, time_frame, create_time):
-        """
-            [time_frame,create_time]
-        """
-        if time_frame == '6个月':
-            return create_time - 86400 * 31 * 6  # 六个月前时间戳
-        elif time_frame == '1年':
-            return create_time - 86400 * 366  # 1年前前时间戳
-        elif time_frame == '全部':
-            return 0  # 全部时间戳
-        else:
-            return create_time - 86400 * 31 * 3  # 三个月前时间戳
-
-    # 上传
-    def up(self):
-
-        import requests
-
-        # 定义目标 URL
-        url = 'https://aitest.dso100.com/api/common/file/upload'
-
-        # 定义请求头
-        headers = {
-            'accept': 'application/json, text/plain, */*',
-            'accept-language': 'zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6',
-            'content-type': 'multipart/form-data; boundary=----WebKitFormBoundarys9RAEXfISllHiC8p',
-            'cookie': 'Hm_lvt_a65de9750f8989adcf4af692ae366a3f=1712413671,1713143431,1713332672,1713422297; token=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI2NjIwYjQzYzNmOTAxYjQyZmNlN2NjNjEiLCJ0ZWFtSWQiOiI2NjIwYjQzYzNmOTAxYjQyZmNlN2NjNjQiLCJ0bWJJZCI6IjY2MjBiNDNjM2Y5MDFiNDJmY2U3Y2M2NiIsImV4cCI6MTcxNDIwMTA4MCwiaWF0IjoxNzEzNTk2MjgwfQ.hq0BaQhwtGyy1uLBOTZxUdC_k3Q7XMkTTTcGLrEHqao; Hm_lpvt_a65de9750f8989adcf4af692ae366a3f=1713601305',
-            'origin': 'https://aitest.dso100.com',
-            'referer': 'https://aitest.dso100.com/dataset/detail?datasetId=662381dd3f901b42fce7f8d6&parentId=&currentTab=import&source=csvTable',
-            'sec-ch-ua': '"Microsoft Edge";v="123", "Not:A-Brand";v="8", "Chromium";v="123"',
-            'sec-ch-ua-mobile': '?0',
-            'sec-ch-ua-platform': '"Windows"',
-            'sec-fetch-dest': 'empty',
-            'sec-fetch-mode': 'cors',
-            'sec-fetch-site': 'same-origin',
-            'token': 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI2NjIwYjQzYzNmOTAxYjQyZmNlN2NjNjEiLCJ0ZWFtSWQiOiI2NjIwYjQzYzNmOTAxYjQyZmNlN2NjNjQiLCJ0bWJJZCI6IjY2MjBiNDNjM2Y5MDFiNDJmY2U3Y2M2NiIsImV4cCI6MTcxNDIwMTA4MCwiaWF0IjoxNzEzNTk2MjgwfQ.hq0BaQhwtGyy1uLBOTZxUdC_k3Q7XMkTTTcGLrEHqao',
-            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36 Edg/123.0.0.0',
-        }
-
-        # 定义文件路径
-        file_path = 'test_data.csv'
-
-        # 以二进制读取文件内容
-        with open(file_path, 'rb') as file:
-            # 构建文件对象
-            files = {'file': file}
-
-            # # 定义表单数据
-            # data = {
-            #     'metadata': {},
-            #     'bucketName': 'dataset',
-            # }
-
-            # 发送 POST 请求，同时上传文件和表单数据
-            response = requests.post(url, headers=headers, files=files)
-
-        print(response.text)
-
-    def te(self):
-
-        # # 定义目标 URL
-        # url = f'{self.base_url}/core/dataset/collection/create/file'
-        #
-        # # 定义文件路径
-        # file_path = 'C:/Users/30844\Documents\project_all\python_project\mofan\gy_pyhton_project/all_project/ai_fastgpt/fastgpt_mode.py'
-        #
-        # # 定义表单数据
-        # data = {"datasetId": "662377893f901b42fce7f115", "parentId": None, "trainingType": "chunk", "chunkSize": 512,
-        #         "chunkSplitter": "", "qaPrompt": "", "metadata": {}}
-        #
-        # # 以二进制读取文件内容
-        # with open(file_path, 'rb') as file:
-        #     # 构建文件对象
-        #     files = {'file': file}
-        #
-        #     # 发送 POST 请求，同时上传文件和表单数据
-        #     response = requests.post(url, headers=self.get_header(), files=files, json=data)
-        #
-        # # 检查响应状态码
-        # print(response.text)
-
-        url = 'https://aitest.dso100.com/api/core/dataset/collection/create/csvTable'
-        data = {
-            "parentId": "",
-            "trainingType": "chunk",
-            "datasetId": "662381dd3f901b42fce7f8d6",
-            "chunkSize": 700,
-            "chunkSplitter": "",
-            "qaPrompt": "<Context></Context> 标记中是一段文本，学习和分析它，并整理学习成果：\n- 提出问题并给出每个问题的答案。\n- 答案需详细完整，尽可能保留原文描述。\n- 答案可以包含普通文字、链接、代码、表格、公示、媒体链接等 Markdown 元素。\n- 最多提出 30 个问题。\n",
-            "name": "聚法帮法律咨询_2024-04-20 14_04_23.csv",
-            "fileId": "662380773f901b42fce7f6e7"
-        }
-        response = requests.post(url, headers=self.get_header(), json=data)
-        print(response.text)
-
-    def api_1(self):
-        headers = {
-            'Authorization': 'Bearer fastgpt-DPOEvxkScPWHI3G3T442ZXTS6KWy9oyMxmttl1obEgyOhOW22RYcjBlfi',
-            'Content-Type': 'application/json',
-        }
-
-        data = {
-            "chatId": "12419",
-            "stream": False,
-            "detail": False,
-            "messages": [
-                {
-                    "content": "如何快速提升",
-                    "role": "user"
-                }
-            ]
-        }
-        response = requests.post('http://101.35.29.36:3020/api/v1/chat/completions', headers=headers, json=data)
-        print(response.text)
-
-        # headers = {
-        #     'Authorization': 'Bearer fastgpt-MdBia1If20J3gKnrHHzHOnNUg4a53FQU8dGEure6QaVK8gJXa5d9VB2Dy',
-        #     'Content-Type': 'application/json',
-        # }
-        #
-        # data = {
-        #     "chatId": "6620b4b13f901b42fce7ccc1",
-        #     "stream": False,
-        #     "detail": False,
-        #     "messages": [
-        #         {
-        #             "content": "导演是谁",
-        #             "role": "user"
-        #         }
-        #     ]
-        # }
-        # response = requests.get('https://aitest.dso100.com/api/core/app/list', headers=headers)
-        # print(response.text)
-
-    # 整合 创建知识库—>
-    def func_create_dataset(self, dataset_name, push_data, save_info):
-        # 根据用户创建知识库
-        dataset_id = self.dataset_create(dataset_name)
-
-        # 增加数据集
-        collection_id = self.collection_create(dataset_id, '抖音文案')
-
-        # 添加数据
-        err = self.collection_push_data(collection_id, push_data)
-        if err:
-            fi = inspect.getframeinfo(inspect.currentframe())
-            mode_pro.err_log(fi, p=5, err_msg=f"创建知识库err，{dataset_name}", err_times=1, sleep=10, save_mysql=1)
-        else:
-            print("创建知识库成功")
-
-            # 标记
-            mode_pro.mysql_db(method='up', table=self.user_text_table, conn_tp=self.conn_tp, save_data=[{
-                'to_dataset': 1,
-                'id': save_info[0],
-            }])
-
-            # 新增知识库
-            mode_pro.mysql_db(method='iss', table=self.all_dataset_table, conn_tp=self.conn_tp, save_data=[{
-                'platform': 'douyin',
-                'user_id': save_info[1],
-                'sec_uid': save_info[2],
-                'nickname': save_info[3],
-                'time_frame_video_count': save_info[6],
-                'time_frame': save_info[5],
-                'text_create_time': save_info[4],
-                'is_upload': 0,
-                'create_time': int(time.time()),
-                'dataset_name': dataset_name,
-                'dataset_id': dataset_id,
-                'collection_id': collection_id,
-            }])
-
-    # 计划任务 达人文案库 -> 知识库
-    def user_text_to_dataset(self, h_id):
-        sql = f"""SELECT id,user_id,sec_uid,nickname,create_time,time_frame,time_frame_video_count,`state`,to_dataset
-         FROM {self.user_text_table} 
-         WHERE id = {h_id}"""  # to_dataset=0|1
-        all_data = mode_pro.mysql_db(method='s', table=self.user_text_table, sql=sql, conn_tp=self.conn_tp)
-        if not all_data:
-            return {'code': -1, 'msg': '数据不存在'}
-
-        i = all_data[0]
-        sec_uid = i[2]
-        nickname = i[3]
-        create_time = i[4]
-        time_frame = i[5]
-        if i[7] != 1:
-            return {'code': -1, 'msg': '数据转译中'}
-
-        if i[8] == 1:
-            return {'code': -1, 'msg': '知识库已添加'}
-
-        tf_stamp = self.time_frame_stamp(time_frame, create_time)
-        # 时间范围 视频
-        query = {
-            "bool": {
-                "must": [
-                    {"match": {"sec_uid": sec_uid}},
-                    {"match": {"aweme_type": 0}},
-                    {"range": {"create_time": {"gte": tf_stamp}}},
-                    {"range": {"create_time": {"lte": create_time}}},
-                ]
-            }
-        }
-        source = ['video_text']
-        data_data = mode_pro.es_search_new_20231215(table=self.es_user_text_table, query=query, _source=source,
-                                                    size=3000)
-
-        push_data = []  # 要添加知识库的文案
-        for v in data_data:
-            data_info = v['_source']
-            push_data.append({
-                "q": data_info.get('video_text', ''),
-                "a": ""
-            })
-
-        # 创建知识库
-        self.func_create_dataset(dataset_name=nickname, push_data=push_data, save_info=i)
-
-        return {'code': 1, 'msg': 'ok'}
-
-    # 计划任务 判断知识库文案装填成功
-    def dataset_is_upload(self):
-        save_data = []
-        sql = f'SELECT id,dataset_id,collection_id FROM {self.all_dataset_table} where is_upload = 0'
-        all_data = mode_pro.mysql_db(method='s', table=self.all_dataset_table, sql=sql, conn_tp=self.conn_tp)
-        for i in all_data:
-            print(i)
-            id_id = i[0]
-            dataset_id = i[1]
-            collection_id = i[2]
-            data_info = self.dataset_collection_list(dataset_id)
-            c_list = data_info['data']['data']
-            for ci in c_list:
-                if ci['_id'] == collection_id:
-                    if ci['trainingAmount'] == 0:
-                        save_data.append({
-                            'is_upload': 1,
-                            'id': id_id
-                        })
-                        continue
-
-        if save_data:
-            mode_pro.mysql_db(method='up', table=self.all_dataset_table, conn_tp=self.conn_tp, save_data=save_data)
-
-
 class RetJson:
 
     @classmethod
     def data_list(cls, data):
         if data is None:
             return []
         return data
@@ -4557,7 +4087,8 @@
 mode_xhs = XhsJike()  # douyin配置
 mode_pros = ModeStatic()  # 其它函数
 mode_cos = Cos()  # cos
 mode_fr_cos = Cos(server_select='personal')  # cos 高阳
 mode_myself = MyGy()
 
 mode_pro = ModeFunc()  # main
+
```

