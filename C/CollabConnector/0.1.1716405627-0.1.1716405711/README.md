# Comparing `tmp/collabconnector-0.1.1716405627.tar.gz` & `tmp/collabconnector-0.1.1716405711.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collabconnector-0.1.1716405627.tar", last modified: Wed May 22 19:20:31 2024, max compression
+gzip compressed data, was "collabconnector-0.1.1716405711.tar", last modified: Wed May 22 19:21:55 2024, max compression
```

## Comparing `collabconnector-0.1.1716405627.tar` & `collabconnector-0.1.1716405711.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.306537 collabconnector-0.1.1716405627/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 collabconnector-0.1.1716405627/LICENSE
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-22 19:20:31.306400 collabconnector-0.1.1716405627/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 collabconnector-0.1.1716405627/README.md
--rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 collabconnector-0.1.1716405627/pyproject.toml
--rw-r--r--   0 jonsnipes   (501) staff       (20)      965 2024-05-22 19:20:31.307058 collabconnector-0.1.1716405627/setup.cfg
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.020774 collabconnector-0.1.1716405627/src/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.032740 collabconnector-0.1.1716405627/src/CollabConnector/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.036346 collabconnector-0.1.1716405627/src/CollabConnector/CER/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2586 2023-07-06 17:16:08.000000 collabconnector-0.1.1716405627/src/CollabConnector/CER/CER.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CER/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.038169 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.039857 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AST/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    10786 2023-08-29 12:33:53.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AST/AST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AST/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.043437 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   357792 2023-08-30 01:25:13.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/AXL.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2023-08-29 16:07:10.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.025198 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.050972 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/10.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.069289 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/10.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.090873 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/11.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.112152 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/11.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.134274 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.175750 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.184572 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/14.0/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.206044 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/7.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.212830 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/8.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.230363 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/8.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.243990 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/9.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.260478 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/9.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.272157 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/CDR/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    20752 2023-08-03 20:55:28.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/CDR/CDR.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/CDR/CDROnDemand.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/CDR/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)    13200 2023-08-30 01:25:13.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/CUCM.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.273784 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/DIME/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/DIME/DIME.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/DIME/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.275428 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/Logs/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/Logs/Logs.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/Logs/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.277545 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/Phone/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    30953 2023-07-06 17:17:27.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/Phone/Phone.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/Phone/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.279199 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/Risport/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/Risport/Risport.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/Risport/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.281095 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/Serviceability/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/Serviceability/Serviceability.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/Serviceability/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.282685 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/UDS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2102 2023-07-06 17:15:02.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/UDS/UDS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/UDS/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCM/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.284664 collabconnector-0.1.1716405627/src/CollabConnector/CUCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    15091 2023-08-29 12:24:59.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCX/CUCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/CUCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.286315 collabconnector-0.1.1716405627/src/CollabConnector/Expressway/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3529 2023-07-06 17:16:00.000000 collabconnector-0.1.1716405627/src/CollabConnector/Expressway/Expressway.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 collabconnector-0.1.1716405627/src/CollabConnector/Expressway/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.288727 collabconnector-0.1.1716405627/src/CollabConnector/IOS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    22137 2023-08-15 19:43:30.000000 collabconnector-0.1.1716405627/src/CollabConnector/IOS/IOS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 collabconnector-0.1.1716405627/src/CollabConnector/IOS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.290511 collabconnector-0.1.1716405627/src/CollabConnector/PAWS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/PAWS/PAWS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/PAWS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.292104 collabconnector-0.1.1716405627/src/CollabConnector/UCCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     8554 2023-07-06 17:17:13.000000 collabconnector-0.1.1716405627/src/CollabConnector/UCCX/UCCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/UCCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.293775 collabconnector-0.1.1716405627/src/CollabConnector/Webex/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.296584 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Connect/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5205 2023-09-29 22:42:01.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Connect/REST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2942 2023-09-29 22:55:16.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Connect/TXT.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1108 2024-05-09 12:42:58.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Connect/WhatsApp.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      224 2024-05-09 12:43:27.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Connect/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.298169 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Consent/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5425 2023-09-29 23:50:27.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Consent/REST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1011 2023-09-29 23:52:18.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Consent/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.299567 collabconnector-0.1.1716405627/src/CollabConnector/Webex/ContactCenter/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    16955 2024-05-22 19:17:01.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/ContactCenter/ContactCenter.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       64 2024-03-08 13:04:39.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/ContactCenter/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.303710 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Engage/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     8235 2023-11-02 16:46:15.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Engage/Chat.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5439 2023-09-29 14:23:57.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Engage/REST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1354 2023-09-29 14:23:57.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Engage/Team.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     4817 2023-11-02 16:51:10.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Engage/User.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      338 2023-09-29 14:23:57.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Engage/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.304996 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Phone/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3412 2024-03-08 12:53:56.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Phone/Phone.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Phone/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)    17743 2024-05-09 19:53:28.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/Webex.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2024-03-08 13:05:25.000000 collabconnector-0.1.1716405627/src/CollabConnector/Webex/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:05:58.000000 collabconnector-0.1.1716405627/src/CollabConnector/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:20:31.305806 collabconnector-0.1.1716405627/src/CollabConnector.egg-info/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-22 19:20:30.000000 collabconnector-0.1.1716405627/src/CollabConnector.egg-info/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     4467 2024-05-22 19:20:31.000000 collabconnector-0.1.1716405627/src/CollabConnector.egg-info/SOURCES.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2024-05-22 19:20:30.000000 collabconnector-0.1.1716405627/src/CollabConnector.egg-info/dependency_links.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       77 2024-05-22 19:20:30.000000 collabconnector-0.1.1716405627/src/CollabConnector.egg-info/requires.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2024-05-22 19:20:30.000000 collabconnector-0.1.1716405627/src/CollabConnector.egg-info/top_level.txt
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.615341 collabconnector-0.1.1716405711/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 collabconnector-0.1.1716405711/LICENSE
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-22 19:21:55.615184 collabconnector-0.1.1716405711/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 collabconnector-0.1.1716405711/README.md
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 collabconnector-0.1.1716405711/pyproject.toml
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      965 2024-05-22 19:21:55.616035 collabconnector-0.1.1716405711/setup.cfg
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.351543 collabconnector-0.1.1716405711/src/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.361392 collabconnector-0.1.1716405711/src/CollabConnector/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.364511 collabconnector-0.1.1716405711/src/CollabConnector/CER/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2586 2023-07-06 17:16:08.000000 collabconnector-0.1.1716405711/src/CollabConnector/CER/CER.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CER/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.366476 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.368257 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AST/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    10786 2023-08-29 12:33:53.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AST/AST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AST/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.371720 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   357792 2023-08-30 01:25:13.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/AXL.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2023-08-29 16:07:10.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.355258 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.378831 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/10.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.398745 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/10.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.417236 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/11.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.436572 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/11.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.455449 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.486352 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.495578 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/14.0/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.513452 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/7.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.519970 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/8.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.534703 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/8.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.552334 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/9.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.569535 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/9.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.581265 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/CDR/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    20752 2023-08-03 20:55:28.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/CDR/CDR.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/CDR/CDROnDemand.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/CDR/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    13200 2023-08-30 01:25:13.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/CUCM.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.582854 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/DIME/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/DIME/DIME.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/DIME/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.584387 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/Logs/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/Logs/Logs.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/Logs/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.587165 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/Phone/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    30953 2023-07-06 17:17:27.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/Phone/Phone.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/Phone/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.589254 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/Risport/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/Risport/Risport.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/Risport/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.591344 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/Serviceability/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/Serviceability/Serviceability.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/Serviceability/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.593210 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/UDS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2102 2023-07-06 17:15:02.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/UDS/UDS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/UDS/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCM/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.594833 collabconnector-0.1.1716405711/src/CollabConnector/CUCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    15091 2023-08-29 12:24:59.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCX/CUCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/CUCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.596840 collabconnector-0.1.1716405711/src/CollabConnector/Expressway/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3529 2023-07-06 17:16:00.000000 collabconnector-0.1.1716405711/src/CollabConnector/Expressway/Expressway.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 collabconnector-0.1.1716405711/src/CollabConnector/Expressway/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.599040 collabconnector-0.1.1716405711/src/CollabConnector/IOS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    22137 2023-08-15 19:43:30.000000 collabconnector-0.1.1716405711/src/CollabConnector/IOS/IOS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 collabconnector-0.1.1716405711/src/CollabConnector/IOS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.600714 collabconnector-0.1.1716405711/src/CollabConnector/PAWS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/PAWS/PAWS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/PAWS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.602134 collabconnector-0.1.1716405711/src/CollabConnector/UCCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     8554 2023-07-06 17:17:13.000000 collabconnector-0.1.1716405711/src/CollabConnector/UCCX/UCCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/UCCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.603841 collabconnector-0.1.1716405711/src/CollabConnector/Webex/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.606578 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Connect/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5205 2023-09-29 22:42:01.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Connect/REST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2942 2023-09-29 22:55:16.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Connect/TXT.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1108 2024-05-09 12:42:58.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Connect/WhatsApp.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      224 2024-05-09 12:43:27.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Connect/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.607864 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Consent/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5425 2023-09-29 23:50:27.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Consent/REST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1011 2023-09-29 23:52:18.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Consent/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.609279 collabconnector-0.1.1716405711/src/CollabConnector/Webex/ContactCenter/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    16955 2024-05-22 19:17:01.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/ContactCenter/ContactCenter.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2024-05-22 19:21:49.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/ContactCenter/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.612659 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Engage/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     8235 2023-11-02 16:46:15.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Engage/Chat.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5439 2023-09-29 14:23:57.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Engage/REST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1354 2023-09-29 14:23:57.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Engage/Team.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     4817 2023-11-02 16:51:10.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Engage/User.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      338 2023-09-29 14:23:57.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Engage/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.613916 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Phone/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3412 2024-03-08 12:53:56.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Phone/Phone.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Phone/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    17743 2024-05-09 19:53:28.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/Webex.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2024-03-08 13:05:25.000000 collabconnector-0.1.1716405711/src/CollabConnector/Webex/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:05:58.000000 collabconnector-0.1.1716405711/src/CollabConnector/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-22 19:21:55.614667 collabconnector-0.1.1716405711/src/CollabConnector.egg-info/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-22 19:21:55.000000 collabconnector-0.1.1716405711/src/CollabConnector.egg-info/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     4467 2024-05-22 19:21:55.000000 collabconnector-0.1.1716405711/src/CollabConnector.egg-info/SOURCES.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2024-05-22 19:21:55.000000 collabconnector-0.1.1716405711/src/CollabConnector.egg-info/dependency_links.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       77 2024-05-22 19:21:55.000000 collabconnector-0.1.1716405711/src/CollabConnector.egg-info/requires.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2024-05-22 19:21:55.000000 collabconnector-0.1.1716405711/src/CollabConnector.egg-info/top_level.txt
```

### Comparing `collabconnector-0.1.1716405627/LICENSE` & `collabconnector-0.1.1716405711/LICENSE`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/PKG-INFO` & `collabconnector-0.1.1716405711/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1716405627
+Version: 0.1.1716405711
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `collabconnector-0.1.1716405627/README.md` & `collabconnector-0.1.1716405711/README.md`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/setup.cfg` & `collabconnector-0.1.1716405711/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CollabConnector
-version = 0.1.1716405627
+version = 0.1.1716405711
 author = Jon Snipes
 author_email = jsnipes@mycollablab.org
 description = An attempt at a simplified API collection for Cisco Collab products
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/mycollablab/CollabConnector
 project_urls =
```

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CER/CER.py` & `collabconnector-0.1.1716405711/src/CollabConnector/CER/CER.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AST/AST.py` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AST/AST.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/AXL.py` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/AXL.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/CDR/CDR.py` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/CDR/CDR.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/CDR/CDROnDemand.py` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/CDR/CDROnDemand.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/CUCM.py` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/CUCM.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/DIME/DIME.py` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/DIME/DIME.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/Logs/Logs.py` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/Logs/Logs.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/Phone/Phone.py` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/Phone/Phone.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/Risport/Risport.py` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/Risport/Risport.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/Serviceability/Serviceability.py` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/Serviceability/Serviceability.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCM/UDS/UDS.py` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCM/UDS/UDS.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/CUCX/CUCX.py` & `collabconnector-0.1.1716405711/src/CollabConnector/CUCX/CUCX.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/Expressway/Expressway.py` & `collabconnector-0.1.1716405711/src/CollabConnector/Expressway/Expressway.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/IOS/IOS.py` & `collabconnector-0.1.1716405711/src/CollabConnector/IOS/IOS.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/PAWS/PAWS.py` & `collabconnector-0.1.1716405711/src/CollabConnector/PAWS/PAWS.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/UCCX/UCCX.py` & `collabconnector-0.1.1716405711/src/CollabConnector/UCCX/UCCX.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/Webex/Connect/REST.py` & `collabconnector-0.1.1716405711/src/CollabConnector/Webex/Connect/REST.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/Webex/Connect/TXT.py` & `collabconnector-0.1.1716405711/src/CollabConnector/Webex/Connect/TXT.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/Webex/Connect/WhatsApp.py` & `collabconnector-0.1.1716405711/src/CollabConnector/Webex/Connect/WhatsApp.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/Webex/Consent/REST.py` & `collabconnector-0.1.1716405711/src/CollabConnector/Webex/Consent/REST.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/Webex/Consent/__init__.py` & `collabconnector-0.1.1716405711/src/CollabConnector/Webex/Consent/__init__.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/Webex/ContactCenter/ContactCenter.py` & `collabconnector-0.1.1716405711/src/CollabConnector/Webex/ContactCenter/ContactCenter.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/Webex/Engage/Chat.py` & `collabconnector-0.1.1716405711/src/CollabConnector/Webex/Engage/Chat.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/Webex/Engage/REST.py` & `collabconnector-0.1.1716405711/src/CollabConnector/Webex/Engage/REST.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/Webex/Engage/Team.py` & `collabconnector-0.1.1716405711/src/CollabConnector/Webex/Engage/Team.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/Webex/Engage/User.py` & `collabconnector-0.1.1716405711/src/CollabConnector/Webex/Engage/User.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/Webex/Phone/Phone.py` & `collabconnector-0.1.1716405711/src/CollabConnector/Webex/Phone/Phone.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector/Webex/Webex.py` & `collabconnector-0.1.1716405711/src/CollabConnector/Webex/Webex.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector.egg-info/PKG-INFO` & `collabconnector-0.1.1716405711/src/CollabConnector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1716405627
+Version: 0.1.1716405711
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `collabconnector-0.1.1716405627/src/CollabConnector.egg-info/SOURCES.txt` & `collabconnector-0.1.1716405711/src/CollabConnector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

