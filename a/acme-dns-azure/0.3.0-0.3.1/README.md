# Comparing `tmp/acme_dns_azure-0.3.0.tar.gz` & `tmp/acme_dns_azure-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acme_dns_azure-0.3.0.tar", max compression
+gzip compressed data, was "acme_dns_azure-0.3.1.tar", max compression
```

## Comparing `acme_dns_azure-0.3.0.tar` & `acme_dns_azure-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1094 2024-04-12 10:16:29.050682 acme_dns_azure-0.3.0/LICENSE
--rw-r--r--   0        0        0     7438 2024-04-12 10:16:29.050682 acme_dns_azure-0.3.0/README.md
--rw-r--r--   0        0        0      458 2024-04-12 10:16:29.050682 acme_dns_azure-0.3.0/acme_dns_azure/___init___.py
--rw-r--r--   0        0        0    17596 2024-04-12 10:16:29.050682 acme_dns_azure-0.3.0/acme_dns_azure/certbot_manager.py
--rw-r--r--   0        0        0     3283 2024-04-12 10:16:29.050682 acme_dns_azure-0.3.0/acme_dns_azure/client.py
--rw-r--r--   0        0        0     2282 2024-04-12 10:16:29.050682 acme_dns_azure-0.3.0/acme_dns_azure/config/__init__.py
--rw-r--r--   0        0        0     2524 2024-04-12 10:16:29.050682 acme_dns_azure-0.3.0/acme_dns_azure/config/schema.py
--rw-r--r--   0        0        0      282 2024-04-12 10:16:29.050682 acme_dns_azure-0.3.0/acme_dns_azure/context/__init__.py
--rw-r--r--   0        0        0     1774 2024-04-12 10:16:29.050682 acme_dns_azure-0.3.0/acme_dns_azure/data.py
--rw-r--r--   0        0        0     4164 2024-04-12 10:16:29.050682 acme_dns_azure-0.3.0/acme_dns_azure/dns_delegation.py
--rw-r--r--   0        0        0      392 2024-04-12 10:16:29.050682 acme_dns_azure-0.3.0/acme_dns_azure/exceptions.py
--rw-r--r--   0        0        0     5873 2024-04-12 10:16:29.050682 acme_dns_azure-0.3.0/acme_dns_azure/key_vault_manager.py
--rw-r--r--   0        0        0     1126 2024-04-12 10:16:29.050682 acme_dns_azure-0.3.0/acme_dns_azure/log/__init__.py
--rw-r--r--   0        0        0     1548 2024-04-12 10:16:29.050682 acme_dns_azure-0.3.0/acme_dns_azure/os_manager.py
--rw-r--r--   0        0        0     2560 2024-04-12 10:16:29.054682 acme_dns_azure-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     9196 1970-01-01 00:00:00.000000 acme_dns_azure-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-05-22 12:49:13.314084 acme_dns_azure-0.3.1/LICENSE
+-rw-r--r--   0        0        0     7471 2024-05-22 12:49:13.314084 acme_dns_azure-0.3.1/README.md
+-rw-r--r--   0        0        0      458 2024-05-22 12:49:13.314084 acme_dns_azure-0.3.1/acme_dns_azure/___init___.py
+-rw-r--r--   0        0        0    17333 2024-05-22 12:49:13.318084 acme_dns_azure-0.3.1/acme_dns_azure/certbot_manager.py
+-rw-r--r--   0        0        0     3283 2024-05-22 12:49:13.318084 acme_dns_azure-0.3.1/acme_dns_azure/client.py
+-rw-r--r--   0        0        0     2282 2024-05-22 12:49:13.318084 acme_dns_azure-0.3.1/acme_dns_azure/config/__init__.py
+-rw-r--r--   0        0        0     2524 2024-05-22 12:49:13.318084 acme_dns_azure-0.3.1/acme_dns_azure/config/schema.py
+-rw-r--r--   0        0        0      282 2024-05-22 12:49:13.318084 acme_dns_azure-0.3.1/acme_dns_azure/context/__init__.py
+-rw-r--r--   0        0        0     1774 2024-05-22 12:49:13.318084 acme_dns_azure-0.3.1/acme_dns_azure/data.py
+-rw-r--r--   0        0        0     5475 2024-05-22 12:49:13.318084 acme_dns_azure-0.3.1/acme_dns_azure/dns_validation.py
+-rw-r--r--   0        0        0      392 2024-05-22 12:49:13.318084 acme_dns_azure-0.3.1/acme_dns_azure/exceptions.py
+-rw-r--r--   0        0        0     5873 2024-05-22 12:49:13.318084 acme_dns_azure-0.3.1/acme_dns_azure/key_vault_manager.py
+-rw-r--r--   0        0        0     1126 2024-05-22 12:49:13.318084 acme_dns_azure-0.3.1/acme_dns_azure/log/__init__.py
+-rw-r--r--   0        0        0     1548 2024-05-22 12:49:13.318084 acme_dns_azure-0.3.1/acme_dns_azure/os_manager.py
+-rw-r--r--   0        0        0     2484 2024-05-22 12:49:13.322084 acme_dns_azure-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     9229 1970-01-01 00:00:00.000000 acme_dns_azure-0.3.1/PKG-INFO
```

### Comparing `acme_dns_azure-0.3.0/LICENSE` & `acme_dns_azure-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.3.0/README.md` & `acme_dns_azure-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
 - `<secret>`: a regular string that is a secret, such as a password
 
 The other placeholders are specified separately.
 
 See [examples](examples/README.md) for configuration examples.
 
 ```yml
+# Client ID of managed identity
 [managed_identity_id: <string>]
 
 [sp_client_id: <string>]
 [sp_client_secret: <secret>]
 
 [azure_environment: <string> | default = "AzurePublicCloud"]
 
@@ -153,15 +154,14 @@
 
 # Secret name within key vault for storing ACME Certificate authority account information
 [keyvault_account_secret_name: <regex> | default "acme-account-$(network location of server)"]
 # when server=https://example.com/something, then keyvault_account_secret_name="acme-account-example-com"
 
 # config file content for certbot client
 [certbot.ini : <string> | default = ""]
-#
 ```
 
 NOTE: Either **managed_identity_id** or **sp_client_id** and **sp_client_secret** must be specified.
 
 NOTE: **certbot.ini** represents the [CERTBOT configuration file](https://eff-certbot.readthedocs.io/en/latest/using.html#configuration-file) and will be passed into certbot by the _acme_dns_azure_ library as defined. Misconfiguration will lead to failures of certbot and therefore of the renewal process.
 
 Following values will be added to the configurataion file by the _acme_dns_azure_ library per default:
@@ -190,15 +190,15 @@
 ### `<certificate>`
 
 ```yml
 # Certbot certficate name. The name will also be used for Azure keyvault certificate name.
 name: <string>
 # Azure dns zone resource ID used for ACME DNS01 challenge
 dns_zone_resource_id: <string>
-# renewal in days before expiry for certificate to be renewed
+# renewal in days before expiry for certificate to be renewed. Default is 30
 [renew_before_expiry: <int>]
 domains:
   - <domain>
 ```
 
 ### `<domain>`
 
@@ -224,15 +224,15 @@
 
 Best follow [security recommendations from Azure](https://docs.certbot-dns-azure.co.uk/en/latest/#:~:text=Example%3A%20Delegation%20%2B%20more,%C2%B6).
 
 When working with shared DNS Zones, one can work with DNS delegation with limited permissions:
 
 Example:
 
-| Record | Name                         | Value                     | Permission           |
-| ------ | ---------------------------- | ------------------------- | -------------------- |
-| TXT    | \_acme-dedicated             | -                         | DNS Zone Contributor |
-| CNAME  | \_acme-challenge.mysubdomain | \_acme-dedicated.mydomain | None                 |
+| Record | Name                         | Value                  | Permission           |
+| ------ | ---------------------------- | ---------------------- | -------------------- |
+| TXT    | \_acme-dedicated             | -                      | DNS Zone Contributor |
+| CNAME  | \_acme-challenge.mysubdomain | \_acme-dedicated.fqdn. | None                 |
 
 The CNAME and TXT record must be created upfront to enable users to use certbot. The permissions are required on the identity triggering certbot.
 
 With this setup, a DNS Zone owner can limit permissions and enable Users to Create/Renew certificates for their subdomain and ensuring that users cannot aquire certificates for other domains or interfer with existsing records.
```

### Comparing `acme_dns_azure-0.3.0/acme_dns_azure/certbot_manager.py` & `acme_dns_azure-0.3.1/acme_dns_azure/certbot_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from acme_dns_azure.os_manager import FileManager
 from acme_dns_azure.data import (
     RotationResult,
     DomainReference,
     RotationCertificate,
     CertbotResult,
 )
-from acme_dns_azure.dns_delegation import DNSDelegation
+from acme_dns_azure.dns_validation import DNSChallenge
 
 logger = setup_custom_logger(__name__)
 
 
 class CertbotManager:
     def __init__(self, ctx: Context) -> None:
         self.ctx = ctx
@@ -133,40 +133,32 @@
             )
         lines.append("dns_azure_tenant_id = %s" % self._config["tenant_id"])
         lines.append("dns_azure_environment = %s" % self._config["azure_environment"])
 
         idx = 0
         for certificate in self._config["certificates"]:
             for domain in certificate["domains"]:
-                name = domain["name"]
-                if name.startswith("*."):
-                    logger.info("Handling wildard request %s", name)
-                    name = name.removeprefix("*.")
                 idx += 1
-                dns_zone_name, cname = DNSDelegation().validate(
-                    "_acme-challenge." + name
-                )
+                domain_name = domain["name"]
+                dns_zone_name, dns_record_name = DNSChallenge().validate(domain_name)
                 azure_resource_id = certificate["dns_zone_resource_id"]
                 if domain["dns_zone_resource_id"]:
                     azure_resource_id = domain["dns_zone_resource_id"]
                 if dns_zone_name != azure_resource_id.split("/")[-1]:
                     logger.error(
                         "Required DNS zone %s doesn't match configured Azure DNS zone %s",
                         dns_zone_name,
                         azure_resource_id,
                     )
                     raise AssertionError
-                if cname:
-                    azure_resource_id = (
-                        azure_resource_id
-                        + "/TXT/"
-                        + cname.removesuffix("." + dns_zone_name)
-                    )
+                if dns_record_name:
+                    azure_resource_id = azure_resource_id + "/TXT/" + dns_record_name
                 lines.append(
-                    "dns_azure_zone%i = %s:%s" % (idx, name, azure_resource_id)
+                    "dns_azure_zone%i = %s:%s"
+                    % (idx, domain_name.removeprefix("*."), azure_resource_id)
                 )
         return lines
 
     def renew_certificates(self) -> List[RotationResult]:
         certs: List[RotationCertificate] = self._get_certificate_from_config()
         results: List[RotationResult] = []
         for cert_def in certs:
```

### Comparing `acme_dns_azure-0.3.0/acme_dns_azure/client.py` & `acme_dns_azure-0.3.1/acme_dns_azure/client.py`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.3.0/acme_dns_azure/config/__init__.py` & `acme_dns_azure-0.3.1/acme_dns_azure/config/__init__.py`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.3.0/acme_dns_azure/config/schema.py` & `acme_dns_azure-0.3.1/acme_dns_azure/config/schema.py`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.3.0/acme_dns_azure/data.py` & `acme_dns_azure-0.3.1/acme_dns_azure/data.py`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.3.0/acme_dns_azure/key_vault_manager.py` & `acme_dns_azure-0.3.1/acme_dns_azure/key_vault_manager.py`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.3.0/acme_dns_azure/log/__init__.py` & `acme_dns_azure-0.3.1/acme_dns_azure/log/__init__.py`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.3.0/acme_dns_azure/os_manager.py` & `acme_dns_azure-0.3.1/acme_dns_azure/os_manager.py`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.3.0/pyproject.toml` & `acme_dns_azure-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 license = "MIT"
 name = "acme-dns-azure"
 packages = [
   {include = "acme_dns_azure"},
 ]
 readme = "README.md"
 repository = "https://github.com/ZEISS/acme-dns-azure"
-version = "0.3.0"
+version = "0.3.1"
 
 [tool.poetry_bumpversion.file."acme_dns_azure/___init___.py"]
 
 [tool.poetry.dependencies]
 azure-identity = ">=1.14.0"
 azure-keyvault-certificates = ">=4.7.0"
 azure-keyvault-secrets = ">=4.7.0"
@@ -52,41 +52,36 @@
 cryptography = ">=42.0.0"
 dnspython = ">=2"
 python = "^3.8"
 pyyaml = ">=3"
 requests = ">=2"
 strictyaml = ">=1.7.3"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 azure-mgmt-authorization = "*"
-black = {version = "*", allow-prereleases = true}
+black = {version = "^24.2.0", allow-prereleases = true}
 coverage = "*"
-flake8 = "*"
 isort = "*"
 mock = "*"
 mypy = "*"
 pdoc3 = "*"
 pytest = "*"
 pytest-cov = "*"
-pytest-xdist = "*"
 tox = ">=4"
 types-PyYAML = "*"
 types-pytz = "*"
 types-requests = "*"
 types-simplejson = "*"
 types-six = "*"
 types-toml = "*"
 vcrpy = "*"
 
 [tool.poetry.scripts]
 acme-dns-azure = "acme_dns_azure.cli:main"
 
-[tool.poetry.group.dev.dependencies]
-black = "^24.2.0"
-
 [tool.mypy]
 show_error_codes = true
 
 [tool.pytest.ini_options]
 addopts = "-s -v --durations=0"
 testpaths = ["tests/app"]
```

### Comparing `acme_dns_azure-0.3.0/PKG-INFO` & `acme_dns_azure-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acme-dns-azure
-Version: 0.3.0
+Version: 0.3.1
 Summary: ACME client setup based on Certbot for dns-01 challenges via Azure Cloud services
 Home-page: https://github.com/ZEISS/acme-dns-azure
 License: MIT
 Keywords: acme,dns,azure,certbot,letsencrypt
 Author: ZEISS Digital Innovation Partners
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -171,14 +171,15 @@
 - `<secret>`: a regular string that is a secret, such as a password
 
 The other placeholders are specified separately.
 
 See [examples](examples/README.md) for configuration examples.
 
 ```yml
+# Client ID of managed identity
 [managed_identity_id: <string>]
 
 [sp_client_id: <string>]
 [sp_client_secret: <secret>]
 
 [azure_environment: <string> | default = "AzurePublicCloud"]
 
@@ -193,15 +194,14 @@
 
 # Secret name within key vault for storing ACME Certificate authority account information
 [keyvault_account_secret_name: <regex> | default "acme-account-$(network location of server)"]
 # when server=https://example.com/something, then keyvault_account_secret_name="acme-account-example-com"
 
 # config file content for certbot client
 [certbot.ini : <string> | default = ""]
-#
 ```
 
 NOTE: Either **managed_identity_id** or **sp_client_id** and **sp_client_secret** must be specified.
 
 NOTE: **certbot.ini** represents the [CERTBOT configuration file](https://eff-certbot.readthedocs.io/en/latest/using.html#configuration-file) and will be passed into certbot by the _acme_dns_azure_ library as defined. Misconfiguration will lead to failures of certbot and therefore of the renewal process.
 
 Following values will be added to the configurataion file by the _acme_dns_azure_ library per default:
@@ -230,15 +230,15 @@
 ### `<certificate>`
 
 ```yml
 # Certbot certficate name. The name will also be used for Azure keyvault certificate name.
 name: <string>
 # Azure dns zone resource ID used for ACME DNS01 challenge
 dns_zone_resource_id: <string>
-# renewal in days before expiry for certificate to be renewed
+# renewal in days before expiry for certificate to be renewed. Default is 30
 [renew_before_expiry: <int>]
 domains:
   - <domain>
 ```
 
 ### `<domain>`
 
@@ -264,16 +264,16 @@
 
 Best follow [security recommendations from Azure](https://docs.certbot-dns-azure.co.uk/en/latest/#:~:text=Example%3A%20Delegation%20%2B%20more,%C2%B6).
 
 When working with shared DNS Zones, one can work with DNS delegation with limited permissions:
 
 Example:
 
-| Record | Name                         | Value                     | Permission           |
-| ------ | ---------------------------- | ------------------------- | -------------------- |
-| TXT    | \_acme-dedicated             | -                         | DNS Zone Contributor |
-| CNAME  | \_acme-challenge.mysubdomain | \_acme-dedicated.mydomain | None                 |
+| Record | Name                         | Value                  | Permission           |
+| ------ | ---------------------------- | ---------------------- | -------------------- |
+| TXT    | \_acme-dedicated             | -                      | DNS Zone Contributor |
+| CNAME  | \_acme-challenge.mysubdomain | \_acme-dedicated.fqdn. | None                 |
 
 The CNAME and TXT record must be created upfront to enable users to use certbot. The permissions are required on the identity triggering certbot.
 
 With this setup, a DNS Zone owner can limit permissions and enable Users to Create/Renew certificates for their subdomain and ensuring that users cannot aquire certificates for other domains or interfer with existsing records.
```

