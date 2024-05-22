# Comparing `tmp/olx-api-wrapper-0.3.4.tar.gz` & `tmp/olx-api-wrapper-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olx-api-wrapper-0.3.4.tar", last modified: Wed May 22 11:20:49 2024, max compression
+gzip compressed data, was "olx-api-wrapper-0.3.5.tar", last modified: Wed May 22 11:36:34 2024, max compression
```

## Comparing `olx-api-wrapper-0.3.4.tar` & `olx-api-wrapper-0.3.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.382879 olx-api-wrapper-0.3.4/olx/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/olx/partner/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/advert_logo.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/advert_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/adverts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/categories_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/cities_districts.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/languages_currencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/olx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/paid_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/payments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/threads_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/user_business.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/olx/public/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/checkout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/olx/public/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/olx/public/models/offers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/models/offers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/models/offers/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/models/offers/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/models/offers/offers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/olx/public/models/seo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/models/seo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/models/seo/offers.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/models/seo/popular_searches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/offers.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/olx_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/seo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/olx_api_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-22 11:20:49.000000 olx-api-wrapper-0.3.4/olx_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-22 11:20:49.000000 olx-api-wrapper-0.3.4/olx_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:20:49.000000 olx-api-wrapper-0.3.4/olx_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 11:20:49.000000 olx-api-wrapper-0.3.4/olx_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:20:49.000000 olx-api-wrapper-0.3.4/olx_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/tests/test_cities_and_districts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/tests/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.835610 olx-api-wrapper-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-05-22 11:36:34.835610 olx-api-wrapper-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.831610 olx-api-wrapper-0.3.5/olx/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.831610 olx-api-wrapper-0.3.5/olx/partner/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/advert_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/advert_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/adverts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/categories_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/cities_districts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/languages_currencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/olx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/paid_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/threads_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/user_business.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.831610 olx-api-wrapper-0.3.5/olx/public/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/checkout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.831610 olx-api-wrapper-0.3.5/olx/public/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.831610 olx-api-wrapper-0.3.5/olx/public/models/offers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/models/offers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/models/offers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/models/offers/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/models/offers/offers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.835610 olx-api-wrapper-0.3.5/olx/public/models/seo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/models/seo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/models/seo/offers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/models/seo/popular_searches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/offers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/olx_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/seo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.835610 olx-api-wrapper-0.3.5/olx_api_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-05-22 11:36:34.000000 olx-api-wrapper-0.3.5/olx_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-22 11:36:34.000000 olx-api-wrapper-0.3.5/olx_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:36:34.000000 olx-api-wrapper-0.3.5/olx_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 11:36:34.000000 olx-api-wrapper-0.3.5/olx_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:36:34.000000 olx-api-wrapper-0.3.5/olx_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 11:36:34.835610 olx-api-wrapper-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.835610 olx-api-wrapper-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/tests/test_cities_and_districts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/tests/test_users.py
```

### Comparing `olx-api-wrapper-0.3.4/LICENSE` & `olx-api-wrapper-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/PKG-INFO` & `olx-api-wrapper-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olx-api-wrapper
-Version: 0.3.4
+Version: 0.3.5
 Summary: Unofficial Wrapper for OLX API
 Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: Paweł Stawikowski
 Author-email: pawikoski@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.11
@@ -154,14 +154,25 @@
      client_id="your_client_id",
      client_secret="your_client_secret",
    )
    auth.authenticate(code='authorization_code')
    access_token = auth.access_token
    ```
 3. Now you have access token which you will need to have an access to OLX API resources.
+4. `authenticate()` method returns `AuthResponse`, so you can get other info like refresh token, scope or information about remaining time left.
+   ```python
+   auth_response = auth.authenticate(code='authorization_code')
+   # AuthResponse(access_token='access_token', expires_in=86367, token_type='bearer', scope='read write v2', refresh_token='refresh_token')
+   ```
+   To refresh expired access token just use refresh method as below:
+   ```python
+   auth.refresh(refresh_token=auth_response.refresh_token)
+   # If token is still valid, the response will be AuthResponse with current access token and time left (in seconds)
+   # If token is expired, the response will be AuthResponse with new access token and fresh expiration time
+   ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.4 Summary: Unofficial
+Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.5 Summary: Unofficial
 Wrapper for OLX API Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: PaweÅ Stawikowski Author-email: pawikoski@gmail.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
