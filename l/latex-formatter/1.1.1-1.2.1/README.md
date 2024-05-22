# Comparing `tmp/latex_formatter-1.1.1.tar.gz` & `tmp/latex_formatter-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latex_formatter-1.1.1.tar", last modified: Tue Jan  9 09:25:41 2024, max compression
+gzip compressed data, was "latex_formatter-1.2.1.tar", last modified: Wed May 22 02:48:01 2024, max compression
```

## Comparing `latex_formatter-1.1.1.tar` & `latex_formatter-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-01-09 09:25:41.076361 latex_formatter-1.1.1/
--rw-rw-rw-   0        0        0      135 2024-01-09 09:25:41.076361 latex_formatter-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-11-17 10:14:19.000000 latex_formatter-1.1.1/README.md
--rw-rw-rw-   0        0        0       52 2023-10-17 03:55:42.000000 latex_formatter-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      231 2024-01-09 09:25:41.078359 latex_formatter-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      318 2024-01-09 09:24:36.000000 latex_formatter-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-09 09:25:40.993935 latex_formatter-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-01-09 09:25:41.010053 latex_formatter-1.1.1/src/latex_formatter/
--rw-rw-rw-   0        0        0      103 2023-12-21 06:45:34.000000 latex_formatter-1.1.1/src/latex_formatter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-09 09:25:41.068911 latex_formatter-1.1.1/src/latex_formatter/converter/
--rw-rw-rw-   0        0        0       62 2023-12-21 06:45:01.000000 latex_formatter-1.1.1/src/latex_formatter/converter/__init__.py
--rw-rw-rw-   0        0        0    16129 2024-01-09 09:24:13.000000 latex_formatter-1.1.1/src/latex_formatter/converter/converter.py
--rw-rw-rw-   0        0        0       71 2023-10-17 07:08:30.000000 latex_formatter-1.1.1/src/latex_formatter/test.py
-drwxrwxrwx   0        0        0        0 2024-01-09 09:25:41.075358 latex_formatter-1.1.1/src/latex_formatter/utils/
--rw-rw-rw-   0        0        0       87 2023-10-17 07:21:19.000000 latex_formatter-1.1.1/src/latex_formatter/utils/__init__.py
--rw-rw-rw-   0        0        0    20221 2023-11-15 07:06:02.000000 latex_formatter-1.1.1/src/latex_formatter/utils/text_to_latex.py
--rw-rw-rw-   0        0        0      233 2023-11-16 06:42:03.000000 latex_formatter-1.1.1/src/latex_formatter/utils/transfer.py
-drwxrwxrwx   0        0        0        0 2024-01-09 09:25:41.044792 latex_formatter-1.1.1/src/latex_formatter.egg-info/
--rw-rw-rw-   0        0        0      135 2024-01-09 09:25:40.000000 latex_formatter-1.1.1/src/latex_formatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      521 2024-01-09 09:25:40.000000 latex_formatter-1.1.1/src/latex_formatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-09 09:25:40.000000 latex_formatter-1.1.1/src/latex_formatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-01-09 09:25:40.000000 latex_formatter-1.1.1/src/latex_formatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-01-09 09:25:40.000000 latex_formatter-1.1.1/src/latex_formatter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 02:48:01.894635 latex_formatter-1.2.1/
+-rw-rw-rw-   0        0        0      135 2024-05-22 02:48:01.894635 latex_formatter-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-11-17 10:14:19.000000 latex_formatter-1.2.1/README.md
+-rw-rw-rw-   0        0        0       52 2023-10-17 03:55:42.000000 latex_formatter-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      231 2024-05-22 02:48:01.899170 latex_formatter-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      318 2024-05-22 02:47:26.000000 latex_formatter-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 02:48:01.784417 latex_formatter-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 02:48:01.790418 latex_formatter-1.2.1/src/latex_formatter/
+-rw-rw-rw-   0        0        0      103 2023-12-21 06:45:34.000000 latex_formatter-1.2.1/src/latex_formatter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 02:48:01.881141 latex_formatter-1.2.1/src/latex_formatter/converter/
+-rw-rw-rw-   0        0        0       62 2023-12-21 06:45:01.000000 latex_formatter-1.2.1/src/latex_formatter/converter/__init__.py
+-rw-rw-rw-   0        0        0    16202 2024-05-22 02:43:32.000000 latex_formatter-1.2.1/src/latex_formatter/converter/converter.py
+-rw-rw-rw-   0        0        0    28889 2024-05-22 02:38:03.000000 latex_formatter-1.2.1/src/latex_formatter/converter/web_converter.py
+-rw-rw-rw-   0        0        0       71 2023-10-17 07:08:30.000000 latex_formatter-1.2.1/src/latex_formatter/test.py
+drwxrwxrwx   0        0        0        0 2024-05-22 02:48:01.894635 latex_formatter-1.2.1/src/latex_formatter/utils/
+-rw-rw-rw-   0        0        0       87 2023-10-17 07:21:19.000000 latex_formatter-1.2.1/src/latex_formatter/utils/__init__.py
+-rw-rw-rw-   0        0        0    20221 2023-11-15 07:06:02.000000 latex_formatter-1.2.1/src/latex_formatter/utils/text_to_latex.py
+-rw-rw-rw-   0        0        0      233 2023-11-16 06:42:03.000000 latex_formatter-1.2.1/src/latex_formatter/utils/transfer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 02:48:01.825635 latex_formatter-1.2.1/src/latex_formatter.egg-info/
+-rw-rw-rw-   0        0        0      135 2024-05-22 02:48:01.000000 latex_formatter-1.2.1/src/latex_formatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2024-05-22 02:48:01.000000 latex_formatter-1.2.1/src/latex_formatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 02:48:01.000000 latex_formatter-1.2.1/src/latex_formatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-22 02:48:01.000000 latex_formatter-1.2.1/src/latex_formatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-22 02:48:01.000000 latex_formatter-1.2.1/src/latex_formatter.egg-info/top_level.txt
```

### Comparing `latex_formatter-1.1.1/src/latex_formatter/converter/converter.py` & `latex_formatter-1.2.1/src/latex_formatter/converter/converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,493 +1,502 @@
-from ..utils.text_to_latex  import conversion_functions
+from ..utils.text_to_latex import conversion_functions
 from ..utils import transfer_to_dict
 from ujson import JSONDecodeError
 from typing import Union
