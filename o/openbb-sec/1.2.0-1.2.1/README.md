# Comparing `tmp/openbb_sec-1.2.0.tar.gz` & `tmp/openbb_sec-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_sec-1.2.0.tar", max compression
+gzip compressed data, was "openbb_sec-1.2.1.tar", max compression
```

## Comparing `openbb_sec-1.2.0.tar` & `openbb_sec-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0      297 2024-05-15 14:25:02.970361 openbb_sec-1.2.0/README.md
--rw-r--r--   0        0        0     1629 2024-05-14 15:30:05.618404 openbb_sec-1.2.0/openbb_sec/__init__.py
--rw-r--r--   0        0        0       27 2024-04-23 10:22:39.680890 openbb_sec-1.2.0/openbb_sec/models/__init__.py
--rw-r--r--   0        0        0     1658 2024-05-09 13:34:29.234211 openbb_sec-1.2.0/openbb_sec/models/cik_map.py
--rw-r--r--   0        0        0    10150 2024-05-09 13:34:29.234378 openbb_sec-1.2.0/openbb_sec/models/company_filings.py
--rw-r--r--   0        0        0     3154 2024-05-09 13:34:29.234542 openbb_sec-1.2.0/openbb_sec/models/equity_ftd.py
--rw-r--r--   0        0        0     2681 2024-05-09 13:34:29.234665 openbb_sec-1.2.0/openbb_sec/models/equity_search.py
--rw-r--r--   0        0        0    39078 2024-05-09 13:34:29.234955 openbb_sec-1.2.0/openbb_sec/models/etf_holdings.py
--rw-r--r--   0        0        0     2820 2024-05-09 13:34:29.235121 openbb_sec-1.2.0/openbb_sec/models/form_13FHR.py
--rw-r--r--   0        0        0     2051 2024-05-09 13:34:29.235238 openbb_sec-1.2.0/openbb_sec/models/institutions_search.py
--rw-r--r--   0        0        0        0 2024-04-02 11:35:59.520014 openbb_sec-1.2.0/openbb_sec/models/py.typed
--rw-r--r--   0        0        0     2916 2024-05-09 13:34:29.235351 openbb_sec-1.2.0/openbb_sec/models/rss_litigation.py
--rw-r--r--   0        0        0     1945 2024-04-08 12:02:16.675933 openbb_sec-1.2.0/openbb_sec/models/schema_files.py
--rw-r--r--   0        0        0     3498 2024-05-09 13:34:29.235482 openbb_sec-1.2.0/openbb_sec/models/sic_search.py
--rw-r--r--   0        0        0     1796 2024-05-09 13:34:29.235747 openbb_sec-1.2.0/openbb_sec/models/symbol_map.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.896831 openbb_sec-1.2.0/openbb_sec/py.typed
--rw-r--r--   0        0        0       17 2024-04-23 10:22:39.682644 openbb_sec-1.2.0/openbb_sec/utils/__init__.py
--rw-r--r--   0        0        0     5511 2024-02-29 11:03:36.896953 openbb_sec-1.2.0/openbb_sec/utils/definitions.py
--rw-r--r--   0        0        0    12574 2024-05-09 13:34:29.235977 openbb_sec-1.2.0/openbb_sec/utils/helpers.py
--rw-r--r--   0        0        0     7587 2024-05-09 13:34:29.236173 openbb_sec-1.2.0/openbb_sec/utils/parse_13f.py
--rw-r--r--   0        0        0        0 2024-04-02 11:35:59.520629 openbb_sec-1.2.0/openbb_sec/utils/py.typed
--rw-r--r--   0        0        0      559 2024-05-15 16:05:42.143525 openbb_sec-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 openbb_sec-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      297 2024-05-22 11:48:40.543330 openbb_sec-1.2.1/README.md
+-rw-r--r--   0        0        0     1773 2024-05-22 11:48:40.543330 openbb_sec-1.2.1/openbb_sec/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-14 16:56:41.957865 openbb_sec-1.2.1/openbb_sec/models/__init__.py
+-rw-r--r--   0        0        0     1658 2024-05-14 16:57:23.606032 openbb_sec-1.2.1/openbb_sec/models/cik_map.py
+-rw-r--r--   0        0        0    10213 2024-05-22 11:48:40.543330 openbb_sec-1.2.1/openbb_sec/models/company_filings.py
+-rw-r--r--   0        0        0     6796 2024-05-22 11:48:40.543330 openbb_sec-1.2.1/openbb_sec/models/compare_company_facts.py
+-rw-r--r--   0        0        0     3154 2024-05-14 16:57:23.606032 openbb_sec-1.2.1/openbb_sec/models/equity_ftd.py
+-rw-r--r--   0        0        0     2681 2024-05-14 16:57:23.606032 openbb_sec-1.2.1/openbb_sec/models/equity_search.py
+-rw-r--r--   0        0        0    39203 2024-05-22 11:48:40.543330 openbb_sec-1.2.1/openbb_sec/models/etf_holdings.py
+-rw-r--r--   0        0        0     2820 2024-05-14 16:57:23.606032 openbb_sec-1.2.1/openbb_sec/models/form_13FHR.py
+-rw-r--r--   0        0        0     2051 2024-05-14 16:57:23.606032 openbb_sec-1.2.1/openbb_sec/models/institutions_search.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.957865 openbb_sec-1.2.1/openbb_sec/models/py.typed
+-rw-r--r--   0        0        0     2916 2024-05-14 16:57:23.606032 openbb_sec-1.2.1/openbb_sec/models/rss_litigation.py
+-rw-r--r--   0        0        0     1945 2024-05-14 16:56:41.957865 openbb_sec-1.2.1/openbb_sec/models/schema_files.py
+-rw-r--r--   0        0        0     3557 2024-05-22 11:48:40.543330 openbb_sec-1.2.1/openbb_sec/models/sic_search.py
+-rw-r--r--   0        0        0     1796 2024-05-14 16:57:23.606032 openbb_sec-1.2.1/openbb_sec/models/symbol_map.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.957865 openbb_sec-1.2.1/openbb_sec/py.typed
+-rw-r--r--   0        0        0       17 2024-05-14 16:56:41.957865 openbb_sec-1.2.1/openbb_sec/utils/__init__.py
+-rw-r--r--   0        0        0     5511 2024-05-22 11:48:40.543330 openbb_sec-1.2.1/openbb_sec/utils/definitions.py
+-rw-r--r--   0        0        0    36879 2024-05-22 13:43:02.476925 openbb_sec-1.2.1/openbb_sec/utils/frames.py
+-rw-r--r--   0        0        0    12735 2024-05-22 11:48:40.543330 openbb_sec-1.2.1/openbb_sec/utils/helpers.py
+-rw-r--r--   0        0        0     7587 2024-05-14 16:57:23.606032 openbb_sec-1.2.1/openbb_sec/utils/parse_13f.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.961865 openbb_sec-1.2.1/openbb_sec/utils/py.typed
+-rw-r--r--   0        0        0      574 2024-05-22 13:57:38.031898 openbb_sec-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 openbb_sec-1.2.1/PKG-INFO
```

### Comparing `openbb_sec-1.2.0/openbb_sec/__init__.py` & `openbb_sec-1.2.1/openbb_sec/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """SEC provider module."""
 
 from openbb_core.provider.abstract.provider import Provider
 from openbb_sec.models.cik_map import SecCikMapFetcher
 from openbb_sec.models.company_filings import SecCompanyFilingsFetcher
