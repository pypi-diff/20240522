# Comparing `tmp/netbox-plugin-auth-saml2-2.4.tar.gz` & `tmp/netbox-plugin-auth-saml2-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-plugin-auth-saml2-2.4.tar", last modified: Tue Oct 19 17:46:14 2021, max compression
+gzip compressed data, was "netbox-plugin-auth-saml2-3.0.tar", last modified: Wed May 22 11:17:37 2024, max compression
```

## Comparing `netbox-plugin-auth-saml2-2.4.tar` & `netbox-plugin-auth-saml2-3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jeremy.schulman   (504) staff       (20)        0 2021-10-19 17:46:14.397700 netbox-plugin-auth-saml2-2.4/
--rw-r--r--   0 jeremy.schulman   (504) staff       (20)     7029 2021-10-19 17:46:14.397465 netbox-plugin-auth-saml2-2.4/PKG-INFO
--rw-r--r--   0 jeremy.schulman   (504) staff       (20)     5734 2021-10-19 17:44:11.000000 netbox-plugin-auth-saml2-2.4/README.md
-drwxr-xr-x   0 jeremy.schulman   (504) staff       (20)        0 2021-10-19 17:46:14.395541 netbox-plugin-auth-saml2-2.4/django3_saml2_nbplugin/
--rw-r--r--   0 jeremy.schulman   (504) staff       (20)     1205 2021-10-19 17:44:11.000000 netbox-plugin-auth-saml2-2.4/django3_saml2_nbplugin/__init__.py
-drwxr-xr-x   0 jeremy.schulman   (504) staff       (20)        0 2021-10-19 17:46:14.395954 netbox-plugin-auth-saml2-2.4/django3_saml2_nbplugin/api/
--rw-r--r--   0 jeremy.schulman   (504) staff       (20)        0 2021-10-19 17:44:11.000000 netbox-plugin-auth-saml2-2.4/django3_saml2_nbplugin/api/__init__.py
--rw-r--r--   0 jeremy.schulman   (504) staff       (20)      140 2021-10-19 17:44:11.000000 netbox-plugin-auth-saml2-2.4/django3_saml2_nbplugin/api/urls.py
--rw-r--r--   0 jeremy.schulman   (504) staff       (20)     7463 2021-10-19 17:44:11.000000 netbox-plugin-auth-saml2-2.4/django3_saml2_nbplugin/backends.py
-drwxr-xr-x   0 jeremy.schulman   (504) staff       (20)        0 2021-10-19 17:46:14.397130 netbox-plugin-auth-saml2-2.4/netbox_plugin_auth_saml2.egg-info/
--rw-r--r--   0 jeremy.schulman   (504) staff       (20)     7029 2021-10-19 17:46:14.000000 netbox-plugin-auth-saml2-2.4/netbox_plugin_auth_saml2.egg-info/PKG-INFO
--rw-r--r--   0 jeremy.schulman   (504) staff       (20)      401 2021-10-19 17:46:14.000000 netbox-plugin-auth-saml2-2.4/netbox_plugin_auth_saml2.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy.schulman   (504) staff       (20)        1 2021-10-19 17:46:14.000000 netbox-plugin-auth-saml2-2.4/netbox_plugin_auth_saml2.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy.schulman   (504) staff       (20)        1 2021-10-19 17:46:14.000000 netbox-plugin-auth-saml2-2.4/netbox_plugin_auth_saml2.egg-info/not-zip-safe
--rw-r--r--   0 jeremy.schulman   (504) staff       (20)       23 2021-10-19 17:46:14.000000 netbox-plugin-auth-saml2-2.4/netbox_plugin_auth_saml2.egg-info/top_level.txt
--rw-r--r--   0 jeremy.schulman   (504) staff       (20)       38 2021-10-19 17:46:14.397771 netbox-plugin-auth-saml2-2.4/setup.cfg
--rw-r--r--   0 jeremy.schulman   (504) staff       (20)      479 2021-10-19 17:45:05.000000 netbox-plugin-auth-saml2-2.4/setup.py
+drwxr-xr-x   0 jeremy.schulman   (503) staff       (20)        0 2024-05-22 11:17:37.707666 netbox-plugin-auth-saml2-3.0/
+-rw-r--r--   0 jeremy.schulman   (503) staff       (20)     6386 2024-05-22 11:17:37.707498 netbox-plugin-auth-saml2-3.0/PKG-INFO
+-rw-r--r--   0 jeremy.schulman   (503) staff       (20)     6197 2024-05-22 11:12:27.000000 netbox-plugin-auth-saml2-3.0/README.md
+drwxr-xr-x   0 jeremy.schulman   (503) staff       (20)        0 2024-05-22 11:17:37.705621 netbox-plugin-auth-saml2-3.0/django3_saml2_nbplugin/
+-rw-r--r--   0 jeremy.schulman   (503) staff       (20)     1205 2024-05-22 11:12:27.000000 netbox-plugin-auth-saml2-3.0/django3_saml2_nbplugin/__init__.py
+drwxr-xr-x   0 jeremy.schulman   (503) staff       (20)        0 2024-05-22 11:17:37.706078 netbox-plugin-auth-saml2-3.0/django3_saml2_nbplugin/api/
+-rw-r--r--   0 jeremy.schulman   (503) staff       (20)        0 2024-05-22 11:12:27.000000 netbox-plugin-auth-saml2-3.0/django3_saml2_nbplugin/api/__init__.py
+-rw-r--r--   0 jeremy.schulman   (503) staff       (20)      140 2024-05-22 11:12:27.000000 netbox-plugin-auth-saml2-3.0/django3_saml2_nbplugin/api/urls.py
+-rw-r--r--   0 jeremy.schulman   (503) staff       (20)     7496 2024-05-22 11:12:27.000000 netbox-plugin-auth-saml2-3.0/django3_saml2_nbplugin/backends.py
+drwxr-xr-x   0 jeremy.schulman   (503) staff       (20)        0 2024-05-22 11:17:37.707203 netbox-plugin-auth-saml2-3.0/netbox_plugin_auth_saml2.egg-info/
+-rw-r--r--   0 jeremy.schulman   (503) staff       (20)     6386 2024-05-22 11:17:37.000000 netbox-plugin-auth-saml2-3.0/netbox_plugin_auth_saml2.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy.schulman   (503) staff       (20)      401 2024-05-22 11:17:37.000000 netbox-plugin-auth-saml2-3.0/netbox_plugin_auth_saml2.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy.schulman   (503) staff       (20)        1 2024-05-22 11:17:37.000000 netbox-plugin-auth-saml2-3.0/netbox_plugin_auth_saml2.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy.schulman   (503) staff       (20)        1 2024-05-22 11:13:31.000000 netbox-plugin-auth-saml2-3.0/netbox_plugin_auth_saml2.egg-info/not-zip-safe
+-rw-r--r--   0 jeremy.schulman   (503) staff       (20)       23 2024-05-22 11:17:37.000000 netbox-plugin-auth-saml2-3.0/netbox_plugin_auth_saml2.egg-info/top_level.txt
+-rw-r--r--   0 jeremy.schulman   (503) staff       (20)       38 2024-05-22 11:17:37.707739 netbox-plugin-auth-saml2-3.0/setup.cfg
+-rw-r--r--   0 jeremy.schulman   (503) staff       (20)      479 2024-05-22 11:16:59.000000 netbox-plugin-auth-saml2-3.0/setup.py
```

### Comparing `netbox-plugin-auth-saml2-2.4/PKG-INFO` & `netbox-plugin-auth-saml2-3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,142 +1,144 @@
-Metadata-Version: 2.1
-Name: netbox-plugin-auth-saml2
-Version: 2.4
-Summary: Netbox plugin for SAML2 auth
-Home-page: UNKNOWN
-Author: Jeremy Schulman
-License: Apache 2.0
-Description: # Netbox Plugin for SSO using SAML2
-        
-        Netbox 2.8 provides enhancements to support remote user authentication uses specific
-        variables defined in the configuration.py file, as described here:
-        
-        https://netbox.readthedocs.io/en/stable/configuration/optional-settings/
-        
-        This repository provides a Netbox plugin that can be used to integrate with a SAML SSO system,
-        such as Okta.
-        
-        *NOTE: This approach uses a reverse-proxy URL rewrite so that the standard Netbox Login will redirect
-        the User to the SSO system.  Please refer to the example [nginx.conf](nginx.conf) file.*
-        
-        *NOTE: Netbox plugin for SSO, v2.0+, supports Netbox 2.8, 2.9, 2.10, 2.11, 3.0.
-        
-        ## System Requirements
-        
-        You will need to install the [django3-auth-saml2](https://github.com/jeremyschulman/django3-auth-saml2)
-        into your Netbox environment.
-        
-        ## Netbox Configuration
-        
-        In the `configuration.py` you will need to enable and configure these
-        `REMOTE_AUTH_xxx` options at a minimum:
-        
-        ```python
-        REMOTE_AUTH_ENABLED = True
-        REMOTE_AUTH_BACKEND = 'utilities.auth_backends.RemoteUserBackend'
-        # For v2.8+:
-        # REMOTE_AUTH_BACKEND = 'netbox.authentication.RemoteUserBackend'
-        # For backends included with this plugin:
-        # REMOTE_AUTH_BACKEND = 'django3_saml2_nbplugin.backends.<Backend>'
-        REMOTE_AUTH_AUTO_CREATE_USER = True
-        ````
-        
-        You can also create the other options **REMOTE_AUTH_DEFAULT_GROUPS** and
-        **REMOTE_AUTH_DEFAULT_PERMISSIONS** as described in the online docs.
-        
-        Next you will need to configure this plugin, provding your specific
-        configuraiton values as described in
-        [django3-okta-saml2](https://github.com/jeremyschulman/django3-okta-saml2)
-        repo, for example:
-        
-        ```python
-        PLUGINS = ['django3_saml2_nbplugin']
-        
-        PLUGINS_CONFIG = {
-            'django3_saml2_nbplugin': {
-        
-                # Use the Netbox default remote backend
-                'AUTHENTICATION_BACKEND': REMOTE_AUTH_BACKEND,
-        
-                # Custom URL to validate incoming SAML requests against
-                'ASSERTION_URL': 'https://netbox.company.com',
-        
-                # Populates the Issuer element in authn reques e.g defined as "Audience URI (SP Entity ID)" in SSO
-                'ENTITY_ID': 'https://netbox.conpany.com/',
-        
-                # Metadata is required, choose either remote url
-                'METADATA_AUTO_CONF_URL': "https://mycorp.okta.com/app/sadjfalkdsflkads/sso/saml/metadata",
-                # or local file path
-                'METADATA_LOCAL_FILE_PATH': '/opt/netbox/saml2.xml',
-        
-                # Settings for SAML2CustomAttrUserBackend. Optional.
-                'CUSTOM_ATTR_BACKEND': {
-                    # Attribute containing the username. Optional.
-                    'USERNAME_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress',
-                    # Attribute containing the user's email. Optional.
-                    'MAIL_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress',
-                    # Attribute containing the user's first name. Optional.
-                    'FIRST_NAME_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname',
-                    # Attribute containing the user's last name. Optional.
-                    'LAST_NAME_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname',
-                    # Set to True to always update the user on logon
-                    # from SAML attributes on logon. Defaults to False.
-                    'ALWAYS_UPDATE_USER': False,
-                    # Attribute that contains groups. Optional.
-                    'GROUP_ATTR': 'http://schemas.microsoft.com/ws/2008/06/identity/claims/groups',
-                    # Dict of user flags to groups.
-                    # If the user is in the group then the flag will be set to True. Optional.
-                    'FLAGS_BY_GROUP': {
-                        'is_staff': 'saml-group1',
-                        'is_superuser': 'saml-group2'
-                    },
-                    # Dict of SAML groups to NetBox groups. Optional.
-                    # Groups must be created beforehand in NetBox.
-                    'GROUP_MAPPINGS': {
-                        'saml-group3': 'netbox-group'
-                    }
-                }
+# Netbox Plugin for SSO using SAML2
+
+Netbox 2.8 provides enhancements to support remote user authentication uses specific
+variables defined in the configuration.py file, as described here:
+
+https://netbox.readthedocs.io/en/stable/configuration/optional-settings/
+
+This repository provides a Netbox plugin that can be used to integrate with a SAML SSO system,
+such as Okta.
+
+*NOTE: This approach uses a reverse-proxy URL rewrite so that the standard Netbox Login will redirect
+the User to the SSO system.  Please refer to the example [nginx.conf](nginx.conf) file.*
+
+*NOTE: Netbox plugin for SSO, v2.0+, supports Netbox 2.8, 2.9, 2.10, 2.11, 3.0.
+
+*NOTE: Netbox plugin for SSO, v3.0+, supports Netbox 4.0.
+
+## System Requirements
+
+You will need to install the [django3-auth-saml2](https://github.com/jeremyschulman/django3-auth-saml2)
+into your Netbox environment.
+
+## Netbox Configuration
+
+In the `configuration.py` you will need to enable and configure these
+`REMOTE_AUTH_xxx` options at a minimum:
+
+```python
+REMOTE_AUTH_ENABLED = True
+REMOTE_AUTH_BACKEND = 'utilities.auth_backends.RemoteUserBackend'
+# For v2.8+:
+# REMOTE_AUTH_BACKEND = 'netbox.authentication.RemoteUserBackend'
+# For backends included with this plugin:
+# REMOTE_AUTH_BACKEND = 'django3_saml2_nbplugin.backends.<Backend>'
+REMOTE_AUTH_AUTO_CREATE_USER = True
+````
+
+You can also create the other options **REMOTE_AUTH_DEFAULT_GROUPS** and
+**REMOTE_AUTH_DEFAULT_PERMISSIONS** as described in the online docs.
+
+Next you will need to configure this plugin, provding your specific
+configuraiton values as described in
+[django3-okta-saml2](https://github.com/jeremyschulman/django3-okta-saml2)
+repo, for example:
+
+```python
+PLUGINS = ['django3_saml2_nbplugin']
+
+PLUGINS_CONFIG = {
+    'django3_saml2_nbplugin': {
+
+        # Use the Netbox default remote backend
+        'AUTHENTICATION_BACKEND': REMOTE_AUTH_BACKEND,
+
+        # Custom URL to validate incoming SAML requests against
+        'ASSERTION_URL': 'https://netbox.company.com',
+
+        # Populates the Issuer element in authn reques e.g defined as "Audience URI (SP Entity ID)" in SSO
+        'ENTITY_ID': 'https://netbox.conpany.com/',
+
+        # Metadata is required, choose either remote url
+        'METADATA_AUTO_CONF_URL': "https://mycorp.okta.com/app/sadjfalkdsflkads/sso/saml/metadata",
+        # or local file path
+        'METADATA_LOCAL_FILE_PATH': '/opt/netbox/saml2.xml',
+
+        # Settings for SAML2CustomAttrUserBackend. Optional.
+        'CUSTOM_ATTR_BACKEND': {
+            # See the note below about SAML attributes
+
+            # Attribute containing the username. Optional.
+            'USERNAME_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress',
+            # Attribute containing the user's email. Optional.
+            'MAIL_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress',
+            # Attribute containing the user's first name. Optional.
+            'FIRST_NAME_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname',
+            # Attribute containing the user's last name. Optional.
+            'LAST_NAME_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname',
+            # Set to True to always update the user on logon
+            # from SAML attributes on logon. Defaults to False.
+            'ALWAYS_UPDATE_USER': False,
+            # Attribute that contains groups. Optional.
+            'GROUP_ATTR': 'http://schemas.microsoft.com/ws/2008/06/identity/claims/groups',
+            # Dict of user flags to groups.
+            # If the user is in the group then the flag will be set to True. Optional.
+            'FLAGS_BY_GROUP': {
+                'is_staff': 'saml-group1',
+                'is_superuser': 'saml-group2'
+            },
+            # Dict of SAML groups to NetBox groups. Optional.
+            # Groups must be created beforehand in NetBox.
+            'GROUP_MAPPINGS': {
+                'saml-group3': 'netbox-group'
             }
         }
-        ```
-        
-        Please note that `METADATA_AUTO_CONF_URL` and `METADATA_LOCAL_FILE_PATH` are
-        mutually exclusive. Don't use both settings at the same time.
-        
-        # New Plugin URLs
-        This plugin will provide two new URLs to Netbox:
-        
-        `/plugins/sso/login/`<br/>
-        This URLs redirects the User login to the SSO system (Okta) for authentication.  This is the URL that needs
-        to be used in the reverse-proxy redirect, for examlple see [nginx.conf](nginx.conf#L35).
-        <br/><br/>
-        `/sso/acs/`<br/>
-        This URLs should be configured into your SSO system as the route to use to single-sign-on/redirection URL the User into Netbox
-        after the User has authenticated with the SSO system.
-        
-        # Customizing on Create New User Configuration
-        If you want to customize the way a User is created, beyond what is provided by the
-        Netbox REMOTE_AUTH variables, you can create a custom RemoteBackend class.  See
-        the samples in [backends.py](django3_saml2_nbplugin/backends.py).
-        
-        # Using A Reverse Proxy Redirect
-        The use of this plugin requires a reverse-proxy URL redirect to override the default Netbox `/login/` URL.  There
-        are two notes in this process:
-        
-           1.  You MAY need to disable port in redirect depending on your Netbox installation.  If your Netbox server URL
-           does _not_ include a port, then you _must_ disable port redirect.  For example see [nginx.conf](nginx.conf#L19).
-           1.  You MUST add the ULR rewrite for the `/login/` URL to use `/plugins/sso/login/`, for example [nginx.conf](nginx.conf#L35).
-        
-        # Adding a SSO Login Button
-        
-        Instead of using a reverse proxy redirect, you can add a SSO login button above
-        the NetBox login form. This has the added benefit of allowing both local
-        and SAML login options.
-        
-        Add the following to your configuration.py:
-        ```python
-        BANNER_LOGIN = '<a href="/api/plugins/sso/login" class="btn btn-primary btn-block">Login with SSO</a>'
-        ```
-        
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+    }
+}
+```
+
+Please note that `METADATA_AUTO_CONF_URL` and `METADATA_LOCAL_FILE_PATH` are
+mutually exclusive. Don't use both settings at the same time.
+
+## Attributes
+
+Newer versions of `pysaml2` uses an attribute map.
+For example, instead of `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress` in the configuration above, `emailAddress` should be used instead.
+
+See [here](https://github.com/IdentityPython/pysaml2/tree/master/src/saml2/attributemaps) for details.
+
+
+
+# New Plugin URLs
+This plugin will provide two new URLs to Netbox:
+
+`/api/plugins/sso/login/`<br/>
+This URLs redirects the User login to the SSO system (Okta) for authentication.  This is the URL that needs
+to be used in the reverse-proxy redirect, for examlple see [nginx.conf](nginx.conf#L35).
+<br/><br/>
+`/api/plugins/sso/acs/`<br/>
+This URLs should be configured into your SSO system as the route to use to single-sign-on/redirection URL the User into Netbox
+after the User has authenticated with the SSO system.
+
+# Customizing on Create New User Configuration
+If you want to customize the way a User is created, beyond what is provided by the
+Netbox REMOTE_AUTH variables, you can create a custom RemoteBackend class.  See
+the samples in [backends.py](django3_saml2_nbplugin/backends.py).
+
+# Using A Reverse Proxy Redirect
+The use of this plugin requires a reverse-proxy URL redirect to override the default Netbox `/login/` URL.  There
+are two notes in this process:
+
+   1.  You MAY need to disable port in redirect depending on your Netbox installation.  If your Netbox server URL
+   does _not_ include a port, then you _must_ disable port redirect.  For example see [nginx.conf](nginx.conf#L19).
+   1.  You MUST add the ULR rewrite for the `/login/` URL to use `/plugins/sso/login/`, for example [nginx.conf](nginx.conf#L35).
+
+# Adding a SSO Login Button
+
+Instead of using a reverse proxy redirect, you can add a SSO login button above
+the NetBox login form. This has the added benefit of allowing both local
+and SAML login options.
+
+Add the following to your configuration.py:
+```python
+BANNER_LOGIN = '<a href="/api/plugins/sso/login" class="btn btn-primary btn-block">Login with SSO</a>'
+```
```

### Comparing `netbox-plugin-auth-saml2-2.4/README.md` & `netbox-plugin-auth-saml2-3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: netbox-plugin-auth-saml2
+Version: 3.0
+Summary: Netbox plugin for SAML2 auth
+Author: Jeremy Schulman
+License: Apache 2.0
+Description-Content-Type: text/markdown
+
 # Netbox Plugin for SSO using SAML2
 
 Netbox 2.8 provides enhancements to support remote user authentication uses specific
 variables defined in the configuration.py file, as described here:
 
 https://netbox.readthedocs.io/en/stable/configuration/optional-settings/
 
@@ -9,14 +17,16 @@
 such as Okta.
 
 *NOTE: This approach uses a reverse-proxy URL rewrite so that the standard Netbox Login will redirect
 the User to the SSO system.  Please refer to the example [nginx.conf](nginx.conf) file.*
 
 *NOTE: Netbox plugin for SSO, v2.0+, supports Netbox 2.8, 2.9, 2.10, 2.11, 3.0.
 
+*NOTE: Netbox plugin for SSO, v3.0+, supports Netbox 4.0.
+
 ## System Requirements
 
 You will need to install the [django3-auth-saml2](https://github.com/jeremyschulman/django3-auth-saml2)
 into your Netbox environment.
 
 ## Netbox Configuration
 
@@ -59,14 +69,16 @@
         # Metadata is required, choose either remote url
         'METADATA_AUTO_CONF_URL': "https://mycorp.okta.com/app/sadjfalkdsflkads/sso/saml/metadata",
         # or local file path
         'METADATA_LOCAL_FILE_PATH': '/opt/netbox/saml2.xml',
 
         # Settings for SAML2CustomAttrUserBackend. Optional.
         'CUSTOM_ATTR_BACKEND': {
+            # See the note below about SAML attributes
+
             # Attribute containing the username. Optional.
             'USERNAME_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress',
             # Attribute containing the user's email. Optional.
             'MAIL_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress',
             # Attribute containing the user's first name. Optional.
             'FIRST_NAME_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname',
             # Attribute containing the user's last name. Optional.
@@ -91,22 +103,31 @@
     }
 }
 ```
 
 Please note that `METADATA_AUTO_CONF_URL` and `METADATA_LOCAL_FILE_PATH` are
 mutually exclusive. Don't use both settings at the same time.
 
+## Attributes
+
+Newer versions of `pysaml2` uses an attribute map.
+For example, instead of `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress` in the configuration above, `emailAddress` should be used instead.
+
+See [here](https://github.com/IdentityPython/pysaml2/tree/master/src/saml2/attributemaps) for details.
+
+
+
 # New Plugin URLs
 This plugin will provide two new URLs to Netbox:
 
-`/plugins/sso/login/`<br/>
+`/api/plugins/sso/login/`<br/>
 This URLs redirects the User login to the SSO system (Okta) for authentication.  This is the URL that needs
 to be used in the reverse-proxy redirect, for examlple see [nginx.conf](nginx.conf#L35).
 <br/><br/>
-`/sso/acs/`<br/>
+`/api/plugins/sso/acs/`<br/>
 This URLs should be configured into your SSO system as the route to use to single-sign-on/redirection URL the User into Netbox
 after the User has authenticated with the SSO system.
 
 # Customizing on Create New User Configuration
 If you want to customize the way a User is created, beyond what is provided by the
 Netbox REMOTE_AUTH variables, you can create a custom RemoteBackend class.  See
 the samples in [backends.py](django3_saml2_nbplugin/backends.py).
@@ -125,8 +146,7 @@
 the NetBox login form. This has the added benefit of allowing both local
 and SAML login options.
 
 Add the following to your configuration.py:
 ```python
 BANNER_LOGIN = '<a href="/api/plugins/sso/login" class="btn btn-primary btn-block">Login with SSO</a>'
 ```
-
```

### Comparing `netbox-plugin-auth-saml2-2.4/django3_saml2_nbplugin/__init__.py` & `netbox-plugin-auth-saml2-3.0/django3_saml2_nbplugin/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 as a dictionary, and this plugin is used to copy the contents provided from the
 PLUGIN_CONFIG in configuration.py into SAML2_AUTH_CONFIG.
 
 Do not try to modify django.conf.settings.SAML2_AUTH_CONFIG since by the time
 this plugin is invoked the settings is already configured, and if you try
 settings.configure(SAML2_AUTH_CONFIG=user_config) an exception will be raised.
 """
-from extras.plugins import PluginConfig
+from netbox.plugins import PluginConfig
 from django3_auth_saml2.config import SAML2_AUTH_CONFIG
 
 
 class Django3AuthSAML2Plugin(PluginConfig):
     name = 'django3_saml2_nbplugin'
     verbose_name = 'Netbox SSO SAML2 plugin'
     description = 'SSO support using SAML 2.0'
```

### Comparing `netbox-plugin-auth-saml2-2.4/django3_saml2_nbplugin/backends.py` & `netbox-plugin-auth-saml2-3.0/django3_saml2_nbplugin/backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional
-from django.contrib.auth.models import User, Group
-from django.core.handlers.wsgi import WSGIRequest
 from django.conf import settings
+from django.contrib.auth.models import User
+from django.core.handlers.wsgi import WSGIRequest
+from netbox.authentication import Group
 from saml2.response import AuthnResponse
 
 # Subclass from the Netbox provided RemoteUserBackend so that we get the
 # benefits of the REMOTE_AUTH_DEFAULT_GROUPS and
 # REMOTE_AUTH_DEFAULT_PERMISSIONS
 
 try:
```

### Comparing `netbox-plugin-auth-saml2-2.4/netbox_plugin_auth_saml2.egg-info/PKG-INFO` & `netbox-plugin-auth-saml2-3.0/netbox_plugin_auth_saml2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,142 +1,152 @@
 Metadata-Version: 2.1
 Name: netbox-plugin-auth-saml2
-Version: 2.4
+Version: 3.0
 Summary: Netbox plugin for SAML2 auth
-Home-page: UNKNOWN
 Author: Jeremy Schulman
 License: Apache 2.0
-Description: # Netbox Plugin for SSO using SAML2
-        
-        Netbox 2.8 provides enhancements to support remote user authentication uses specific
-        variables defined in the configuration.py file, as described here:
-        
-        https://netbox.readthedocs.io/en/stable/configuration/optional-settings/
-        
-        This repository provides a Netbox plugin that can be used to integrate with a SAML SSO system,
-        such as Okta.
-        
-        *NOTE: This approach uses a reverse-proxy URL rewrite so that the standard Netbox Login will redirect
-        the User to the SSO system.  Please refer to the example [nginx.conf](nginx.conf) file.*
-        
-        *NOTE: Netbox plugin for SSO, v2.0+, supports Netbox 2.8, 2.9, 2.10, 2.11, 3.0.
-        
-        ## System Requirements
-        
-        You will need to install the [django3-auth-saml2](https://github.com/jeremyschulman/django3-auth-saml2)
-        into your Netbox environment.
-        
-        ## Netbox Configuration
-        
-        In the `configuration.py` you will need to enable and configure these
-        `REMOTE_AUTH_xxx` options at a minimum:
-        
-        ```python
-        REMOTE_AUTH_ENABLED = True
-        REMOTE_AUTH_BACKEND = 'utilities.auth_backends.RemoteUserBackend'
-        # For v2.8+:
-        # REMOTE_AUTH_BACKEND = 'netbox.authentication.RemoteUserBackend'
-        # For backends included with this plugin:
-        # REMOTE_AUTH_BACKEND = 'django3_saml2_nbplugin.backends.<Backend>'
-        REMOTE_AUTH_AUTO_CREATE_USER = True
-        ````
-        
-        You can also create the other options **REMOTE_AUTH_DEFAULT_GROUPS** and
-        **REMOTE_AUTH_DEFAULT_PERMISSIONS** as described in the online docs.
-        
-        Next you will need to configure this plugin, provding your specific
-        configuraiton values as described in
-        [django3-okta-saml2](https://github.com/jeremyschulman/django3-okta-saml2)
-        repo, for example:
-        
-        ```python
-        PLUGINS = ['django3_saml2_nbplugin']
-        
-        PLUGINS_CONFIG = {
-            'django3_saml2_nbplugin': {
-        
-                # Use the Netbox default remote backend
-                'AUTHENTICATION_BACKEND': REMOTE_AUTH_BACKEND,
-        
-                # Custom URL to validate incoming SAML requests against
-                'ASSERTION_URL': 'https://netbox.company.com',
-        
-                # Populates the Issuer element in authn reques e.g defined as "Audience URI (SP Entity ID)" in SSO
-                'ENTITY_ID': 'https://netbox.conpany.com/',
-        
-                # Metadata is required, choose either remote url
-                'METADATA_AUTO_CONF_URL': "https://mycorp.okta.com/app/sadjfalkdsflkads/sso/saml/metadata",
-                # or local file path
-                'METADATA_LOCAL_FILE_PATH': '/opt/netbox/saml2.xml',
-        
-                # Settings for SAML2CustomAttrUserBackend. Optional.
-                'CUSTOM_ATTR_BACKEND': {
-                    # Attribute containing the username. Optional.
-                    'USERNAME_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress',
-                    # Attribute containing the user's email. Optional.
-                    'MAIL_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress',
-                    # Attribute containing the user's first name. Optional.
-                    'FIRST_NAME_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname',
-                    # Attribute containing the user's last name. Optional.
-                    'LAST_NAME_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname',
-                    # Set to True to always update the user on logon
-                    # from SAML attributes on logon. Defaults to False.
-                    'ALWAYS_UPDATE_USER': False,
-                    # Attribute that contains groups. Optional.
-                    'GROUP_ATTR': 'http://schemas.microsoft.com/ws/2008/06/identity/claims/groups',
-                    # Dict of user flags to groups.
-                    # If the user is in the group then the flag will be set to True. Optional.
-                    'FLAGS_BY_GROUP': {
-                        'is_staff': 'saml-group1',
-                        'is_superuser': 'saml-group2'
-                    },
-                    # Dict of SAML groups to NetBox groups. Optional.
-                    # Groups must be created beforehand in NetBox.
-                    'GROUP_MAPPINGS': {
-                        'saml-group3': 'netbox-group'
-                    }
-                }
+Description-Content-Type: text/markdown
+
+# Netbox Plugin for SSO using SAML2
+
+Netbox 2.8 provides enhancements to support remote user authentication uses specific
+variables defined in the configuration.py file, as described here:
+
+https://netbox.readthedocs.io/en/stable/configuration/optional-settings/
+
+This repository provides a Netbox plugin that can be used to integrate with a SAML SSO system,
+such as Okta.
+
+*NOTE: This approach uses a reverse-proxy URL rewrite so that the standard Netbox Login will redirect
+the User to the SSO system.  Please refer to the example [nginx.conf](nginx.conf) file.*
+
+*NOTE: Netbox plugin for SSO, v2.0+, supports Netbox 2.8, 2.9, 2.10, 2.11, 3.0.
+
+*NOTE: Netbox plugin for SSO, v3.0+, supports Netbox 4.0.
+
+## System Requirements
+
+You will need to install the [django3-auth-saml2](https://github.com/jeremyschulman/django3-auth-saml2)
+into your Netbox environment.
+
+## Netbox Configuration
+
+In the `configuration.py` you will need to enable and configure these
+`REMOTE_AUTH_xxx` options at a minimum:
+
+```python
+REMOTE_AUTH_ENABLED = True
+REMOTE_AUTH_BACKEND = 'utilities.auth_backends.RemoteUserBackend'
+# For v2.8+:
+# REMOTE_AUTH_BACKEND = 'netbox.authentication.RemoteUserBackend'
+# For backends included with this plugin:
+# REMOTE_AUTH_BACKEND = 'django3_saml2_nbplugin.backends.<Backend>'
+REMOTE_AUTH_AUTO_CREATE_USER = True
+````
+
+You can also create the other options **REMOTE_AUTH_DEFAULT_GROUPS** and
+**REMOTE_AUTH_DEFAULT_PERMISSIONS** as described in the online docs.
+
+Next you will need to configure this plugin, provding your specific
+configuraiton values as described in
+[django3-okta-saml2](https://github.com/jeremyschulman/django3-okta-saml2)
+repo, for example:
+
+```python
+PLUGINS = ['django3_saml2_nbplugin']
+
+PLUGINS_CONFIG = {
+    'django3_saml2_nbplugin': {
+
+        # Use the Netbox default remote backend
+        'AUTHENTICATION_BACKEND': REMOTE_AUTH_BACKEND,
+
+        # Custom URL to validate incoming SAML requests against
+        'ASSERTION_URL': 'https://netbox.company.com',
+
+        # Populates the Issuer element in authn reques e.g defined as "Audience URI (SP Entity ID)" in SSO
+        'ENTITY_ID': 'https://netbox.conpany.com/',
+
+        # Metadata is required, choose either remote url
+        'METADATA_AUTO_CONF_URL': "https://mycorp.okta.com/app/sadjfalkdsflkads/sso/saml/metadata",
+        # or local file path
+        'METADATA_LOCAL_FILE_PATH': '/opt/netbox/saml2.xml',
+
+        # Settings for SAML2CustomAttrUserBackend. Optional.
+        'CUSTOM_ATTR_BACKEND': {
+            # See the note below about SAML attributes
+
+            # Attribute containing the username. Optional.
+            'USERNAME_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress',
+            # Attribute containing the user's email. Optional.
+            'MAIL_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress',
+            # Attribute containing the user's first name. Optional.
+            'FIRST_NAME_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname',
+            # Attribute containing the user's last name. Optional.
+            'LAST_NAME_ATTR': 'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname',
+            # Set to True to always update the user on logon
+            # from SAML attributes on logon. Defaults to False.
+            'ALWAYS_UPDATE_USER': False,
+            # Attribute that contains groups. Optional.
+            'GROUP_ATTR': 'http://schemas.microsoft.com/ws/2008/06/identity/claims/groups',
+            # Dict of user flags to groups.
+            # If the user is in the group then the flag will be set to True. Optional.
+            'FLAGS_BY_GROUP': {
+                'is_staff': 'saml-group1',
+                'is_superuser': 'saml-group2'
+            },
+            # Dict of SAML groups to NetBox groups. Optional.
+            # Groups must be created beforehand in NetBox.
+            'GROUP_MAPPINGS': {
+                'saml-group3': 'netbox-group'
             }
         }
-        ```
-        
-        Please note that `METADATA_AUTO_CONF_URL` and `METADATA_LOCAL_FILE_PATH` are
-        mutually exclusive. Don't use both settings at the same time.
-        
-        # New Plugin URLs
-        This plugin will provide two new URLs to Netbox:
-        
-        `/plugins/sso/login/`<br/>
-        This URLs redirects the User login to the SSO system (Okta) for authentication.  This is the URL that needs
-        to be used in the reverse-proxy redirect, for examlple see [nginx.conf](nginx.conf#L35).
-        <br/><br/>
-        `/sso/acs/`<br/>
-        This URLs should be configured into your SSO system as the route to use to single-sign-on/redirection URL the User into Netbox
-        after the User has authenticated with the SSO system.
-        
-        # Customizing on Create New User Configuration
-        If you want to customize the way a User is created, beyond what is provided by the
-        Netbox REMOTE_AUTH variables, you can create a custom RemoteBackend class.  See
-        the samples in [backends.py](django3_saml2_nbplugin/backends.py).
-        
-        # Using A Reverse Proxy Redirect
-        The use of this plugin requires a reverse-proxy URL redirect to override the default Netbox `/login/` URL.  There
-        are two notes in this process:
-        
-           1.  You MAY need to disable port in redirect depending on your Netbox installation.  If your Netbox server URL
-           does _not_ include a port, then you _must_ disable port redirect.  For example see [nginx.conf](nginx.conf#L19).
-           1.  You MUST add the ULR rewrite for the `/login/` URL to use `/plugins/sso/login/`, for example [nginx.conf](nginx.conf#L35).
-        
-        # Adding a SSO Login Button
-        
-        Instead of using a reverse proxy redirect, you can add a SSO login button above
-        the NetBox login form. This has the added benefit of allowing both local
-        and SAML login options.
-        
-        Add the following to your configuration.py:
-        ```python
-        BANNER_LOGIN = '<a href="/api/plugins/sso/login" class="btn btn-primary btn-block">Login with SSO</a>'
-        ```
-        
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+    }
+}
+```
+
+Please note that `METADATA_AUTO_CONF_URL` and `METADATA_LOCAL_FILE_PATH` are
+mutually exclusive. Don't use both settings at the same time.
+
+## Attributes
+
+Newer versions of `pysaml2` uses an attribute map.
+For example, instead of `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress` in the configuration above, `emailAddress` should be used instead.
+
+See [here](https://github.com/IdentityPython/pysaml2/tree/master/src/saml2/attributemaps) for details.
+
+
+
+# New Plugin URLs
+This plugin will provide two new URLs to Netbox:
+
+`/api/plugins/sso/login/`<br/>
+This URLs redirects the User login to the SSO system (Okta) for authentication.  This is the URL that needs
+to be used in the reverse-proxy redirect, for examlple see [nginx.conf](nginx.conf#L35).
+<br/><br/>
+`/api/plugins/sso/acs/`<br/>
+This URLs should be configured into your SSO system as the route to use to single-sign-on/redirection URL the User into Netbox
+after the User has authenticated with the SSO system.
+
+# Customizing on Create New User Configuration
+If you want to customize the way a User is created, beyond what is provided by the
+Netbox REMOTE_AUTH variables, you can create a custom RemoteBackend class.  See
+the samples in [backends.py](django3_saml2_nbplugin/backends.py).
+
+# Using A Reverse Proxy Redirect
+The use of this plugin requires a reverse-proxy URL redirect to override the default Netbox `/login/` URL.  There
+are two notes in this process:
+
+   1.  You MAY need to disable port in redirect depending on your Netbox installation.  If your Netbox server URL
+   does _not_ include a port, then you _must_ disable port redirect.  For example see [nginx.conf](nginx.conf#L19).
+   1.  You MUST add the ULR rewrite for the `/login/` URL to use `/plugins/sso/login/`, for example [nginx.conf](nginx.conf#L35).
+
+# Adding a SSO Login Button
+
+Instead of using a reverse proxy redirect, you can add a SSO login button above
+the NetBox login form. This has the added benefit of allowing both local
+and SAML login options.
+
+Add the following to your configuration.py:
+```python
+BANNER_LOGIN = '<a href="/api/plugins/sso/login" class="btn btn-primary btn-block">Login with SSO</a>'
+```
```