+from .web_converter import LatexRender
+
 
 def converter(data: Union[dict, str]):
     if isinstance(data, list):
         res = []
         for d in data:
             converter(d)
 
     try:
         content_dict = transfer_to_dict(data)
-    except (JSONDecodeError):
+    except JSONDecodeError:
         # print("load err")
         # print(type(data))
         return data
     question = content_dict["caption"] if "caption" in content_dict else content_dict
-    
+
     answer = content_dict.get("answer", None)
-    types = (question['type'])
-    
+    types = question["type"]
+
     print(f"type is {types}")
-    
+
     try:
-        if types =="wave":
+        if types == "wave":
             print(f"wave")
             print(conversion_functions.get(types))
         conversion_func = conversion_functions.get(types)
         print(f"con func is {conversion_func}")
         if conversion_func:
             print(f"yes")
             # maybe \\newline
             # return conversion_func(te).replace("[br]", "<br />")
             question_part = conversion_func(question)
         else:
-            
             raise ValueError(f"No conversion function for type {types} found.")
     except Exception as e:
         #  print(f"error for {type(data)}")
         #  print(e)
         pass
-    
+
     if not answer:
         # return 'error'
-        try: 
-            
+        try:
             return question_part
         except:
             return "error"
     else:
         if answer_converter(answer):
             return question_part + answer_converter(answer)
         return question_part
-    
+
 
 def answer_converter(answer: dict):
     print(f"answer is {answer}")
     try:
         answer_dict = transfer_to_dict(answer)
-    except (JSONDecodeError):
+    except JSONDecodeError:
         # print("load err")
         # print(type(data))
         return answer
 
-    
     if answer_dict:
         types = answer.get("type", None)
         print(f"answer type is {types}")
         try:
             conversion_func = conversion_functions.get(types)
             print(f"type is {types}")
             if conversion_func:
                 # maybe \\newline
                 # return conversion_func(te).replace("[br]", "<br />")
                 print(f"start")
                 print(f"ans dict is {answer_dict}")
                 answer_part = conversion_func(answer_dict)
                 return answer_part
             else:
-                
                 raise ValueError(f"No conversion function for type {types} found.")
         except Exception as e:
-                #  print(f"error for {type(data)}")
-                #  print(e)
+            #  print(f"error for {type(data)}")
+            #  print(e)
             pass
         return []