@@ -49,14 +49,24 @@
 olx-api-wrapper ``` 2. In order to get access token you need to authenticate
 with authorization code. [How to get authorization code?](https://
 developer.olx.pl/api/doc#section/Authentication/Grant-type:-authorization_code)
 ```python from olx.partner import Auth auth = Auth( client_id="your_client_id",
 client_secret="your_client_secret", ) auth.authenticate
 (code='authorization_code') access_token = auth.access_token ``` 3. Now you
 have access token which you will need to have an access to OLX API resources.
+4. `authenticate()` method returns `AuthResponse`, so you can get other info
+like refresh token, scope or information about remaining time left. ```python
+auth_response = auth.authenticate(code='authorization_code') # AuthResponse
+(access_token='access_token', expires_in=86367, token_type='bearer',
+scope='read write v2', refresh_token='refresh_token') ``` To refresh expired
+access token just use refresh method as below: ```python auth.refresh
+(refresh_token=auth_response.refresh_token) # If token is still valid, the
+response will be AuthResponse with current access token and time left (in
+seconds) # If token is expired, the response will be AuthResponse with new
+access token and fresh expiration time ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Usage Using `olx-api-wrapper` in Your Project Below are examples
 demonstrating the usage of `olx-api-wrapper` in your project. Please note that
 you require an access token to execute the actions described below. Each
 section from the OLX API documentation corresponds to a separate object within
 `olx-api-wrapper`. For instance, the section Users in the documentation is
 represented as olx.Users. Additionally, each endpoint mentioned in the
```

### Comparing `olx-api-wrapper-0.3.4/README.md` & `olx-api-wrapper-0.3.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -139,14 +139,25 @@
      client_id="your_client_id",
      client_secret="your_client_secret",
    )
    auth.authenticate(code='authorization_code')
    access_token = auth.access_token
    ```
 3. Now you have access token which you will need to have an access to OLX API resources.
+4. `authenticate()` method returns `AuthResponse`, so you can get other info like refresh token, scope or information about remaining time left.
+   ```python
+   auth_response = auth.authenticate(code='authorization_code')
+   # AuthResponse(access_token='access_token', expires_in=86367, token_type='bearer', scope='read write v2', refresh_token='refresh_token')
+   ```
+   To refresh expired access token just use refresh method as below:
+   ```python
+   auth.refresh(refresh_token=auth_response.refresh_token)
+   # If token is still valid, the response will be AuthResponse with current access token and time left (in seconds)
+   # If token is expired, the response will be AuthResponse with new access token and fresh expiration time
+   ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
```

#### html2text {}

```diff
@@ -43,14 +43,24 @@
 olx-api-wrapper ``` 2. In order to get access token you need to authenticate
 with authorization code. [How to get authorization code?](https://
 developer.olx.pl/api/doc#section/Authentication/Grant-type:-authorization_code)
 ```python from olx.partner import Auth auth = Auth( client_id="your_client_id",
 client_secret="your_client_secret", ) auth.authenticate
 (code='authorization_code') access_token = auth.access_token ``` 3. Now you
 have access token which you will need to have an access to OLX API resources.
+4. `authenticate()` method returns `AuthResponse`, so you can get other info
+like refresh token, scope or information about remaining time left. ```python
+auth_response = auth.authenticate(code='authorization_code') # AuthResponse
+(access_token='access_token', expires_in=86367, token_type='bearer',
+scope='read write v2', refresh_token='refresh_token') ``` To refresh expired
+access token just use refresh method as below: ```python auth.refresh
+(refresh_token=auth_response.refresh_token) # If token is still valid, the
+response will be AuthResponse with current access token and time left (in
+seconds) # If token is expired, the response will be AuthResponse with new
+access token and fresh expiration time ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Usage Using `olx-api-wrapper` in Your Project Below are examples
 demonstrating the usage of `olx-api-wrapper` in your project. Please note that
 you require an access token to execute the actions described below. Each
 section from the OLX API documentation corresponds to a separate object within
 `olx-api-wrapper`. For instance, the section Users in the documentation is
 represented as olx.Users. Additionally, each endpoint mentioned in the
