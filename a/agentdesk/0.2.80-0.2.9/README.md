# Comparing `tmp/agentdesk-0.2.80.tar.gz` & `tmp/agentdesk-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentdesk-0.2.80.tar", max compression
+gzip compressed data, was "agentdesk-0.2.9.tar", max compression
```

## Comparing `agentdesk-0.2.80.tar` & `agentdesk-0.2.9.tar`

### file list

```diff
@@ -1,25 +1,23 @@
--rw-r--r--   0        0        0     1069 2024-03-01 19:15:51.792143 agentdesk-0.2.80/LICENSE
--rw-r--r--   0        0        0     3029 2024-05-03 15:04:00.536834 agentdesk-0.2.80/README.md
--rw-r--r--   0        0        0       83 2024-04-17 17:32:38.870115 agentdesk-0.2.80/agentdesk/__init__.py
--rw-r--r--   0        0        0    12362 2024-05-18 02:14:18.056612 agentdesk-0.2.80/agentdesk/cli/main.py
--rw-r--r--   0        0        0      833 2024-05-21 15:14:44.473803 agentdesk-0.2.80/agentdesk/config.py
--rw-r--r--   0        0        0     2134 2024-05-17 22:07:49.472658 agentdesk-0.2.80/agentdesk/db/conn.py
--rw-r--r--   0        0        0     1423 2024-04-19 02:59:06.695025 agentdesk-0.2.80/agentdesk/db/models.py
--rw-r--r--   0        0        0    19391 2024-05-03 00:48:26.115100 agentdesk-0.2.80/agentdesk/device.py
--rw-r--r--   0        0        0     5994 2024-05-17 15:25:52.698051 agentdesk-0.2.80/agentdesk/key.py
--rw-r--r--   0        0        0       61 2024-03-09 05:02:55.881908 agentdesk-0.2.80/agentdesk/processors/__init__.py
--rw-r--r--   0        0        0      583 2024-03-09 05:02:55.882503 agentdesk-0.2.80/agentdesk/processors/base.py
--rw-r--r--   0        0        0     2302 2024-02-17 04:35:39.829916 agentdesk-0.2.80/agentdesk/processors/grid.py
--rw-r--r--   0        0        0    11138 2024-05-21 15:14:44.474565 agentdesk-0.2.80/agentdesk/proxy.py
--rw-r--r--   0        0        0     1372 2024-05-02 15:58:52.210179 agentdesk-0.2.80/agentdesk/server/models.py
--rw-r--r--   0        0        0      391 2024-05-02 15:58:53.468446 agentdesk-0.2.80/agentdesk/server/server.py
--rw-r--r--   0        0        0     5348 2024-05-02 15:58:44.008493 agentdesk-0.2.80/agentdesk/util.py
--rw-r--r--   0        0        0      136 2024-04-19 02:59:23.167006 agentdesk-0.2.80/agentdesk/vm/__init__.py
--rw-r--r--   0        0        0    14142 2024-05-18 02:32:52.782893 agentdesk-0.2.80/agentdesk/vm/base.py
--rw-r--r--   0        0        0    18660 2024-05-21 15:14:44.475101 agentdesk-0.2.80/agentdesk/vm/ec2.py
--rw-r--r--   0        0        0    16185 2024-05-21 15:14:44.475603 agentdesk-0.2.80/agentdesk/vm/gce.py
--rw-r--r--   0        0        0      490 2024-04-19 02:59:20.485682 agentdesk-0.2.80/agentdesk/vm/img.py
--rw-r--r--   0        0        0      578 2024-04-19 02:59:18.523492 agentdesk-0.2.80/agentdesk/vm/load.py
--rw-r--r--   0        0        0    13386 2024-05-21 15:14:44.476154 agentdesk-0.2.80/agentdesk/vm/qemu.py
--rw-r--r--   0        0        0     1571 2024-05-21 20:29:20.338431 agentdesk-0.2.80/pyproject.toml
--rw-r--r--   0        0        0     4440 1970-01-01 00:00:00.000000 agentdesk-0.2.80/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-08 22:45:37.309736 agentdesk-0.2.9/LICENSE
+-rw-r--r--   0        0        0     3026 2024-02-26 21:41:53.951319 agentdesk-0.2.9/README.md
+-rw-r--r--   0        0        0       49 2024-02-21 20:55:04.924191 agentdesk-0.2.9/agentdesk/__init__.py
+-rw-r--r--   0        0        0     7094 2024-02-14 04:00:04.398474 agentdesk-0.2.9/agentdesk/cli/main.py
+-rw-r--r--   0        0        0     1866 2024-01-31 16:53:44.642711 agentdesk-0.2.9/agentdesk/db/conn.py
+-rw-r--r--   0        0        0     1075 2024-02-10 17:59:13.694187 agentdesk-0.2.9/agentdesk/db/models.py
+-rw-r--r--   0        0        0       32 2024-02-16 20:22:08.955828 agentdesk-0.2.9/agentdesk/processors/__init__.py
+-rw-r--r--   0        0        0      588 2024-02-16 18:30:50.330971 agentdesk-0.2.9/agentdesk/processors/base.py
+-rw-r--r--   0        0        0     2302 2024-02-17 04:35:39.829916 agentdesk-0.2.9/agentdesk/processors/grid.py
+-rw-r--r--   0        0        0     9825 2024-02-11 00:43:28.862801 agentdesk-0.2.9/agentdesk/proxy.py
+-rw-r--r--   0        0        0     1165 2024-02-10 18:30:36.328489 agentdesk-0.2.9/agentdesk/server/models.py
+-rw-r--r--   0        0        0     1297 2024-02-01 20:00:04.347080 agentdesk-0.2.9/agentdesk/server/server.py
+-rw-r--r--   0        0        0    20511 2024-02-29 04:52:13.540525 agentdesk-0.2.9/agentdesk/tool.py
+-rw-r--r--   0        0        0     4949 2024-02-11 00:02:25.072183 agentdesk-0.2.9/agentdesk/util.py
+-rw-r--r--   0        0        0       76 2024-02-29 04:51:40.258667 agentdesk-0.2.9/agentdesk/vm/__init__.py
+-rw-r--r--   0        0        0    11720 2024-02-12 05:16:51.561490 agentdesk-0.2.9/agentdesk/vm/base.py
+-rw-r--r--   0        0        0    15220 2024-02-11 21:41:49.898874 agentdesk-0.2.9/agentdesk/vm/ec2.py
+-rw-r--r--   0        0        0    12805 2024-02-16 18:12:02.591435 agentdesk-0.2.9/agentdesk/vm/gce.py
+-rw-r--r--   0        0        0      490 2024-02-16 18:10:25.600966 agentdesk-0.2.9/agentdesk/vm/img.py
+-rw-r--r--   0        0        0      578 2024-02-10 16:50:22.116036 agentdesk-0.2.9/agentdesk/vm/load.py
+-rw-r--r--   0        0        0     9623 2024-02-14 05:53:59.478961 agentdesk-0.2.9/agentdesk/vm/qemu.py
+-rw-r--r--   0        0        0     1198 2024-02-29 17:27:54.875647 agentdesk-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4097 1970-01-01 00:00:00.000000 agentdesk-0.2.9/PKG-INFO
```

### Comparing `agentdesk-0.2.80/README.md` & `agentdesk-0.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   <br>
 </p>
 
 Agentdesk provides full featured desktop environments which can be programatically controlled by AI agents. Spin them up locally or in the cloud.
 
 ▶ Built on [agentd](https://github.com/agentsea/agentd) a runtime daemon which exposes a REST API for interacting with the desktop.
 
-▶ Implements the [DeviceBay Protocol](https://github.com/agentsea/devicebay)
+▶ Implements the [ToolsV1 protocol](https://github.com/agentsea/opentool)
 
 ## Installation
 
 ```
 pip install agentdesk
 ```
 
@@ -101,15 +101,15 @@
 ```
 
 _\*requires docker_
 
 ### List desktops
 
 ```python
-Desktop.find()
+Desktop.list()
 ```
 
 ```bash
 $ agentdesk get
 ```
 
 ### Delete a desktop
```

#### html2text {}

```diff
@@ -5,28 +5,28 @@
 
                   _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
 Agentdesk provides full featured desktop environments which can be
 programatically controlled by AI agents. Spin them up locally or in the cloud.
 â¶ Built on [agentd](https://github.com/agentsea/agentd) a runtime daemon
 which exposes a REST API for interacting with the desktop. â¶ Implements the
-[DeviceBay Protocol](https://github.com/agentsea/devicebay) ## Installation ```
+[ToolsV1 protocol](https://github.com/agentsea/opentool) ## Installation ```
 pip install agentdesk ``` ## Quick Start ```python from agentdesk import
 Desktop # Create a local VM desktop = Desktop.local() # Launch the UI for it
 desktop.view(background=True) # Open a browser to Google desktop.open_url
 ("https://google.com") # Take actions on the desktop desktop.move_mouse(500,
 500) desktop.click() img = desktop.take_screenshot() ``` ## Usage ### Create a
 local desktop ```python from agentdesk import Desktop desktop = Desktop.local()
 ``` ```bash $ agentdesk create --provider qemu ``` _\*requires [qemu](https://
 www.qemu.org/)_ ### Create a remote desktop on GCE ```python desktop =
 Desktop.gce() ``` ```bash $ agentdesk create --provider gce ``` ### Create a
 remote desktop on EC2 ```python desktop = Desktop.ec2() ``` ```bash $ agentdesk
 create --provider ec2 ``` ### View the desktop in the UI ```python desktop.view
 () ``` ```bash $ agentdesk view old_mckinny ``` _\*requires docker_ ### List
-desktops ```python Desktop.find() ``` ```bash $ agentdesk get ``` ### Delete a
+desktops ```python Desktop.list() ``` ```bash $ agentdesk get ``` ### Delete a
 desktop ```python Desktop.delete("old_mckinny") ``` ```bash $ agentdesk delete
 old_mckinny ``` ### Use the desktop ```python desktop.open_url("https://
 google.com") coords = desktop.mouse_coordinates() desktop.move_mouse(500, 500)
 desktop.click() desktop.type_text("What kind of ducks are in Canada?")
 desktop.press_key('Enter') desktop.scroll() img = desktop.take_screenshot() ```
 ### Processors Process images to make them more accessible to LMMs. #### Grid
 Add a coordinate grid on top of the image ```python from agentdesk.processors
```

### Comparing `agentdesk-0.2.80/agentdesk/db/conn.py` & `agentdesk-0.2.9/agentdesk/db/conn.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,47 @@
 import os
-import time
-import logging
 
 from sqlalchemy import create_engine, Engine
 from sqlalchemy.orm import sessionmaker
 
 from .models import Base
 
-from agentdesk import config
-
-logger = logging.getLogger(__name__)
 
 DB_TYPE = os.environ.get("DB_TYPE", "sqlite")
 
 
 def get_pg_conn() -> Engine:
-    # Helper function to get environment variable with fallback
-    def get_env_var(key: str) -> str:
-        task_key = f"DESKS_{key}"
-        value = os.environ.get(task_key)
-        if value is None:
-            value = os.environ.get(key)
-            if value is None:
-                raise ValueError(f"${key} must be set")
-        return value
-
-    # Retrieve environment variables with fallbacks
-    db_user = get_env_var("DB_USER")
-    db_password = get_env_var("DB_PASS")
-    db_host = get_env_var("DB_HOST")
-    db_name = get_env_var("DB_NAME")
+    # Env Vars
+    db_user = os.environ.get("DB_USER")
+    if not db_user:
+        raise ValueError("$DB_USER must be set to a valid postgres db user")
+
+    db_password = os.environ.get("DB_PASS")
+    if not db_password:
+        raise ValueError("$DB_PASS must be set to a valid postgres db user password")
+
+    db_host = os.environ.get("DB_HOST")
+    if not db_user:
+        raise ValueError("$DB_HOST must be set to a running postgres server")
+
+    db_name = os.environ.get("DB_NAME")
+    if not db_name:
+        raise ValueError("$DB_NAME must be set to a postgres db name")
 
-    logger.debug(f"connecting to db on postgres host '{db_host}' with db '{db_name}'")
     engine = create_engine(
         f"postgresql+psycopg2://{db_user}:{db_password}@{db_host}/{db_name}",
         client_encoding="utf8",
     )
 
     return engine
 
 
 def get_sqlite_conn() -> Engine:
-    db_path = os.path.join(config.AGENTSEA_DB_DIR, config.DB_NAME)
-    logger.debug(f"connecting to local sqlite db {db_path}")
-    os.makedirs(os.path.dirname(f"{db_path}"), exist_ok=True)
-    engine = create_engine(f"sqlite:///{db_path}")
+    os.makedirs(os.path.dirname("./data/agentdesk.db"), exist_ok=True)
+    engine = create_engine("sqlite:///./data/agentdesk.db")
     return engine
 
 
 if DB_TYPE == "postgres":
     engine = get_pg_conn()
 else:
     engine = get_sqlite_conn()
```

### Comparing `agentdesk-0.2.80/agentdesk/device.py` & `agentdesk-0.2.9/agentdesk/tool.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 # from __future__ import annotations
 import base64
 import io
 from enum import Enum
 import time
 import os
-from typing import Tuple, Optional, List, Any, Type
-import atexit
+from typing import Tuple, Optional, List
 
 import requests
-from pydantic import BaseModel
+
 from PIL import Image
 from google.cloud import storage
-from devicebay import Device, action, observation, Action, ReactComponent
+from opentool import Tool, action, observation, Action, Observation
 
-from .server.models import V1ProviderData
-from .vm.base import DesktopVM
-from .vm.load import load_provider
-from .key import SSHKeyPair
+from .vm.base import DesktopVM, DesktopProvider
 
 try:
     from .vm.gce import GCEProvider
 except ImportError:
     print(
         "GCE provider unavailable, install with `pip install agentdesk[gce] if desired"
     )
@@ -28,254 +24,160 @@
     from .vm.ec2 import EC2Provider
 except ImportError:
     print(
         "AWS provider unavailable, install with `pip install agentdesk[aws] if desired"
     )
 
 from .vm.qemu import QemuProvider
-from .util import (
-    extract_file_path,
-    extract_gcs_info,
-    generate_random_string,
-)
-from .proxy import ensure_ssh_proxy, cleanup_proxy
+from .util import extract_file_path, extract_gcs_info, generate_random_string
 
 
 class StorageStrategy(Enum):
     GCS = "gcs"
     LOCAL = "local"
 
 
-class ConnectConfig(BaseModel):
-    agentd_url: Optional[str] = None
-    vm: Optional[str] = None
-    storage_uri: str = "file://.media"
-    type_min_interval: float = 0.05
-    type_max_interval: float = 0.25
-    move_mouse_duration: float = 1.0
-    mouse_tween: str = "easeInOutQuad"
-    store_img: bool = False
-    requires_proxy: bool = True
-    proxy_type: str = "process"
-    proxy_port: int = 8000
-    private_ssh_key: Optional[str] = None
-    ssh_port: int = 22
-
-
-class ProvisionConfig(BaseModel):
-    provider: V1ProviderData = V1ProviderData(type="qemu")
-    image: Optional[str] = None
-    memory: int = 4
-    cpus: int = 2
-    disk: str = "30gb"
-    reserve_ip: bool = False
-    ssh_key_pair: Optional[str] = None
-    proxy_port: int = 8000
-
-
-class Desktop(Device):
-    """Desktop OS as a device via agentd"""
+class Desktop(Tool):
+    """Desktop OS as a tool via agentd"""
 
     def __init__(
         self,
         agentd_url: Optional[str] = None,
         vm: Optional[DesktopVM] = None,
         storage_uri: str = "file://.media",
         type_min_interval: float = 0.05,
         type_max_interval: float = 0.25,
         move_mouse_duration: float = 1.0,
         mouse_tween: str = "easeInOutQuad",
         store_img: bool = False,
-        requires_proxy: bool = True,
-        proxy_type: str = "process",
-        proxy_port: int = 8000,
-        private_ssh_key: Optional[str] = None,
-        ssh_port: int = 22,
-        check_health: bool = True,
     ) -> None:
         """Connect to an agent desktop
 
         Args:
             agentd_url (str, optional): URL of a running agentd server. Defaults to None.
             vm (str, optional): Optional desktop VM to use. Defaults to None.
             storage_uri (str): The directory where to store images or videos taken of the VM, supports gs:// or file://. Defaults to file://.media.
             type_min_interval (float, optional): Min interval between pressing next key. Defaults to 0.05.
             type_max_interval (float, optional): Max interval between pressing next key. Defaults to 0.25.
             move_mouse_duration (float, optional): How long should it take to move. Defaults to 1.0.
             mouse_tween (str, optional): The movement tween. Defaults to "easeInOutQuad".
             store_img (bool, optional): Whether to store the image in the cloud. Defaults to false
-            requires_proxy (bool, optional): Whether to use a proxy. Defaults to True.
-            proxy_type (str, optional): The type of proxy to use. Defaults to process.
-            proxy_port (int, optional): The port to use for the proxy. Defaults to 8000.
-            private_ssh_key (str, optional): The private ssh key to use for the proxy. Defaults to None.
-            ssh_port (int, optional): The port to use for the ssh connection. Defaults to 22.
-            check_health (bool, optional): Whether to check the health of the server. Defaults to True.
         """
         super().__init__()
         self._vm = vm
-        self._agentd_url = agentd_url
 
-        self._key_pair_name = None
         if vm:
-            if vm.requires_proxy:
-                self._agentd_url = vm.addr
-                self.base_url = f"localhost:{proxy_port}"
-            else:
-                self.base_url = vm.addr
-                if vm.provider and vm.provider.type == "qemu":
-                    self.base_url = f"{vm.addr}:8000"
-                self._agentd_url = self.base_url
-
-            self._key_pair_name = vm.key_pair_name
-            keys = SSHKeyPair.find(name=self._key_pair_name)
-            if not keys:
-                raise ValueError(f"No key found with name {self._key_pair_name}")
-            key_pair = keys[0]
-
-            private_ssh_key = key_pair.decrypt_private_key(key_pair.private_key)
-
+            self.base_url = f"{vm.addr}:8000"
         else:
             self.base_url = agentd_url
 
-        if not self.base_url.startswith("http"):  # type: ignore
+        if not self.base_url.startswith("http"):
             self.base_url = f"http://{self.base_url}"
 
         self.storage_uri = storage_uri
         self._type_min_interval = type_min_interval
         self._type_max_interval = type_max_interval
         self._move_mouse_duration = move_mouse_duration
         self._mouse_tween = mouse_tween
         self._store_img = store_img
-        self._proxy_port = proxy_port
-        self._requires_proxy = requires_proxy if vm is None else vm.requires_proxy
-        self._private_ssh_key = private_ssh_key
-        self._ssh_port = ssh_port
-        self._proxy_type = proxy_type
-
-        if self._requires_proxy:
-            if proxy_type == "process":
-                print("starting proxy to vm...")
-                # if check_port_in_use(proxy_port):
-                #     raise ValueError(
-                #         f"Port {proxy_port} is already in use"
-                #     )  # TODO: remove this restriction
-                proxy_pid = ensure_ssh_proxy(
-                    local_port=proxy_port,
-                    remote_port=8000,
-                    ssh_port=vm.ssh_port if vm else ssh_port,
-                    ssh_user="agentsea",
-                    ssh_host=vm.addr if vm else agentd_url,  # type: ignore
-                    ssh_key=private_ssh_key,
-                )
-                atexit.register(cleanup_proxy, proxy_pid)
-                print(
-                    f"proxy from local port {proxy_port} to remote port 8000 started..."
-                )
-                self.base_url = f"http://localhost:{proxy_port}"
-            if proxy_type == "mock":
-                pass
-        else:
-            print("vm doesn't require proxy")
 
         try:
-            if check_health:
-                resp = self.health()
-                if resp["status"] != "ok":
-                    raise ValueError("agentd status is not ok")
-                print("connected to desktop via agentd")
+            resp = self.health()
+            if resp["status"] != "ok":
+                raise ValueError("agentd status is not ok")
         except Exception as e:
             raise SystemError(f"could not connect to desktop, is agentd running? {e}")
 
+        print("connected to desktop via agentd")
+
     @classmethod
     def ensure(
         cls,
         name: str,
-        config: ProvisionConfig,
+        provider: DesktopProvider = QemuProvider(),
+        image: Optional[str] = None,
+        memory: int = 4,
+        cpus: int = 2,
+        disk: str = "30gb",
+        reserve_ip: bool = False,
+        ssh_key: Optional[str] = None,
     ) -> "Desktop":
         """Find or create a desktop"""
-        vm = DesktopVM.get(name)
+        vm = DesktopVM.find(name)
         if vm:
             return cls.from_vm(vm)
 
         return cls.create(
-            name=name,
-            config=config,
+            name, provider, image, memory, cpus, disk, reserve_ip, ssh_key
         )
 
     @classmethod
     def create(
         cls,
         name: Optional[str] = None,
-        config: ProvisionConfig = ProvisionConfig(),
+        provider: DesktopProvider = QemuProvider(),
+        image: Optional[str] = None,
+        memory: int = 4,
+        cpus: int = 2,
+        disk: str = "30gb",
+        reserve_ip: bool = False,
+        ssh_key: Optional[str] = None,
     ) -> "Desktop":
         """Create a desktop VM"""
-
-        provider = load_provider(config.provider)
-        vm = provider.create(
-            name=name,
-            image=config.image,
-            memory=config.memory,
-            cpu=config.cpus,
-            disk=config.disk,
-            reserve_ip=config.reserve_ip,
-            ssh_key_pair=config.ssh_key_pair,
-        )
-        return cls.from_vm(vm, proxy_port=config.proxy_port)
+        vm = provider.create(name, image, memory, cpus, disk, reserve_ip, ssh_key)
+        return cls.from_vm(vm)
 
     @classmethod
     def ec2(
         cls,
         name: Optional[str] = None,
         region: Optional[str] = None,
         image: Optional[str] = None,
         memory: int = 4,
         cpus: int = 2,
         disk: str = "30gb",
         reserve_ip: bool = False,
-        ssh_key_pair: Optional[str] = None,
+        ssh_key: Optional[str] = None,
     ) -> "Desktop":
         """Create a desktop VM on EC2"""
-        if not region:
-            region = "us-east-1"
-
-        config = ProvisionConfig(
-            provider=EC2Provider(region=region).to_data(),  # type: ignore
+        return cls.create(
+            name=name,
+            provider=EC2Provider(region),
             image=image,
             memory=memory,
             cpus=cpus,
             disk=disk,
             reserve_ip=reserve_ip,
-            ssh_key_pair=ssh_key_pair,
+            ssh_key=ssh_key,
         )
-        return cls.create(name=name, config=config)
 
     @classmethod
     def gce(
         cls,
         name: Optional[str] = None,
         project: Optional[str] = None,
         zone: Optional[str] = None,
         image: Optional[str] = None,
         memory: int = 4,
         cpus: int = 2,
         disk: str = "30gb",
         reserve_ip: bool = False,
-        ssh_key_pair: Optional[str] = None,
+        ssh_key: Optional[str] = None,
     ) -> "Desktop":
         """Create a desktop VM on GCE"""
-        config = ProvisionConfig(
-            provider=GCEProvider(project_id=project, zone=zone).to_data(),  # type: ignore
+        return cls.create(
+            name=name,
+            provider=GCEProvider(project, zone),
             image=image,
             memory=memory,
             cpus=cpus,
             disk=disk,
             reserve_ip=reserve_ip,
-            ssh_key_pair=ssh_key_pair,
+            ssh_key=ssh_key,
         )
-        return cls.create(name=name, config=config)
 
     @classmethod
     def local(
         cls,
         name: Optional[str] = None,
         memory: int = 4,
         cpus: int = 2,
@@ -286,130 +188,51 @@
             name (str, optional): Name of the vm. Defaults to None.
             memory (int, optional): Memory the VM has. Defaults to 4.
             cpus (int, optional): CPUs the VM has. Defaults to 2.
 
         Returns:
             Desktop: A desktop
         """
-        config = ProvisionConfig(
-            provider=QemuProvider().to_data(), memory=memory, cpus=cpus
-        )
-        return cls.create(name=name, config=config)
+        return cls.create(name=name, provider=QemuProvider(), memory=memory, cpus=cpus)
 
     @classmethod
-    def connect(cls, config: ConnectConfig) -> "Desktop":
-        vm = None
-        if config.vm:
-            vms = DesktopVM.find(name=config.vm)
-            if not vms:
-                raise ValueError(f"VM {config.vm} was not found")
-            vm = vms[0]
-        return cls(
-            agentd_url=config.agentd_url,
-            private_ssh_key=config.private_ssh_key,
-            vm=vm,
-            storage_uri=config.storage_uri,
-            type_min_interval=config.type_min_interval,
-            type_max_interval=config.type_max_interval,
-            move_mouse_duration=config.move_mouse_duration,
-            mouse_tween=config.mouse_tween,
-            store_img=config.store_img,
-            requires_proxy=config.requires_proxy,
-            proxy_type=config.proxy_type,
-            proxy_port=config.proxy_port,
-            ssh_port=config.ssh_port,
-        )
-
-    def disconnect(self) -> None:
-        """Disconnect from the device"""
-        pass
-
-    def connect_config(self) -> ConnectConfig:
-        ssh_private_key = None
-        if self._key_pair_name:
-            keys = SSHKeyPair.find(name=self._key_pair_name)
-            if not keys:
-                raise ValueError(f"No key found with name {self._key_pair_name}")
-            key_pair = keys[0]
-
-            ssh_private_key = key_pair.decrypt_private_key(key_pair.private_key)
-
-        return ConnectConfig(
-            agentd_url=self._agentd_url,
-            storage_uri=self.storage_uri,
-            type_min_interval=self._type_min_interval,
-            type_max_interval=self._type_max_interval,
-            move_mouse_duration=self._move_mouse_duration,
-            mouse_tween=self._mouse_tween,
-            store_img=self._store_img,
-            requires_proxy=self._requires_proxy,
-            proxy_type=self._proxy_type,
-            proxy_port=self._proxy_port,
-            private_ssh_key=ssh_private_key,
-            ssh_port=self._ssh_port,
-        )
-
-    @classmethod
-    def connect_config_type(cls) -> Type[ConnectConfig]:
-        return ConnectConfig
-
-    @classmethod
-    def provision_config_type(cls) -> Type[ProvisionConfig]:
-        return ProvisionConfig
-
-    @classmethod
-    def react_component(cls) -> ReactComponent:
-        return ReactComponent()
-
-    @classmethod
-    def from_vm(
-        cls,
-        vm: DesktopVM,
-        proxy_type: str = "process",
-        proxy_port: int = 8000,
-        check_health: bool = True,
-    ) -> "Desktop":
+    def from_vm(cls, vm: DesktopVM) -> "Desktop":
         """Create a desktop from a VM
 
         Args:
             vm (DesktopVM): VM to use
-            proxy_type (str, optional): The type of proxy to use. Defaults to process.
-            proxy_port (int, optional): The port to use for the proxy. Defaults to 8000.
-            check_health (bool, optional): Check the health of the VM. Defaults to True.
 
         Returns:
             Desktop: A desktop
         """
-        return Desktop(
-            vm=vm,
-            proxy_type=proxy_type,
-            proxy_port=proxy_port,
-            check_health=check_health,
-        )
+        return Desktop(vm=vm)
 
     @classmethod
-    def get(cls, name: str) -> Optional[DesktopVM]:
-        """Get a desktop by name
+    def find(cls, name: str) -> "Desktop":
+        """Find a desktop by name
 
         Args:
             name (str): Name of the desktop
 
         Returns:
             Desktop: A desktop
         """
-        return DesktopVM.get(name)
+        found = DesktopVM.find(name)
+        if not found:
+            raise ValueError(f"could not find desktop with name {name}")
+        return cls.from_vm(found)
 
     @classmethod
-    def find(cls, **kwargs: Any) -> list[DesktopVM]:
+    def list(cls) -> list[DesktopVM]:
         """List all desktops
 
         Returns:
             list[DesktopVM]: A list of desktop vms
         """
-        return DesktopVM.find(**kwargs)
+        return DesktopVM.list()
 
     def info(self) -> dict:
         """Get info on the desktop runtime
 
         Returns:
             dict: A dictionary of info
         """
@@ -475,15 +298,15 @@
         Args:
             button (str, optional): Button to click. Defaults to "left".
             x (Optional[int], optional): X coordinate to move to, if not provided it will click on current location. Defaults to None.
             y (Optional[int], optional): Y coordinate to move to, if not provided it will click on current location. Defaults to None.
         """
         body = {"button": button}
         if x and y:
-            body["location"] = {"x": x, "y": y}  # type: ignore
+            body["location"] = {"x": x, "y": y}
 
         requests.post(f"{self.base_url}/click", json=body)
         return
 
     @action
     def press_key(self, key: str) -> None:
         """Press a key
@@ -599,19 +422,264 @@
     def actions(self) -> List[Action]:
         """Actions the agent can take
 
         Returns:
             List[Action]: List of actions
         """
         out = []
-        for actionv in self._actions_list:
-            if actionv.name in [
+        for action in self._actions_list:
+            if action.name in [
                 "open_url",
                 "type_text",
                 "click",
                 "scroll",
                 "press_key",
                 "move_mouse",
             ]:
-                out.append(actionv)
+                out.append(action)
 
         return out
+
+
+class WebApp(Desktop):
+    """A web application running on a desktop vm"""
+
+    def __init__(
+        self,
+        url: str,
+        agentd_url: Optional[str] = None,
+        vm: Optional[DesktopVM] = None,
+        storage_uri: str = "file://.media",
+        type_min_interval: float = 0.05,
+        type_max_interval: float = 0.25,
+        move_mouse_duration: float = 1.0,
+        mouse_tween: str = "easeInOutQuad",
+        store_img: bool = False,
+    ) -> None:
+        """
+        Initialize and open a URL in the application.
+
+        Args:
+            url: URL to open upon initialization.
+            agentd_url: URL of a running agentd server. Defaults to None.
+            vm: Optional desktop VM to use. Defaults to None.
+            storage_uri: The directory where to store images or videos taken of the VM, supports gs:// or file://. Defaults to "file://.media".
+            type_min_interval: Min interval between pressing the next key. Defaults to 0.05.
+            type_max_interval: Max interval between pressing the next key. Defaults to 0.25.
+            move_mouse_duration: How long it should take to move the mouse. Defaults to 1.0.
+            mouse_tween: The movement tween. Defaults to "easeInOutQuad".
+            store_img: Whether to store the image in the cloud. Defaults to False.
+        """
+        super().__init__(
+            agentd_url=agentd_url,
+            vm=vm,
+            storage_uri=storage_uri,
+            type_min_interval=type_min_interval,
+            type_max_interval=type_max_interval,
+            move_mouse_duration=move_mouse_duration,
+            mouse_tween=mouse_tween,
+            store_img=store_img,
+        )
+        self.open_url(url)
+
+    @classmethod
+    def create(
+        cls,
+        url: str,
+        name: Optional[str] = None,
+        image: Optional[str] = None,
+        memory: int = 4,
+        cpus: int = 2,
+        disk: str = "30gb",
+        reserve_ip: bool = False,
+        ssh_key: Optional[str] = None,
+    ) -> "WebApp":
+        """
+        Create a desktop VM and open a URL.
+
+        Args:
+            url: URL to open after creation.
+            name: Name of the VM. Defaults to None.
+            image: Image to use for the VM. Defaults to None.
+            memory: Memory the VM has. Defaults to 4.
+            cpus: CPUs the VM has. Defaults to 2.
+            disk: Disk size for the VM. Defaults to "30gb".
+            reserve_ip: Whether to reserve IP for the VM. Defaults to False.
+            ssh_key: SSH key for the VM. Defaults to None.
+
+        Returns:
+            An instance of the WebApp class.
+        """
+        desktop = super(WebApp, cls).create(
+            name=name,
+            provider=QemuProvider(),
+            image=image,
+            memory=memory,
+            cpus=cpus,
+            disk=disk,
+            reserve_ip=reserve_ip,
+            ssh_key=ssh_key,
+        )
+        desktop.open_url(url)
+        return desktop
+
+    @classmethod
+    def ec2(
+        cls,
+        url: str,
+        name: Optional[str] = None,
+        region: Optional[str] = None,
+        image: Optional[str] = None,
+        memory: int = 4,
+        cpus: int = 2,
+        disk: str = "30gb",
+        reserve_ip: bool = False,
+        ssh_key: Optional[str] = None,
+    ) -> "WebApp":
+        """
+        Create a desktop VM on EC2 and open a URL.
+
+        Args:
+            url: URL to open after creation.
+            name: Name of the VM. Defaults to None.
+            region: AWS region for the VM. Defaults to None.
+            image: AMI to use for the VM. Defaults to None.
+            memory: Memory the VM has. Defaults to 4.
+            cpus: CPUs the VM has. Defaults to 2.
+            disk: Disk size for the VM. Defaults to "30gb".
+            reserve_ip: Whether to reserve IP for the VM. Defaults to False.
+            ssh_key: SSH key for the VM. Defaults to None.
+
+        Returns:
+            An instance of the WebApp class.
+        """
+        desktop = super(WebApp, cls).ec2(
+            name=name,
+            region=region,
+            image=image,
+            memory=memory,
+            cpus=cpus,
+            disk=disk,
+            reserve_ip=reserve_ip,
+            ssh_key=ssh_key,
+        )
+        desktop.open_url(url)
+        return desktop
+
+    @classmethod
+    def gce(
+        cls,
+        url: str,
+        name: Optional[str] = None,
+        project: Optional[str] = None,
+        zone: Optional[str] = None,
+        image: Optional[str] = None,
+        memory: int = 4,
+        cpus: int = 2,
+        disk: str = "30gb",
+        reserve_ip: bool = False,
+        ssh_key: Optional[str] = None,
+    ) -> "WebApp":
+        """
+        Create a desktop VM on GCE and open a URL.
+
+        Args:
+            url: URL to open after creation.
+            name: Name of the VM. Defaults to None.
+            project: GCP project for the VM. Defaults to None.
+            zone: GCP zone for the VM. Defaults to None.
+            image: Image to use for the VM. Defaults to None.
+            memory: Memory the VM has. Defaults to 4.
+            cpus: CPUs the VM has. Defaults to 2.
+            disk: Disk size for the VM. Defaults to "30gb".
+            reserve_ip: Whether to reserve IP for the VM. Defaults to False.
+            ssh_key: SSH key for the VM. Defaults to None.
+
+        Returns:
+            An instance of the WebApp class.
+        """
+        desktop = super(WebApp, cls).gce(
+            name=name,
+            project=project,
+            zone=zone,
+            image=image,
+            memory=memory,
+            cpus=cpus,
+            disk=disk,
+            reserve_ip=reserve_ip,
+            ssh_key=ssh_key,
+        )
+        desktop.open_url(url)
+        return desktop
+
+    @classmethod
+    def local(
+        cls,
+        url: str,
+        name: Optional[str] = None,
+        memory: int = 4,
+        cpus: int = 2,
+    ) -> "WebApp":
+        """
+        Create a local VM and open a URL.
+
+        Args:
+            url: URL to open after creation.
+            name: Name of the VM. Defaults to None.
+            memory: Memory the VM has. Defaults to 4.
+            cpus: CPUs the VM has. Defaults to 2.
+
+        Returns:
+            An instance of the WebApp class.
+        """
+        desktop = super(WebApp, cls).local(
+            name=name,
+            memory=memory,
+            cpus=cpus,
+        )
+        desktop.open_url(url)
+        return desktop
+
+    @classmethod
+    def ensure(
+        cls,
+        url: str,
+        name: str,
+        provider: Optional[DesktopProvider] = QemuProvider(),
+        image: Optional[str] = None,
+        memory: int = 4,
+        cpus: int = 2,
+        disk: str = "30gb",
+        reserve_ip: bool = False,
+        ssh_key: Optional[str] = None,
+    ) -> "WebApp":
+        """
+        Ensure a desktop VM exists with the given name, or create it if it does not, and open a URL.
+
+        Args:
+            url: URL to open after ensuring the VM exists.
+            name: Name of the VM to find or create.
+            provider: The provider for VM creation, defaults to QemuProvider if not specified.
+            image: Image to use for the VM. Defaults to None.
+            memory: Memory the VM has. Defaults to 4.
+            cpus: CPUs the VM has. Defaults to 2.
+            disk: Disk size for the VM. Defaults to "30gb".
+            reserve_ip: Whether to reserve an IP for the VM. Defaults to False.
+            ssh_key: SSH key for the VM. Defaults to None.
+
+        Returns:
+            An instance of the WebApp class.
+        """
+        desktop = super(WebApp, cls).ensure(
+            name=name,
+            provider=provider,
+            image=image,
+            memory=memory,
+            cpus=cpus,
+            disk=disk,
+            reserve_ip=reserve_ip,
+            ssh_key=ssh_key,
+        )
+
+        desktop.open_url(url)
+
+        return desktop
```

### Comparing `agentdesk-0.2.80/agentdesk/processors/base.py` & `agentdesk-0.2.9/agentdesk/processors/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 
 
 class ImgProcessor:
     """Preprocess screenshots"""
 
     @abstractmethod
     def process_path(self, img_path: str, output_path: str) -> None:
```

### Comparing `agentdesk-0.2.80/agentdesk/processors/grid.py` & `agentdesk-0.2.9/agentdesk/processors/grid.py`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.80/agentdesk/proxy.py` & `agentdesk-0.2.9/agentdesk/proxy.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,23 +3,19 @@
 import subprocess
 from typing import Optional, Generator
 import threading
 import socket
 import select
 import time
 import contextlib
-import logging
 
 import paramiko
 import psutil
 
-from .config import AGENTSEA_KEY_DIR
-from .util import generate_short_hash
-
-logger = logging.getLogger(__name__)
+from .util import check_port_in_use
 
 
 class SSHPortForwarding:
     """Port forwarding using SSH"""
 
     def __init__(
         self,
@@ -66,15 +62,15 @@
         return self
 
     def accept_connections(self):
         while not self.shutdown_event.is_set():
             ready, _, _ = select.select([self.server], [], [], 0.5)
             if ready and not self.shutdown_event.is_set():
                 try:
-                    client_socket, addr = self.server.accept()  # type: ignore
+                    client_socket, addr = self.server.accept()
                     print(f"Received connection from {addr}")
                     if (
                         self.shutdown_event.is_set()
                     ):  # Check again to avoid handling during shutdown
                         client_socket.close()
                         break
                     thread = threading.Thread(
@@ -86,15 +82,15 @@
                 except Exception as e:
                     if not self.shutdown_event.is_set():
                         print(f"Error accepting connections: {e}")
                     break
 
     def handle_client(self, client_socket):
         try:
-            channel = self.transport.open_channel(  # type: ignore
+            channel = self.transport.open_channel(
                 kind="direct-tcpip",
                 dest_addr=(self.remote_host, self.remote_port),
                 src_addr=client_socket.getpeername(),
             )
             if channel is None:
                 raise Exception("Channel opening failed.")
         except Exception as e:
@@ -131,202 +127,143 @@
                 try:
                     temp_sock.connect(("localhost", self.local_port))
                 except socket.error:
                     pass  # Ignore errors here as we're just trying to unblock accept()
         finally:
             # Close the server socket to ensure no new connections are accepted
             print("Closing server socket...")
-            self.server.close()  # type: ignore
+            self.server.close()
 
             # Closing the SSH client connection
             print("Closing SSH client...")
             self.client.close()
 
         print("SSH tunnel and all related resources have been closed.")
 
 
 def check_ssh_proxy_running(
     local_port: int, remote_port: int, ssh_port: int, ssh_user: str, ssh_host: str
 ) -> Optional[int]:
-    """Check if an SSH proxy process is running based on the local and remote port, SSH port, user, and host."""
+    """Check if an SSH proxy process is running with the given user, host, and port, and return its PID."""
 
-    logger.debug("checking if ssh proxy is running...")
-    # Construct a partial command pattern to match.
-    # Since we don't know the temporary key file name, we'll omit it from the search.
-    partial_command_pattern = (
-        f"-L 127.0.0.1:{local_port}:localhost:{remote_port} "
-        f"-p {ssh_port} {ssh_user}@{ssh_host}"
+    search_command = (
+        "ssh -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null "
+        f"-N -L 127.0.0.1:{local_port}:localhost:{remote_port} -p {ssh_port} {ssh_user}@{ssh_host}"
     )
-
     for proc in psutil.process_iter(["cmdline", "pid"]):
         try:
-            if "cmdline" not in proc.info:  # type: ignore
-                continue
-            cmdline: list[str] = proc.info["cmdline"]  # type: ignore
-            cmdline_str = " ".join(cmdline)
-            if partial_command_pattern in cmdline_str:
-                return proc.info["pid"]  # type: ignore
-        except Exception:
-            pass
-
+            cmdline: list[str] = proc.info["cmdline"]
+            if cmdline and search_command in " ".join(
+                cmdline
+            ):  # Check if command line matches
+                return proc.info["pid"]  # Return the PID of the process
+        except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
+            pass  # Process has terminated or we don't have permission to access its info
     return None
 
 
 def setup_ssh_proxy(
     local_port: int = 6080,
     remote_port: int = 6080,
     ssh_port: int = 22,
     ssh_user: str = "agentsea",
     ssh_host: str = "localhost",
-    ssh_key: Optional[str] = None,
-    log_error: bool = True,
 ) -> Optional[subprocess.Popen]:
     """Set up an SSH proxy if it's not already running."""
 
-    # Handle SSH key temporary file creation
-    key_filepath = None
-    if ssh_key:
-        os.makedirs(AGENTSEA_KEY_DIR, exist_ok=True)
-        os.chmod(AGENTSEA_KEY_DIR, 0o700)
-
-        key_filepath = os.path.join(
-            AGENTSEA_KEY_DIR, f"id_rsa_{generate_short_hash(ssh_key)}"
-        )
-
-        with open(key_filepath, "wb") as f:
-            f.write(ssh_key.encode())
-
-        os.chmod(key_filepath, 0o600)
+    def check_port_in_use(port: int) -> bool:
+        # Dummy implementation; replace with actual check
+        return False
+
+    if check_port_in_use(local_port):
+        print(f"Port {local_port} is already in use. Assuming SSH proxy is running.")
+        return None
 
     ssh_command = (
-        "ssh "
-        "-o StrictHostKeyChecking=no "
-        "-o UserKnownHostsFile=/dev/null "
-        "-o IdentitiesOnly=yes "
-        "-N "
-        f"-L 127.0.0.1:{local_port}:localhost:{remote_port} "
-        f"-p {ssh_port} "
+        "ssh -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null "
+        f"-N -L 127.0.0.1:{local_port}:localhost:{remote_port} -p {ssh_port} {ssh_user}@{ssh_host}"
     )
-    if ssh_key:
-        ssh_command += f"-i {key_filepath} "  # type: ignore
-    ssh_command += f"{ssh_user}@{ssh_host}"
-
-    logger.debug(f"Executing command: {ssh_command}")
+    print("Executing command: ", ssh_command)
     try:
         proxy_process = subprocess.Popen(
             ssh_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
         )
         # Give it a moment to fail, SSH should exit immediately if there's an error
-        time.sleep(0.5)
-        if proxy_process.poll() is not None:
+        time.sleep(1)
+        if proxy_process.poll() is not None:  # None means the process is still running
+            # The process has exited, indicating failure
             _, err = proxy_process.communicate()
-            if log_error:
-                logger.error(f"SSH proxy failed to start. Error: {err.decode()}")
+            print(f"SSH proxy failed to start. Error: {err.decode()}")
             return None
     except Exception as e:
-        if log_error:
-            logger.error(f"Error starting SSH proxy: {e}")
+        print(f"Error starting SSH proxy: {e}")
         raise
-    finally:
-        if key_filepath:
-            os.unlink(key_filepath)  # Clean up the temporary file
-
-    logger.debug(f"SSH proxy setup on local port {local_port}")
+    print(f"SSH proxy setup on local port {local_port}")
     return proxy_process
 
 
-def cleanup_proxy(pid: int, log_error: bool = True) -> None:
+def cleanup_proxy(pid: int) -> None:
     """Terminate the SSH proxy process with the given PID."""
 
     try:
         proc = psutil.Process(pid)
         proc.terminate()  # Terminate the process
         proc.wait()  # Wait for the process to terminate
-        logger.debug(f"SSH proxy with PID {pid} terminated.")
+        print(f"SSH proxy with PID {pid} terminated.")
     except psutil.NoSuchProcess:
-        if log_error:
-            logger.error(f"No process found with PID {pid}.")
+        print(f"No process found with PID {pid}.")
     except psutil.AccessDenied:
-        if log_error:
-            logger.error(
-                f"Access denied when trying to terminate the process with PID {pid}."
-            )
+        print(f"Access denied when trying to terminate the process with PID {pid}.")
     except Exception as e:
-        if log_error:
-            logger.error(
-                f"An error occurred while trying to terminate the process with PID {pid}: {e}"
-            )
+        print(
+            f"An error occurred while trying to terminate the process with PID {pid}: {e}"
+        )
 
 
 def ensure_ssh_proxy(
     local_port: int = 6080,
     remote_port: int = 6080,
     ssh_port: int = 22,
     ssh_user: str = "agentsea",
     ssh_host: str = "localhost",
-    ssh_key: Optional[str] = None,
-    log_error: bool = True,
 ) -> int:
     """Ensure that an SSH proxy is running and return its PID."""
-    pid = None
-    try:
-        pid = check_ssh_proxy_running(
-            local_port, remote_port, ssh_port, ssh_user, ssh_host
-        )
-    except Exception as e:
-        if log_error:
-            logger.error(f"Failed to check if proxy is running: {e}")
-        pass
+    pid = check_ssh_proxy_running(local_port, remote_port, ssh_port, ssh_user, ssh_host)
     if pid:
-        logger.debug("Existing SSH proxy found.")
+        print("Existing SSH proxy found.")
         return pid  # PID of the already running process
 
-    logger.debug("SSH proxy not found, starting one...")
-    process = setup_ssh_proxy(
-        local_port,
-        remote_port,
-        ssh_port,
-        ssh_user,
-        ssh_host,
-        ssh_key,
-        log_error=log_error,
-    )
+    print("SSH proxy not found, starting one...")
+    process = setup_ssh_proxy(local_port, remote_port, ssh_port, ssh_user, ssh_host)
     if process is None:
         # If setup_ssh_proxy returned None, it means the port is in use but no PID was found.
         # It might be necessary to refine check_ssh_proxy_running or setup_ssh_proxy to ensure consistency.
         raise RuntimeError(
             f"Failed to start SSH proxy on local port {local_port}, and no existing process was found."
         )
     time.sleep(1)  # Adjust sleep time as needed
     return process.pid  # Assuming the process started successfully
 
 
 @contextlib.contextmanager
 def ensure_managed_ssh_proxy(
-    local_port: int,
-    remote_port: int,
-    ssh_port: int,
-    ssh_user: str,
-    ssh_host: str,
-    ssh_key: Optional[str] = None,
+    local_port: int, remote_port: int, ssh_port: int, ssh_user: str, ssh_host: str
 ) -> Generator[Optional[int], None, None]:
     pid: Optional[int] = check_ssh_proxy_running(
         local_port, remote_port, ssh_port, ssh_user, ssh_host
     )
     process_started: bool = False
 
     if pid is None:
-        logger.debug("SSH proxy not found, starting one...")
-        process = setup_ssh_proxy(
-            local_port, remote_port, ssh_port, ssh_user, ssh_host, ssh_key
-        )
+        print("SSH proxy not found, starting one...")
+        process = setup_ssh_proxy(local_port, remote_port, ssh_port, ssh_user, ssh_host)
         if process is None:
             raise RuntimeError("Failed to ensure SSH proxy is running.")
         pid = process.pid
         process_started = True
 
     try:
         yield pid
     finally:
         if process_started:
-            logger.debug(f"Cleaning up newly started SSH proxy with PID {pid}...")
+            print(f"Cleaning up newly started SSH proxy with PID {pid}...")
             cleanup_proxy(pid)
```

### Comparing `agentdesk-0.2.80/agentdesk/server/models.py` & `agentdesk-0.2.9/agentdesk/server/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,21 +40,11 @@
     disk: Optional[str] = None
     memory_usage: Optional[float] = None
     cpu_usage: Optional[float] = None
     disk_usage: Optional[float] = None
     reserved_ip: Optional[bool] = None
     provider: Optional[V1ProviderData] = None
     meta: Optional[dict] = None
-    owner_id: Optional[str] = None
-    key_pair_name: Optional[str] = None
 
 
 class V1Desktops(BaseModel):
     desktops: List[V1Desktop]
-
-
-class V1SSHKey(BaseModel):
-    name: str
-    public_key: str
-    created: float
-    id: str
-    private_key: Optional[str] = None
```

### Comparing `agentdesk-0.2.80/agentdesk/util.py` & `agentdesk-0.2.9/agentdesk/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import random
 import string
 import subprocess
 from typing import Optional
 import socket
 from subprocess import CalledProcessError, DEVNULL
 from datetime import datetime
-import hashlib
-import base64
 
 from google.cloud import storage
 from PIL import Image
 
 
 def extract_file_path(uri):
     """Extracts the file path from a URI"""
@@ -44,15 +42,15 @@
     bucket_name = parsed_uri.netloc
     object_path = parsed_uri.path.lstrip("/")  # Remove leading '/' from the path
 
     return bucket_name, object_path
 
 
 def upload_image_to_gcs(
-    bucket_name: str, destination_blob_name: str, image: Image  # type: ignore
+    bucket_name: str, destination_blob_name: str, image: Image
 ) -> str:
     """
     Uploads a PIL image to Google Cloud Storage, makes it public, and returns the public URL.
 
     Args:
     bucket_name (str): Name of the GCS bucket.
     destination_blob_name (str): Destination blob name in the GCS bucket.
@@ -65,15 +63,15 @@
     storage_client = storage.Client()
 
     # Get the bucket
     bucket = storage_client.bucket(bucket_name)
 
     # Convert PIL image to bytes
     img_byte_arr = io.BytesIO()
-    image.save(img_byte_arr, format="PNG")  # type: ignore
+    image.save(img_byte_arr, format="PNG")
     img_byte_arr = img_byte_arr.getvalue()
 
     # Create a new blob and upload the image
     blob = bucket.blob(destination_blob_name)
     blob.upload_from_string(img_byte_arr, content_type="image/png")
 
     # Make the blob publicly accessible
@@ -100,15 +98,14 @@
         # Inspect the current Docker context and extract the host
         context_info = subprocess.check_output(
             f"docker context inspect {current_context}", shell=True
         ).decode()
         for line in context_info.split("\n"):
             if '"Host"' in line:
                 return line.split('"')[3]
-        return ""
     except subprocess.CalledProcessError as e:
         print(f"Error: {e.output.decode()}")
         return ""
 
 
 def find_ssh_public_key() -> Optional[str]:
     """Try to find the SSH public key in the default location."""
@@ -159,15 +156,7 @@
     return None  # No open port found
 
 
 def convert_unix_to_datetime(unix_timestamp: int) -> str:
     dt = datetime.utcfromtimestamp(unix_timestamp)
     friendly_format = dt.strftime("%Y-%m-%d %H:%M:%S")
     return friendly_format
-
-
-def generate_short_hash(data: str) -> str:
-    hash_object = hashlib.sha256(data.encode())  # You can use sha1 or sha256
-    hash_digest = hash_object.digest()
-    # Using urlsafe base64 encoding to get URL-friendly hash
-    short_hash = base64.urlsafe_b64encode(hash_digest).decode("utf-8")
-    return short_hash[:6]
```

### Comparing `agentdesk-0.2.80/agentdesk/vm/base.py` & `agentdesk-0.2.9/agentdesk/vm/ec2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,443 +1,429 @@
 from __future__ import annotations
-from abc import ABC, abstractmethod
-from typing import List, Optional, TypeVar, Generic, Dict, Any
-import uuid
-import time
-import json
-import webbrowser
-import random
-import os
+from typing import List, Optional, Dict
 import atexit
+import time
 
-import docker
-from docker.models.containers import Container
-
-from agentdesk.db.conn import WithDB
-from agentdesk.db.models import V1DesktopRecord
-from agentdesk.server.models import V1Desktop, V1ProviderData
-from agentdesk.util import (
-    get_docker_host,
-    check_command_availability,
-    check_port_in_use,
-)
+import boto3
+from boto3.resources.base import ServiceResource
+from mypy_boto3_ec2.service_resource import EC2ServiceResource, Instance as EC2Instance
+from namesgenerator import get_random_name
+from botocore.exceptions import ClientError
+import requests
+
+from .base import DesktopVM, DesktopProvider
+from .img import JAMMY
+from agentdesk.server.models import V1ProviderData
+from agentdesk.util import find_ssh_public_key, find_open_port
 from agentdesk.proxy import ensure_ssh_proxy, cleanup_proxy
-from agentdesk.key import SSHKeyPair
 
 
-UI_IMG = "us-central1-docker.pkg.dev/agentsea-dev/agentdesk/ui:634820941cbbba4b3cd51149b25d0a4c8d1a35f4"
+class EC2Provider(DesktopProvider):
+    """A VM provider using AWS EC2"""
 
+    def __init__(self, region: Optional[str] = None) -> None:
+        self.region = region
+        self.ec2: EC2ServiceResource = boto3.resource("ec2", region_name=region)
+        self.ec2_client = boto3.client("ec2", region_name=self.region)
 
-class DesktopVM(WithDB):
-    """A remote desktop VM which is accesible for AI agents"""
-
-    def __init__(
+    def create(
         self,
-        name: str,
-        addr: str,
-        id: Optional[str] = None,
-        cpu: Optional[int] = None,
-        memory: Optional[str] = None,
-        disk: Optional[str] = None,
-        pid: Optional[int] = None,
-        status: str = "running",
+        name: Optional[str] = None,
         image: Optional[str] = None,
-        provider: Optional[V1ProviderData] = None,
-        reserved_ip: bool = False,
-        requires_proxy: bool = True,
-        metadata: Optional[dict] = None,
-        ssh_port: int = 22,
-        owner_id: Optional[str] = None,
-        key_pair_name: Optional[str] = None,
-    ) -> None:
-        if not id:
-            id = str(uuid.uuid4())
-        self.name = name
-        self.addr = addr
-        self.cpu = cpu
-        self.memory = memory
-        self.disk = disk
-        self.pid = pid
-        self.id = id
-        self.created = time.time()
-        self.status = status
-        self.image = image
-        self.provider = provider
-        self.reserved_ip = reserved_ip
-        self.requires_proxy = requires_proxy
-        self.metadata = metadata
-        self.ssh_port = ssh_port
-        self.owner_id = owner_id
-        self.key_pair_name = key_pair_name
-
-        self.save()
-
-    def to_record(self) -> V1DesktopRecord:
-        provider = None
-        if self.provider:
-            provider = json.dumps(self.provider.__dict__)
-
-        metadata = None
-        if self.metadata:
-            metadata = json.dumps(self.metadata)
-
-        return V1DesktopRecord(
-            id=self.id,
-            name=self.name,
-            addr=self.addr,
-            cpu=self.cpu,
-            created=self.created,
-            memory=self.memory,
-            disk=self.disk,
-            pid=self.pid,
-            status=self.status,
-            image=self.image,
-            provider=provider,
-            reserved_ip=self.reserved_ip,
-            requires_proxy=self.requires_proxy,
-            ssh_port=self.ssh_port,
-            meta=metadata,
-            owner_id=self.owner_id,
-            key_pair_name=self.key_pair_name,
-        )
+        memory: int = 4,
+        cpu: int = 2,
+        disk: str = "30gb",
+        tags: Optional[Dict[str, str]] = None,
+        reserve_ip: bool = False,
+        ssh_key: Optional[str] = None,
+    ) -> DesktopVM:
+        if not name:
+            name = get_random_name(sep="-")
 
-    def save(self) -> None:
-        for db in self.get_db():
-            try:
-                record = self.to_record()
-                db.merge(record)
-                db.commit()
-            except Exception as e:
-                db.rollback()
-                print(f"Error saving DesktopVM: {e}")
-                raise
+        if DesktopVM.name_exists(name):
+            raise ValueError(f"VM name '{name}' already exists")
 
-    @classmethod
-    def from_record(cls, record: V1DesktopRecord) -> DesktopVM:
-        out = cls.__new__(DesktopVM)  # type: ignore
-        out.id = record.id
-        out.name = record.name
-        out.addr = record.addr
-        out.cpu = record.cpu
-        out.created = record.created
-        out.memory = record.memory
-        out.disk = record.disk
-        out.pid = record.pid
-        out.status = record.status
-        out.image = record.image
-        out.reserved_ip = record.reserved_ip
-        out.requires_proxy = record.requires_proxy
-        out.ssh_port = record.ssh_port
-        out.owner_id = record.owner_id
-        out.key_pair_name = record.key_pair_name
-        if record.provider:  # type: ignore
-            dct = json.loads(str(record.provider))
-            out.provider = V1ProviderData(**dct)
-        out.metadata = {}
-        if record.meta:  # type: ignore
-            dct = json.loads(str(record.meta))
-            out.metadata = dct
-        return out
+        if not image:
+            # Dynamically select the latest custom AMI based on a naming pattern
+            # custom_ami = self._get_latest_custom_ami()
+            # if not custom_ami:
+            #     raise ValueError("Custom AMI not found")
+            # image = custom_ami
+            image = JAMMY.ec2
+
+        ssh_key = ssh_key or find_ssh_public_key()
+
+        user_data = f"""#cloud-config
+users:
+  - name: agentsea
+    ssh_authorized_keys:
+      - {ssh_key}
+    sudo: ['ALL=(ALL) NOPASSWD:ALL']
+    groups: ['sudo']
+    shell: /bin/bash
+"""
+        instance_type = self._choose_instance_type(cpu, memory)
+
+        ssh_key_name = self._ensure_ssh_key(name, ssh_key)
+        if not ssh_key_name:
+            raise ValueError("SSH key name not provided or found")
+
+        disk_size_gib = self._convert_disk_size_to_gib(disk)
+        security_group_id = self._ensure_sg(
+            "agentdesk-default", "agentdesk default vm sg"
+        )
 
-    @classmethod
-    def load(cls, id: str) -> DesktopVM:
-        for db in cls.get_db():
-            record = db.query(V1DesktopRecord).filter(V1DesktopRecord.id == id).first()
-            if record is None:
-                raise ValueError(f"Desktop with id {id} not found")
-            return cls.from_record(record)
-        raise ValueError("no session")
+        tag_specifications = [
+            {
+                "ResourceType": "instance",
+                "Tags": [
+                    {"Key": "Name", "Value": name},
+                    {"Key": "provisioner", "Value": "agentdesk"},
+                ]
+                + [{"Key": k, "Value": v} for k, v in (tags or {}).items()],
+            }
+        ]
+
+        instances = self.ec2.create_instances(
+            ImageId=image,
+            MinCount=1,
+            MaxCount=1,
+            InstanceType=instance_type,
+            KeyName=ssh_key_name,
+            SecurityGroupIds=[security_group_id],
+            BlockDeviceMappings=[
+                {
+                    "DeviceName": "/dev/sdh",
+                    "Ebs": {"VolumeSize": disk_size_gib},
+                }
+            ],
+            TagSpecifications=tag_specifications,
+            UserData=user_data,
+        )
+        instance_id = instances[0].id
+        instances[0].wait_until_running()
 
-    @classmethod
-    def get(cls, name: str, owner_id: Optional[str] = None) -> Optional[DesktopVM]:
-        for db in cls.get_db():
-            record = (
-                db.query(V1DesktopRecord)
-                .filter_by(name=name, owner_id=owner_id)
-                .first()
+        if reserve_ip:
+            eip = boto3.client("ec2", region_name=self.region).allocate_address(
+                Domain="vpc"
             )
-            if record is None:
-                return None
-            return cls.from_record(record)
-
-    @classmethod
-    def find(cls, **kwargs) -> List[DesktopVM]:
-        """Find desktops by given keyword arguments."""
-        out = []
-        for db in cls.get_db():
-            records = db.query(V1DesktopRecord).filter_by(**kwargs).all()
-            for record in records:
-                out.append(cls.from_record(record))
-        return out
-
-    @classmethod
-    def find_v1(cls, **kwargs) -> List[V1Desktop]:
-        """Find desktops by given keyword arguments."""
-        out = []
-        for db in cls.get_db():
-            records = db.query(V1DesktopRecord).filter_by(**kwargs).all()
-            for record in records:
-                out.append(cls.from_record(record).to_v1_schema())
-        return out
-
-    @classmethod
-    def delete(cls, id: str) -> None:
-        for db in cls.get_db():
-            record = db.query(V1DesktopRecord).filter(V1DesktopRecord.id == id).first()
-            if record is None:
-                raise ValueError(f"Desktop with id {id} not found")
-            db.delete(record)
-            db.commit()
-
-    @classmethod
-    def name_exists(cls, name: str, owner_id: Optional[str] = None) -> bool:
-        for db in cls.get_db():
-            record = (
-                db.query(V1DesktopRecord)
-                .filter_by(name=name, owner_id=owner_id)
-                .first()
+            boto3.client("ec2", region_name=self.region).associate_address(
+                InstanceId=instance_id, AllocationId=eip["AllocationId"]
             )
-            if record is None:
-                return False
 
-            return True
+        instance = self.ec2.Instance(instance_id)
+        public_ip = instance.public_ip_address
 
-        raise ValueError("no session")
+        # wait till agentd is ready
+        self._wait_till_ready(public_ip)
 
-    def remove(self) -> None:
-        for db in self.get_db():
-            record = (
-                db.query(V1DesktopRecord).filter(V1DesktopRecord.id == self.id).first()
-            )
-            if record is None:
-                raise ValueError(f"Desktop with id {self.id} not found")
-            db.delete(record)
-            db.commit()
-
-    def to_v1_schema(self) -> V1Desktop:
-        return V1Desktop(
-            id=self.id,
-            name=self.name,
-            addr=self.addr,
-            status=self.status,
-            created=self.created,
-            memory=self.memory,  # type: ignore
-            cpu=self.cpu,
-            disk=self.disk,
-            image=self.image,
-            reserved_ip=self.reserved_ip,
-            provider=self.provider,
-            meta=self.metadata,
-            owner_id=self.owner_id,
-            key_pair_name=self.key_pair_name,
+        desktop = DesktopVM(
+            name=name,
+            id=instance_id,
+            addr=public_ip,
+            cpu=cpu,
+            memory=memory,
+            disk=disk,
+            image=image,
+            provider=self.to_data(),
+            requires_proxy=True,
         )
 
-    def view(self, background: bool = False) -> None:
-        """Opens the desktop in a browser window"""
+        print(f"\nsuccessfully created desktop '{name}'")
+        return desktop
 
-        if self.requires_proxy:
-            keys = SSHKeyPair.find(name=self.key_pair_name)
-            if not keys:
-                raise ValueError(
-                    f"No key pair found with name {self.key_pair_name} and is required for this desktop"
+    def _wait_till_ready(
+        self, addr: str, local_agentd_port: Optional[int] = None
+    ) -> None:
+        if not local_agentd_port:
+            local_agentd_port = find_open_port(8000, 9000)
+        print("waiting for desktop to be ready...")
+
+        ready = False
+        while not ready:
+            print("waiting for desktop to be ready...")
+            time.sleep(3)
+            try:
+                print("ensuring up ssh proxy...")
+                pid = ensure_ssh_proxy(
+                    local_port=local_agentd_port, remote_port=8000, ssh_host=addr
                 )
-            key_pair = keys[0]
+                atexit.register(cleanup_proxy, pid)
 
-            if check_port_in_use(6080):
-                raise ValueError(
-                    "Port 6080 is already in use, UI requires this port"
-                )  # TODO: remove this restriction
-            proxy_pid = ensure_ssh_proxy(
-                6080,
-                6080,
-                self.ssh_port,
-                "agentsea",
-                self.addr,
-                key_pair.decrypt_private_key(key_pair.private_key),
-            )
-            atexit.register(cleanup_proxy, proxy_pid)
-
-        check_command_availability("docker")
+                print("calling agentd...")
+                response = requests.get(f"http://localhost:{local_agentd_port}/health")
+                print("agentd response: ", response)
+                if response.status_code == 200:
+                    ready = True
+                cleanup_proxy(pid)
+                atexit.unregister(cleanup_proxy)
+            except:
+                try:
+                    cleanup_proxy(pid)
+                except Exception:
+                    pass
+
+        print("cleaning up tunnel")
+        cleanup_proxy(pid)
+        atexit.unregister(cleanup_proxy)
+
+    def _ensure_sg(self, name: str, description: str) -> str:
+        # Attempt to find the default VPC
+        vpcs = self.ec2_client.describe_vpcs(
+            Filters=[{"Name": "isDefault", "Values": ["true"]}]
+        )
+        if not vpcs["Vpcs"]:
+            raise Exception("No default VPC found in this region.")
+        default_vpc_id = vpcs["Vpcs"][0]["VpcId"]
 
-        host = get_docker_host()
-        os.environ["DOCKER_HOST"] = host
-        client = docker.from_env()
-
-        host_port = None
-        ui_container: Optional[Container] = None
-
-        for container in client.containers.list():
-            if container.image.tags[0] == UI_IMG:  # type: ignore
-                print("found running UI container")
-                # Retrieve the host port for the existing container
-                host_port = container.attrs["NetworkSettings"]["Ports"]["3000/tcp"][0][  # type: ignore
-                    "HostPort"
+        # Check if the security group already exists
+        try:
+            security_groups = self.ec2_client.describe_security_groups(
+                Filters=[
+                    {"Name": "group-name", "Values": [name]},
+                    {"Name": "vpc-id", "Values": [default_vpc_id]},
                 ]
-                ui_container = container  # type: ignore
-                break
-
-        if not ui_container:
-            print("creating UI container...")
-            host_port = random.randint(1024, 65535)
-            ui_container = client.containers.run(  # type: ignore
-                UI_IMG, ports={"3000/tcp": host_port}, detach=True
             )
-            print("waiting for UI container to start...")
-            time.sleep(10)
-
-        webbrowser.open(f"http://localhost:{host_port}")
-
-        if background:
-            return
-
-        def onexit():
-            nonlocal proxy_pid
-            print("Cleaning up resources...")
+            if security_groups["SecurityGroups"]:
+                # Security group already exists
+                return security_groups["SecurityGroups"][0]["GroupId"]
+        except ClientError as e:
+            print(f"Error checking for existing security group: {e}")
 
-            # Check if the UI container still exists and stop/remove it if so
-            if ui_container:
-                try:
-                    container_status = client.containers.get(ui_container.id).status  # type: ignore
-                    if container_status in ["running", "paused"]:
-                        print("stopping UI container...")
-                        ui_container.stop()
-                        print("removing UI container...")
-                        ui_container.remove()
-                except docker.errors.NotFound:  # type: ignore
-                    print("UI container already stopped/removed.")
-
-            # Stop the SSH proxy if required and not already stopped
-            if self.requires_proxy and proxy_pid:
-                try:
-                    print("stopping ssh proxy...")
-                    cleanup_proxy(proxy_pid)
-                except Exception as e:
-                    print(f"Error stopping SSH proxy: {e}")
-                finally:
-                    proxy_pid = None  # Ensure we don't try to stop it again
-
-        atexit.register(onexit)
+        # Security group does not exist, create it
         try:
-            while True:
-                print(f"proxying desktop vnc '{self.name}' to localhost:6080...")
-                time.sleep(20)
-        except KeyboardInterrupt:
-            print("Keyboard interrupt received, exiting...")
-            onexit()
-
+            response = self.ec2_client.create_security_group(
+                GroupName=name, Description=description, VpcId=default_vpc_id
+            )
+            security_group_id = response["GroupId"]
 
-DP = TypeVar("DP", bound="DesktopProvider")
+            # Add inbound rules
+            self.ec2_client.authorize_security_group_ingress(
+                GroupId=security_group_id,
+                IpPermissions=[
+                    {
+                        "IpProtocol": "tcp",
+                        "FromPort": 22,
+                        "ToPort": 22,
+                        "IpRanges": [{"CidrIp": "0.0.0.0/0"}],
+                    },
+                ],
+            )
+            return security_group_id
+        except ClientError as e:
+            raise Exception(f"Failed to create security group: {e}")
 
+    def _convert_disk_size_to_gib(self, disk_size: str) -> int:
+        """
+        Converts a disk size specification string with units (e.g., "30gb", "1tb")
+        to an integer representing the disk size in GiB.
 
-class DesktopProvider(ABC, Generic[DP]):
-    """A provider of desktop virtual machines"""
+        :param disk_size: Disk size string with units.
+        :return: Disk size in GiB as an integer.
+        """
+        unit = disk_size[-2:].lower()
+        size = int(disk_size[:-2])
+        if unit == "gb":
+            return size  # Assuming input in GiB, direct conversion for simplicity
+        elif unit == "tb":
+            return size * 1024  # Convert TB to GiB
+        else:
+            raise ValueError(f"Unsupported disk size unit: {unit}")
 
-    @abstractmethod
-    def create(
-        self,
-        name: Optional[str] = None,
-        image: Optional[str] = None,
-        memory: int = 4,
-        cpu: int = 2,
-        disk: str = "30gb",
-        tags: Optional[Dict[str, str]] = None,
-        reserve_ip: bool = False,
-        ssh_key_pair: Optional[str] = None,
-        owner_id: Optional[str] = None,
-        metadata: Optional[Dict[str, Any]] = None,
-    ) -> DesktopVM:
-        """Create a Desktop
+    def _choose_instance_type(self, cpu: int, memory: int) -> str:
+        """
+        Choose an EC2 instance type based on CPU and memory requirements.
+        """
+        # This is a simple mapping. Update it according to your needs.
+        if cpu <= 2:
+            if memory <= 4:
+                return "t2.micro"
+            elif memory <= 8:
+                return "t2.small"
+            else:
+                return "t2.medium"
+        elif cpu <= 4:
+            if memory <= 16:
+                return "t2.large"
+            else:
+                return "t2.xlarge"
+        else:
+            # Default to a larger instance for higher requirements
+            return "t2.2xlarge"
 
-        Args:
-            name (str, optional): Name of the VM. Defaults to random generation.
-            image (str, optional): Image of the VM. Defaults to Ubuntu Jammy.
-            memory (int): Memory allotment. Defaults to 4gb.
-            cpu (int): CPU allotment. Defaults to 2.
-            disk (str): Disk allotment. Defaults to 30gb.
-            tags (List[str], optional): Tags to apply to the VM. Defaults to None.
-            reserve_ip (bool, optional): Reserve an IP address. Defaults to False.
-            ssh_key_pair (str, optional): SSH key pair name to use. Defaults to None.
-            owner_id (str, optional): Owner of the VM. Defaults to None.
-            metadata (Dict[str, Any], optional): Metadata to apply to the VM. Defaults to None.
+    def _ensure_ssh_key(self, key_name: str, public_key_material: str) -> str:
+        """
+        Uploads an SSH public key to AWS EC2, if it does not already exist.
+        """
+        ec2_client = boto3.client("ec2", region_name=self.region)
+        try:
+            ec2_client.describe_key_pairs(KeyNames=[key_name])
+            print(f"Key pair '{key_name}' already exists. Skipping import.")
+            return key_name
+        except ec2_client.exceptions.ClientError as e:
+            if "InvalidKeyPair.NotFound" in str(e):
+                ec2_client.import_key_pair(
+                    KeyName=key_name, PublicKeyMaterial=public_key_material
+                )
+                print(f"Key pair '{key_name}' successfully imported.")
+                return key_name
+            raise
 
-        Returns:
-            VM: A VM
+    def _get_latest_custom_ami(self) -> Optional[str]:
         """
-        pass
+        Find the latest custom AMI based on a specific naming pattern.
 
-    @abstractmethod
-    def delete(self, name: str, owner_id: Optional[str] = None) -> None:
-        """Delete a VM
-
-        Args:
-            name (str): Name of the VM
-            owner_id (str, optional): Owner of the VM. Defaults to None
+        Returns:
+            The AMI ID of the latest custom AMI if found, otherwise None.
         """
-        pass
+        ec2_client = boto3.client("ec2", region_name=self.region)
+        filters = [
+            {"Name": "name", "Values": ["agentd-ubuntu-22.04-*"]},
+            {
+                "Name": "owner-id",
+                "Values": ["596381348884"],
+            },  # Ubuntu's owner ID, adjust if your AMI has a different owner
+        ]
+        # Describe images with the specified filters
+        response = ec2_client.describe_images(Filters=filters)
+
+        images = response.get("Images", [])
+        if not images:
+            return None
+
+        # Sort images by creation date in descending order
+        sorted_images = sorted(images, key=lambda x: x["CreationDate"], reverse=True)
+
+        # Return the AMI ID of the latest image
+        latest_ami = sorted_images[0]["ImageId"]
+        return latest_ami
+
+    def _release_eip(self, instance: EC2Instance) -> None:
+        # Assuming you have tagged your EIPs or have a way to associate them with instances
+        filters = [{"Name": "instance-id", "Values": [instance.id]}]
+        addresses = self.ec2_client.describe_addresses(Filters=filters)
+        for address in addresses.get("Addresses", []):
+            self.ec2_client.release_address(AllocationId=address["AllocationId"])
+            print(f"Released EIP: {address['PublicIp']}")
 
-    @abstractmethod
-    def start(
-        self,
-        name: str,
-        private_ssh_key: Optional[str] = None,
-        owner_id: Optional[str] = None,
-    ) -> None:
-        """Start a VM
+    def _delete_ssh_key(self, name: str) -> None:
 
-        Args:
-            name (str): Name of the VM
-            private_ssh_key (str, optional): SSH key to use. Defaults to use ~/.ssh/id_rsa.
-        """
-        pass
+        try:
+            self.ec2_client.delete_key_pair(KeyName=name)
+            print(f"Deleted SSH key: {name}")
+        except self.ec2_client.exceptions.ClientError as e:
+            print(f"Failed to delete SSH key {name}: {e}")
+
+    def delete(self, name: str) -> None:
+        instance = self._get_instance_by_name(name)
+        if instance:
+            # Release EIP if reserved for the instance
+            # self._release_eip(instance) # TODO
+
+            # Terminate the instance
+            instance.terminate()
+            instance.wait_until_terminated()
+            print("Remote instance terminated")
+
+            # TODO: for now we always create the key
+            self._delete_ssh_key(name)
+
+            # Remove the desktop VM from local state
+            desk = DesktopVM.find(name)
+            if not desk:
+                raise ValueError(
+                    f"Desktop '{name}' not found in state, but deleted from provider"
+                )
+            desk.remove()
 
-    @abstractmethod
-    def stop(self, name: str, owner_id: Optional[str] = None) -> None:
-        """Stop a VM
-
-        Args:
-            name (str): Name of the VM
-            owner_id (str, optional): Owner of the VM. Defaults to None
-        """
-        pass
+    def start(self, name: str) -> None:
+        desk = DesktopVM.find(name)
+        if not desk:
+            raise ValueError(f"Desktop {name} not found")
+        instance = self._get_instance_by_name(name)
+        if instance:
+            instance.start()
+            instance.wait_until_running()
+
+        public_ip = instance.public_ip_address
+        self._wait_till_ready(public_ip)
+        desk.addr = public_ip
+        desk.status = "running"
+        desk.save()
+
+    def stop(self, name: str) -> None:
+        desk = DesktopVM.find(name)
+        if not desk:
+            raise ValueError(f"Desktop {name} not found")
+        instance = self._get_instance_by_name(name)
+        if instance:
+            instance.stop()
+            instance.wait_until_stopped()
+        desk.status = "stopped"
+        desk.save()
+
+    def list_remote(self) -> List[DesktopVM]:
+        instances = self.ec2.instances.filter(
+            Filters=[{"Name": "instance-state-name", "Values": ["running", "stopped"]}]
+        )
+        desktops = []
+        for instance in instances:
+            desktops.append(DesktopVM.load(instance.id))
+        return desktops
 
-    @abstractmethod
     def list(self) -> List[DesktopVM]:
-        """List VMs
+        return DesktopVM.list()
 
-        Returns:
-            List[VM]: A list of VMs
-        """
-        pass
+    def get_remote(self, name: str) -> Optional[DesktopVM]:
+        instance = self._get_instance_by_name(name)
+        return DesktopVM.load(instance.id)
 
-    @abstractmethod
-    def get(self, name: str, owner_id: Optional[str] = None) -> Optional[DesktopVM]:
-        """Get a VM
-
-        Args:
-            name (str): Name of the VM
-            owner_id (str, optional): Owner of the VM. Defaults to None
-        """
-        pass
+    def get(self, name: str) -> Optional[DesktopVM]:
+        return DesktopVM.find(name)
 
-    @abstractmethod
     def to_data(self) -> V1ProviderData:
-        """Convert to a ProviderData object
-
-        Returns:
-            ProviderData: ProviderData object
-        """
-        pass
+        provider = V1ProviderData(type="ec2")
+        if self.region:
+            provider.args = {"region": self.region}
+        return provider
 
     @classmethod
-    @abstractmethod
-    def from_data(cls, data: V1ProviderData) -> DP:
-        """From provider data
+    def from_data(cls, data: V1ProviderData) -> EC2Provider:
+        if data.args and "region" in data.args:
+            return cls(data.args["region"])
+        return cls()
+
+    def _get_instance_by_name(self, name: str) -> Optional[EC2Instance]:
+        instances = self.ec2.instances.filter(
+            Filters=[{"Name": "tag:Name", "Values": [name]}]
+        )
+        return next((instance for instance in instances), None)
 
-        Args:
-            data (ProviderData): Provider data
-        """
-        pass
+    def _get_root_device_size(self, instance: EC2Instance) -> str:
+        for device in instance.block_device_mappings:
+            if device.get("DeviceName") == instance.root_device_name:
+                volume_id = device.get("Ebs", {}).get("VolumeId")
+                if volume_id:
+                    volume = boto3.resource("ec2").Volume(volume_id)
+                    return f"{volume.size}gb"
+        return "unknown"
 
-    @abstractmethod
     def refresh(self, log: bool = True) -> None:
         """Refresh state"""
-        pass
+        for vm in DesktopVM.list():
+            if vm.provider.type != "ec2":
+                continue
+
+            instance = self._get_instance_by_name(vm.name)
+            if not instance:
+                if log:
+                    print(f"removing vm '{vm.name}' from state")
+                vm.remove()
+                return
+
+            if not vm.reserved_ip:
+                if vm.addr != instance.public_ip_address:
+                    if log:
+                        print(f"updating vm '{vm.name}' state")
+                    vm.addr = instance.public_ip_address
+                    vm.save()
+                    return
```

### Comparing `agentdesk-0.2.80/agentdesk/vm/load.py` & `agentdesk-0.2.9/agentdesk/vm/load.py`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.80/pyproject.toml` & `agentdesk-0.2.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,53 @@
 [tool.poetry]
 name = "agentdesk"
-version = "0.2.80"
+version = "0.2.9"
 description = "A desktop for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
-license = "MIT"
+license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "agentdesk"}]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<4.0"
+python = ">=3.10,<3.12"
 pillow = "^10.2.0"
 requests = "^2.31.0"
 fastapi = {extras = ["all"], version = "^0.109.0"}
 sqlalchemy = "^2.0.25"
 psycopg2-binary = "^2.9.9"
 psutil = "^5.9.8"
 docker = "^7.0.0"
 pycdlib = "^1.14.0"
 namesgenerator = "^0.3"
 paramiko = "^3.4.0"
 typer = "^0.9.0"
 tabulate = "^0.9.0"
 tqdm = "^4.66.2"
 tenacity = "^8.2.3"
-google-cloud-storage = "^2.14.0"
-google-cloud-compute = "^1.15.0"
-google-cloud-container = "^2.38.0"
-boto3 = "^1.34.28"
-boto3-stubs = {extras = ["ec2"], version = "^1.34.28"}
-mypy-boto3-ec2 = "^1.34.52"
-toolfuse = "^0.1.13"
-devicebay = "^0.1.24"
+opentool-ai = "^0.1.7"
 
 
 [tool.poetry.group.gcp.dependencies]
 google-cloud-compute = "^1.15.0"
 google-cloud-container = "^2.38.0"
+google-cloud-storage = "^2.14.0"
 
 
 [tool.poetry.group.aws.dependencies]
 boto3 = "^1.34.28"
 boto3-stubs = {extras = ["ec2"], version = "^1.34.28"}
 mypy-boto3-ec2 = "^1.34.52"
 
 
 [tool.poetry.group.demo.dependencies]
 openai = "^1.12.0"
 
 [tool.poetry.scripts]
 agentdesk = "agentdesk.cli.main:app"
 agentd = "agentdesk.cli.main:app"
-build-docs = "scripts.build_docs:main"
-lint = "scripts.lint:main"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.0"
-sphinx = "^7.2.6"
-sphinx-rtd-theme = "^2.0.0"
-recommonmark = "^0.7.1"
-flake8 = "^7.0.0"
-black = "^24.2.0"
-pytest = "^8.0.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `agentdesk-0.2.80/PKG-INFO` & `agentdesk-0.2.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 Metadata-Version: 2.1
 Name: agentdesk
-Version: 0.2.80
+Version: 0.2.9
 Summary: A desktop for AI agents
-License: MIT
+License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.10,<3.12
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: boto3 (>=1.34.28,<2.0.0)
-Requires-Dist: boto3-stubs[ec2] (>=1.34.28,<2.0.0)
-Requires-Dist: devicebay (>=0.1.24,<0.2.0)
 Requires-Dist: docker (>=7.0.0,<8.0.0)
 Requires-Dist: fastapi[all] (>=0.109.0,<0.110.0)
-Requires-Dist: google-cloud-compute (>=1.15.0,<2.0.0)
-Requires-Dist: google-cloud-container (>=2.38.0,<3.0.0)
-Requires-Dist: google-cloud-storage (>=2.14.0,<3.0.0)
-Requires-Dist: mypy-boto3-ec2 (>=1.34.52,<2.0.0)
 Requires-Dist: namesgenerator (>=0.3,<0.4)
+Requires-Dist: opentool-ai (>=0.1.7,<0.2.0)
 Requires-Dist: paramiko (>=3.4.0,<4.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
 Requires-Dist: pycdlib (>=1.14.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.25,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
-Requires-Dist: toolfuse (>=0.1.13,<0.2.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
@@ -58,15 +51,15 @@
   <br>
 </p>
 
 Agentdesk provides full featured desktop environments which can be programatically controlled by AI agents. Spin them up locally or in the cloud.
 
 ▶ Built on [agentd](https://github.com/agentsea/agentd) a runtime daemon which exposes a REST API for interacting with the desktop.
 
-▶ Implements the [DeviceBay Protocol](https://github.com/agentsea/devicebay)
+▶ Implements the [ToolsV1 protocol](https://github.com/agentsea/opentool)
 
 ## Installation
 
 ```
 pip install agentdesk
 ```
 
@@ -137,15 +130,15 @@
 ```
 
 _\*requires docker_
 
 ### List desktops
 
 ```python
-Desktop.find()
+Desktop.list()
 ```
 
 ```bash
 $ agentdesk get
 ```
 
 ### Delete a desktop
```

#### html2text {}

```diff
@@ -1,51 +1,46 @@
-Metadata-Version: 2.1 Name: agentdesk Version: 0.2.80 Summary: A desktop for AI
-agents License: MIT Author: Patrick Barker Author-email:
-patrickbarkerco@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
-OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Metadata-Version: 2.1 Name: agentdesk Version: 0.2.9 Summary: A desktop for AI
+agents License: Apache 2.0 Author: Patrick Barker Author-email:
+patrickbarkerco@gmail.com Requires-Python: >=3.10,<3.12 Classifier: License ::
+Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: boto3 (>=1.34.28,<2.0.0) Requires-
-Dist: boto3-stubs[ec2] (>=1.34.28,<2.0.0) Requires-Dist: devicebay
-(>=0.1.24,<0.2.0) Requires-Dist: docker (>=7.0.0,<8.0.0) Requires-Dist: fastapi
-[all] (>=0.109.0,<0.110.0) Requires-Dist: google-cloud-compute
-(>=1.15.0,<2.0.0) Requires-Dist: google-cloud-container (>=2.38.0,<3.0.0)
-Requires-Dist: google-cloud-storage (>=2.14.0,<3.0.0) Requires-Dist: mypy-
-boto3-ec2 (>=1.34.52,<2.0.0) Requires-Dist: namesgenerator (>=0.3,<0.4)
-Requires-Dist: paramiko (>=3.4.0,<4.0.0) Requires-Dist: pillow
-(>=10.2.0,<11.0.0) Requires-Dist: psutil (>=5.9.8,<6.0.0) Requires-Dist:
-psycopg2-binary (>=2.9.9,<3.0.0) Requires-Dist: pycdlib (>=1.14.0,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: sqlalchemy
-(>=2.0.25,<3.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist:
-tenacity (>=8.2.3,<9.0.0) Requires-Dist: toolfuse (>=0.1.13,<0.2.0) Requires-
+Language :: Python :: 3.11 Requires-Dist: docker (>=7.0.0,<8.0.0) Requires-
+Dist: fastapi[all] (>=0.109.0,<0.110.0) Requires-Dist: namesgenerator
+(>=0.3,<0.4) Requires-Dist: opentool-ai (>=0.1.7,<0.2.0) Requires-Dist:
+paramiko (>=3.4.0,<4.0.0) Requires-Dist: pillow (>=10.2.0,<11.0.0) Requires-
+Dist: psutil (>=5.9.8,<6.0.0) Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
+Requires-Dist: pycdlib (>=1.14.0,<2.0.0) Requires-Dist: requests
+(>=2.31.0,<3.0.0) Requires-Dist: sqlalchemy (>=2.0.25,<3.0.0) Requires-Dist:
+tabulate (>=0.9.0,<0.10.0) Requires-Dist: tenacity (>=8.2.3,<9.0.0) Requires-
 Dist: tqdm (>=4.66.2,<5.0.0) Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
                             ************ AAggeennttDDeesskk ************
                      Desktops for AI agents   :computer:
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                   _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
 Agentdesk provides full featured desktop environments which can be
 programatically controlled by AI agents. Spin them up locally or in the cloud.
 â¶ Built on [agentd](https://github.com/agentsea/agentd) a runtime daemon
 which exposes a REST API for interacting with the desktop. â¶ Implements the
-[DeviceBay Protocol](https://github.com/agentsea/devicebay) ## Installation ```
+[ToolsV1 protocol](https://github.com/agentsea/opentool) ## Installation ```
 pip install agentdesk ``` ## Quick Start ```python from agentdesk import
 Desktop # Create a local VM desktop = Desktop.local() # Launch the UI for it
 desktop.view(background=True) # Open a browser to Google desktop.open_url
 ("https://google.com") # Take actions on the desktop desktop.move_mouse(500,
 500) desktop.click() img = desktop.take_screenshot() ``` ## Usage ### Create a
 local desktop ```python from agentdesk import Desktop desktop = Desktop.local()
 ``` ```bash $ agentdesk create --provider qemu ``` _\*requires [qemu](https://
 www.qemu.org/)_ ### Create a remote desktop on GCE ```python desktop =
 Desktop.gce() ``` ```bash $ agentdesk create --provider gce ``` ### Create a
 remote desktop on EC2 ```python desktop = Desktop.ec2() ``` ```bash $ agentdesk
 create --provider ec2 ``` ### View the desktop in the UI ```python desktop.view
 () ``` ```bash $ agentdesk view old_mckinny ``` _\*requires docker_ ### List
-desktops ```python Desktop.find() ``` ```bash $ agentdesk get ``` ### Delete a
+desktops ```python Desktop.list() ``` ```bash $ agentdesk get ``` ### Delete a
 desktop ```python Desktop.delete("old_mckinny") ``` ```bash $ agentdesk delete
 old_mckinny ``` ### Use the desktop ```python desktop.open_url("https://
 google.com") coords = desktop.mouse_coordinates() desktop.move_mouse(500, 500)
 desktop.click() desktop.type_text("What kind of ducks are in Canada?")
 desktop.press_key('Enter') desktop.scroll() img = desktop.take_screenshot() ```
 ### Processors Process images to make them more accessible to LMMs. #### Grid
 Add a coordinate grid on top of the image ```python from agentdesk.processors
```

