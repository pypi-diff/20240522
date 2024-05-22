# Comparing `tmp/rest_solace-0.2.0.tar.gz` & `tmp/rest_solace-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_solace-0.2.0.tar", last modified: Sun May 19 20:19:35 2024, max compression
+gzip compressed data, was "rest_solace-0.2.1.tar", last modified: Wed May 22 06:18:23 2024, max compression
```

## Comparing `rest_solace-0.2.0.tar` & `rest_solace-0.2.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-19 20:19:35.666236 rest_solace-0.2.0/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      132 2024-05-14 15:14:18.000000 rest_solace-0.2.0/.gitignore
--rw-r--r--   0 skyler    (1000) skyler    (1000)    10178 2024-05-07 08:54:03.000000 rest_solace-0.2.0/LICENSE.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1694 2024-05-19 20:16:27.000000 rest_solace-0.2.0/NOTICE.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)     9553 2024-05-19 20:19:35.666236 rest_solace-0.2.0/PKG-INFO
--rw-r--r--   0 skyler    (1000) skyler    (1000)     8615 2024-05-19 20:01:09.000000 rest_solace-0.2.0/README.rst
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-19 20:19:35.634236 rest_solace-0.2.0/docs/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      579 2024-05-10 11:24:36.000000 rest_solace-0.2.0/docs/development_refrences.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1288 2024-05-10 17:40:06.000000 rest_solace-0.2.0/docs/getting_started_with_solace.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)      276 2024-05-10 17:58:06.000000 rest_solace-0.2.0/docs/index.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)      214 2024-05-14 15:11:52.000000 rest_solace-0.2.0/docs/semp_v2_endpoint_support.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2318 2024-05-19 20:14:39.000000 rest_solace-0.2.0/pyproject.toml
--rw-r--r--   0 skyler    (1000) skyler    (1000)       38 2024-05-19 20:19:35.666236 rest_solace-0.2.0/setup.cfg
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-19 20:19:35.630236 rest_solace-0.2.0/src/
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-19 20:19:35.638236 rest_solace-0.2.0/src/rest_solace/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      520 2024-04-20 20:43:31.000000 rest_solace-0.2.0/src/rest_solace/__init__.py
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-19 20:19:35.654236 rest_solace-0.2.0/src/rest_solace/__pycache__/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      359 2024-04-20 20:55:30.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2040 2024-04-07 08:23:01.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/action.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2224 2024-04-07 06:29:02.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5734 2024-04-21 05:54:01.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/consumer.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4876 2024-04-22 07:47:41.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/http_client.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4128 2024-04-07 19:18:05.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/manage.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)    20533 2024-04-22 10:02:53.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/manager.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1227 2024-03-31 13:04:04.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2742 2024-04-07 20:21:55.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/publish.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4538 2024-04-21 19:21:45.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/publisher.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4246 2024-04-07 18:11:44.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/semp_client.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     7341 2024-03-31 19:33:25.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5358 2024-04-20 19:56:40.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/subscriber.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5927 2024-05-19 16:38:53.000000 rest_solace-0.2.0/src/rest_solace/consumer.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)      125 2024-05-06 18:10:17.000000 rest_solace-0.2.0/src/rest_solace/exceptions.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5439 2024-05-19 19:45:08.000000 rest_solace-0.2.0/src/rest_solace/http_client.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)    31160 2024-05-19 19:46:54.000000 rest_solace-0.2.0/src/rest_solace/manager.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)    34588 2024-05-19 19:35:16.000000 rest_solace-0.2.0/src/rest_solace/publisher.py
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-19 20:19:35.666236 rest_solace-0.2.0/src/rest_solace.egg-info/
--rw-r--r--   0 skyler    (1000) skyler    (1000)     9553 2024-05-19 20:19:35.000000 rest_solace-0.2.0/src/rest_solace.egg-info/PKG-INFO
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1413 2024-05-19 20:19:35.000000 rest_solace-0.2.0/src/rest_solace.egg-info/SOURCES.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)        1 2024-05-19 20:19:35.000000 rest_solace-0.2.0/src/rest_solace.egg-info/dependency_links.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)       32 2024-05-19 20:19:35.000000 rest_solace-0.2.0/src/rest_solace.egg-info/requires.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)       12 2024-05-19 20:19:35.000000 rest_solace-0.2.0/src/rest_solace.egg-info/top_level.txt
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-19 20:19:35.662236 rest_solace-0.2.0/tests/
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-19 20:19:35.662236 rest_solace-0.2.0/tests/__pycache__/
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1419 2024-04-21 18:34:05.000000 rest_solace-0.2.0/tests/__pycache__/manager_unittest.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)      864 2024-05-06 18:46:43.000000 rest_solace-0.2.0/tests/consumer_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)      654 2024-05-12 08:11:53.000000 rest_solace-0.2.0/tests/empty_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     6920 2024-05-12 17:08:22.000000 rest_solace-0.2.0/tests/manager_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2835 2024-05-19 15:56:09.000000 rest_solace-0.2.0/tests/pub_sub_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     6499 2024-05-19 19:40:09.000000 rest_solace-0.2.0/tests/publisher_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)      891 2024-04-28 09:19:07.000000 rest_solace-0.2.0/tests/util.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-22 06:18:23.116738 rest_solace-0.2.1/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      132 2024-05-14 15:14:18.000000 rest_solace-0.2.1/.gitignore
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    10178 2024-05-07 08:54:03.000000 rest_solace-0.2.1/LICENSE.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1694 2024-05-19 20:16:27.000000 rest_solace-0.2.1/NOTICE.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     9649 2024-05-22 06:18:23.116738 rest_solace-0.2.1/PKG-INFO
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     8711 2024-05-22 06:16:03.000000 rest_solace-0.2.1/README.rst
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-22 06:18:23.096738 rest_solace-0.2.1/docs/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      579 2024-05-10 11:24:36.000000 rest_solace-0.2.1/docs/development_refrences.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2301 2024-05-22 06:14:30.000000 rest_solace-0.2.1/docs/getting_started_with_solace.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      276 2024-05-10 17:58:06.000000 rest_solace-0.2.1/docs/index.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      214 2024-05-14 15:11:52.000000 rest_solace-0.2.1/docs/semp_v2_endpoint_support.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2318 2024-05-22 06:16:45.000000 rest_solace-0.2.1/pyproject.toml
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       38 2024-05-22 06:18:23.116738 rest_solace-0.2.1/setup.cfg
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-22 06:18:23.092738 rest_solace-0.2.1/src/
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-22 06:18:23.100738 rest_solace-0.2.1/src/rest_solace/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      520 2024-04-20 20:43:31.000000 rest_solace-0.2.1/src/rest_solace/__init__.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-22 06:18:23.112738 rest_solace-0.2.1/src/rest_solace/__pycache__/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      359 2024-04-20 20:55:30.000000 rest_solace-0.2.1/src/rest_solace/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2040 2024-04-07 08:23:01.000000 rest_solace-0.2.1/src/rest_solace/__pycache__/action.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2224 2024-04-07 06:29:02.000000 rest_solace-0.2.1/src/rest_solace/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5734 2024-04-21 05:54:01.000000 rest_solace-0.2.1/src/rest_solace/__pycache__/consumer.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4876 2024-04-22 07:47:41.000000 rest_solace-0.2.1/src/rest_solace/__pycache__/http_client.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4128 2024-04-07 19:18:05.000000 rest_solace-0.2.1/src/rest_solace/__pycache__/manage.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    20533 2024-04-22 10:02:53.000000 rest_solace-0.2.1/src/rest_solace/__pycache__/manager.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1227 2024-03-31 13:04:04.000000 rest_solace-0.2.1/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2742 2024-04-07 20:21:55.000000 rest_solace-0.2.1/src/rest_solace/__pycache__/publish.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4538 2024-04-21 19:21:45.000000 rest_solace-0.2.1/src/rest_solace/__pycache__/publisher.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4246 2024-04-07 18:11:44.000000 rest_solace-0.2.1/src/rest_solace/__pycache__/semp_client.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     7341 2024-03-31 19:33:25.000000 rest_solace-0.2.1/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5358 2024-04-20 19:56:40.000000 rest_solace-0.2.1/src/rest_solace/__pycache__/subscriber.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5927 2024-05-19 16:38:53.000000 rest_solace-0.2.1/src/rest_solace/consumer.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      125 2024-05-06 18:10:17.000000 rest_solace-0.2.1/src/rest_solace/exceptions.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5439 2024-05-19 19:45:08.000000 rest_solace-0.2.1/src/rest_solace/http_client.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    31160 2024-05-19 19:46:54.000000 rest_solace-0.2.1/src/rest_solace/manager.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    34588 2024-05-19 19:35:16.000000 rest_solace-0.2.1/src/rest_solace/publisher.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-22 06:18:23.116738 rest_solace-0.2.1/src/rest_solace.egg-info/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     9649 2024-05-22 06:18:23.000000 rest_solace-0.2.1/src/rest_solace.egg-info/PKG-INFO
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1413 2024-05-22 06:18:23.000000 rest_solace-0.2.1/src/rest_solace.egg-info/SOURCES.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)        1 2024-05-22 06:18:23.000000 rest_solace-0.2.1/src/rest_solace.egg-info/dependency_links.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       32 2024-05-22 06:18:23.000000 rest_solace-0.2.1/src/rest_solace.egg-info/requires.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       12 2024-05-22 06:18:23.000000 rest_solace-0.2.1/src/rest_solace.egg-info/top_level.txt
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-22 06:18:23.112738 rest_solace-0.2.1/tests/
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-22 06:18:23.112738 rest_solace-0.2.1/tests/__pycache__/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1419 2024-04-21 18:34:05.000000 rest_solace-0.2.1/tests/__pycache__/manager_unittest.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      864 2024-05-06 18:46:43.000000 rest_solace-0.2.1/tests/consumer_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      654 2024-05-12 08:11:53.000000 rest_solace-0.2.1/tests/empty_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     6920 2024-05-12 17:08:22.000000 rest_solace-0.2.1/tests/manager_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2835 2024-05-19 15:56:09.000000 rest_solace-0.2.1/tests/pub_sub_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     6499 2024-05-19 19:40:09.000000 rest_solace-0.2.1/tests/publisher_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      891 2024-04-28 09:19:07.000000 rest_solace-0.2.1/tests/util.py
```

### Comparing `rest_solace-0.2.0/LICENSE.txt` & `rest_solace-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/NOTICE.txt` & `rest_solace-0.2.1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/PKG-INFO` & `rest_solace-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-solace
-Version: 0.2.0
+Version: 0.2.1
 Summary: REST API library for Solace Message Broker. Publish, Consume, & Manage!!
 Author-email: Skyler Guha <skylerguha@gmail.com>
 Maintainer-email: Skyler Guha <skylerguha@gmail.com>
 License: apache 2.0
 Project-URL: pypi, https://pypi.org/project/rest-solace/
 Project-URL: documentation, https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst
 Project-URL: repository, https://github.com/skyler-guha/rest-solace
