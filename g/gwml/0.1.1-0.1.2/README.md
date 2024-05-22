# Comparing `tmp/gwml-0.1.1-py3-none-any.whl.zip` & `tmp/gwml-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,25 @@
-Zip file size: 75837 bytes, number of entries: 50
+Zip file size: 98365 bytes, number of entries: 63
 -rw-r--r--  2.0 unx        0 b- defN 24-May-14 09:40 gwml/__init__.py
--rw-r--r--  2.0 unx     1521 b- defN 24-May-16 05:28 gwml/command.py
--rw-r--r--  2.0 unx      206 b- defN 24-May-16 05:31 gwml/main.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-May-16 05:28 gwml/_command.py
+-rw-r--r--  2.0 unx      206 b- defN 24-May-16 05:31 gwml/_main.py
+-rw-r--r--  2.0 unx     6030 b- defN 24-May-22 09:12 gwml/command.py
+-rw-r--r--  2.0 unx      792 b- defN 24-May-22 09:13 gwml/main.py
 -rw-r--r--  2.0 unx      104 b- defN 24-May-16 05:28 gwml/mldump.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 09:12 gwml/cmdLib/__init__.py
+-rw-r--r--  2.0 unx     2437 b- defN 24-May-21 00:19 gwml/cmdLib/envCollector.py
+-rw-r--r--  2.0 unx     2233 b- defN 24-May-21 05:40 gwml/cmdLib/getHyperParam.py
+-rw-r--r--  2.0 unx     1818 b- defN 24-May-22 02:14 gwml/cmdLib/getLagacyFile.py
+-rw-r--r--  2.0 unx     3639 b- defN 24-May-22 07:34 gwml/cmdLib/organizeModel.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 09:12 gwml/lagacy/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 09:12 gwml/lagacy/train/__init__.py
+-rw-r--r--  2.0 unx     4932 b- defN 24-May-22 05:45 gwml/lagacy/train/classification.py
+-rw-r--r--  2.0 unx     4932 b- defN 24-May-22 05:45 gwml/lagacy/train/clustering.py
+-rw-r--r--  2.0 unx     4932 b- defN 24-May-22 05:45 gwml/lagacy/train/regression.py
+-rw-r--r--  2.0 unx     4932 b- defN 24-May-22 05:45 gwml/lagacy/train/timeseries.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-14 09:40 gwml/lib/__init__.py
 -rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:48 gwml/lib/common/__init__.py
 -rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:48 gwml/lib/common/Environment/__init__.py
 -rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:48 gwml/lib/common/Environment/oracle/__init__.py
 -rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:48 gwml/lib/common/Environment/oracle/lib/__init__.py
 -rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:48 gwml/lib/common/automl/__init__.py
 -rw-r--r--  2.0 unx    16836 b- defN 24-May-16 05:48 gwml/lib/common/automl/automl.py
@@ -40,13 +53,13 @@
 -rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:48 gwml/lib/common/trainer/__init__.py
 -rw-r--r--  2.0 unx    11894 b- defN 24-May-16 06:40 gwml/lib/common/trainer/customTrainer.py
 -rw-r--r--  2.0 unx    10834 b- defN 24-May-16 05:48 gwml/lib/common/trainer/regTrainer.py
 -rw-r--r--  2.0 unx     2317 b- defN 24-May-16 05:48 gwml/lib/common/utils/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-16 06:46 gwml/lib/reg/__init__.py
 -rw-r--r--  2.0 unx     5131 b- defN 24-May-16 06:41 gwml/lib/reg/regDecorator.py
 -rw-r--r--  2.0 unx    24563 b- defN 24-May-16 06:42 gwml/lib/reg/regTrainer.py
--rw-r--r--  2.0 unx       49 b- defN 24-May-16 06:49 gwml-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-16 06:49 gwml-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 24-May-16 06:49 gwml-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-May-16 06:49 gwml-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4445 b- defN 24-May-16 06:49 gwml-0.1.1.dist-info/RECORD
-50 files, 283666 bytes uncompressed, 68635 bytes compressed:  75.8%
+-rw-r--r--  2.0 unx       49 b- defN 24-May-22 09:15 gwml-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-22 09:15 gwml-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 24-May-22 09:15 gwml-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 24-May-22 09:15 gwml-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5519 b- defN 24-May-22 09:15 gwml-0.1.2.dist-info/RECORD
+63 files, 321417 bytes uncompressed, 89489 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -1,19 +1,58 @@
 Filename: gwml/__init__.py
 Comment: 
 
