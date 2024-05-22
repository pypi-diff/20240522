# Comparing `tmp/openai_priority_loadbalancer-1.0.8.tar.gz` & `tmp/openai_priority_loadbalancer-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_priority_loadbalancer-1.0.8.tar", last modified: Tue May 21 16:17:33 2024, max compression
+gzip compressed data, was "openai_priority_loadbalancer-1.0.9.tar", last modified: Wed May 22 20:48:02 2024, max compression
```

## Comparing `openai_priority_loadbalancer-1.0.8.tar` & `openai_priority_loadbalancer-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 16:17:33.406986 openai_priority_loadbalancer-1.0.8/
--rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-1.0.8/LICENSE
--rw-rw-rw-   0        0        0    13852 2024-05-17 10:36:38.000000 openai_priority_loadbalancer-1.0.8/PACKAGE_README.md
--rw-rw-rw-   0        0        0    14716 2024-05-21 16:17:33.400874 openai_priority_loadbalancer-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    12849 2024-05-21 16:03:56.000000 openai_priority_loadbalancer-1.0.8/README.md
--rw-rw-rw-   0        0        0      724 2024-05-21 16:08:10.000000 openai_priority_loadbalancer-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 16:17:33.407849 openai_priority_loadbalancer-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-21 16:17:33.287318 openai_priority_loadbalancer-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-05-21 16:17:33.315135 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer/
--rw-rw-rw-   0        0        0       45 2024-05-14 20:10:13.000000 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer/__init__.py
--rw-rw-rw-   0        0        0    13344 2024-05-21 15:51:47.000000 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:17:33.397151 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer.egg-info/
--rw-rw-rw-   0        0        0    14716 2024-05-21 16:17:33.000000 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2024-05-21 16:17:33.000000 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 16:17:33.000000 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-21 16:17:33.000000 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-05-21 16:17:33.000000 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 20:48:02.811741 openai_priority_loadbalancer-1.0.9/
+-rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0    14306 2024-05-22 20:45:17.000000 openai_priority_loadbalancer-1.0.9/PACKAGE_README.md
+-rw-rw-rw-   0        0        0    15618 2024-05-22 20:48:02.797445 openai_priority_loadbalancer-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    13421 2024-05-22 00:04:54.000000 openai_priority_loadbalancer-1.0.9/README.md
+-rw-rw-rw-   0        0        0     1309 2024-05-22 20:46:08.000000 openai_priority_loadbalancer-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 20:48:02.812507 openai_priority_loadbalancer-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 20:48:02.643262 openai_priority_loadbalancer-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 20:48:02.698776 openai_priority_loadbalancer-1.0.9/src/openai_priority_loadbalancer/
+-rw-rw-rw-   0        0        0       70 2024-05-21 18:38:30.000000 openai_priority_loadbalancer-1.0.9/src/openai_priority_loadbalancer/__init__.py
+-rw-rw-rw-   0        0        0    14823 2024-05-22 20:45:17.000000 openai_priority_loadbalancer-1.0.9/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:48:02.791829 openai_priority_loadbalancer-1.0.9/src/openai_priority_loadbalancer.egg-info/
+-rw-rw-rw-   0        0        0    15618 2024-05-22 20:48:02.000000 openai_priority_loadbalancer-1.0.9/src/openai_priority_loadbalancer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2024-05-22 20:48:02.000000 openai_priority_loadbalancer-1.0.9/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:48:02.000000 openai_priority_loadbalancer-1.0.9/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-22 20:48:02.000000 openai_priority_loadbalancer-1.0.9/src/openai_priority_loadbalancer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-22 20:48:02.000000 openai_priority_loadbalancer-1.0.9/src/openai_priority_loadbalancer.egg-info/top_level.txt
```

### Comparing `openai_priority_loadbalancer-1.0.8/LICENSE` & `openai_priority_loadbalancer-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-1.0.8/PACKAGE_README.md` & `openai_priority_loadbalancer-1.0.9/PACKAGE_README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,234 +1,237 @@
-# OpenAI Priority Load Balancer
-
-Many AI workloads require using more than one Azure OpenAI instance to prioritize Provisioned Throughput Units (PTUs) and insulate themselves from timeouts. In having worked with customers on Azure OpenAI implementations, there are a few common, desired configurations:
-
-- Distribution of requests over multiple consumption instances to mitigate throttling.
-- Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
-- Tiered prioritization of multiple consumption instances (e.g. use instances first that are geographically closer).
-
-While the [OpenAI Python API library](https://github.com/openai/openai-python) respects HTTP 429 and automatically retries after the requested wait period, the library is not set up to support the aforementioned customer desires. The library does, however, allow for the injection of custom httpx clients. This gave rise to this project.
-
-And while there are other Python OpenAI load balancers freely available, I have not seen one yet that addresses the aforementioned scenarios.
-
-Python OpenAI Load Balancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) file in this repo.
-
-**Please refer to the GitHub repo for detailed test harnesses for the use cases described below.**
-
-## Disclaimer
-
-**This is a pseudo load-balancer.**
-
-When executing this code in parallel, there is no way to distribute requests uniformly across all Azure OpenAI instances. Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would also imply a locking mechanism for updates, which would
-immediately inhibit the performance benefits of the load balancer. Without knowledge of any other python workers, we can only randomize selection of an available backend.
-
-Furthermore, while the load balancer handles retries across available backends, the [OpenAI Python API library](https://github.com/openai/openai-python) is not fully insulated from failing on multiple HTTP 429s when all backends are returning HTTP 429s. It is advised to load-test with multiple concurrent python workers to understand how your specific Azure OpenAI instances, your limits, and your load balancer configuration function.
-
-## Attribution
-
-This project would not have been possible without the incredible work that [@andredewes](https://github.com/andredewes) has done with his [Smart Load Balancing for OpenAI Endpoints and Azure API Management](https://github.com/Azure-Samples/openai-apim-lb). If you use Azure API Management in your infrastructure, I highly recommend you consider his policy.
-
-## Prerequisites
-
-It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in the [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) test harness for this package will look very familiar to you.
-It's also good to have some knowledge of authentication and identities.
-
-## Getting Started
-
-The steps below are not comprehensive for every way to set up Azure OpenAI integration with the [OpenAI Python API library](https://github.com/openai/openai-python) (e.g. the token provider). You can see specific implementation examples in [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) in the GitHub repo.
-
-### Installing the Package
-
-You should already have the `openai` package set up.
-
-1. Add `openai_priority_loadbalancer` to your *requirements.txt* file.
-
-    ```text
-    openai_priority_loadbalancer
-    ```
-
-1. Run `pip install -r </path/to/requirements.txt>`.
-
-### Importing Classes
-
-Either import the **synchronous** `AzureOpenAI` and `LoadBalancer`:
-
-```python
-# openai & other imports
-from azure.identity import DefaultAzureCredential, get_bearer_token_provider
-from openai import AzureOpenAI
-
-# openai-priority-loadbalancer imports
-from typing import List
-import httpx
-from openai_priority_loadbalancer import LoadBalancer, Backend
-```
-
-Or import the **asynchronous** `AsyncAzureOpenAI` and `AsyncLoadBalancer`:
-
-```python
-# openai & other imports
-from azure.identity import DefaultAzureCredential, get_bearer_token_provider
-from openai import AsyncAzureOpenAI
-
-# openai-priority-loadbalancer imports
-from typing import List
-import httpx
-from openai_priority_loadbalancer import AsyncLoadBalancer, Backend
-```
-
-*Importing `httpx` lets us use `httpx.Client` and `httpx.AsyncClient`. This avoids having to update openai to at least
-[1.17.0](https://github.com/openai/openai-python/releases/tag/v1.17.0). The `openai` properties for `DefaultHttpxClient` and `DefaultAsyncHttpxClient` are mere wrappers for `httpx.Client` and `httpx.AsyncClient`.*
-
-### Configuring the Backends and Load Balancer
-
-1. Define a list of backends according to the *Load Balancer Backend Configuration* section below.
-
-    ```python
-    backends: List[Backend] = [
-        Backend("oai-eastus.openai.azure.com", 1),
-        Backend("oai-southcentralus.openai.azure.com", 1)
-    ]
-    ```
-
-1. Instantiate the load balancer and inject a new httpx client with the load balancer as the new transport.
-
-    **Synchronous**
-
-    ```python
-    lb = LoadBalancer(backends)
-
-    client = AzureOpenAI(
-        azure_endpoint = f"https://{backends[0].host}",         # Must be seeded, so we use the first host. It will get overwritten by the load balancer.
-        azure_ad_token_provider = token_provider,               # Your authentication may vary. Please adjust accordingly.
-        api_version = "2024-04-01-preview",
-        http_client = httpx.Client(transport = lb)              # Inject the synchronous load balancer as the transport in a new default httpx client.
-    )
-    ```
-
-    **Asynchronous**
-
-    ```python
-    lb = AsyncLoadBalancer(backends)
-
-    client = AsyncAzureOpenAI(
-        azure_endpoint = f"https://{backends[0].host}",         # Must be seeded, so we use the first host. It will get overwritten by the load balancer.
-        azure_ad_token_provider = token_provider,               # Your authentication may vary. Please adjust accordingly.
-        api_version = "2024-04-01-preview",
-        http_client = httpx.AsyncClient(transport = lb)         # Inject the asynchronous load balancer as the transport in a new default async httpx client.
-    )
-    ```
-
-## Load Balancer Backend Configuration
-
-At its core, the Load Balancer Backend configuration requires one or more backend hosts and a numeric priority starting at 1. Please take note that you define a host, not a URL.
-
-I use a total of three Azure OpenAI instances in three regions. These instances are set up with intentionally small tokens-per-minute (tpm) to trigger HTTP 429s.
-The standard approach never changes and uses the same host (first in the backend list), which provides a stable comparison to the load-balanced approach.
-While the number of requests differs per tests below, we issue the same number of requests against standard and load-balanced approaches.
-
-### One Backend
-
-This is logically equivalent to what the standard approach does. This configuration does not provide value over the standard approach.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1)
-]
-```
-
-### Two Backends with Same Priority
-
-Load-balancing evenly between Azure OpenAI instances hedges you against being stalled due to a 429 from a single instance.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1)
-]
-```
-
-### Three Backends with Same Priority
-
-Adding a third backend with same priority exacerbates the difference to the standard approach further. Here, we need to use 20 requests to incur more HTTP 429s.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-westus-xxxxxxxx.openai.azure.com", 1)
-]
-```
-
-### Three Backends with Two Different Priorities
-
-The most common reason for this approach may well be the prioritization of Provisioned Throughput Units (PTUs). This is a reserved capacity over a period of time that is billed at that reservation and not flexible as consumption instances. Aside from guaranteed capacity, latency is also much more stable. Naturally, this is an instance that you would want to prioritize over all others but allow yourself to have fallbacks if you burst over what the PTU provides.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
-    Backends("oai-westus-xxxxxxxx.openai.azure.com", 2)
-]
-```
-
-### Three Backends with Three Different Priorities
-
-An example of this setup may be that most of your assets reside in one region (e.g. East US). It stands to reason that you want to use the Azure OpenAI instance in that region. To hedge yourself against HTTP 429s, you decide to add a second region that's geographically close (e.g. East US 2) as well as a third (e.g. West US).
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
-    Backends("oai-westus-xxxxxxxx.openai.azure.com", 3)
-]
-```
-
-### Using the Load Balancer
-
-As these are the only changes to the [OpenAI Python API library](https://github.com/openai/openai-python) implementation, simply execute your python code.
-
-### Logging
-
-OpenAI Priority Load Balancer uses Python's [logging](https://docs.python.org/3/library/logging.html) module. The name of the logger is `openai-priority-loadbalancer`.
-
-## Distribution of Requests
-
-### Across Different Priorities
-
-Requests are made to the highest priority backend that is available. For example:
-
-- Priority 1, when available, will always supersede priority 2.
-- Priority 2, when available, will always supersede an unavailable priority 1.
-- Priority 3, when available, will always supersede unavailable priorities 1 & 2.
-
-### Across Multiple Backends of Same Priority
-
-In the single-requestor model, the distribution of attempts over available backends should be fairly uniform for backends of the same priority.
-
-There is no likelihood of a uniform distribution across available endpoints when running multiple python workers in parallel. In the below example, each terminal is executing 20 requests over two Azure OpenAI instances, both set up with the lowest of tokens-per-minute setting. Available backends are selected randomly (see the first request in each terminal). No sharing of data between the two terminals exists. Recovery takes place, when possible; otherwise, an HTTP 429 is returned to the OpenAI Python API library.
-
-## Backoff & Retries
-
-When no backends are available (e.g. all timed out), Python OpenAI Load Balancer returns the soonest retry in seconds determined based on the `retry_after` value on each backend.
-You may notice a delay in the logs between when the load balancer returns and when the next request is made. In addition to the `Retry-After` header value, the OpenAI Python library [uses a short exponential backoff](https://github.com/openai/openai-python?tab=readme-ov-file#retries).
-
-In this log excerpt, we see that all three backends are timing out. As the standard behavior returns an HTTP 429 from a single backend, we do the same here with the load-balanced approach. This allows the OpenAI Python library to handle the HTTP 429 that it believes it received from a singular backend.
-The wait periods are 44 seconds (westus), 4 seconds (eastus), and 7 seconds (southcentralus) in this log. Our logic determines that eastus will become available soonest. Therefore, we return a `Retry-After` header with a value of `4`. The OpenAI Python library then adds its exponential backoff (~2 seconds here).
-
-```text
-2024-05-11 00:56:32.299477:   Request sent to server: https://oai-westus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.299477:   Backend oai-westus-20240509.openai.azure.com is throttling. Retry after 44 second(s).
-2024-05-11 00:56:32.394350:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.395578:   Backend oai-eastus-20240509.openai.azure.com is throttling. Retry after 4 second(s).
-2024-05-11 00:56:32.451891:   Request sent to server: https://oai-southcentralus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.452883:   Backend oai-southcentralus-20240509.openai.azure.com is throttling. Retry after 7 second(s).
-2024-05-11 00:56:32.452883:   No backends available. Exiting.
-2024-05-11 00:56:32.453891:   Soonest Retry After: oai-eastus-20240509.openai.azure.com - 4 second(s)
-2024-05-11 00:56:38.551672:   Backend oai-eastus-20240509.openai.azure.com is no longer throttling.
-2024-05-11 00:56:39.851076:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status code: 200
-```
+# OpenAI Priority Load Balancer
+
+Many AI workloads require using more than one Azure OpenAI instance to prioritize Provisioned Throughput Units (PTUs) and insulate themselves from timeouts. In having worked with customers on Azure OpenAI implementations, there are a few common, desired configurations:
+
+- Distribution of requests over multiple consumption instances to mitigate throttling.
+- Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
+- Tiered prioritization of multiple consumption instances (e.g. use instances first that are geographically closer).
+
+While the [OpenAI Python API library](https://github.com/openai/openai-python) respects HTTP 429 and automatically retries after the requested wait period, the library is not set up to support the aforementioned customer desires. The library does, however, allow for the injection of custom httpx clients. This gave rise to this project.
+
+And while there are other Python OpenAI load balancers freely available, I have not seen one yet that addresses the aforementioned scenarios.
+
+Python OpenAI Load Balancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) file in this repo.
+
+**Please refer to the GitHub repo for detailed test harnesses for the use cases described below.**
+
+## Disclaimer
+
+**This is a pseudo load-balancer.**
+
+When executing this code in parallel, there is no way to distribute requests uniformly across all Azure OpenAI instances. Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would also imply a locking mechanism for updates, which would
+immediately inhibit the performance benefits of the load balancer. Without knowledge of any other python workers, we can only randomize selection of an available backend.
+
+Furthermore, while the load balancer handles retries across available backends, the [OpenAI Python API library](https://github.com/openai/openai-python) is not fully insulated from failing on multiple HTTP 429s when all backends are returning HTTP 429s. It is advised to load-test with multiple concurrent python workers to understand how your specific Azure OpenAI instances, your limits, and your load balancer configuration function.
+
+## Attribution
+
+This project would not have been possible without the incredible work that [@andredewes](https://github.com/andredewes) has done with his [Smart Load Balancing for OpenAI Endpoints and Azure API Management](https://github.com/Azure-Samples/openai-apim-lb). If you use Azure API Management in your infrastructure, I highly recommend you consider his policy.
+
+## Prerequisites
+
+It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in the [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) test harness for this package will look very familiar to you.
+It's also good to have some knowledge of authentication and identities.
+
+## Getting Started
+
+The steps below are not comprehensive for every way to set up Azure OpenAI integration with the [OpenAI Python API library](https://github.com/openai/openai-python) (e.g. the token provider). You can see specific implementation examples in [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) in the GitHub repo.
+
+### Installing the Package
+
+You should already have the `openai` package set up.
+
+1. Add `openai_priority_loadbalancer` to your *requirements.txt* file.
+
+    ```text
+    openai_priority_loadbalancer
+    ```
+
+1. Run `pip install -r </path/to/requirements.txt>`.
+
+### Importing Classes
+
+Either import the **synchronous** `AzureOpenAI` and `LoadBalancer`:
+
+```python
+# openai & other imports
+from azure.identity import DefaultAzureCredential, get_bearer_token_provider
+from openai import AzureOpenAI
+
+# openai-priority-loadbalancer imports
+from typing import List
+import httpx
+from openai_priority_loadbalancer import LoadBalancer, Backend
+```
+
+Or import the **asynchronous** `AsyncAzureOpenAI` and `AsyncLoadBalancer`:
+
+```python
+# openai & other imports
+from azure.identity import DefaultAzureCredential, get_bearer_token_provider
+from openai import AsyncAzureOpenAI
+
+# openai-priority-loadbalancer imports
+from typing import List
+import httpx
+from openai_priority_loadbalancer import AsyncLoadBalancer, Backend
+```
+
+*Importing `httpx` lets us use `httpx.Client` and `httpx.AsyncClient`. This avoids having to update openai to at least
+[1.17.0](https://github.com/openai/openai-python/releases/tag/v1.17.0). The `openai` properties for `DefaultHttpxClient` and `DefaultAsyncHttpxClient` are mere wrappers for `httpx.Client` and `httpx.AsyncClient`.*
+
+### Configuring the Backends and Load Balancer
+
+1. Define a list of backends according to the *Load Balancer Backend Configuration* section below.
+
+   *Optionally, a path can be added (e.g. `"/ai"`), which gets prepended to the request path. This is an extraordinary, not a commonly needed functionality.*
+
+    ```python
+    backends: List[Backend] = [
+        Backend("oai-eastus.openai.azure.com", 1),
+        Backend("oai-eastus.openai.azure.com", 1, "/ai"),
+        Backend("oai-southcentralus.openai.azure.com", 1)
+    ]
+    ```
+
+1. Instantiate the load balancer and inject a new httpx client with the load balancer as the new transport.
+
+    **Synchronous**
+
+    ```python
+    lb = LoadBalancer(backends)
+
+    client = AzureOpenAI(
+        azure_endpoint = f"https://{backends[0].host}",         # Must be seeded, so we use the first host. It will get overwritten by the load balancer.
+        azure_ad_token_provider = token_provider,               # Your authentication may vary. Please adjust accordingly.
+        api_version = "2024-04-01-preview",
+        http_client = httpx.Client(transport = lb)              # Inject the synchronous load balancer as the transport in a new default httpx client.
+    )
+    ```
+
+    **Asynchronous**
+
+    ```python
+    lb = AsyncLoadBalancer(backends)
+
+    client = AsyncAzureOpenAI(
+        azure_endpoint = f"https://{backends[0].host}",         # Must be seeded, so we use the first host. It will get overwritten by the load balancer.
+        azure_ad_token_provider = token_provider,               # Your authentication may vary. Please adjust accordingly.
+        api_version = "2024-04-01-preview",
+        http_client = httpx.AsyncClient(transport = lb)         # Inject the asynchronous load balancer as the transport in a new default async httpx client.
+    )
+    ```
+
+## Load Balancer Backend Configuration
+
+At its core, the Load Balancer Backend configuration requires one or more backend hosts and a numeric priority starting at 1. Please take note that you define a host, not a URL.
+
+I use a total of three Azure OpenAI instances in three regions. These instances are set up with intentionally small tokens-per-minute (tpm) to trigger HTTP 429s.
+The standard approach never changes and uses the same host (first in the backend list), which provides a stable comparison to the load-balanced approach.
+While the number of requests differs per tests below, we issue the same number of requests against standard and load-balanced approaches.
+
+### One Backend
+
+This is logically equivalent to what the standard approach does. This configuration does not provide value over the standard approach.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1)
+]
+```
+
+### Two Backends with Same Priority
+
+Load-balancing evenly between Azure OpenAI instances hedges you against being stalled due to a 429 from a single instance.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1)
+]
+```
+
+### Three Backends with Same Priority
+
+Adding a third backend with same priority exacerbates the difference to the standard approach further. Here, we need to use 20 requests to incur more HTTP 429s.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-westus-xxxxxxxx.openai.azure.com", 1)
+]
+```
+
+### Three Backends with Two Different Priorities
+
+The most common reason for this approach may well be the prioritization of Provisioned Throughput Units (PTUs). This is a reserved capacity over a period of time that is billed at that reservation and not flexible as consumption instances. Aside from guaranteed capacity, latency is also much more stable. Naturally, this is an instance that you would want to prioritize over all others but allow yourself to have fallbacks if you burst over what the PTU provides.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
+    Backends("oai-westus-xxxxxxxx.openai.azure.com", 2)
+]
+```
+
+### Three Backends with Three Different Priorities
+
+An example of this setup may be that most of your assets reside in one region (e.g. East US). It stands to reason that you want to use the Azure OpenAI instance in that region. To hedge yourself against HTTP 429s, you decide to add a second region that's geographically close (e.g. East US 2) as well as a third (e.g. West US).
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
+    Backends("oai-westus-xxxxxxxx.openai.azure.com", 3)
+]
+```
+
+### Using the Load Balancer
+
+As these are the only changes to the [OpenAI Python API library](https://github.com/openai/openai-python) implementation, simply execute your python code.
+
+### Logging
+
+OpenAI Priority Load Balancer uses Python's [logging](https://docs.python.org/3/library/logging.html) module. The name of the logger is `openai-priority-loadbalancer`.
+
+## Distribution of Requests
+
+### Across Different Priorities
+
+Requests are made to the highest priority backend that is available. For example:
+
+- Priority 1, when available, will always supersede priority 2.
+- Priority 2, when available, will always supersede an unavailable priority 1.
+- Priority 3, when available, will always supersede unavailable priorities 1 & 2.
+
+### Across Multiple Backends of Same Priority
+
+In the single-requestor model, the distribution of attempts over available backends should be fairly uniform for backends of the same priority.
+
+There is no likelihood of a uniform distribution across available endpoints when running multiple python workers in parallel. In the below example, each terminal is executing 20 requests over two Azure OpenAI instances, both set up with the lowest of tokens-per-minute setting. Available backends are selected randomly (see the first request in each terminal). No sharing of data between the two terminals exists. Recovery takes place, when possible; otherwise, an HTTP 429 is returned to the OpenAI Python API library.
+
+## Backoff & Retries
+
+When no backends are available (e.g. all timed out), Python OpenAI Load Balancer returns the soonest retry in seconds determined based on the `retry_after` value on each backend.
+You may notice a delay in the logs between when the load balancer returns and when the next request is made. In addition to the `Retry-After` header value, the OpenAI Python library [uses a short exponential backoff](https://github.com/openai/openai-python?tab=readme-ov-file#retries).
+
+In this log excerpt, we see that all three backends are timing out. As the standard behavior returns an HTTP 429 from a single backend, we do the same here with the load-balanced approach. This allows the OpenAI Python library to handle the HTTP 429 that it believes it received from a singular backend.
+The wait periods are 44 seconds (westus), 4 seconds (eastus), and 7 seconds (southcentralus) in this log. Our logic determines that eastus will become available soonest. Therefore, we return a `Retry-After` header with a value of `4`. The OpenAI Python library then adds its exponential backoff (~2 seconds here).
+
+```text
+2024-05-11 00:56:32.299477:   Request sent to server: https://oai-westus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.299477:   Backend oai-westus-20240509.openai.azure.com is throttling. Retry after 44 second(s).
+2024-05-11 00:56:32.394350:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.395578:   Backend oai-eastus-20240509.openai.azure.com is throttling. Retry after 4 second(s).
+2024-05-11 00:56:32.451891:   Request sent to server: https://oai-southcentralus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.452883:   Backend oai-southcentralus-20240509.openai.azure.com is throttling. Retry after 7 second(s).
+2024-05-11 00:56:32.452883:   No backends available. Exiting.
+2024-05-11 00:56:32.453891:   Soonest Retry After: oai-eastus-20240509.openai.azure.com - 4 second(s)
+2024-05-11 00:56:38.551672:   Backend oai-eastus-20240509.openai.azure.com is no longer throttling.
+2024-05-11 00:56:39.851076:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status code: 200
+```
```

### Comparing `openai_priority_loadbalancer-1.0.8/PKG-INFO` & `openai_priority_loadbalancer-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 1.0.8
+Version: 1.0.9
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
+Project-URL: Changelog, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/releases
+Project-URL: Documentation, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/README.md
+Project-URL: GitHub-Statistics, https://shields.io/github/stars/simonkurtz-MSFT/python-openai-loadbalancer?style=social
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
-Classifier: Programming Language :: Python :: 3
+Project-URL: Repository, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 
 # OpenAI Priority Load Balancer
 
@@ -94,17 +103,20 @@
 *Importing `httpx` lets us use `httpx.Client` and `httpx.AsyncClient`. This avoids having to update openai to at least
 [1.17.0](https://github.com/openai/openai-python/releases/tag/v1.17.0). The `openai` properties for `DefaultHttpxClient` and `DefaultAsyncHttpxClient` are mere wrappers for `httpx.Client` and `httpx.AsyncClient`.*
 
 ### Configuring the Backends and Load Balancer
 
 1. Define a list of backends according to the *Load Balancer Backend Configuration* section below.
 
+   *Optionally, a path can be added (e.g. `"/ai"`), which gets prepended to the request path. This is an extraordinary, not a commonly needed functionality.*
+
     ```python
     backends: List[Backend] = [
         Backend("oai-eastus.openai.azure.com", 1),
+        Backend("oai-eastus.openai.azure.com", 1, "/ai"),
         Backend("oai-southcentralus.openai.azure.com", 1)
     ]
     ```
 
 1. Instantiate the load balancer and inject a new httpx client with the load balancer as the new transport.
 
     **Synchronous**
```

### Comparing `openai_priority_loadbalancer-1.0.8/README.md` & `openai_priority_loadbalancer-1.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,193 +1,195 @@
-# Python OpenAI Load Balancer
-
-TL;DR! How do I [start](#getting-started)?
-
----
-
-Many AI workloads require using more than one Azure OpenAI instance to prioritize Provisioned Throughput Units (PTUs) and insulate themselves from timeouts. In having worked with customers on Azure OpenAI implementations, there are a few common, desired configurations:
-
-- Distribution of requests over multiple consumption instances to mitigate throttling.
-- Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
-- Tiered prioritization of multiple consumption instances (e.g. use instances first that are geographically closer).
-
-While the [OpenAI Python API library](https://github.com/openai/openai-python) respects HTTP 429 and automatically retries after the requested wait period, the library is not set up to support the aforementioned customer desires. The library does, however, allow for the injection of custom httpx clients. This gave rise to this project.
-
-And while there are other Python OpenAI load balancers freely available, I have not seen one yet that addresses the aforementioned scenarios.
-
-Python OpenAI LoadBalancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](./aoai.py) file in this repo.
-
-## Disclaimer
-
-**This is a pseudo load-balancer.**
-
-When executing this code in parallel, there is no way to distribute requests uniformly across all Azure OpenAI instances. Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would also imply a locking mechanism for updates, which would
-immediately inhibit the performance benefits of the load balancer. Without knowledge of any other python workers, we can only randomize selection of an available backend.
-
-Furthermore, while the load balancer handles retries across available backends, the [OpenAI Python API library](https://github.com/openai/openai-python) is not fully insulated from failing on multiple HTTP 429s when all backends are returning HTTP 429s. It is advised to load-test with multiple concurrent python workers to understand how your specific Azure OpenAI instances, your limits, and your load balancer configuration function.
-
-## Attribution
-
-This project would not have been possible without the incredible work that [@andredewes](https://github.com/andredewes) has done with his [Smart Load Balancing for OpenAI Endpoints and Azure API Management](https://github.com/Azure-Samples/openai-apim-lb). If you use Azure API Management in your infrastructure, I highly recommend you consider his policy.
-
-## Prerequisites
-
-It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in `aoai.py` here will look very familiar to you.
-It's also good to have some knowledge of authentication and identities.
-
-## Authentication
-
-Locally, you can log into Azure via the CLI and the steps below and use the `AzureDefaultCredential` (what I use in my example). When deploying this application in Azure, it's recommended to use a managed identity for authentication. It's best to avoid using the Azure OpenAI instances' keys as that could a) accidentally leave credentials in your source code, and b) the keys are different for each instance, which would probably require expanding upon the `Backends` class. Best to just avoid keys.
-
-## Getting Started
-
-### Cloning the repo & Preparing the python environment
-
-1. Clone the repo.
-1. Open the cloned repo folder in VS Code.
-1. Open a terminal session in VS Code.
-1. Run [setup-python.ps1](./setup-python.ps1) to prepare the python environment.
-
-### Configuration
-
-For the load-balanced approach, please use the same model across all instances.
-
-1. Open [aoai.py](./aoai.py).
-1. Replace `<your-aoai-model>` with the name of your Azure OpenAI model.
-1. Replace `<your-aoai-instance>` with the primary/single Azure OpenAI instance.
-1. Replace `<your-aoai-instance-1>`, `<your-aoai-instance-2>`, `<your-aoai-instance-3>` with all the Azure OpenAI instances you want to load-balance across. Delete entries you don't need. See [Load Balancer Backend Configuration](#load-balancer-backend-configuration) for details.
-1. Replace the value for variable `num_of_requests` with the number of requests you wish to execute.
-
-### Credentials
-
-Locally, your `AzureDefaultCredential` is used. Each Azure OpenAI instance must be configured with the `Cognitive Services OpenAI` User role for your Azure credential (the identity you use after logging in). This ensures that you can use your credential across all Azure OpenAI instances.
-
-When running in Azure, it's advised to use managed identities.
-
-1. Log in with `az login`.
-1. Set your subscription in which your Azure OpenAI assets reside: `az account set -s <name or id>`
-
-    *Missing this step may result in HTTP 400 errors for a tenant mismatch.*
-
-## Execution
-
-1. Initially, [python-aoai.ps1](./python-aoai.ps1) once to ensure it executes correctly.
-1. Run [python-aoai.ps1](./python-aoai.ps1) concurrently in multiple terminals to simulate parallel requests from multiple python workers.
-
-## Testing
-
-OpenAI Priority Load Balancer uses `pytest` and `coverage`. The test files can be found in the `tests\lib` directory. Executing `pytest -v` from the root will show test results. Note that these are rudimentary tests still and in the process of being built out further.
-
-To obtain coverage, execute `coverage run -m pytest -v` from the root. This generates a *.coverage* file. Then run `coverage report -m` or, for a nicer presentation, `coverage html`.
-
-Details on `coverage` can be found [here](https://coverage.readthedocs.io/).
-
-Pull requests for improvements are very much appreciated!
-
-## Distribution of Requests
-
-### Across Different Priorities
-
-Requests are made to the highest priority backend that is available. For example:
-
-- Priority 1, when available, will always supersede priority 2.
-- Priority 2, when available, will always supersede an unavailable priority 1.
-- Priority 3, when available, will always supersede unavailable priorities 1 & 2.
-
-### Across Multiple Backends of Same Priority
-
-In the single-requestor model, the distribution of attempts over available backends should be fairly uniform for backends of the same priority.
-
-There is no likelihood of a uniform distribution across available endpoints when running multiple python workers in parallel. In the below example, each terminal is executing 20 requests over two Azure OpenAI instances, both set up with the lowest of tokens-per-minute setting. Available backends are selected randomly (see the first request in each terminal). No sharing of data between the two terminals exists. Recovery takes place, when possible; otherwise, an HTTP 429 is returned to the OpenAI Python API library.
-
-![Parallel Execution](./assets/parallel-execution.png)
-
-## Backoff & Retries
-
-When no backends are available (e.g. all timed out), Python OpenAI Load Balancer returns the soonest retry in seconds determined based on the `retry_after` value on each backend.
-You may notice a delay in the logs between when the load balancer returns and when the next request is made. In addition to the `Retry-After` header value, the OpenAI Python library [uses a short exponential backoff](https://github.com/openai/openai-python?tab=readme-ov-file#retries).
-
-In this log excerpt, we see that all three backends are timing out. As the standard behavior returns an HTTP 429 from a single backend, we do the same here with the load-balanced approach. This allows the OpenAI Python library to handle the HTTP 429 that it believes it received from a singular backend.
-The wait periods are 44 seconds (westus), 4 seconds (eastus), and 7 seconds (southcentralus) in this log. Our logic determines that eastus will become available soonest. Therefore, we return a `Retry-After` header with a value of `4`. The OpenAI Python library then adds its exponential backoff (~2 seconds here).
-
-```text
-2024-05-11 00:56:32.299477:   Request sent to server: https://oai-westus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.299477:   Backend oai-westus-20240509.openai.azure.com is throttling. Retry after 44 second(s).
-2024-05-11 00:56:32.394350:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.395578:   Backend oai-eastus-20240509.openai.azure.com is throttling. Retry after 4 second(s).
-2024-05-11 00:56:32.451891:   Request sent to server: https://oai-southcentralus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.452883:   Backend oai-southcentralus-20240509.openai.azure.com is throttling. Retry after 7 second(s).
-2024-05-11 00:56:32.452883:   No backends available. Exiting.
-2024-05-11 00:56:32.453891:   Soonest Retry After: oai-eastus-20240509.openai.azure.com - 4 second(s)
-2024-05-11 00:56:38.551672:   Backend oai-eastus-20240509.openai.azure.com is no longer throttling.
-2024-05-11 00:56:39.851076:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status code: 200
-```
-
-## Load Balancer Backend Configuration
-
-At its core, the Load Balancer Backend configuration requires one or more backend hosts and a numeric priority starting at 1. Please take note that you define a host, not a URL.
-
-I use a total of three Azure OpenAI instances in three regions. These instances are set up with intentionally small tokens-per-minute (tpm) to trigger HTTP 429s.
-The standard approach never changes and uses the same host (first in the backend list), which provides a stable comparison to the load-balanced approach.
-While the number of requests differs per tests below, we issue the same number of requests against standard and load-balanced approaches.
-
-### One Backend
-
-This is logically equivalent to what the standard approach does. This configuration does not provide value over the standard approach.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1)
-]
-```
-
-### Two Backends with Same Priority
-
-Load-balancing evenly between Azure OpenAI instances hedges you against being stalled due to a 429 from a single instance.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1)
-]
-```
-
-### Three Backends with Same Priority
-
-Adding a third backend with same priority exacerbates the difference to the standard approach further. Here, we need to use 20 requests to incur more HTTP 429s.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-westus-xxxxxxxx.openai.azure.com", 1)
-]
-```
-
-### Three Backends with Two Different Priorities
-
-The most common reason for this approach may well be the prioritization of Provisioned Throughput Units (PTUs). This is a reserved capacity over a period of time that is billed at that reservation and not flexible as consumption instances. Aside from guaranteed capacity, latency is also much more stable. Naturally, this is an instance that you would want to prioritize over all others but allow yourself to have fallbacks if you burst over what the PTU provides.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
-    Backends("oai-westus-xxxxxxxx.openai.azure.com", 2)
-]
-```
-
-### Three Backends with Three Different Priorities
-
-An example of this setup may be that most of your assets reside in one region (e.g. East US). It stands to reason that you want to use the Azure OpenAI instance in that region. To hedge yourself against HTTP 429s, you decide to add a second region that's geographically close (e.g. East US 2) as well as a third (e.g. West US).
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
-    Backends("oai-westus-xxxxxxxx.openai.azure.com", 3)
-]
-```
+# Python OpenAI Load Balancer
+
+[![Python application](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/actions/workflows/python-app.yml) [![Python](https://img.shields.io/pypi/pyversions/azure-core.svg?maxAge=2592000)](https://pypi.org/project/openai-priority-loadbalancer/)
+
+TL;DR! How do I [start](#getting-started)?
+
+---
+
+Many AI workloads require using more than one Azure OpenAI instance to prioritize Provisioned Throughput Units (PTUs) and insulate themselves from timeouts. In having worked with customers on Azure OpenAI implementations, there are a few common, desired configurations:
+
+- Distribution of requests over multiple consumption instances to mitigate throttling.
+- Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
+- Tiered prioritization of multiple consumption instances (e.g. use instances first that are geographically closer).
+
+While the [OpenAI Python API library](https://github.com/openai/openai-python) respects HTTP 429 and automatically retries after the requested wait period, the library is not set up to support the aforementioned customer desires. The library does, however, allow for the injection of custom httpx clients. This gave rise to this project.
+
+And while there are other Python OpenAI load balancers freely available, I have not seen one yet that addresses the aforementioned scenarios.
+
+Python OpenAI LoadBalancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](./aoai.py) file in this repo.
+
+## Disclaimer
+
+**This is a pseudo load-balancer.**
+
+When executing this code in parallel, there is no way to distribute requests uniformly across all Azure OpenAI instances. Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would also imply a locking mechanism for updates, which would
+immediately inhibit the performance benefits of the load balancer. Without knowledge of any other python workers, we can only randomize selection of an available backend.
+
+Furthermore, while the load balancer handles retries across available backends, the [OpenAI Python API library](https://github.com/openai/openai-python) is not fully insulated from failing on multiple HTTP 429s when all backends are returning HTTP 429s. It is advised to load-test with multiple concurrent python workers to understand how your specific Azure OpenAI instances, your limits, and your load balancer configuration function.
+
+## Attribution
+
+This project would not have been possible without the incredible work that [@andredewes](https://github.com/andredewes) has done with his [Smart Load Balancing for OpenAI Endpoints and Azure API Management](https://github.com/Azure-Samples/openai-apim-lb). If you use Azure API Management in your infrastructure, I highly recommend you consider his policy.
+
+## Prerequisites
+
+It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in `aoai.py` here will look very familiar to you.
+It's also good to have some knowledge of authentication and identities.
+
+## Authentication
+
+Locally, you can log into Azure via the CLI and the steps below and use the `AzureDefaultCredential` (what I use in my example). When deploying this application in Azure, it's recommended to use a managed identity for authentication. It's best to avoid using the Azure OpenAI instances' keys as that could a) accidentally leave credentials in your source code, and b) the keys are different for each instance, which would probably require expanding upon the `Backends` class. Best to just avoid keys.
+
+## Getting Started
+
+### Cloning the repo & Preparing the python environment
+
+1. Clone the repo.
+1. Open the cloned repo folder in VS Code.
+1. Open a terminal session in VS Code.
+1. Run [setup-python.ps1](./setup-python.ps1) to prepare the python environment.
+
+### Configuration
+
+For the load-balanced approach, please use the same model across all instances.
+
+1. Open [aoai.py](./aoai.py).
+1. Replace `<your-aoai-model>` with the name of your Azure OpenAI model.
+1. Replace `<your-aoai-instance>` with the primary/single Azure OpenAI instance.
+1. Replace `<your-aoai-instance-1>`, `<your-aoai-instance-2>`, `<your-aoai-instance-3>` with all the Azure OpenAI instances you want to load-balance across. Delete entries you don't need. See [Load Balancer Backend Configuration](#load-balancer-backend-configuration) for details.
+1. Replace the value for variable `num_of_requests` with the number of requests you wish to execute.
+
+### Credentials
+
+Locally, your `AzureDefaultCredential` is used. Each Azure OpenAI instance must be configured with the `Cognitive Services OpenAI` User role for your Azure credential (the identity you use after logging in). This ensures that you can use your credential across all Azure OpenAI instances.
+
+When running in Azure, it's advised to use managed identities.
+
+1. Log in with `az login`.
+1. Set your subscription in which your Azure OpenAI assets reside: `az account set -s <name or id>`
+
+    *Missing this step may result in HTTP 400 errors for a tenant mismatch.*
+
+## Execution
+
+1. Initially, [python-aoai.ps1](./python-aoai.ps1) once to ensure it executes correctly.
+1. Run [python-aoai.ps1](./python-aoai.ps1) concurrently in multiple terminals to simulate parallel requests from multiple python workers.
+
+## Testing
+
+OpenAI Priority Load Balancer uses `pytest` and `coverage`. The test files can be found in the `tests\lib` directory. Executing `pytest -v` from the root will show test results. Note that these are rudimentary tests still and in the process of being built out further.
+
+To obtain coverage, execute `coverage run -m pytest -v` from the root. This generates a *.coverage* file. Then run `coverage report -m` or, for a nicer presentation, `coverage html`.
+
+Details on `coverage` can be found [here](https://coverage.readthedocs.io/).
+
+Pull requests for improvements are very much appreciated!
+
+## Distribution of Requests
+
+### Across Different Priorities
+
+Requests are made to the highest priority backend that is available. For example:
+
+- Priority 1, when available, will always supersede priority 2.
+- Priority 2, when available, will always supersede an unavailable priority 1.
+- Priority 3, when available, will always supersede unavailable priorities 1 & 2.
+
+### Across Multiple Backends of Same Priority
+
+In the single-requestor model, the distribution of attempts over available backends should be fairly uniform for backends of the same priority.
+
+There is no likelihood of a uniform distribution across available endpoints when running multiple python workers in parallel. In the below example, each terminal is executing 20 requests over two Azure OpenAI instances, both set up with the lowest of tokens-per-minute setting. Available backends are selected randomly (see the first request in each terminal). No sharing of data between the two terminals exists. Recovery takes place, when possible; otherwise, an HTTP 429 is returned to the OpenAI Python API library.
+
+![Parallel Execution](./assets/parallel-execution.png)
+
+## Backoff & Retries
+
+When no backends are available (e.g. all timed out), Python OpenAI Load Balancer returns the soonest retry in seconds determined based on the `retry_after` value on each backend.
+You may notice a delay in the logs between when the load balancer returns and when the next request is made. In addition to the `Retry-After` header value, the OpenAI Python library [uses a short exponential backoff](https://github.com/openai/openai-python?tab=readme-ov-file#retries).
+
+In this log excerpt, we see that all three backends are timing out. As the standard behavior returns an HTTP 429 from a single backend, we do the same here with the load-balanced approach. This allows the OpenAI Python library to handle the HTTP 429 that it believes it received from a singular backend.
+The wait periods are 44 seconds (westus), 4 seconds (eastus), and 7 seconds (southcentralus) in this log. Our logic determines that eastus will become available soonest. Therefore, we return a `Retry-After` header with a value of `4`. The OpenAI Python library then adds its exponential backoff (~2 seconds here).
+
+```text
+2024-05-11 00:56:32.299477:   Request sent to server: https://oai-westus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.299477:   Backend oai-westus-20240509.openai.azure.com is throttling. Retry after 44 second(s).
+2024-05-11 00:56:32.394350:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.395578:   Backend oai-eastus-20240509.openai.azure.com is throttling. Retry after 4 second(s).
+2024-05-11 00:56:32.451891:   Request sent to server: https://oai-southcentralus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.452883:   Backend oai-southcentralus-20240509.openai.azure.com is throttling. Retry after 7 second(s).
+2024-05-11 00:56:32.452883:   No backends available. Exiting.
+2024-05-11 00:56:32.453891:   Soonest Retry After: oai-eastus-20240509.openai.azure.com - 4 second(s)
+2024-05-11 00:56:38.551672:   Backend oai-eastus-20240509.openai.azure.com is no longer throttling.
+2024-05-11 00:56:39.851076:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status code: 200
+```
+
+## Load Balancer Backend Configuration
+
+At its core, the Load Balancer Backend configuration requires one or more backend hosts and a numeric priority starting at 1. Please take note that you define a host, not a URL.
+
+I use a total of three Azure OpenAI instances in three regions. These instances are set up with intentionally small tokens-per-minute (tpm) to trigger HTTP 429s.
+The standard approach never changes and uses the same host (first in the backend list), which provides a stable comparison to the load-balanced approach.
+While the number of requests differs per tests below, we issue the same number of requests against standard and load-balanced approaches.
+
+### One Backend
+
+This is logically equivalent to what the standard approach does. This configuration does not provide value over the standard approach.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1)
+]
+```
+
+### Two Backends with Same Priority
+
+Load-balancing evenly between Azure OpenAI instances hedges you against being stalled due to a 429 from a single instance.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1)
+]
+```
+
+### Three Backends with Same Priority
+
+Adding a third backend with same priority exacerbates the difference to the standard approach further. Here, we need to use 20 requests to incur more HTTP 429s.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-westus-xxxxxxxx.openai.azure.com", 1)
+]
+```
+
+### Three Backends with Two Different Priorities
+
+The most common reason for this approach may well be the prioritization of Provisioned Throughput Units (PTUs). This is a reserved capacity over a period of time that is billed at that reservation and not flexible as consumption instances. Aside from guaranteed capacity, latency is also much more stable. Naturally, this is an instance that you would want to prioritize over all others but allow yourself to have fallbacks if you burst over what the PTU provides.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
+    Backends("oai-westus-xxxxxxxx.openai.azure.com", 2)
+]
+```
+
+### Three Backends with Three Different Priorities
+
+An example of this setup may be that most of your assets reside in one region (e.g. East US). It stands to reason that you want to use the Azure OpenAI instance in that region. To hedge yourself against HTTP 429s, you decide to add a second region that's geographically close (e.g. East US 2) as well as a third (e.g. West US).
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
+    Backends("oai-westus-xxxxxxxx.openai.azure.com", 3)
+]
+```
```

### Comparing `openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py` & `openai_priority_loadbalancer-1.0.9/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,256 +1,283 @@
-"""Module providing a prioritized load-balancing for Azure OpenAI."""
-
-# Python Standard Library
-import logging
-import random
-from typing import List
-from datetime import datetime, MAXYEAR, MINYEAR, timedelta, timezone
-
-# Third-Party Libraries
-import httpx    # import the entirety of the httpx module to avoid potential conflicts with AsyncClient in the openai package by using httpx. notation
-
-class Backend:
-    """Class representing a backend object used with Azure OpenAI, etc."""
-
-    # Constructor
-    def __init__(self, host: str, priority: int):
-        # Public instance variables
-        self.host = host
-        self.is_throttling = False
-        self.priority = priority
-        self.retry_after = datetime.min
-        self.successful_call_count = 0
-
-# Reference design at https://github.com/encode/httpx/blob/master/httpx/_transports/base.py
-# BaseLoadBalancer providing functionality to both synchronous and asynchronous load balancers
-class BaseLoadBalancer():
-    """Logically abstracts the BaseLoadBalancer class which should be inherited by the synchronous and asynchronous load balancer classes."""
-
-    # Constructor
-    def __init__(self, transport, backends: List[Backend]):
-        # Public instance variables
-        self.backends = backends
-
-        # "Private" instance variables
-        self._backend_index = -1
-        self._log = logging.getLogger("openai-priority-loadbalancer")     # https://www.loggly.com/ultimate-guide/python-logging-basics/
-        self._available_backends = 1
-        self._transport = transport
-
-    # "Protected" Methods
-    def _check_throttling(self) -> None:
-        """Check if any backend is throttling and reset if necessary."""
-
-        min_datetime = datetime(MINYEAR, 1, 1, tzinfo = timezone.utc)
-
-        for backend in self.backends:
-            if backend.is_throttling and datetime.now(timezone.utc) >= backend.retry_after:
-                backend.is_throttling = False
-                backend.retry_after = min_datetime
-                self._log.info("Backend %s is no longer throttling.", backend.host)
-
-    def _get_backend_index(self) -> int:
-        """Return a backend list index of a highest-priority available backend to be used. If no backend is available, -1 will be returned."""
-
-        selected_priority = float('inf')
-        available_backends: List[int] = []      # This is a list of indices of available backends
-        index = -1
-
-        # 1) Evaluate all defined backends for availability and priority, leaving only the highest-priority available backends from which to select an index.
-        for i, backend in enumerate(self.backends):
-            if not backend.is_throttling:
-                backend_priority = backend.priority
-
-                # If a backend has a (logically) higher priority (1 would be logically higher than 2, etc.), we select that priority, clear the available
-                # backends index list which contains lower-priority backend indices thus far, then add the higher-priority backend(s) index to the list.
-                if backend_priority < selected_priority:
-                    selected_priority = backend_priority
-                    available_backends.clear()
-                    available_backends.append(i)
-                elif backend_priority == selected_priority:
-                    available_backends.append(i)
-
-        # 2) Out of the available backends indices, select a random index to use.
-        if len(available_backends) > 0:
-            # Since this code is very likely being called from multiple python instances with multiple workers in parallel executions, there's no way to distribute requests
-            # uniformly across all Azure OpenAI instances. Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would
-            # also imply a locking mechanism for updates, which would immediately inhibit the performance benefits of the load balancer. This is why this is more of a
-            # pseudo load-balancer. Therefore, we'll just randomize across the available backends.
-            index = random.choice(available_backends)
-
-        # If there are no available backends, None will be returned to indicate that nothing is available (and that we consequently need to bail by returning an HTTP 429).
-        return index
-
-    def _get_available_backends(self) -> int:
-        """Return the count of backends that are not actively throttled."""
-
-        self._available_backends = 0
-
-        for backend in self.backends:
-            if not backend.is_throttling:
-                self._available_backends += 1
-
-        self._log.info("Available backends: %s/%s", self._available_backends, len(self.backends))
-
-        return self._available_backends
-
-    def _get_soonest_retry_after(self) -> int:
-        """Return the soonest retry-after time in seconds among all throttling backends. This provides for the quickest retry time to be returned with the HTTP 429."""
-
-        soonest_retry_after = datetime(MAXYEAR, 1, 1, tzinfo = timezone.utc)
-
-        for backend in self.backends:
-            if backend.is_throttling and backend.retry_after < soonest_retry_after:
-                soonest_retry_after = backend.retry_after
-                soonest_backend = backend.host
-
-        # As the `int` cast truncates the decimal, we need to add 1 to the result to ensure that the delay is at least the number of seconds needed.
-        delay = int((soonest_retry_after - datetime.now(timezone.utc)).total_seconds()) + 1
-        self._log.info("The soonest retry to an available backend would be to %s after %s %s.", soonest_backend, delay, "second" if delay == 1 else "seconds")
-
-        return delay
-
-    def _handle_200_399_response(self, request, response, backend_index) -> httpx.Response:
-        """Handle a successful response from the backend."""
-
-        self._log.info("Request sent to server: %s, Status code: %s", request.url, response.status_code)
-        self.backends[backend_index].successful_call_count += 1
-
-        return response
-
-    def _handle_429_5xx_response(self, request, response, backend_index) -> None:
-        """Handle a 429 or 5xx response from the backend by identifying the retry-after interval, if available, and updating the available backends."""
-
-        self._log.info("Request sent to server: %s, Status code: %s - FAIL", request.url, response.status_code)
-
-        # 1) Determine the retry-after interval, if possible; otherwise, assign -1 to indicate that no delay is needed.
-        retry_after = int(response.headers.get('Retry-After', '-1'))
-
-        if retry_after == -1:
-            retry_after = int(response.headers.get('x-ratelimit-reset-requests', '-1'))
-
-        if retry_after == -1:
-            retry_after = int(response.headers.get('x-ratelimit-reset-requests', '10'))
-
-        self._log.info("Backend %s is throttling. Retry after %s %s.", self.backends[backend_index].host, retry_after, "second" if retry_after == 1 else "seconds")
-
-        # 2) Regardless of whether the response indicates a 429 or 5xx error, we mark the backend as throttling to temporarily take it out of the available backend pool.
-        backend = self.backends[backend_index]
-        backend.is_throttling = True
-        backend.retry_after = datetime.now(timezone.utc) + timedelta(seconds = retry_after)
-
-        # 3) Update the available backends.
-        self._get_available_backends()
-
-    def _handle_4xx_response(self, request, response) -> httpx.Response:
-        """Handle a 4xx response other than 429 from the backend."""
-
-        self._log.warning("Request sent to server: %s, Status code: %s - FAIL", request.url, response.status_code)
-
-        return response
-
-    def _modify_request(self, request, backend_index) -> None:
-        """Modifies the URL and Host header with the desired backend target. This ensures that the request is sent to the chosen backend server."""
-
-        # Modify the request. Note that only the URL and Host header are being modified on the original request object. We make the smallest incision possible to avoid side effects.
-        # Update URL and host header as both must match the backend server.
-        request.url = request.url.copy_with(host = self.backends[backend_index].host)
-        request.headers = request.headers.copy()    # We need to create a mutable copy of the headers before we modify and assign them back to the request object.
-        request.headers['host'] = self.backends[backend_index].host
-
-    def _return_429(self) -> httpx.Response:
-        """Return an HTTP 429 response with a Retry-After header value. This is returned to the caller of this load balancer when no backends are available."""
-
-        self._log.warning("No backend available!")
-        retry_after = str(self._get_soonest_retry_after())
-        self._log.info("Returning HTTP 429 with Retry-After header value of %s %s.", retry_after, "second" if retry_after == "1" else "seconds")
-
-        return httpx.Response(429, content = '', headers={'Retry-After': retry_after})
-
-class AsyncLoadBalancer(BaseLoadBalancer):
-    """Asynchronous Load Balancer class based on BaseLoadBalancer"""
-
-    # Constructor
-    def __init__(self, backends: List[Backend]):
-        super().__init__(httpx.AsyncClient(), backends)
-
-    # Public Methods
-    async def handle_async_request(self, request) -> httpx.Response:
-        """Handles an asynchronous request by issuing an asynchronous request to an available backed."""
-
-        self._log.info("Intercepted and now handling an asynchronous request.")
-
-        # Identify whether any backend is throttling and reset if necessary, then update the remaning available backends prior to any request handling.
-        self._check_throttling()
-        self._get_available_backends()
-        response = None
-
-        while self._available_backends > 0:
-            # 1) Since we have available backends determine the appropriate backend to use.
-            backend_index = self._get_backend_index()
-
-            # 2) Modify the intercepted request.
-            self._modify_request(request, backend_index)
-
-            # 3) Send the request to the selected backend (via async). If an error occurs, it will just bubble up, which is fine.
-            response = await self._transport.send(request)
-
-            # 4) Evaluate the response from the backend:
-            #    If 429 or a 5xx error, we continue the loop and retry with another backend, if available.
-            #    If 200-399, we return the successful response.
-            #    If any other 4xx error, we break the loop and return the response as we don't explicitly handle these client errors.
-            if response is not None and (response.status_code == 429 or response.status_code >= 500):
-                self._handle_429_5xx_response(request, response, backend_index)
-                continue
-
-            if response is not None and (response.status_code >= 200 and response.status_code <= 399):
-                return self._handle_200_399_response(request, response, backend_index)
-
-            return self._handle_4xx_response(request, response)
-
-        # Since no backends are available, we must return a 429.
-        return self._return_429()
-
-class LoadBalancer(BaseLoadBalancer):
-    """Synchronous Load Balancer class based on BaseLoadBalancer"""
-
-    # Constructor
-    def __init__(self, backends: List[Backend]):
-        super().__init__(httpx.Client(), backends)
-
-    # Public Methods
-    def handle_request(self, request) -> httpx.Response:
-        """Handles a synchronous request by issuing a request to an available backed."""
-
-        self._log.info("Intercepted and now handling a synchronous request.")
-
-        # Identify whether any backend is throttling and reset if necessary, then update the remaning available backends prior to any request handling.
-        self._check_throttling()
-        self._get_available_backends()
-        response = None
-
-        while self._available_backends > 0:
-            # 1) Since we have available backends determine the appropriate backend to use.
-            backend_index = self._get_backend_index()
-
-            # 2) Modify the intercepted request.
-            self._modify_request(request, backend_index)
-
-            # 3) Send the request to the selected backend. If an error occurs, it will just bubble up, which is fine.
-            response = self._transport.send(request)
-
-            # 4) Evaluate the response from the backend:
-            #    If 429 or a 5xx error, we continue the loop and retry with another backend, if available.
-            #    If 200-399, we return the successful response.
-            #    If any other 4xx error, we break the loop and return the response as we don't explicitly handle these client errors.
-            if response is not None and (response.status_code == 429 or response.status_code >= 500):
-                self._handle_429_5xx_response(request, response, backend_index)
-                continue
-
-            if response is not None and (response.status_code >= 200 and response.status_code <= 399):
-                return self._handle_200_399_response(request, response, backend_index)
-
-            return self._handle_4xx_response(request, response)
-
-        # Since no backends are available, we must return a 429.
-        return self._return_429()
+"""Module providing a prioritized load-balancing for Azure OpenAI."""
+
+# Python Standard Library
+import logging
+import random
+from typing import List
+from datetime import datetime, MAXYEAR, MINYEAR, timedelta, timezone
+
+# Third-Party Libraries
+import httpx    # import the entirety of the httpx module to avoid potential conflicts with AsyncClient in the openai package by using httpx. notation
+
+class Backend:
+    """Class representing a backend object used with Azure OpenAI, etc."""
+
+    # Constructor
+    def __init__(self, host: str, priority: int, path: str = None):
+        # Public instance variables
+        self.host = host
+        self.path = '' if path is None else path
+        self.is_throttling = False
+        self.priority = priority
+        self.retry_after = datetime.min
+        self.successful_call_count = 0
+
+# Reference design at https://github.com/encode/httpx/blob/master/httpx/_transports/base.py
+# BaseLoadBalancer providing functionality to both synchronous and asynchronous load balancers
+class BaseLoadBalancer():
+    """Logically abstracts the BaseLoadBalancer class which should be inherited by the synchronous and asynchronous load balancer classes."""
+
+    # Constructor
+    def __init__(self, transport: httpx.BaseTransport, backends: List[Backend]):
+        # Public instance variables
+        self.backends = backends
+
+        # "Private" instance variables
+        self._backend_index = -1
+        self._log = logging.getLogger("openai-priority-loadbalancer")     # https://www.loggly.com/ultimate-guide/python-logging-basics/
+        self._available_backends = 1
+        self._transport = transport
+
+    # "Protected" Methods
+    def _check_throttling(self) -> None:
+        """Check if any backend is throttling and reset if necessary."""
+
+        min_datetime = datetime(MINYEAR, 1, 1, tzinfo = timezone.utc)
+
+        for backend in self.backends:
+            if backend.is_throttling and datetime.now(timezone.utc) >= backend.retry_after:
+                backend.is_throttling = False
+                backend.retry_after = min_datetime
+                self._log.info("Backend %s is no longer throttling.", backend.host)
+
+    def _get_backend_index(self) -> int:
+        """Return a backend list index of a highest-priority available backend to be used. If no backend is available, -1 will be returned."""
+
+        selected_priority = float('inf')
+        available_backends: List[int] = []      # This is a list of indices of available backends
+        index = -1
+
+        # 1) Evaluate all defined backends for availability and priority, leaving only the highest-priority available backends from which to select an index.
+        for i, backend in enumerate(self.backends):
+            if not backend.is_throttling:
+                backend_priority = backend.priority
+
+                # If a backend has a (logically) higher priority (1 would be logically higher than 2, etc.), we select that priority, clear the available
+                # backends index list which contains lower-priority backend indices thus far, then add the higher-priority backend(s) index to the list.
+                if backend_priority < selected_priority:
+                    selected_priority = backend_priority
+                    available_backends.clear()
+                    available_backends.append(i)
+                elif backend_priority == selected_priority:
+                    available_backends.append(i)
+
+        # 2) Out of the available backends indices, select a random index to use.
+        if len(available_backends) > 0:
+            # Since this code is very likely being called from multiple python instances with multiple workers in parallel executions, there's no way to distribute requests
+            # uniformly across all Azure OpenAI instances. Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would
+            # also imply a locking mechanism for updates, which would immediately inhibit the performance benefits of the load balancer. This is why this is more of a
+            # pseudo load-balancer. Therefore, we'll just randomize across the available backends.
+            index = random.choice(available_backends)
+
+        # If there are no available backends, None will be returned to indicate that nothing is available (and that we consequently need to bail by returning an HTTP 429).
+        return index
+
+    def _get_available_backends(self) -> int:
+        """Return the count of backends that are not actively throttled."""
+
+        self._available_backends = 0
+
+        for backend in self.backends:
+            if not backend.is_throttling:
+                self._available_backends += 1
+
+        self._log.info("Available backends: %s/%s", self._available_backends, len(self.backends))
+
+        return self._available_backends
+
+    def _get_soonest_retry_after(self) -> int:
+        """Return the soonest retry-after time in seconds among all throttling backends. This provides for the quickest retry time to be returned with the HTTP 429."""
+
+        delay = 0
+        soonest_backend = ""
+        soonest_retry_after = datetime(MAXYEAR, 1, 1, tzinfo = timezone.utc)
+
+        for backend in self.backends:
+            if backend.is_throttling and backend.retry_after < soonest_retry_after:
+                soonest_retry_after = backend.retry_after
+                soonest_backend = backend.host
+
+        if soonest_backend != "":
+            # As the `int` cast truncates the decimal, we need to add 1 to the result to ensure that the delay is at least the number of seconds needed.
+            delay = int((soonest_retry_after - datetime.now(timezone.utc)).total_seconds()) + 1
+            self._log.info("The soonest retry to an available backend would be to %s after %s %s.", soonest_backend, delay, "second" if delay == 1 else "seconds")
+
+        return delay
+
+    def _handle_200_399_response(self, request: httpx.Request, response: httpx.Response, backend_index: int) -> httpx.Response:
+        """Handle a successful response from the backend."""
+
+        self._log.info("Request sent to server: %s, Status code: %s", request.url, response.status_code)
+        self.backends[backend_index].successful_call_count += 1
+
+        return response
+
+    def _handle_429_5xx_response(self, request: httpx.Request, response: httpx.Response, backend_index: int) -> None:
+        """Handle a 429 or 5xx response from the backend by identifying the retry-after interval, if available, and updating the available backends."""
+
+        self._log.info("Request sent to server: %s, Status code: %s - FAIL", request.url, response.status_code)
+
+        # 1) Determine the retry-after interval, if possible; otherwise, assign -1 to indicate that no delay is needed.
+        retry_after = int(response.headers.get('Retry-After', '-1'))
+
+        if retry_after == -1:
+            retry_after = int(response.headers.get('x-ratelimit-reset-requests', '-1'))
+
+        if retry_after == -1:
+            retry_after = int(response.headers.get('x-ratelimit-reset-requests', '10'))
+
+        self._log.info("Backend %s is throttling. Retry after %s %s.", self.backends[backend_index].host, retry_after, "second" if retry_after == 1 else "seconds")
+
+        # 2) Regardless of whether the response indicates a 429 or 5xx error, we mark the backend as throttling to temporarily take it out of the available backend pool.
+        backend = self.backends[backend_index]
+        backend.is_throttling = True
+        backend.retry_after = datetime.now(timezone.utc) + timedelta(seconds = retry_after)
+
+        # 3) Update the available backends.
+        self._get_available_backends()
+
+    def _handle_4xx_response(self, request: httpx.Request, response: httpx.Response) -> httpx.Response:
+        """Handle a 4xx response other than 429 from the backend."""
+
+        self._log.warning("Request sent to server: %s, Status code: %s - FAIL", request.url, response.status_code)
+
+        return response
+
+    def _modify_request(self, request: httpx.Request, backend_index: int) -> None:
+        """Modifies the URL and Host header with the desired backend target. This ensures that the request is sent to the chosen backend server."""
+
+        backend: Backend = self.backends[backend_index]
+
+        # Modify the request. Note that only the URL and Host header are being modified on the original request object. We make the smallest incision possible to avoid side effects.
+        # Update URL and host header as both must match the backend server.
+        request.url = request.url.copy_with(host = backend.host)
+
+        # Path is optional and used more so for extraordinary setups.
+        if backend.path is not None and backend.path != "":
+            backend_path = "/" + backend.path.lstrip('/').rstrip('/')  # Ensure that the path is formatted as "/<path>"
+
+            # Convert the URL to a string
+            url_str = str(request.url)
+
+            # Find the third slash (after the scheme and the host)
+            third_slash_index = url_str.find('/', url_str.find('/', url_str.find('/') + 1) + 1)
+
+            # Insert the backend path into the path string
+            new_url_str = url_str[:third_slash_index] + backend_path + url_str[third_slash_index:]
+
+            # Convert the string back to a URL
+            request.url = httpx.URL(new_url_str)
+
+        request.headers = request.headers.copy()    # We need to create a mutable copy of the headers before we modify and assign them back to the request object.
+        request.headers['host'] = backend.host
+
+        self._log.debug("URL %s and host %s", request.url, request.headers['host'])
+
+    def _return_429(self) -> httpx.Response:
+        """Return an HTTP 429 response with a Retry-After header value. This is returned to the caller of this load balancer when no backends are available."""
+
+        self._log.warning("No backend available!")
+        retry_after = str(self._get_soonest_retry_after())
+        self._log.info("Returning HTTP 429 with Retry-After header value of %s %s.", retry_after, "second" if retry_after == "1" else "seconds")
+
+        return httpx.Response(429, content = '', headers={'Retry-After': retry_after})
+
+class AsyncLoadBalancer(BaseLoadBalancer):
+    """Asynchronous Load Balancer class based on BaseLoadBalancer"""
+
+    # Constructor
+    def __init__(self, backends: List[Backend]):
+        super().__init__(httpx.AsyncClient(), backends)
+
+    # Public Methods
+    async def handle_async_request(self, request: httpx.Request) -> httpx.Response:
+        """Handles an asynchronous request by issuing an asynchronous request to an available backed."""
+
+        self._log.info("Intercepted and now handling an asynchronous request.")
+
+        # Identify whether any backend is throttling and reset if necessary, then update the remaning available backends prior to any request handling.
+        self._check_throttling()
+        self._get_available_backends()
+        response = None
+
+        while self._available_backends > 0:
+            # 1) Since we have available backends, determine the appropriate backend to use.
+            backend_index = self._get_backend_index()
+
+            # 2) Modify the intercepted request.
+            self._modify_request(request, backend_index)
+
+            # 3) Send the request to the selected backend (via async). If an error occurs, it will just bubble up, which is fine.
+            response = await self._transport.send(request)
+
+            # 4) Evaluate the response from the backend:
+            #    If 429 or a 5xx error, we continue the loop and retry with another backend, if available.
+            #    If 200-399, we return the successful response.
+            #    If any other 4xx error, we break the loop and return the response as we don't explicitly handle these client errors.
+            if response is not None:
+                if response.status_code == 429 or response.status_code >= 500:
+                    self._handle_429_5xx_response(request, response, backend_index)
+                    continue
+
+                if response.status_code >= 200 and response.status_code <= 399:
+                    return self._handle_200_399_response(request, response, backend_index)
+
+            return self._handle_4xx_response(request, response)
+
+        # Since no backends are available, we must return a 429.
+        return self._return_429()
+
+class LoadBalancer(BaseLoadBalancer):
+    """Synchronous Load Balancer class based on BaseLoadBalancer"""
+
+    # Constructor
+    def __init__(self, backends: List[Backend]):
+        super().__init__(httpx.Client(), backends)
+
+    # Public Methods
+    def handle_request(self, request: httpx.Request) -> httpx.Response:
+        """Handles a synchronous request by issuing a request to an available backed."""
+
+        self._log.info("Intercepted and now handling a synchronous request.")
+
+        # Identify whether any backend is throttling and reset if necessary, then update the remaning available backends prior to any request handling.
+        self._check_throttling()
+        self._get_available_backends()
+        response = None
+
+        while self._available_backends > 0:
+            # 1) Since we have available backends, determine the appropriate backend to use.
+            backend_index = self._get_backend_index()
+
+            # 2) Modify the intercepted request.
+            self._modify_request(request, backend_index)
+
+            # 3) Send the request to the selected backend. If an error occurs, it will just bubble up, which is fine.
+            response = self._transport.send(request)
+
+            # 4) Evaluate the response from the backend:
+            #    If 429 or a 5xx error, we continue the loop and retry with another backend, if available.
+            #    If 200-399, we return the successful response.
+            #    If any other 4xx error, we break the loop and return the response as we don't explicitly handle these client errors.
+            if response is not None:
+                if response.status_code == 429 or response.status_code >= 500:
+                    self._handle_429_5xx_response(request, response, backend_index)
+                    continue
+
+                if response.status_code >= 200 and response.status_code <= 399:
+                    return self._handle_200_399_response(request, response, backend_index)
+
+            return self._handle_4xx_response(request, response)
+
+        # Since no backends are available, we must return a 429.
+        return self._return_429()
```

### Comparing `openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer.egg-info/PKG-INFO` & `openai_priority_loadbalancer-1.0.9/src/openai_priority_loadbalancer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 1.0.8
+Version: 1.0.9
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
+Project-URL: Changelog, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/releases
+Project-URL: Documentation, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/README.md
+Project-URL: GitHub-Statistics, https://shields.io/github/stars/simonkurtz-MSFT/python-openai-loadbalancer?style=social
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
-Classifier: Programming Language :: Python :: 3
+Project-URL: Repository, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 
 # OpenAI Priority Load Balancer
 
@@ -94,17 +103,20 @@
 *Importing `httpx` lets us use `httpx.Client` and `httpx.AsyncClient`. This avoids having to update openai to at least
 [1.17.0](https://github.com/openai/openai-python/releases/tag/v1.17.0). The `openai` properties for `DefaultHttpxClient` and `DefaultAsyncHttpxClient` are mere wrappers for `httpx.Client` and `httpx.AsyncClient`.*
 
 ### Configuring the Backends and Load Balancer
 
 1. Define a list of backends according to the *Load Balancer Backend Configuration* section below.
 
+   *Optionally, a path can be added (e.g. `"/ai"`), which gets prepended to the request path. This is an extraordinary, not a commonly needed functionality.*
+
     ```python
     backends: List[Backend] = [
         Backend("oai-eastus.openai.azure.com", 1),
+        Backend("oai-eastus.openai.azure.com", 1, "/ai"),
         Backend("oai-southcentralus.openai.azure.com", 1)
     ]
     ```
 
 1. Instantiate the load balancer and inject a new httpx client with the load balancer as the new transport.
 
     **Synchronous**
```

