# Comparing `tmp/Fiicen-py-1.0.0.tar.gz` & `tmp/Fiicen-py-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fiicen-py-1.0.0.tar", last modified: Wed May 22 09:51:44 2024, max compression
+gzip compressed data, was "Fiicen-py-1.1.0.tar", last modified: Wed May 22 12:25:04 2024, max compression
```

## Comparing `Fiicen-py-1.0.0.tar` & `Fiicen-py-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 09:51:44.835387 Fiicen-py-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-05-22 09:51:44.815436 Fiicen-py-1.0.0/Fiicen_py.egg-info/
--rw-rw-rw-   0        0        0     2258 2024-05-22 09:51:44.000000 Fiicen-py-1.0.0/Fiicen_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-22 09:51:44.000000 Fiicen-py-1.0.0/Fiicen_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 09:51:44.000000 Fiicen-py-1.0.0/Fiicen_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-22 09:51:44.000000 Fiicen-py-1.0.0/Fiicen_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2258 2024-05-22 09:51:44.835387 Fiicen-py-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1771 2024-05-22 09:48:32.000000 Fiicen-py-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 09:51:44.834867 Fiicen-py-1.0.0/fiicen_py/
--rw-rw-rw-   0        0        0      113 2024-05-22 09:13:24.000000 Fiicen-py-1.0.0/fiicen_py/__init__.py
--rw-rw-rw-   0        0        0     3417 2024-05-22 09:44:22.000000 Fiicen-py-1.0.0/fiicen_py/main.py
--rw-rw-rw-   0        0        0       42 2024-05-22 09:51:44.835387 Fiicen-py-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      740 2024-05-22 09:12:35.000000 Fiicen-py-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:25:04.472274 Fiicen-py-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-05-22 12:25:04.454332 Fiicen-py-1.1.0/Fiicen_py.egg-info/
+-rw-rw-rw-   0        0        0     2987 2024-05-22 12:25:04.000000 Fiicen-py-1.1.0/Fiicen_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-22 12:25:04.000000 Fiicen-py-1.1.0/Fiicen_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 12:25:04.000000 Fiicen-py-1.1.0/Fiicen_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 12:25:04.000000 Fiicen-py-1.1.0/Fiicen_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2987 2024-05-22 12:25:04.471057 Fiicen-py-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2486 2024-05-22 12:22:13.000000 Fiicen-py-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 12:25:04.469910 Fiicen-py-1.1.0/fiicen_py/
+-rw-rw-rw-   0        0        0      113 2024-05-22 12:01:12.000000 Fiicen-py-1.1.0/fiicen_py/__init__.py
+-rw-rw-rw-   0        0        0     5426 2024-05-22 12:00:56.000000 Fiicen-py-1.1.0/fiicen_py/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 12:25:04.472274 Fiicen-py-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      740 2024-05-22 12:01:00.000000 Fiicen-py-1.1.0/setup.py
```

### Comparing `Fiicen-py-1.0.0/Fiicen_py.egg-info/PKG-INFO` & `Fiicen-py-1.1.0/Fiicen_py.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fiicen-py
-Version: 1.0.0
+Version: 1.1.0
 Summary: FiicenというSNSに使えるAPIラッパー
 Home-page: https://github.com/taka-4602/Fiicen-py
 Author: taka4602
 Author-email: shun4602@gmail.com
 Keywords: fiicen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,29 +24,43 @@
 from fiicen_py import Fiicen
 
 fiicen=Fiicen(name="ユーザー名",password="パスワード")#ログイン、nameとpasswordを設定しなかったらログインをスキップします
 print(fiicen.fly_circle(contents="メインの文章",vote_choices1="投票の選択肢1",vote_choices2="投票の選択肢2"))
 print(fiicen.change_profile(display_name="表示名",introduce="自己紹介"))
 print(fiicen.follow(followed_id="ユーザーID"))#ユーザーIDの取得方法がリクエスト見るしかなさそうなので使い道ナシ？
 print(fiicen.get_topic())#タイムラインをhtmlで取得する