@@ -22,26 +22,28 @@
 
 rest-solace
 ===============
 
 **rest-solace** is a rest based python library for Solace Message Broker that allows you to Publish, Consume, & Manage!!
 
 It is written with the intent to be easy to understand, functional, and pythonic.
-Input and output parameters for every function is always one of int, float, str, bool, list, dict and None; 
+Input and output parameters for almost every function is always one of int, float, str, bool, list, dict and None; 
 making them directly compatible with json data types. 
 
-| Check it out at `PyPI <https://pypi.org/project/rest-solace/>`_.
-| View the code at `Github <https://github.com/skyler-guha/rest-solace/>`_.
-| Read the docs from `Here <https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst/>`_.
-
 Note: 
     | Right now the focus of this library is on the 'messaging' mode for solace message VPNs.
     | In the future I plan to add better support for 'gateway' mode as well.
     | This library currently uses SEMPv2 for management. 
 
+|
+| Check it out at `PyPI <https://pypi.org/project/rest-solace/>`_.
+| View the code at `Github <https://github.com/skyler-guha/rest-solace/>`_.
+| Read the docs from `Here <https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst/>`_.
+
+
 Getting started with Solace:
 -----------------------------
 If you are new to solace and confused about the terminology and workflows around it, it is **highly** recommended 
 that you read `this <https://github.com/skyler-guha/rest-solace/blob/master/docs/getting_started_with_solace.rst/>`_ document first.
 It gives a brief explanation on the different components of solace; and that too within the context of this library.
 
 |