+from openbb_sec.models.compare_company_facts import SecCompareCompanyFactsFetcher
 from openbb_sec.models.equity_ftd import SecEquityFtdFetcher
 from openbb_sec.models.equity_search import SecEquitySearchFetcher
 from openbb_sec.models.etf_holdings import SecEtfHoldingsFetcher
 from openbb_sec.models.form_13FHR import SecForm13FHRFetcher
 from openbb_sec.models.institutions_search import SecInstitutionsSearchFetcher
 from openbb_sec.models.rss_litigation import SecRssLitigationFetcher
 from openbb_sec.models.schema_files import SecSchemaFilesFetcher
@@ -17,14 +18,15 @@
     name="sec",
     website="https://www.sec.gov/data",
     description="SEC is the public listings regulatory body for the United States.",
     credentials=None,
     fetcher_dict={
         "CikMap": SecCikMapFetcher,
         "CompanyFilings": SecCompanyFilingsFetcher,
+        "CompareCompanyFacts": SecCompareCompanyFactsFetcher,
         "EquityFTD": SecEquityFtdFetcher,
         "EquitySearch": SecEquitySearchFetcher,
         "EtfHoldings": SecEtfHoldingsFetcher,
         "Filings": SecCompanyFilingsFetcher,
         "Form13FHR": SecForm13FHRFetcher,
         "InstitutionsSearch": SecInstitutionsSearchFetcher,
         "RssLitigation": SecRssLitigationFetcher,
```

### Comparing `openbb_sec-1.2.0/openbb_sec/models/cik_map.py` & `openbb_sec-1.2.1/openbb_sec/models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.2.0/openbb_sec/models/company_filings.py` & `openbb_sec-1.2.1/openbb_sec/models/company_filings.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         description=QUERY_DESCRIPTIONS.get("symbol", ""),
         default=None,
     )
     cik: Optional[Union[str, int]] = Field(
         description="Lookup filings by Central Index Key (CIK) instead of by symbol.",
         default=None,
     )
