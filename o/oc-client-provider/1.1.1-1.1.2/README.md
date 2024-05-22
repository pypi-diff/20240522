# Comparing `tmp/oc_client_provider-1.1.1-py3-none-any.whl.zip` & `tmp/oc_client_provider-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 15728 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 15:08 oc_client_provider/__init__.py
--rw-r--r--  2.0 unx       60 b- defN 24-May-16 15:08 oc_client_provider/config.py
--rw-r--r--  2.0 unx      900 b- defN 24-May-16 15:08 oc_client_provider/wsgi.py
--rw-r--r--  2.0 unx      282 b- defN 24-May-16 15:08 oc_client_provider/app/__init__.py
--rw-r--r--  2.0 unx     1535 b- defN 24-May-16 15:08 oc_client_provider/app/client_counterparty.py
--rw-r--r--  2.0 unx    17637 b- defN 24-May-16 15:08 oc_client_provider/app/client_getter.py
--rw-r--r--  2.0 unx     3828 b- defN 24-May-16 15:08 oc_client_provider/app/client_tf.py
--rw-r--r--  2.0 unx     7103 b- defN 24-May-16 15:08 oc_client_provider/app/routes.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-16 15:08 oc_client_provider-1.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      408 b- defN 24-May-16 15:08 oc_client_provider-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-16 15:08 oc_client_provider-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-May-16 15:08 oc_client_provider-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1160 b- defN 24-May-16 15:08 oc_client_provider-1.1.1.dist-info/RECORD
-13 files, 44381 bytes uncompressed, 13752 bytes compressed:  69.0%
+Zip file size: 15956 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 07:58 oc_client_provider/__init__.py
+-rw-r--r--  2.0 unx       60 b- defN 24-May-22 07:58 oc_client_provider/config.py
+-rw-r--r--  2.0 unx      900 b- defN 24-May-22 07:58 oc_client_provider/wsgi.py
+-rw-r--r--  2.0 unx      282 b- defN 24-May-22 07:58 oc_client_provider/app/__init__.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-May-22 07:58 oc_client_provider/app/client_counterparty.py
+-rw-r--r--  2.0 unx    17637 b- defN 24-May-22 07:58 oc_client_provider/app/client_getter.py
+-rw-r--r--  2.0 unx     3828 b- defN 24-May-22 07:58 oc_client_provider/app/client_tf.py
+-rw-r--r--  2.0 unx     7777 b- defN 24-May-22 07:58 oc_client_provider/app/routes.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-22 07:58 oc_client_provider-1.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      408 b- defN 24-May-22 07:58 oc_client_provider-1.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-22 07:58 oc_client_provider-1.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-May-22 07:58 oc_client_provider-1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1160 b- defN 24-May-22 07:58 oc_client_provider-1.1.2.dist-info/RECORD
+13 files, 45055 bytes uncompressed, 13980 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: oc_client_provider/app/client_tf.py
 Comment: 
 
 Filename: oc_client_provider/app/routes.py
 Comment: 
 
-Filename: oc_client_provider-1.1.1.dist-info/LICENSE
+Filename: oc_client_provider-1.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: oc_client_provider-1.1.1.dist-info/METADATA
+Filename: oc_client_provider-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: oc_client_provider-1.1.1.dist-info/WHEEL
+Filename: oc_client_provider-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: oc_client_provider-1.1.1.dist-info/top_level.txt
+Filename: oc_client_provider-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: oc_client_provider-1.1.1.dist-info/RECORD
+Filename: oc_client_provider-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oc_client_provider/app/routes.py