@@ -56,29 +58,29 @@
 
     publish = MessagingPublisher(user_name= "admin", 
                                        password=" admin", 
                                        host= BROKER_IP, 
                                        rest_vpn_port= VPN_PORT #For 'default' VPN it is 9000
                                        )
 
-    #Publish to a queue and (only confirms if the message was received by the broker)
+    #Publish to a queue (only confirms if the message was received by the broker)
     publish.direct_message_to_queue(queue_name= "my_queue",
                                     message= "hello world!!")
     
     #Publish for a topic string (only confirms if the message was received by the broker)
     publish.direct_message_for_topic(topic_string= "test_topic", 
                                      message= "hello world!!")
 
 
-    #Publish to a queue and wait for confirmation on if the message was spooled into a queue
+    #Publish to a queue and wait to confirm if the message was spooled into a queue
     publish.persistent_message_to_queue(queue_name= "my_queue", 
                                         message= "hello world!!",
                                         request_reply= False)                               
 
-    #Publish for a topic string and wait for confirmation on if the message was spooled into a queue
+    #Publish for a topic string and wait to confirm if the message was spooled into a queue
     publish.persistent_message_for_topic(topic_string= "test_topic", 
                                          message= "hello world!!",
                                          request_reply= False)
 
 
     #Publish to a queue and wait for reply from a consumer
     response = publish.persistent_message_to_queue(queue_name= "my_queue", 
@@ -177,19 +179,21 @@
 
                                               
     #Doing the same setup manually (Shown for comparison)
     manager.update_client_profile(msgVpnName= NEW_VPN_NAME, 
                                   clientProfileName= "default",
                                   allowGuaranteedMsgReceiveEnabled= True,
                                   allowGuaranteedMsgSendEnabled= True)
-    manager.update_client_username(msgVpnName=NEW_VPN_NAME, 
+    manager.update_client_username(msgVpnName= NEW_VPN_NAME, 
                                    clientUsername= "default",
                                    enabled= True)
     manager.create_queue_endpoint(queueName='my_queue', msgVpnName=NEW_VPN_NAME)
-    manager.subscribe_to_topic_on_queue(subscriptionTopic= "test_topic", queueName= 'my_queue')
+    manager.subscribe_to_topic_on_queue(msgVpnName= NEW_VPN_NAME,
+                                        subscriptionTopic= "test_topic", 
+                                        queueName= 'my_queue')
     manager.create_rest_delivery_point(msgVpnName= NEW_VPN_NAME, 
                                        restDeliveryPointName= 'myRDP', 
                                        clientProfileName= "default")
     manager.specify_rest_consumer(msgVpnName= NEW_VPN_NAME, 
                                   restDeliveryPointName= 'myRDP',
                                   restConsumerName= 'myConsumer',
                                   remoteHost= CONSUMER_HOST,
```

### Comparing `rest_solace-0.2.0/README.rst` & `rest_solace-0.2.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 rest-solace
 ===============
 
 **rest-solace** is a rest based python library for Solace Message Broker that allows you to Publish, Consume, & Manage!!
 
 It is written with the intent to be easy to understand, functional, and pythonic.
-Input and output parameters for every function is always one of int, float, str, bool, list, dict and None; 
+Input and output parameters for almost every function is always one of int, float, str, bool, list, dict and None; 
 making them directly compatible with json data types. 
 
-| Check it out at `PyPI <https://pypi.org/project/rest-solace/>`_.
-| View the code at `Github <https://github.com/skyler-guha/rest-solace/>`_.
-| Read the docs from `Here <https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst/>`_.
-
 Note: 
     | Right now the focus of this library is on the 'messaging' mode for solace message VPNs.
     | In the future I plan to add better support for 'gateway' mode as well.
     | This library currently uses SEMPv2 for management. 
 
+|
+| Check it out at `PyPI <https://pypi.org/project/rest-solace/>`_.
+| View the code at `Github <https://github.com/skyler-guha/rest-solace/>`_.
+| Read the docs from `Here <https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst/>`_.
+
+
 Getting started with Solace:
 -----------------------------
 If you are new to solace and confused about the terminology and workflows around it, it is **highly** recommended 
 that you read `this <https://github.com/skyler-guha/rest-solace/blob/master/docs/getting_started_with_solace.rst/>`_ document first.
 It gives a brief explanation on the different components of solace; and that too within the context of this library.
 
 |
@@ -34,29 +36,29 @@
 
     publish = MessagingPublisher(user_name= "admin", 
                                        password=" admin", 
                                        host= BROKER_IP, 
                                        rest_vpn_port= VPN_PORT #For 'default' VPN it is 9000
                                        )
 
-    #Publish to a queue and (only confirms if the message was received by the broker)
+    #Publish to a queue (only confirms if the message was received by the broker)
     publish.direct_message_to_queue(queue_name= "my_queue",
                                     message= "hello world!!")
     
     #Publish for a topic string (only confirms if the message was received by the broker)
     publish.direct_message_for_topic(topic_string= "test_topic", 
                                      message= "hello world!!")
 
 
-    #Publish to a queue and wait for confirmation on if the message was spooled into a queue
+    #Publish to a queue and wait to confirm if the message was spooled into a queue
     publish.persistent_message_to_queue(queue_name= "my_queue", 
                                         message= "hello world!!",
                                         request_reply= False)                               
 
-    #Publish for a topic string and wait for confirmation on if the message was spooled into a queue
+    #Publish for a topic string and wait to confirm if the message was spooled into a queue
     publish.persistent_message_for_topic(topic_string= "test_topic", 
                                          message= "hello world!!",
                                          request_reply= False)
 
 
     #Publish to a queue and wait for reply from a consumer
     response = publish.persistent_message_to_queue(queue_name= "my_queue", 
@@ -155,19 +157,21 @@
 
                                               
     #Doing the same setup manually (Shown for comparison)
     manager.update_client_profile(msgVpnName= NEW_VPN_NAME, 
                                   clientProfileName= "default",
                                   allowGuaranteedMsgReceiveEnabled= True,
                                   allowGuaranteedMsgSendEnabled= True)
-    manager.update_client_username(msgVpnName=NEW_VPN_NAME, 
+    manager.update_client_username(msgVpnName= NEW_VPN_NAME, 
                                    clientUsername= "default",
                                    enabled= True)
     manager.create_queue_endpoint(queueName='my_queue', msgVpnName=NEW_VPN_NAME)
-    manager.subscribe_to_topic_on_queue(subscriptionTopic= "test_topic", queueName= 'my_queue')
+    manager.subscribe_to_topic_on_queue(msgVpnName= NEW_VPN_NAME,
+                                        subscriptionTopic= "test_topic", 
+                                        queueName= 'my_queue')
     manager.create_rest_delivery_point(msgVpnName= NEW_VPN_NAME, 
                                        restDeliveryPointName= 'myRDP', 
                                        clientProfileName= "default")
     manager.specify_rest_consumer(msgVpnName= NEW_VPN_NAME, 
                                   restDeliveryPointName= 'myRDP',
                                   restConsumerName= 'myConsumer',
                                   remoteHost= CONSUMER_HOST,
```

### Comparing `rest_solace-0.2.0/docs/development_refrences.rst` & `rest_solace-0.2.1/docs/development_refrences.rst`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/pyproject.toml` & `rest_solace-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     #"threading",       #part of the standard library
     #"time"             #part of the standard library
     #"json",            #part of the standard library
     #"urllib"           #part of the standard library
     #"asyncio"          #part of the standard library
     #"logging"          #part of the standard library
 ]
-version = "0.2.0"
+version = "0.2.1"
 
 [project.urls]
 pypi = "https://pypi.org/project/rest-solace/"
 documentation = "https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst"
 repository = "https://github.com/skyler-guha/rest-solace"
 
 #Doing an editable install: pip install --editable .
```

### Comparing `rest_solace-0.2.0/src/rest_solace/__init__.py` & `rest_solace-0.2.1/src/rest_solace/__init__.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace/__pycache__/action.cpython-311.pyc` & `rest_solace-0.2.1/src/rest_solace/__pycache__/action.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace/__pycache__/config.cpython-311.pyc` & `rest_solace-0.2.1/src/rest_solace/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace/__pycache__/consumer.cpython-311.pyc` & `rest_solace-0.2.1/src/rest_solace/__pycache__/consumer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace/__pycache__/http_client.cpython-311.pyc` & `rest_solace-0.2.1/src/rest_solace/__pycache__/http_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace/__pycache__/manage.cpython-311.pyc` & `rest_solace-0.2.1/src/rest_solace/__pycache__/manage.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace/__pycache__/manager.cpython-311.pyc` & `rest_solace-0.2.1/src/rest_solace/__pycache__/manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc` & `rest_solace-0.2.1/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace/__pycache__/publish.cpython-311.pyc` & `rest_solace-0.2.1/src/rest_solace/__pycache__/publish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace/__pycache__/publisher.cpython-311.pyc` & `rest_solace-0.2.1/src/rest_solace/__pycache__/publisher.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace/__pycache__/semp_client.cpython-311.pyc` & `rest_solace-0.2.1/src/rest_solace/__pycache__/semp_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc` & `rest_solace-0.2.1/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace/__pycache__/subscriber.cpython-311.pyc` & `rest_solace-0.2.1/src/rest_solace/__pycache__/subscriber.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace/consumer.py` & `rest_solace-0.2.1/src/rest_solace/consumer.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace/http_client.py` & `rest_solace-0.2.1/src/rest_solace/http_client.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace/manager.py` & `rest_solace-0.2.1/src/rest_solace/manager.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace/publisher.py` & `rest_solace-0.2.1/src/rest_solace/publisher.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/src/rest_solace.egg-info/PKG-INFO` & `rest_solace-0.2.1/src/rest_solace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-solace
-Version: 0.2.0
+Version: 0.2.1
 Summary: REST API library for Solace Message Broker. Publish, Consume, & Manage!!
 Author-email: Skyler Guha <skylerguha@gmail.com>
 Maintainer-email: Skyler Guha <skylerguha@gmail.com>
 License: apache 2.0
 Project-URL: pypi, https://pypi.org/project/rest-solace/
 Project-URL: documentation, https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst
 Project-URL: repository, https://github.com/skyler-guha/rest-solace
@@ -22,26 +22,28 @@
 
 rest-solace
 ===============
 
 **rest-solace** is a rest based python library for Solace Message Broker that allows you to Publish, Consume, & Manage!!
 
 It is written with the intent to be easy to understand, functional, and pythonic.
-Input and output parameters for every function is always one of int, float, str, bool, list, dict and None; 
+Input and output parameters for almost every function is always one of int, float, str, bool, list, dict and None; 
 making them directly compatible with json data types. 
 
-| Check it out at `PyPI <https://pypi.org/project/rest-solace/>`_.
-| View the code at `Github <https://github.com/skyler-guha/rest-solace/>`_.
-| Read the docs from `Here <https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst/>`_.
-
 Note: 
     | Right now the focus of this library is on the 'messaging' mode for solace message VPNs.
     | In the future I plan to add better support for 'gateway' mode as well.
     | This library currently uses SEMPv2 for management. 
 
+|
+| Check it out at `PyPI <https://pypi.org/project/rest-solace/>`_.
+| View the code at `Github <https://github.com/skyler-guha/rest-solace/>`_.
+| Read the docs from `Here <https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst/>`_.
+
+
 Getting started with Solace:
 -----------------------------
 If you are new to solace and confused about the terminology and workflows around it, it is **highly** recommended 
 that you read `this <https://github.com/skyler-guha/rest-solace/blob/master/docs/getting_started_with_solace.rst/>`_ document first.
 It gives a brief explanation on the different components of solace; and that too within the context of this library.
 
 |
@@ -56,29 +58,29 @@
 
     publish = MessagingPublisher(user_name= "admin", 
                                        password=" admin", 
                                        host= BROKER_IP, 
                                        rest_vpn_port= VPN_PORT #For 'default' VPN it is 9000
                                        )
 
-    #Publish to a queue and (only confirms if the message was received by the broker)
+    #Publish to a queue (only confirms if the message was received by the broker)
     publish.direct_message_to_queue(queue_name= "my_queue",
                                     message= "hello world!!")
     
     #Publish for a topic string (only confirms if the message was received by the broker)
     publish.direct_message_for_topic(topic_string= "test_topic", 
                                      message= "hello world!!")
 
 
-    #Publish to a queue and wait for confirmation on if the message was spooled into a queue
+    #Publish to a queue and wait to confirm if the message was spooled into a queue
     publish.persistent_message_to_queue(queue_name= "my_queue", 
                                         message= "hello world!!",
                                         request_reply= False)                               
 
-    #Publish for a topic string and wait for confirmation on if the message was spooled into a queue
+    #Publish for a topic string and wait to confirm if the message was spooled into a queue
     publish.persistent_message_for_topic(topic_string= "test_topic", 
                                          message= "hello world!!",
                                          request_reply= False)
 
 
     #Publish to a queue and wait for reply from a consumer
     response = publish.persistent_message_to_queue(queue_name= "my_queue", 
@@ -177,19 +179,21 @@
 
                                               
     #Doing the same setup manually (Shown for comparison)
     manager.update_client_profile(msgVpnName= NEW_VPN_NAME, 
                                   clientProfileName= "default",
                                   allowGuaranteedMsgReceiveEnabled= True,
                                   allowGuaranteedMsgSendEnabled= True)
-    manager.update_client_username(msgVpnName=NEW_VPN_NAME, 
+    manager.update_client_username(msgVpnName= NEW_VPN_NAME, 
                                    clientUsername= "default",
                                    enabled= True)
     manager.create_queue_endpoint(queueName='my_queue', msgVpnName=NEW_VPN_NAME)
-    manager.subscribe_to_topic_on_queue(subscriptionTopic= "test_topic", queueName= 'my_queue')
+    manager.subscribe_to_topic_on_queue(msgVpnName= NEW_VPN_NAME,
+                                        subscriptionTopic= "test_topic", 
+                                        queueName= 'my_queue')
     manager.create_rest_delivery_point(msgVpnName= NEW_VPN_NAME, 
                                        restDeliveryPointName= 'myRDP', 
                                        clientProfileName= "default")
     manager.specify_rest_consumer(msgVpnName= NEW_VPN_NAME, 
                                   restDeliveryPointName= 'myRDP',
                                   restConsumerName= 'myConsumer',
                                   remoteHost= CONSUMER_HOST,
```

### Comparing `rest_solace-0.2.0/src/rest_solace.egg-info/SOURCES.txt` & `rest_solace-0.2.1/src/rest_solace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/tests/__pycache__/manager_unittest.cpython-311.pyc` & `rest_solace-0.2.1/tests/__pycache__/manager_unittest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/tests/consumer_test.py` & `rest_solace-0.2.1/tests/consumer_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/tests/empty_test.py` & `rest_solace-0.2.1/tests/empty_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/tests/manager_test.py` & `rest_solace-0.2.1/tests/manager_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/tests/pub_sub_test.py` & `rest_solace-0.2.1/tests/pub_sub_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/tests/publisher_test.py` & `rest_solace-0.2.1/tests/publisher_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.0/tests/util.py` & `rest_solace-0.2.1/tests/util.py`

 * *Files identical despite different names*