-    form_type: Union[None, FORM_TYPES] = Field(
+    form_type: Optional[FORM_TYPES] = Field(
         description="Type of the SEC filing form.",
         default=None,
     )
     use_cache: bool = Field(
         description="Whether or not to use cache.  If True, cache will store for one day.",
         default=True,
     )
@@ -167,15 +167,15 @@
             cik_: str = ""
             temp = 10 - len(query.cik)  # type: ignore
             for i in range(temp):
                 cik_ = cik_ + "0"
             query.cik = cik_ + str(query.cik)  # type: ignore
 
         url = f"https://data.sec.gov/submissions/CIK{query.cik}.json"
-
+        data: Union[dict, List[dict]] = []
         if query.use_cache is True:
             cache_dir = f"{get_user_cache_directory()}/http/sec_company_filings"
             async with CachedSession(
                 cache=SQLiteBackend(cache_dir, expire_after=3600 * 24)
             ) as session:
                 try:
                     data = await amake_request(url, headers=HEADERS, session=session)  # type: ignore
@@ -202,15 +202,15 @@
             async def callback(response, session):
                 """Response callback for excess company filings."""
                 result = await response.json()
                 if result:
                     new_data = DataFrame.from_records(result)
                     results.extend(new_data.to_dict("records"))
 
-            urls = []
+            urls: List = []
             new_urls = (
                 DataFrame(data["filings"].get("files"))  # type: ignore
                 if "filings" in data
                 else DataFrame()
             )
             for i in new_urls.index:
                 new_cik: str = data["filings"]["files"][i]["name"]  # type: ignore
@@ -272,15 +272,15 @@
         filings["completeSubmissionUrl"] = (
             base_url + filings["accessionNumber"] + ".txt"
         )
         filings["filingDetailUrl"] = (
             base_url + filings["accessionNumber"] + "-index.htm"
         )
         if query.form_type:
-            filings = filings[filings["form"] == query.form_type]
+            filings = filings[filings["form"] == query.form_type.replace("_", " ")]
 
         if query.limit:
             filings = filings.head(query.limit) if query.limit != 0 else filings
 
         if len(filings) == 0:
             raise EmptyDataError("No filings were found using the filters provided.")
```

### Comparing `openbb_sec-1.2.0/openbb_sec/models/equity_ftd.py` & `openbb_sec-1.2.1/openbb_sec/models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.2.0/openbb_sec/models/equity_search.py` & `openbb_sec-1.2.1/openbb_sec/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.2.0/openbb_sec/models/etf_holdings.py` & `openbb_sec-1.2.1/openbb_sec/models/etf_holdings.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,14 +367,15 @@
         else:
             filing_url = filing_candidates["primary_doc"].values[0]
 
         async def callback(response, session):
             """Response callback for the request."""
             return await response.read()
 
+        response: Union[dict, List[dict]] = []
         if query.use_cache is True:
             cache_dir = f"{get_user_cache_directory()}/http/sec_etf"
             async with CachedSession(cache=SQLiteBackend(cache_dir)) as session:
                 try:
                     response = await amake_request(
                         filing_url, headers=HEADERS, session=session, response_callback=callback  # type: ignore
                     )
@@ -743,14 +744,17 @@
                 df.fillna("N/A")
                 .replace("N/A", None)
                 .sort_values(by="pctVal", ascending=False)
                 .to_dict(orient="records")
             )
         # Extract additional information from the form that doesn't belong in the holdings table.
         metadata = {}