-    
+
 
 def is_final_object(obj):
     if isinstance(obj, dict):
         print(f"is dict")
         for key, val in obj.items():
             if isinstance(val, dict):
-                if 'type' in val:
+                if "type" in val:
                     return False
                 if not is_final_object(val):
                     return False
     elif isinstance(obj, list):
         for item in obj:
             if isinstance(item, dict):
-                if 'type' in item:
+                if "type" in item:
                     return False
                 if not is_final_object(item):
                     return False
     return True
-    
+
 
 def render(obj):
     print(f"start re")
-    if isinstance(obj, dict) and 'type' in obj and obj['type']:
-        obj_type = obj['type'].lower()
+    if isinstance(obj, dict) and "type" in obj and obj["type"]:
+        obj_type = obj["type"].lower()
         conversion_func = conversion_functions.get(obj_type)
         if conversion_func:
             print(f"{obj_type}", obj)
             # maybe \\newline
             # return conversion_func(te).replace("[br]", "<br />")
             question_part = conversion_func(obj)
             print(f"fi ")
             print(question_part)
             return question_part
-        
+
     elif isinstance(obj, str):
         print(f"str is {obj}")
         return obj.replace("[br]", "\n")
     elif isinstance(obj, list):
         return " ".join(obj)
     else:
         return "Invalid object type"
 
+
 def to_old_version(obj):
     if isinstance(obj, dict):
-        if 'type' in obj:
-            if obj['type'] in ['merge', 'equation', 'latexarray']:
-                nobjs = [to_old_version(o) for o in obj['value']]
-                obj['value'] = nobjs
+        if "type" in obj:
+            if obj["type"] in ["merge", "equation", "latexarray"]:
+                nobjs = [to_old_version(o) for o in obj["value"]]
+                obj["value"] = nobjs
                 return obj
-            elif obj['type'] in ['select', 'multiselect']:
-                nobjs = [to_old_version(o) for o in obj['options']]
-                obj['options'] = nobjs
+            elif obj["type"] in ["select", "multiselect"]:
+                nobjs = [to_old_version(o) for o in obj["options"]]
+                obj["options"] = nobjs
                 return obj
-            elif obj['type'] in ['table', 'matrix', 'grid']:
-                for col in obj['value']:
+            elif obj["type"] in ["table", "matrix", "grid"]:
+                for col in obj["value"]:
                     for i, row in enumerate(col):
                         col[i] = to_old_version(row)
                 return obj
             else:
                 for k, val in obj.items():
                     obj[k] = to_old_version(val)
                 return obj
         else:
             nobjs = {}
             is_list = all(isinstance(k, int) for k in obj.keys())
             for k, o in obj.items():
                 nobjs[k] = to_old_version(o)
             if is_list:
-                return {'type': 'merge', 'value': list(nobjs.values())}
+                return {"type": "merge", "value": list(nobjs.values())}
             else:
                 return nobjs
     elif isinstance(obj, list):
         # 对列表中的每个值递归调用
         print("list")
         print([to_old_version(val) for val in obj])
         print(f"s")
         return [to_old_version(val) for val in obj]
     else:
         return obj
 
 
-    
 def c2(obj):
     if not obj:
         return ""
     print(f"obj type is {type(obj)}")
     # if not isinstance(obj, dict):
     #     try:
     #         obj = transfer_to_dict(obj)
     #     except (JSONDecodeError):
     #         # print("load err")
     #         # print(type(data))
-    #         return obj 
+    #         return obj
     print(f"obj is {obj}")
     obj = to_old_version(obj)
     print(f"obj is {obj}")
-    
+
     while True:
         current_obj = obj
         if is_final_object(obj):
             return render(obj)
         print(f"not final")
         found = False
         if isinstance(obj, dict):
             for key, val in current_obj.items():
                 print("keys is", key)
                 if not isinstance(val, dict):
                     continue
                 if is_final_object(val):
                     print(f"true")
-                    if 'type' in val:
+                    if "type" in val:
                         print(f"key is {key}")
                         current_obj[key] = render(val)
                         print(f"cu is {current_obj}")
             else:
                 current_obj = val
                 found = True
                 break
         elif isinstance(obj, list):
             l = len(obj)
             print(f"len is {l}")
             for i in range(l):
                 current_obj[i] = render(current_obj[i])
             print(f"final obj i is {current_obj}")
-                
-
 
         if not found:
             break
 
         if current_obj is obj:
             break
     print(f"type if {type(current_obj)}")
     print(f"obj before render is {current_obj}")
     print(current_obj)