+Filename: gwml/_command.py
+Comment: 
+
+Filename: gwml/_main.py
+Comment: 
+
 Filename: gwml/command.py
 Comment: 
 
 Filename: gwml/main.py
 Comment: 
 
 Filename: gwml/mldump.py
 Comment: 
 
+Filename: gwml/cmdLib/__init__.py
+Comment: 
+
+Filename: gwml/cmdLib/envCollector.py
+Comment: 
+
+Filename: gwml/cmdLib/getHyperParam.py
+Comment: 
+
+Filename: gwml/cmdLib/getLagacyFile.py
+Comment: 
+
+Filename: gwml/cmdLib/organizeModel.py
+Comment: 
+
+Filename: gwml/lagacy/__init__.py
+Comment: 
+
+Filename: gwml/lagacy/train/__init__.py
+Comment: 
+
+Filename: gwml/lagacy/train/classification.py
+Comment: 
+
+Filename: gwml/lagacy/train/clustering.py
+Comment: 
+
+Filename: gwml/lagacy/train/regression.py
+Comment: 
+
+Filename: gwml/lagacy/train/timeseries.py
+Comment: 
+
 Filename: gwml/lib/__init__.py
 Comment: 
 
 Filename: gwml/lib/common/__init__.py
 Comment: 
 
 Filename: gwml/lib/common/Environment/__init__.py
@@ -129,23 +168,23 @@
 
 Filename: gwml/lib/reg/regDecorator.py
 Comment: 
 
 Filename: gwml/lib/reg/regTrainer.py
 Comment: 
 
-Filename: gwml-0.1.1.dist-info/METADATA
+Filename: gwml-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: gwml-0.1.1.dist-info/WHEEL
+Filename: gwml-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: gwml-0.1.1.dist-info/entry_points.txt
+Filename: gwml-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: gwml-0.1.1.dist-info/top_level.txt
+Filename: gwml-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: gwml-0.1.1.dist-info/RECORD
+Filename: gwml-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gwml/command.py