+        month_1: str = ""
+        month_2: str = ""
+        month_3: str = ""
         try:
             gen_info = response["edgarSubmission"]["formData"].get("genInfo", {})  # type: ignore
             if gen_info:
                 metadata["fund_name"] = gen_info.get("seriesName")
                 metadata["series_id"] = gen_info.get("seriesId")
                 metadata["lei"] = gen_info.get("seriesLei")
                 metadata["period_ending"] = gen_info.get("repPdDate")
```

### Comparing `openbb_sec-1.2.0/openbb_sec/models/form_13FHR.py` & `openbb_sec-1.2.1/openbb_sec/models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.2.0/openbb_sec/models/institutions_search.py` & `openbb_sec-1.2.1/openbb_sec/models/institutions_search.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.2.0/openbb_sec/models/rss_litigation.py` & `openbb_sec-1.2.1/openbb_sec/models/rss_litigation.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.2.0/openbb_sec/models/schema_files.py` & `openbb_sec-1.2.1/openbb_sec/models/schema_files.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.2.0/openbb_sec/models/sic_search.py` & `openbb_sec-1.2.1/openbb_sec/models/sic_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """SEC Standard Industrial Classification Code (SIC) Model."""
 
 # pylint: disable=unused-argument
 
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 import pandas as pd
 from aiohttp_client_cache import SQLiteBackend
 from aiohttp_client_cache.session import CachedSession
 from openbb_core.app.utils import get_user_cache_directory
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.fetcher import Fetcher
@@ -58,14 +58,15 @@
         """Extract data from the SEC website table."""
         data = pd.DataFrame()
         results: List[Dict] = []
         url = (
             "https://www.sec.gov/corpfin/"
             "division-of-corporation-finance-standard-industrial-classification-sic-code-list"
         )