```

### Comparing `olx-api-wrapper-0.3.4/olx/partner/advert_logo.py` & `olx-api-wrapper-0.3.5/olx/partner/advert_logo.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/partner/advert_statistics.py` & `olx-api-wrapper-0.3.5/olx/partner/advert_statistics.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/partner/adverts.py` & `olx-api-wrapper-0.3.5/olx/partner/adverts.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/partner/auth.py` & `olx-api-wrapper-0.3.5/olx/partner/auth.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/partner/categories_attributes.py` & `olx-api-wrapper-0.3.5/olx/partner/categories_attributes.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/partner/cities_districts.py` & `olx-api-wrapper-0.3.5/olx/partner/cities_districts.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/partner/languages_currencies.py` & `olx-api-wrapper-0.3.5/olx/partner/languages_currencies.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/partner/models.py` & `olx-api-wrapper-0.3.5/olx/partner/models.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/partner/olx.py` & `olx-api-wrapper-0.3.5/olx/partner/olx.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/partner/paid_features.py` & `olx-api-wrapper-0.3.5/olx/partner/paid_features.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/partner/payments.py` & `olx-api-wrapper-0.3.5/olx/partner/payments.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/partner/threads_messages.py` & `olx-api-wrapper-0.3.5/olx/partner/threads_messages.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/partner/users.py` & `olx-api-wrapper-0.3.5/olx/partner/users.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/public/checkout.py` & `olx-api-wrapper-0.3.5/olx/public/checkout.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/public/models/offers/filters.py` & `olx-api-wrapper-0.3.5/olx/public/models/offers/filters.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/public/models/offers/offers.py` & `olx-api-wrapper-0.3.5/olx/public/models/offers/offers.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/public/offers.py` & `olx-api-wrapper-0.3.5/olx/public/offers.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx/public/seo.py` & `olx-api-wrapper-0.3.5/olx/public/seo.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/olx_api_wrapper.egg-info/PKG-INFO` & `olx-api-wrapper-0.3.5/olx_api_wrapper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olx-api-wrapper
-Version: 0.3.4
+Version: 0.3.5
 Summary: Unofficial Wrapper for OLX API
 Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: Paweł Stawikowski
 Author-email: pawikoski@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.11
@@ -154,14 +154,25 @@
      client_id="your_client_id",
      client_secret="your_client_secret",
    )
    auth.authenticate(code='authorization_code')
    access_token = auth.access_token
    ```
 3. Now you have access token which you will need to have an access to OLX API resources.
+4. `authenticate()` method returns `AuthResponse`, so you can get other info like refresh token, scope or information about remaining time left.
+   ```python
+   auth_response = auth.authenticate(code='authorization_code')
+   # AuthResponse(access_token='access_token', expires_in=86367, token_type='bearer', scope='read write v2', refresh_token='refresh_token')
+   ```
+   To refresh expired access token just use refresh method as below:
+   ```python
+   auth.refresh(refresh_token=auth_response.refresh_token)
+   # If token is still valid, the response will be AuthResponse with current access token and time left (in seconds)
+   # If token is expired, the response will be AuthResponse with new access token and fresh expiration time
+   ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.4 Summary: Unofficial
+Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.5 Summary: Unofficial
 Wrapper for OLX API Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: PaweÅ Stawikowski Author-email: pawikoski@gmail.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
@@ -49,14 +49,24 @@
 olx-api-wrapper ``` 2. In order to get access token you need to authenticate
 with authorization code. [How to get authorization code?](https://
 developer.olx.pl/api/doc#section/Authentication/Grant-type:-authorization_code)
 ```python from olx.partner import Auth auth = Auth( client_id="your_client_id",
 client_secret="your_client_secret", ) auth.authenticate
 (code='authorization_code') access_token = auth.access_token ``` 3. Now you
 have access token which you will need to have an access to OLX API resources.
+4. `authenticate()` method returns `AuthResponse`, so you can get other info
+like refresh token, scope or information about remaining time left. ```python
+auth_response = auth.authenticate(code='authorization_code') # AuthResponse
+(access_token='access_token', expires_in=86367, token_type='bearer',
+scope='read write v2', refresh_token='refresh_token') ``` To refresh expired
+access token just use refresh method as below: ```python auth.refresh
+(refresh_token=auth_response.refresh_token) # If token is still valid, the
+response will be AuthResponse with current access token and time left (in
+seconds) # If token is expired, the response will be AuthResponse with new
+access token and fresh expiration time ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Usage Using `olx-api-wrapper` in Your Project Below are examples
 demonstrating the usage of `olx-api-wrapper` in your project. Please note that
 you require an access token to execute the actions described below. Each
 section from the OLX API documentation corresponds to a separate object within
 `olx-api-wrapper`. For instance, the section Users in the documentation is
 represented as olx.Users. Additionally, each endpoint mentioned in the
```

### Comparing `olx-api-wrapper-0.3.4/olx_api_wrapper.egg-info/SOURCES.txt` & `olx-api-wrapper-0.3.5/olx_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/setup.py` & `olx-api-wrapper-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="olx-api-wrapper",
-    version="0.3.4",
+    version="0.3.5",
     description="Unofficial Wrapper for OLX API",
     author="Paweł Stawikowski",
     author_email="pawikoski@gmail.com",
     packages=find_packages(),
     url="https://github.com/Pawikoski/olx-api-wrapper",
     install_requires=["requests", "dacite"],
     long_description=long_description,
```

### Comparing `olx-api-wrapper-0.3.4/tests/test_cities_and_districts.py` & `olx-api-wrapper-0.3.5/tests/test_cities_and_districts.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.4/tests/test_users.py` & `olx-api-wrapper-0.3.5/tests/test_users.py`

 * *Files identical despite different names*