```diff
@@ -1,47 +1,194 @@
-import argparse
-
-
-class CommandParser:
-    def __init__(self) -> None:
-        self.parser = argparse.ArgumentParser(prog="gwml")
-        self.subparser = self.parser.add_subparsers(
-            dest="command", help="Available commands"
-        )
-
-    def get_args(self) -> argparse.Namespace:
-        pull_parser = self.subparser.add_parser(
-            "pull", help="You can download ML writing samples."
-        )
-        push_parser = self.subparser.add_parser(
-            "push", help="You can deploy the model you wrote in GreenWales"
-        )
-
-        pull_option = pull_parser.add_mutually_exclusive_group(required=False)
-        pull_option.add_argument(
-            "-l",
-            "-list",
-            help=f"Displays a list of available samples",
-        )
-        pull_option.add_argument("-n", help=f"Choose a sample name")
-
-        push_option = push_parser.add_mutually_exclusive_group(required=False)
-        push_option.add_argument(
-            "-H",
-            "--host",
-            help=f"* Enter your Green Wales address.",
-        )
-        push_option.add_argument(
-            "-U",
-            "--user",
-            help=f"* Enter your Green Wales login ID",
-        )
-        push_option.add_argument(
-            "-P",
-            help=f"* Enter your Green Wales login Password",
-        )
-        push_option.add_argument(
-            "-m",
-            help=f"Select when you don't need automatic generation of the setting.yaml file.",
-        )
-
-        return self.parser.parse_args()
+import os
+import sys
+import json
+import yaml
+import requests
+import getpass
+from cmdLib.getHyperParam import extractHyperParamstoFile
+from cmdLib.envCollector import generate_requirements
+from cmdLib.organizeModel import ModelOrganizer
+
+
+def yaml_to_json(yaml_file):
+    with open(yaml_file, "r", encoding="utf-8") as yf:
+        yaml_data = yaml.safe_load(yf)
+
+    return yaml_data
+
+
+def post_request(url, data, headers=None):
+    response = requests.post(url, json=data, headers=headers)
+    return response.json()
+
+
+def send_post_request(url, file_path, data, jwt_token):
+    url += "/api/model"
+    headers = {"Authorization": f"Bearer {jwt_token}"}
+
+    files = {"file": open(file_path, "rb")}
+
+    print(url)
+    print(headers)
+    print(data)
+
+    response = requests.post(url, headers=headers, files=files, data=data)
+
+    return response.json()
+
+
+def handle_pull():
+    print("Executing pull command...")
+
+
+def save_json_to_file(json_data, file_path):
+    with open(file_path, "w") as file:
+        json.dump(json_data, file, indent=4)
+
+
+def handle_push(string1, string2):
+
+    # 필수 파일이 있는지 여부 검사
+    if fileCheck()["code"] == 400:
+        print(fileCheck()["msg"])
+        sys.exit()
+
+    # 설정 파일 불러오기
+    opt = yaml_to_json("setting.yaml")
+
+    # 설정에 호스트가 있느지, 없다면 사용자 입력 받기
+    if "host" not in opt:
+        q = input("Host information is missing. Please enter it: ").strip().lower()
+        opt["host"] = q
+
+    url = opt["host"] + "/api/user-auth/login"
+    id = input("Please enter your Login ID: ").strip().lower()
+    pwd = getpass.getpass("Please enter your Login Passowrd: ")
+    data = {"userId": id, "password": pwd}
+    headers = {"Content-Type": "application/json"}
+
+    # 로그인
+    response = post_request(url, data, headers)
+    if "userInfo" not in response:
+        print(response["message"])
+        sys.exit()
+
+    types = ["regression", "classification", "clustering", "timeseries"]
+
+    if "modelName" not in opt:
+        environment = (
+            input("Please enter the name of your deployment model: ").strip().lower()
+        )
+        opt["environment"] = environment
+
+    if "purposeType" not in opt:
+        purposeType = (
+            input(
+                "The machine learning objective type has not been defined. Please input one of the following: \n(regression, Classification, clustering, timeseries) :"
+            )
+            .strip()
+            .lower()
+        )
+        opt["purposeType"] = purposeType
+
+    if opt["purposeType"] not in types:
+        print("You did not enter the correct objective type.")
+        sys.exit()
+
+    # 설정을 테스트파일을 통해 자동 생성할지, 수동으로 진행할지 여부 설정
+    if "hpoOpt" not in opt:
+        manualOptQ = "n"
+        if "manualOpt" not in opt or opt["manualOpt"] == False:
+            manualOptQ = (
+                input(
+                    "Should we automatically configure the options through test.py? (y/n): "
+                )
+                .strip()
+                .lower()
+            )
+        if manualOptQ == "y" or opt["manualOpt"]:
+            filename = (
+                input(
+                    "What is the file name of the test code you wrote? For example ('test.py'): "
+                )
+                .strip()
+                .lower()
+            )
+            hyperparm = ""
+            try:
+                hyperparm = extractHyperParamstoFile(filename)
+                if len(hyperparm) == 0:
+                    hyperparm = {}
+                else:
+                    hyperparm = hyperparm[0]
+                opt["hpoOpt"] = hyperparm
+            except:
+                print("The {} file could not be found.".format(filename))
+                sys.exit()
+
+    # ENV 파일을 자동으로 설정할지 여부 검사
+    requirementsAutoCollectQ = "n"
+    if "requirementsAutoCollect" not in opt or opt["requirementsAutoCollect"] == False:
+        requirementsAutoCollectQ = (
+            input("Should we automatically collect the requirements.txt file? (y/n): ")
+            .strip()
+            .lower()
+        )
+    if requirementsAutoCollectQ == "y" or opt["requirementsAutoCollect"]:
+        requirements = generate_requirements("model.py")
+        requirements = generate_requirements("predict.py")
+
+    modelInfo = {
+        "environment": opt["environment"],
+        "mlType": "tabular",
+        "purposeType": opt["purposeType"],
+        "customTF": True,
+        "trainTf": False,
+        "baseModelName": "XGBoost-Regression",
+        "baseModelVersion": "latest",
+    }
+
+    # 모델 tar파일 만들기
+    base_directory = "."  # 현재 디렉토리
+    output_filename = "model.tar.gz"
+
+    organizer = ModelOrganizer(base_directory)
+    organizer.organize_and_compress(
+        output_filename, opt["purposeType"] + ".py", modelInfo, opt["hpoOpt"]
+    )
+
+    sendData = {"modelName": opt["environment"]}
+    mhResult = send_post_request(
+        response["systemInfo"]["mhUrl"], output_filename, sendData, response["jwt"]
+    )
+    print(mhResult)
+    print(
+        "You have successfully registered {}/{}".format(
+            response["systemInfo"]["mhUrl"], opt["environment"]
+        )
+    )
+
+
+def fileCheck():
+    # 현재 디렉토리 경로를 가져옵니다.
+    current_directory = os.getcwd()
+
+    # 현재 디렉토리 내부의 파일 및 디렉토리 리스트를 가져옵니다.
+    files = os.listdir(current_directory)
+
+    if "model.py" not in files:
+        return {
+            "code": 400,
+            "msg": "'model.py' is not present in the current directory.",
+        }
+    elif "predict.py" not in files:
+        return {
+            "code": 400,
+            "msg": "'predict.py' is not present in the current directory.",
+        }
+    elif "setting.yaml" not in files:
+        return {
+            "code": 400,
+            "msg": "'setting.yaml' is not present in the current directory.",
+        }
+    else:
+        return {"code": 200}
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## gwml/main.py

```diff
@@ -1,10 +1,27 @@
-from gwml.mldump import MLdump
-from gwml.command import CommandParser
+import argparse
+from command import handle_pull, handle_push
 
 
 def main():