```diff
@@ -57,14 +57,42 @@
         dict_writer.writerows(data)
 
     return Response(
         status=code,
         mimetype='text/csv',
         response=si.getvalue())
 
+
+def _adjust_arguments(args):
+    """
+    Convert and filter arguments
+    Do not raise any exception, just remove invalid
+    :param dict args: what to filter
+    """
+    if not args:
+        return args
+
+    for __k in list(args.keys()):
+        # non-string arguments is not allowed for this exact service
+        __v = args.get(__k)
+
+        if not isinstance(__v, str):
+            continue
+
+        __v = __v.strip().replace("\t", " ").replace(" ", "_")
+
+        if not __v:
+            del(args[__k])
+            continue
+
+        args[__k] = __v
+
+    return args
+
+
 @client_provider_bp.route('/rundeck/clients', methods=['GET'])
 @client_provider_bp.route('/clients', methods=['GET'])
 def get_client_list():
     """
     Endpoint returning list of active clients
     The difference between '/rundeck/clients' and general '/clients' endpoints:
     1. Clients are sorted alphabetically
@@ -193,20 +221,23 @@
 def sync_customer_tf():
     """
     Synchronize client record and return filtered list as requested
     """
     # doing our business depending on request type
     # returning normal JSON response
     logging.info("/sync_customer_tf from [%s]" % request.remote_addr)
-    logging.debug(f"Args: [{request.args}]")
+    _rq_args = _adjust_arguments(request.args.to_dict())
+    logging.debug(f"Args: [{_rq_args}]")
 
     _client_tf = ClientTF()
     # fork upon method used
     if request.method in ['PUT', 'DELETE']:
-        logging.debug(f"JSON: [{request.json}]")
+        _rq_json = _adjust_arguments(request.json)
+        logging.debug(f"JSON: [{_rq_json}]")
+        
         try:
-            getattr(_client_tf, f"{request.method.lower()}_client")(**request.json)
+            getattr(_client_tf, f"{request.method.lower()}_client")(**_rq_json)
         except Exception as _e:
             logging.exception(_e)
             return response_json(400, {"result": f"{repr(_e)}"})
 
-    return response_json(201 if request.method == 'PUT' else 200, _client_tf.get_client(**request.args))
+    return response_json(201 if request.method == 'PUT' else 200, _client_tf.get_client(**_rq_args))
```

## Comparing `oc_client_provider-1.1.1.dist-info/LICENSE` & `oc_client_provider-1.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `oc_client_provider-1.1.1.dist-info/RECORD` & `oc_client_provider-1.1.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 oc_client_provider/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 oc_client_provider/config.py,sha256=pdpVJleEvrb0NxkUCEaUfMsBaAcxumd3V-md-85g5JI,60
 oc_client_provider/wsgi.py,sha256=th56IJgqbOPvFIU97bKhNHjOracvebHWhlSSQ7jSKSg,900
 oc_client_provider/app/__init__.py,sha256=zS5TIy4y5ZDJnUdqvT04uP_fsgnMnT_UrpqgoW1CoNM,282
 oc_client_provider/app/client_counterparty.py,sha256=K39bmfFBfw2zg4eTn5yCOPqKaRziwWPx80F_RrDTB5Q,1535
 oc_client_provider/app/client_getter.py,sha256=2kmR3y8LovUza8-pjzHuDKkeife4g2iipfpYu8iKoTQ,17637
 oc_client_provider/app/client_tf.py,sha256=5gRYxfBr-uH0AYqxfEY5DdKBvLRmmmEzpvdvUlp0B8A,3828
-oc_client_provider/app/routes.py,sha256=jN8OszPO_0NcJCmUKlHe9lhP3-WyC9xHgdjmsea1YAI,7103
-oc_client_provider-1.1.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-oc_client_provider-1.1.1.dist-info/METADATA,sha256=d7PbbJRaHRKxPM52bNXBFG1Urb9kLnLV4X5QgI_RCRU,408
-oc_client_provider-1.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-oc_client_provider-1.1.1.dist-info/top_level.txt,sha256=8gL7z8xH1Rv4dE4wObBVzSaSzUcZeMVCQKkxtpCr0qI,19
-oc_client_provider-1.1.1.dist-info/RECORD,,
+oc_client_provider/app/routes.py,sha256=xpazJWu_uV4SpxlJLzkmgaN7d1PcZRSYoh-9yIgU0Ag,7777
+oc_client_provider-1.1.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+oc_client_provider-1.1.2.dist-info/METADATA,sha256=zjV5M_ToXVvXMsaySsov9BUmuwX9zEDjob8akGqAnIA,408
+oc_client_provider-1.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+oc_client_provider-1.1.2.dist-info/top_level.txt,sha256=8gL7z8xH1Rv4dE4wObBVzSaSzUcZeMVCQKkxtpCr0qI,19
+oc_client_provider-1.1.2.dist-info/RECORD,,
```