-    
+
     return render(current_obj)
 
+
 def c_by_type(data: dict):
     print(f"data is  {data}")
-    
+
     data_type = data.get("type")
     solution = transfer_to_dict(data.get("solution", ""))
     content = transfer_to_dict(data.get("content"))
     explains = transfer_to_dict(data.get("explains"))
     knowledge_point = data.get("knowledge_point", None)
     answer = content.get("answer", None)
     # Check for empty solutions in certain question types
     if data_type in [1, 2, 3] and not solution:
-        errorMsg('填空答案错误')
+        errorMsg("填空答案错误")
         return
 
     # Check for empty content in single and multiple choice questions
-    if data_type in [2, 3] and ('answer' not in content or not answer):
-        errorMsg('单选题干错误')
+    if data_type in [2, 3] and ("answer" not in content or not answer):
+        errorMsg("单选题干错误")
         return
 
     # Initialize the structure to store the processed data
-    json_data = {'type': data_type, 'solution': None, "caption": None}
+    json_data = {"type": data_type, "solution": None, "caption": None}
 
-
-    json_data["caption"] = c2(content["caption"])
+    json_data["caption"] = LatexRender.html_render(content["caption"])
     json_data["knowledge_point"] = knowledge_point
 
-    if data_type == 1 or data_type =="填空":
+    if data_type == 1 or data_type == "填空":
         # Fill-in-the-blank
-        answer_index = get_answer_index(content['caption'])
+        answer_index = get_answer_index(content["caption"])
         answer_index_count = len(answer_index)
 
-        json_data['solution'] = []
+        json_data["solution"] = []
         for sk, s in enumerate(solution):
             if sk > (answer_index_count - 1):
                 continue
 
             # if not validate_solution(s, qid):
             #     return
 
             # Process the solution based on its type
-            # json_data['solution'].append(render_solution(s))# 
-            # Todo: add render 
-            json_data['solution'].append(s)
+            # json_data['solution'].append(render_solution(s))#
+            # Todo: add render
+            json_data["solution"].append(s)
 
     elif data_type == 2:
         # Single choice
         print(solution)
         print(type(solution))
-        if not solution[0]['value']:
-            errorMsg('单选题答案为空')
+        if not solution[0]["value"]:
+            errorMsg("单选题答案为空")
             return
 
-        json_data['option'] = c2(content['answer'])
-        json_data['solution'] = solution[0]['value']
+        json_data["option"] = LatexRender.html_render(content["answer"])
+        json_data["solution"] = solution[0]["value"]
 
     elif data_type == 3:
         # Multiple choice
-        if not solution[0]['value']:
-            errorMsg('多选题答案为空')
+        if not solution[0]["value"]:
+            errorMsg("多选题答案为空")
             return
 
-        json_data['option'] = c2(content['answer'])
-        json_data['solution'] = solution[0]['value']
+        json_data["option"] = LatexRender.html_render(content["answer"])
+        json_data["solution"] = solution[0]["value"]
 
     elif data_type == 4:
         # Custom question type handling
-        qq = {'type': data_type, 'content': content, 'solution': solution, 'explains': explains}
-        
+        qq = {
+            "type": data_type,
+            "content": content,
+            "solution": solution,
+            "explains": explains,
+        }
+
         splits = ttl_question_show_answer(qq)
 
         if solution and splits is False:
             print(f"json data is {json_data}")
-            errorMsg('答案拆分失败, c_b_type')
+            errorMsg("答案拆分失败, c_b_type")
             return
 
         # json_data['solution'] = process_splits_solution(splits)
-        
+
         # Todo: add render
-        json_data['solution'] = splits
+        json_data["solution"] = splits
 
     else:
-        errorMsg('题目type错误')
+        errorMsg("题目type错误")
         return
-    
-    invalid = ['略', '详见答案']
+
+    invalid = ["略", "详见答案"]
     try:
-        ss = explains.get('解答设置')
+        ss = explains.get("解答设置")
     except:
-        print("Ex is ",explains)
-    if explains.get('解答设置') == 'same':
-        json_data['explain'] = ''
+        print("Ex is ", explains)
+    if explains.get("解答设置") == "same":
+        json_data["explain"] = ""
     else:
-        jieda = explains.get('解答')
+        jieda = explains.get("解答")
         if jieda:
             jieda = jieda.strip() if isinstance(jieda, str) else jieda
             if isinstance(jieda, str) and jieda in invalid:
-                json_data['explain'] = ''
+                json_data["explain"] = ""
             else:
                 # 假设 LatexRender.to_html 是一个已定义的函数，用来转换 LaTeX 字符串为 HTML
-                json_data['explain'] = c2(jieda)
+                json_data["explain"] = LatexRender.html_render(jieda)
         else:
-            json_data['explain'] = ''
+            json_data["explain"] = ""
 
     return json_data
 
-    
-    
+
 def errorMsg(msg, qid=1):
     print(f"Error in question {qid}: {msg}")
 
-    
 
 def get_answer_index(caption):
-        if isinstance(caption, dict):
-            index = []
-            if 'index' in caption and 'type' in caption:
-                index.append(caption)
-            else:
-                for key, value in caption.items():
-                    if isinstance(value, dict) and 'index' in value and 'type' in value:
-                        index.append(value)
-                    elif isinstance(value, (dict, list)):
-                        temp = get_answer_index(value)
-                        if temp:
-                            index.extend(temp)
-            return index if index else False
-
-        elif isinstance(caption, list):
-            index = []
-            for item in caption:
-                if isinstance(item, dict) and 'index' in item and 'type' in item:
-                    index.append(item)
-                elif isinstance(item, (dict, list)):
-                    temp = get_answer_index(item)
+    if isinstance(caption, dict):
+        index = []
+        if "index" in caption and "type" in caption:
+            index.append(caption)
+        else:
+            for key, value in caption.items():
+                if isinstance(value, dict) and "index" in value and "type" in value:
+                    index.append(value)
+                elif isinstance(value, (dict, list)):
+                    temp = get_answer_index(value)
                     if temp:
                         index.extend(temp)
-            return index if index else False
-        
-        
+        return index if index else False
+
+    elif isinstance(caption, list):
+        index = []
+        for item in caption:
+            if isinstance(item, dict) and "index" in item and "type" in item:
+                index.append(item)
+            elif isinstance(item, (dict, list)):
+                temp = get_answer_index(item)
+                if temp:
+                    index.extend(temp)
+        return index if index else False
+
+
 def ttl_question_show_answer(question, q_type=1, mode=0):
-        if question['type'] != 4:
-            return False
+    if question["type"] != 4:
+        return False
 
-        splits = split_question(question['type'], question['content'], question['solution'], question['explains'], True, mode)
-        if splits is False:
-            return False
+    splits = split_question(
+        question["type"],
+        question["content"],
+        question["solution"],
+        question["explains"],
+        True,
+        mode,
+    )
+    if splits is False:
+        return False
 
-        return splits
+    return splits
 
 
 def split_question(q_type, content, solution, explains, flag, mode):
     # Implementation of split_question method
     pass
 
 
 def c_by_type_new(data: dict):
+    print("new")
     print(f"data is  {data}")
-    
+
     data_id = data.get("id")
     data_type = data.get("type")
     solution = transfer_to_dict(data.get("solution", ""))
     content = transfer_to_dict(data.get("content"))
     explains = transfer_to_dict(data.get("explain"))
     print(f"explains is {explains}")
     knowledge_point = data.get("knowledge_point", None)
     difficulty = data.get("difficulty", None)
     answer = content.get("answer", None)
     # Check for empty solutions in certain question types
     if data_type in [1, 2, 3] and not solution:
-        errorMsg('填空答案错误')
+        errorMsg("填空答案错误")
         return
 
     # Check for empty content in single and multiple choice questions
-    if data_type in [2, 3] and ('answer' not in content or not answer):
-        errorMsg('单选题干错误')
+    if data_type in [2, 3] and ("answer" not in content or not answer):
+        errorMsg("单选题干错误")
         return
 
     # Initialize the structure to store the processed data
-    json_data = {'type': data_type, 'solution': None, "caption": None ,"id": data_id}
-
+    json_data = {"type": data_type, "solution": None, "caption": None, "id": data_id}
 
-    json_data["caption"] = c2(content["caption"])
+    json_data["caption"] = LatexRender.html_render(content["caption"])
     json_data["knowledge_point"] = knowledge_point
     json_data["difficulty"] = difficulty
-    
-    
 
     if data_type == 1:
         # Fill-in-the-blank
-        answer_index = get_answer_index(content['caption'])
+        answer_index = get_answer_index(content["caption"])
         answer_index_count = len(answer_index)
 