-    args = CommandParser().get_args()
-    mldump = MLdump()
+    parser = argparse.ArgumentParser(description="CLI for pull and push commands")
 
-    if args.command == "push":
-        mldump.initPush(args)
+    subparsers = parser.add_subparsers(dest="command")
+
+    pull_parser = subparsers.add_parser("pull", help="Execute pull command")
+
+    push_parser = subparsers.add_parser("push", help="Execute push command")
+    push_parser.add_argument("-s", "--string1", type=str, help="First string option")
+    push_parser.add_argument("-j", "--string2", type=str, help="Second string option")
+
+    args = parser.parse_args()
+
+    if args.command == "pull":
+        handle_pull()
+    elif args.command == "push":
+        handle_push(args.string1, args.string2)
+    else:
+        parser.print_help()
+
+
+# if __name__ == '__main__':
+#     main()
```

## Comparing `gwml-0.1.1.dist-info/RECORD` & `gwml-0.1.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 gwml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gwml/command.py,sha256=TaBIi24kTzCexXpTyxsbaFYmT5rVavItqnMh1RZI-8A,1521
-gwml/main.py,sha256=jTS67aubfEs7U4uCU7a7gWlOllWm0AUjfvVKiXSIQEs,206
+gwml/_command.py,sha256=TaBIi24kTzCexXpTyxsbaFYmT5rVavItqnMh1RZI-8A,1521
+gwml/_main.py,sha256=jTS67aubfEs7U4uCU7a7gWlOllWm0AUjfvVKiXSIQEs,206
+gwml/command.py,sha256=cH3QbTY8bimiy-tlJObgccpZg1vvf4RmRMAp6RhzklI,6030
+gwml/main.py,sha256=QlMbccUH-CEWeeLvHJh3y0aVRmNeBb8jdWxiY2xAWPo,792
 gwml/mldump.py,sha256=BhfNWnOwFqjgwkH7CPDDwL4FfA1L-QKGvD4u5lKzhCA,104