+        response: Union[dict, List[dict], str] = {}
         if query.use_cache is True:
             cache_dir = f"{get_user_cache_directory()}/http/sec_sic"
             async with CachedSession(
                 cache=SQLiteBackend(cache_dir, expire_after=3600 * 24 * 30)
             ) as session:
                 try:
                     response = await amake_request(
```

### Comparing `openbb_sec-1.2.0/openbb_sec/models/symbol_map.py` & `openbb_sec-1.2.1/openbb_sec/models/symbol_map.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.2.0/openbb_sec/utils/definitions.py` & `openbb_sec-1.2.1/openbb_sec/utils/definitions.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,18 @@
     "Accept-Encoding": "gzip, deflate",
 }
 
 
 FORM_TYPES = Literal[
     "1",
     "1-A",
-    "1-A POS",
+    "1-A_POS",
     "1-A-W",
     "1-E",
-    "1-E AD",
+    "1-E_AD",
     "1-K",
     "1-SA",
     "1-U",
     "1-Z",
     "1-Z-W",
     "10-12B",
     "10-12G",
@@ -108,44 +108,44 @@
     "497H2",
     "497J",
     "497K",
     "497VPI",
     "497VPU",
     "5",
     "6-K",
-    "6B NTC",
-    "6B ORDR",
+    "6B_NTC",
+    "6B_ORDR",
     "8-A12B",
     "8-A12G",
     "8-K",
     "8-K12B",
     "8-K12G3",
     "8-K15D5",
     "8-M",
-    "8F-2 NTC",
-    "8F-2 ORDR",
+    "8F-2_NTC",
+    "8F-2_ORDR",
     "9-M",
     "ABS-15G",
     "ABS-EE",
     "ADN-MTL",
     "ADV-E",
     "ADV-H-C",
     "ADV-H-T",
     "ADV-NR",
     "ANNLRPT",
-    "APP NTC",
-    "APP ORDR",
-    "APP WD",
-    "APP WDG",
+    "APP_NTC",
+    "APP_ORDR",
+    "APP_WD",
+    "APP_WDG",
     "ARS",
     "ATS-N",
     "ATS-N-C",
     "ATS-N/UA",
     "AW",
-    "AW WD",
+    "AW_WD",
     "C",
     "C-AR",
     "C-AR-W",
     "C-TR",
     "C-TR-W",
     "C-U",
     "C-U-W",
@@ -157,28 +157,28 @@
     "CERTCBO",
     "CERTNAS",
     "CERTNYS",
     "CERTPAC",
     "CFPORTAL",
     "CFPORTAL-W",
     "CORRESP",
-    "CT ORDER",
+    "CT_ORDER",
     "D",
-    "DEF 14A",
-    "DEF 14C",
+    "DEF_14A",
+    "DEF_14C",
     "DEFA14A",
     "DEFA14C",
     "DEFC14A",
     "DEFC14C",
     "DEFM14A",
     "DEFM14C",
     "DEFN14A",
     "DEFR14A",
     "DEFR14C",
-    "DEL AM",
+    "DEL_AM",
     "DFAN14A",
     "DFRN14A",
     "DOS",
     "DOSLTR",
     "DRS",
     "DRSLTR",
     "DSTRBRPT",
@@ -190,27 +190,27 @@
     "F-1MEF",
     "F-3",
     "F-3ASR",
     "F-3D",
     "F-3DPOS",
     "F-3MEF",
     "F-4",
-    "F-4 POS",
+    "F-4_POS",
     "F-4MEF",
     "F-6",
-    "F-6 POS",
+    "F-6_POS",
     "F-6EF",
     "F-7",
-    "F-7 POS",
+    "F-7_POS",
     "F-8",
-    "F-8 POS",
+    "F-8_POS",
     "F-80",
     "F-80POS",
     "F-9",
-    "F-9 POS",
+    "F-9_POS",
     "F-N",
     "F-X",
     "FOCUSN",
     "FWP",
     "G-405",
     "G-405N",
     "G-FIN",
@@ -221,20 +221,20 @@
     "MA-I",
     "MA-W",
     "MSD",
     "MSDCO",
     "MSDW",
     "N-1",
     "N-14",
-    "N-14 8C",
+    "N-14_8C",
     "N-14MEF",
     "N-18F1",
     "N-1A",
     "N-2",
-    "N-2 POSASR",
+    "N-2_POSASR",
     "N-23C-2",
     "N-23C3A",
     "N-23C3B",
     "N-23C3C",
     "N-2ASR",
     "N-2MEF",
     "N-30B-2",
@@ -244,70 +244,70 @@
     "N-54A",
     "N-54C",
     "N-6",
     "N-6F",
     "N-8A",
     "N-8B-2",
     "N-8F",
-    "N-8F NTC",
-    "N-8F ORDR",
+    "N-8F_NTC",
+    "N-8F_ORDR",
     "N-CEN",
     "N-CR",
     "N-CSR",
     "N-CSRS",
     "N-MFP",
     "N-MFP1",
     "N-MFP2",
     "N-PX",
     "N-Q",
     "N-VP",
     "N-VPFS",
-    "NO ACT",
+    "NO_ACT",
     "NPORT-EX",
     "NPORT-NP",
     "NPORT-P",
     "NRSRO-CE",
     "NRSRO-UPD",
     "NSAR-A",
     "NSAR-AT",
     "NSAR-B",
     "NSAR-BT",
     "NSAR-U",
-    "NT 10-D",
-    "NT 10-K",
-    "NT 10-Q",
-    "NT 11-K",
-    "NT 20-F",
-    "NT N-CEN",
-    "NT N-MFP",
-    "NT N-MFP1",
-    "NT N-MFP2",
-    "NT NPORT-EX",
-    "NT NPORT-P",
+    "NT_10-D",
+    "NT_10-K",
+    "NT_10-Q",
+    "NT_11-K",
+    "NT_20-F",
+    "NT_N-CEN",
+    "NT_N-MFP",
+    "NT_N-MFP1",
+    "NT_N-MFP2",
+    "NT_NPORT-EX",
+    "NT_NPORT-P",
     "NT-NCEN",
     "NT-NCSR",
     "NT-NSAR",
     "NTFNCEN",
     "NTFNCSR",
     "NTFNSAR",
-    "NTN 10D",
-    "NTN 10K",
-    "NTN 10Q",
-    "NTN 20F",
-    "OIP NTC",
-    "OIP ORDR",
-    "POS 8C",
-    "POS AM",
-    "POS AMI",
-    "POS EX",
+    "NTN_10D",
+    "NTN_10K",
+    "NTN_10Q",
+    "NTN_20F",
+    "OIP_NTC",
+    "OIP_ORDR",
+    "POS_8C",
+    "POS_AM",
+    "POS_AMI",
+    "POS_EX",
     "POS462B",
     "POS462C",
     "POSASR",
-    "PRE 14A",
-    "PRE 14C",
+    "PRE_14A",
+    "PRE_14C",
     "PREC14A",
     "PREC14C",
     "PREM14A",
     "PREM14C",
     "PREN14A",
     "PRER14A",
     "PRER14C",
@@ -315,64 +315,64 @@
     "PX14A6G",
     "PX14A6N",
     "QRTLYRPT",
     "QUALIF",
     "REG-NR",
     "REVOKED",
     "RW",
-    "RW WD",
+    "RW_WD",
     "S-1",
     "S-11",
     "S-11MEF",
     "S-1MEF",
     "S-20",
     "S-3",
     "S-3ASR",
     "S-3D",
     "S-3DPOS",
     "S-3MEF",
     "S-4",
-    "S-4 POS",
+    "S-4_POS",
     "S-4EF",
     "S-4MEF",
     "S-6",
     "S-8",
-    "S-8 POS",
+    "S-8_POS",
     "S-B",
     "S-BMEF",
     "SBSE",
     "SBSE-A",
     "SBSE-BD",
     "SBSE-C",
     "SBSE-W",
-    "SC 13D",
-    "SC 13E1",
-    "SC 13E3",
-    "SC 13G",
-    "SC 14D9",
-    "SC 14F1",
-    "SC 14N",
-    "SC TO-C",
-    "SC TO-I",
-    "SC TO-T",
+    "SC_13D",
+    "SC_13E1",
+    "SC_13E3",
+    "SC_13G",
+    "SC_14D9",
+    "SC_14F1",
+    "SC_14N",
+    "SC_TO-C",
+    "SC_TO-I",
+    "SC_TO-T",
     "SC13E4F",
     "SC14D1F",
     "SC14D9C",
     "SC14D9F",
     "SD",
     "SDR",
     "SE",
-    "SEC ACTION",
-    "SEC STAFF ACTION",
-    "SEC STAFF LETTER",
+    "SEC_ACTION",
+    "SEC_STAFF_ACTION",
+    "SEC_STAFF_LETTER",
     "SF-1",
     "SF-3",
     "SL",
-    "SP 15D2",
-    "STOP ORDER",
+    "SP_15D2",
+    "STOP_ORDER",
     "SUPPL",
     "T-3",
     "TA-1",
     "TA-2",
     "TA-W",
     "TACO",
     "TH",
```

### Comparing `openbb_sec-1.2.0/openbb_sec/utils/helpers.py` & `openbb_sec-1.2.1/openbb_sec/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     pd.DataFrame: Pandas DataFrame with columns for Symbol, Company Name, and CIK Number.
 
     Example
     -------
     >>> tickers = get_all_companies()
     """
     url = "https://www.sec.gov/files/company_tickers.json"
-
+    response: Union[dict, List[dict]] = {}
     if use_cache is True:
         cache_dir = f"{get_user_cache_directory()}/http/sec_companies"
         async with CachedSession(
             cache=SQLiteBackend(cache_dir, expire_after=3600 * 24 * 2)
         ) as session:
             try:
                 response = await amake_request(url, headers=SEC_HEADERS, session=session)  # type: ignore
@@ -61,14 +61,15 @@
     """Get a list of entity names and their CIK number."""
     url = "https://www.sec.gov/Archives/edgar/cik-lookup-data.txt"
 
     async def callback(response, session):
         """Response callback for CIK lookup data."""
         return await response.text(encoding="latin-1")
 
+    response: Union[dict, List[dict], str] = {}
     if use_cache is True:
         cache_dir = f"{get_user_cache_directory()}/http/sec_ciks"
         async with CachedSession(
             cache=SQLiteBackend(cache_dir, expire_after=3600 * 24 * 2)
         ) as session:
             try:
                 response = await amake_request(url, headers=SEC_HEADERS, session=session, response_callback=callback)  # type: ignore
@@ -93,14 +94,15 @@
 
 
 async def get_mf_and_etf_map(use_cache: bool = True) -> pd.DataFrame:
     """Return the CIK number of a ticker symbol for querying the SEC API."""
     symbols = pd.DataFrame()
 
     url = "https://www.sec.gov/files/company_tickers_mf.json"
+    response: Union[dict, List[dict]] = {}
     if use_cache is True:
         cache_dir = f"{get_user_cache_directory()}/http/sec_mf_etf_map"
         async with CachedSession(
             cache=SQLiteBackend(cache_dir, expire_after=3600 * 24 * 2)
         ) as session:
             try:
                 response = await amake_request(url, headers=SEC_HEADERS, session=session, response_callback=sec_callback)  # type: ignore
@@ -185,14 +187,15 @@
     """Download a list of files from URLs."""
     results = pd.DataFrame()
 
     async def callback(response, session):
         """Response callback for ZIP file downloads."""
         return await response.read()
 
+    response: Union[dict, List[dict]] = {}
     if use_cache is True:
         cache_dir = f"{get_user_cache_directory()}/http/sec_ftd"
         async with CachedSession(cache=SQLiteBackend(cache_dir)) as session:
             try:
                 response = await amake_request(url, session=session, headers=HEADERS, response_callback=callback)  # type: ignore
             finally:
                 await session.close()
@@ -223,23 +226,20 @@
                 "SYMBOL": "symbol",
                 "CUSIP": "cusip",
                 "QUANTITY (FAILS)": "quantity",
                 "PRICE": "price",
                 "DESCRIPTION": "description",
             }
         )
-        if symbol is not None:
+        if symbol:
             results = results[results["symbol"] == symbol]
         results["date"] = pd.to_datetime(results["date"], format="%Y%m%d").dt.date
+        # Replace invalid decimal values with None
         results["price"] = results["price"].mask(
-            results["price"].str.contains(  # pylint: disable=C0121
-                r"^\d+(?:\.\d+)?$", regex=True
-            )
-            == False,  # noqa
-            None,
+            ~results["price"].str.contains(r"^\d+(?:\.\d+)?$", regex=True), None
         )
         results["price"] = results["price"].astype(float)
 
     return results.reset_index(drop=True).to_dict("records")
 
 
 async def get_ftd_urls() -> Dict:
@@ -311,15 +311,15 @@
         )
     except IndexError as e:
         raise ValueError("Fund not found for, the symbol: " + symbol) from e
     if series_id == "" or series_id is None:
         raise ValueError("Fund not found for, the symbol: " + symbol)
 
     url = f"https://efts.sec.gov/LATEST/search-index?q={series_id}&dateRange=all&forms=NPORT-P"
-
+    response: Union[dict, List[dict]] = {}
     if use_cache is True:
         cache_dir = f"{get_user_cache_directory()}/http/sec_etf"
         async with CachedSession(cache=SQLiteBackend(cache_dir)) as session:
             try:
                 response = await amake_request(url, session=session, headers=HEADERS, response_callback=sec_callback)  # type: ignore
             finally:
                 await session.close()
```

### Comparing `openbb_sec-1.2.0/openbb_sec/utils/parse_13f.py` & `openbb_sec-1.2.1/openbb_sec/utils/parse_13f.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.2.0/pyproject.toml` & `openbb_sec-1.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "openbb-sec"
-version = "1.2.0"
+version = "1.2.1"
 description = "SEC extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_sec" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 aiohttp-client-cache = "^0.11.0"
 aiosqlite = "^0.20.0"
 xmltodict = "^0.13.0"
+bs4 = "^0.0.2"
 lxml = "^5.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
```

### Comparing `openbb_sec-1.2.0/PKG-INFO` & `openbb_sec-1.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: openbb-sec
-Version: 1.2.0
+Version: 1.2.1
 Summary: SEC extension for OpenBB
 License: AGPL-3.0-only
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp-client-cache (>=0.11.0,<0.12.0)
 Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
+Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: lxml (>=5.2.1,<6.0.0)
-Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.3,<2.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
 # OpenBB SEC Provider
 
 This extension integrates the [SEC](https://www.sec.gov/edgar) data provider into the OpenBB Platform.
```