-        json_data['solution'] = []
+        json_data["solution"] = []
         for sk, s in enumerate(solution):
             if sk > (answer_index_count - 1):
                 continue
 
             # if not validate_solution(s, qid):
             #     return
 
             # Process the solution based on its type
-            # json_data['solution'].append(render_solution(s))# 
-            # Todo: add render 
-            json_data['solution'].append(s)
+            # json_data['solution'].append(render_solution(s))#
+            # Todo: add render
+            json_data["solution"].append(s)
 
     elif data_type == 2:
         # Single choice
         print(solution)
         print(type(solution))
-        if not solution[0]['value']:
-            errorMsg('单选题答案为空')
+        if not solution[0]["value"]:
+            errorMsg("单选题答案为空")
             return
 
-        json_data['option'] = c2(content['answer'])
-        json_data['solution'] = solution[0]['value']
+        json_data["option"] = LatexRender.html_render(content["answer"])
+        json_data["solution"] = solution[0]["value"]
 
     elif data_type == 3:
         # Multiple choice
-        if not solution[0]['value']:
-            errorMsg('多选题答案为空')
+        if not solution[0]["value"]:
+            errorMsg("多选题答案为空")
             return
 
-        json_data['option'] = c2(content['answer'])
-        json_data['solution'] = solution[0]['value']
+        json_data["option"] = LatexRender.html_render(content["answer"])
+        json_data["solution"] = solution[0]["value"]
 
     elif data_type == 4:
         # Custom question type handling
-        qq = {'type': data_type, 'content': content, 'solution': solution, 'explains': explains}
-        
+        qq = {
+            "type": data_type,
+            "content": content,
+            "solution": solution,
+            "explains": explains,
+        }
+
         splits = ttl_question_show_answer(qq)
 
         if solution and splits is False:
             print(f"ddd")
             print(f"json data is {json_data}")
-            errorMsg('答案拆分失败')
+            errorMsg("答案拆分失败")
             return
 
         # json_data['solution'] = process_splits_solution(splits)
-        
+
         # Todo: add render
-        json_data['solution'] = splits
+        json_data["solution"] = splits
 
     else:
         print(f"data type is {data_type}")
-        errorMsg('题目type错误')
+        errorMsg("题目type错误")
         return
-    
-    invalid = ['略', '详见答案']
+
+    invalid = ["略", "详见答案"]
     try:
-        ss = explains.get('解答设置')
+        ss = explains.get("解答设置")
     except:
-        print("Ex is ",explains)
-    if explains.get('解答设置') == 'same':
-        json_data['explain'] = ''
+        print("Ex is ", explains)
+    if explains.get("解答设置") == "same":
+        json_data["explain"] = ""
     else:
-        jieda = explains.get('解答')
+        jieda = explains.get("解答")
         if jieda:
             jieda = jieda.strip() if isinstance(jieda, str) else jieda
             if isinstance(jieda, str) and jieda in invalid:
-                json_data['explain'] = ''
+                json_data["explain"] = ""
             else:
                 # 假设 LatexRender.to_html 是一个已定义的函数，用来转换 LaTeX 字符串为 HTML
-                json_data['explain'] = c2(jieda)
+                json_data["explain"] = LatexRender.html_render(jieda)
         else:
-            json_data['explain'] = ''
+            json_data["explain"] = ""
 
-    return json_data
+    return json_data
```

### Comparing `latex_formatter-1.1.1/src/latex_formatter/utils/text_to_latex.py` & `latex_formatter-1.2.1/src/latex_formatter/utils/text_to_latex.py`

 * *Files identical despite different names*

### Comparing `latex_formatter-1.1.1/src/latex_formatter.egg-info/SOURCES.txt` & `latex_formatter-1.2.1/src/latex_formatter.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,10 +7,11 @@
 src/latex_formatter.egg-info/PKG-INFO
 src/latex_formatter.egg-info/SOURCES.txt
 src/latex_formatter.egg-info/dependency_links.txt
 src/latex_formatter.egg-info/requires.txt
 src/latex_formatter.egg-info/top_level.txt
 src/latex_formatter/converter/__init__.py
 src/latex_formatter/converter/converter.py
+src/latex_formatter/converter/web_converter.py
 src/latex_formatter/utils/__init__.py
 src/latex_formatter/utils/text_to_latex.py
 src/latex_formatter/utils/transfer.py
```