+print(fiicen.notification())#通知の数をintで返す
+print(fiicen.like(circle_id="サークルID"))#いいね！
+print(fiicen.refly(circle_id="サークルID"))#リフライ
+print(fiicen.fix_circle(circle_id="サークルID"))#プロフィールにサークルを固定
+print(fiicen.report(circle_id="サークルID",type="通報理由"))#サークルを通報、理由は：harassment / sensitive / spam / suicide / spoofing / privacy / violence / misinformation / discrimination から選ぶ
 
 fiicen=Fiicen()#アカウント作成の時はログインをスキップ
 print(fiicen.create_account(name="ユーザー名",display_name="表示名",password="パスワード"))
 print(fiicen.check_account_name(name="ユーザー名"))#ユーザー名が使用されているかどうか確認する...使いどころは不明
 ```
 使い方は#コメントに書いてある通りで、それ以上はなにもないです  
 返される値もステータスコードくらいで重要なものはありません  
 ### 返される値  
-```.fly_circle()``` / ```.change_profile()``` / ```.follow()``` / ```.create_account()``` 
+```.fly_circle()``` / ```.change_profile()``` / ```.follow()``` / ```.create_account()``` / ```.like()``` / ```.refly()``` / ```.report()``` 
 - **ステータスコード**  
-  言わずもがな200が成功、それ以外はエラー  
+  言わずもがな200が成功、それ以外はエラーになる  
 
 ```get_topic()``` 
 - **html**  
   bs4などで要素を抽出する必要アリ
 
 ```.check_account_name()```
 - **bool**  
   ```True``` or ```False```
+
+```.fix_circle()```
+- **dict**  
+  ```{result: "fixed"}``` or ```{result: "unfixed"}```
+
+```.notification()```
+- **int**  
+  ```0,1,2,3,4,5,6......```
+  
 ## コンタクト
-Discord サーバー / https://discord.gg/aSyaAK7Ktm
+Discord サーバー / https://discord.gg/aSyaAK7Ktm  
 Discord ユーザー名 / .taka.
```

### Comparing `Fiicen-py-1.0.0/PKG-INFO` & `Fiicen-py-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fiicen-py
-Version: 1.0.0
+Version: 1.1.0
 Summary: FiicenというSNSに使えるAPIラッパー
 Home-page: https://github.com/taka-4602/Fiicen-py
 Author: taka4602
 Author-email: shun4602@gmail.com
 Keywords: fiicen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,29 +24,43 @@
 from fiicen_py import Fiicen
 
 fiicen=Fiicen(name="ユーザー名",password="パスワード")#ログイン、nameとpasswordを設定しなかったらログインをスキップします
 print(fiicen.fly_circle(contents="メインの文章",vote_choices1="投票の選択肢1",vote_choices2="投票の選択肢2"))
 print(fiicen.change_profile(display_name="表示名",introduce="自己紹介"))
 print(fiicen.follow(followed_id="ユーザーID"))#ユーザーIDの取得方法がリクエスト見るしかなさそうなので使い道ナシ？
 print(fiicen.get_topic())#タイムラインをhtmlで取得する
+print(fiicen.notification())#通知の数をintで返す
+print(fiicen.like(circle_id="サークルID"))#いいね！
+print(fiicen.refly(circle_id="サークルID"))#リフライ
+print(fiicen.fix_circle(circle_id="サークルID"))#プロフィールにサークルを固定
+print(fiicen.report(circle_id="サークルID",type="通報理由"))#サークルを通報、理由は：harassment / sensitive / spam / suicide / spoofing / privacy / violence / misinformation / discrimination から選ぶ
 
 fiicen=Fiicen()#アカウント作成の時はログインをスキップ
 print(fiicen.create_account(name="ユーザー名",display_name="表示名",password="パスワード"))
 print(fiicen.check_account_name(name="ユーザー名"))#ユーザー名が使用されているかどうか確認する...使いどころは不明
 ```
 使い方は#コメントに書いてある通りで、それ以上はなにもないです  
 返される値もステータスコードくらいで重要なものはありません  
 ### 返される値  
-```.fly_circle()``` / ```.change_profile()``` / ```.follow()``` / ```.create_account()``` 
+```.fly_circle()``` / ```.change_profile()``` / ```.follow()``` / ```.create_account()``` / ```.like()``` / ```.refly()``` / ```.report()``` 
 - **ステータスコード**  
-  言わずもがな200が成功、それ以外はエラー  
+  言わずもがな200が成功、それ以外はエラーになる  
 
 ```get_topic()``` 
 - **html**  
   bs4などで要素を抽出する必要アリ
 
 ```.check_account_name()```
 - **bool**  
   ```True``` or ```False```
+
+```.fix_circle()```
+- **dict**  
+  ```{result: "fixed"}``` or ```{result: "unfixed"}```
+
+```.notification()```
+- **int**  
+  ```0,1,2,3,4,5,6......```
+  
 ## コンタクト
-Discord サーバー / https://discord.gg/aSyaAK7Ktm
+Discord サーバー / https://discord.gg/aSyaAK7Ktm  
 Discord ユーザー名 / .taka.
```

### Comparing `Fiicen-py-1.0.0/setup.py` & `Fiicen-py-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 def load_readme() -> str:
     with open("README.md",encoding="utf-8_sig") as fin:
         return fin.read()
 setup(
     name='Fiicen-py',
-    version='1.0.0',
+    version='1.1.0',
     keywords = "fiicen",
     long_description=load_readme(),
     long_description_content_type="text/markdown",
     author='taka4602',
     author_email='shun4602@gmail.com',
     url='https://github.com/taka-4602/Fiicen-py',
     description='FiicenというSNSに使えるAPIラッパー',
```