+gwml/cmdLib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+gwml/cmdLib/envCollector.py,sha256=QNRM6w69zpac7IHmn3SIVcn-5EKUfmaEtb_BUAbReR0,2437
+gwml/cmdLib/getHyperParam.py,sha256=3Yj28_WM759mx3jAzfHRpjWdYbYn-HYU3Q0eFyHq8qQ,2233
+gwml/cmdLib/getLagacyFile.py,sha256=LLzHq9j56jI6ZBC4_zxQ6iGiYfgiThDrguNytwOm00o,1818
+gwml/cmdLib/organizeModel.py,sha256=KGmc4jxtoKqAEVYLk3QHfeBjAoIUVFDP-t-ZMUux7WQ,3639
+gwml/lagacy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+gwml/lagacy/train/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+gwml/lagacy/train/classification.py,sha256=CTX1E-vZBO7ypSe3HXYKRI1G6WKaxUCWXOoNzwCCHw8,4932
+gwml/lagacy/train/clustering.py,sha256=CTX1E-vZBO7ypSe3HXYKRI1G6WKaxUCWXOoNzwCCHw8,4932
+gwml/lagacy/train/regression.py,sha256=CTX1E-vZBO7ypSe3HXYKRI1G6WKaxUCWXOoNzwCCHw8,4932
+gwml/lagacy/train/timeseries.py,sha256=CTX1E-vZBO7ypSe3HXYKRI1G6WKaxUCWXOoNzwCCHw8,4932
 gwml/lib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gwml/lib/common/__init__.py,sha256=46Yjk3fz9o8aTN8E95McnzpJcjGzVJmHmQqUZ5mXzfc,22
 gwml/lib/common/Environment/__init__.py,sha256=46Yjk3fz9o8aTN8E95McnzpJcjGzVJmHmQqUZ5mXzfc,22
 gwml/lib/common/Environment/oracle/__init__.py,sha256=46Yjk3fz9o8aTN8E95McnzpJcjGzVJmHmQqUZ5mXzfc,22
 gwml/lib/common/Environment/oracle/lib/__init__.py,sha256=46Yjk3fz9o8aTN8E95McnzpJcjGzVJmHmQqUZ5mXzfc,22
 gwml/lib/common/automl/__init__.py,sha256=46Yjk3fz9o8aTN8E95McnzpJcjGzVJmHmQqUZ5mXzfc,22
 gwml/lib/common/automl/automl.py,sha256=TC6DG4go2IYLmJw9D36xoCvz-FErcNaZFZZ8CaTUvZk,16836
@@ -39,12 +52,12 @@
 gwml/lib/common/trainer/__init__.py,sha256=46Yjk3fz9o8aTN8E95McnzpJcjGzVJmHmQqUZ5mXzfc,22
 gwml/lib/common/trainer/customTrainer.py,sha256=05rWhPyD0xcbBV8FTkHBR2igBlEZPOfyyJhekcjuzUQ,11894
 gwml/lib/common/trainer/regTrainer.py,sha256=BXupe-vk72dLZ0Bp8NZq5O2bJ4sHVYQVeFg-SDQyOfw,10834
 gwml/lib/common/utils/utils.py,sha256=auXrdDqukRQnAOsRBAxioLvsocyniZeoh3eGjnZlrsA,2317
 gwml/lib/reg/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gwml/lib/reg/regDecorator.py,sha256=lkN5pxnutUvjWjk44Uz1w3QGCSVYuYZirSCrIL7VlSQ,5131
 gwml/lib/reg/regTrainer.py,sha256=6Qv1ploKZpGGCpEu4_7k4zLaEaAUOv8IrTuVMOoddvk,24563
-gwml-0.1.1.dist-info/METADATA,sha256=Dx8YUBLI5ddUVtErS1UytvlPkjgBXbmjNsmzguNtMEM,49
-gwml-0.1.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-gwml-0.1.1.dist-info/entry_points.txt,sha256=imL6Gb7yRsNcKwqqUM7kpMULMW5smUSYZSX7i_BVdmo,40
-gwml-0.1.1.dist-info/top_level.txt,sha256=-Ib3RiOMqlhiZ_idfsP2Unxpw70_Lzk5xN0I7vWHuAQ,5
-gwml-0.1.1.dist-info/RECORD,,
+gwml-0.1.2.dist-info/METADATA,sha256=KVQGBqT-6qGG3ksPHIN_2Cvb1JtZfxTVsDO_uodHTWA,49
+gwml-0.1.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+gwml-0.1.2.dist-info/entry_points.txt,sha256=imL6Gb7yRsNcKwqqUM7kpMULMW5smUSYZSX7i_BVdmo,40
+gwml-0.1.2.dist-info/top_level.txt,sha256=-Ib3RiOMqlhiZ_idfsP2Unxpw70_Lzk5xN0I7vWHuAQ,5
+gwml-0.1.2.dist-info/RECORD,,
```

