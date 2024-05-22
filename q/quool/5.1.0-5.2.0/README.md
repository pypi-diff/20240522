# Comparing `tmp/quool-5.1.0.tar.gz` & `tmp/quool-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quool-5.1.0.tar", last modified: Mon May 20 03:34:13 2024, max compression
+gzip compressed data, was "quool-5.2.0.tar", last modified: Wed May 22 04:19:20 2024, max compression
```

## Comparing `quool-5.1.0.tar` & `quool-5.2.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:34:13.413856 quool-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-20 03:33:40.000000 quool-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-20 03:34:13.413856 quool-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-20 03:33:40.000000 quool-5.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:34:13.413856 quool-5.1.0/quool/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-20 03:33:40.000000 quool-5.1.0/quool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-20 03:33:40.000000 quool-5.1.0/quool/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-05-20 03:33:40.000000 quool-5.1.0/quool/factor.py
--rw-r--r--   0 runner    (1001) docker     (127)    20456 2024-05-20 03:33:40.000000 quool-5.1.0/quool/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-20 03:33:40.000000 quool-5.1.0/quool/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-20 03:33:40.000000 quool-5.1.0/quool/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:34:13.413856 quool-5.1.0/quool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-20 03:34:13.000000 quool-5.1.0/quool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-20 03:34:13.000000 quool-5.1.0/quool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 03:34:13.000000 quool-5.1.0/quool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 03:34:13.000000 quool-5.1.0/quool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 03:34:13.000000 quool-5.1.0/quool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 03:34:13.413856 quool-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-20 03:33:40.000000 quool-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:19:20.148576 quool-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-22 04:18:55.000000 quool-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-22 04:19:20.148576 quool-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-22 04:18:55.000000 quool-5.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:19:20.148576 quool-5.2.0/quool/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 04:18:55.000000 quool-5.2.0/quool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-05-22 04:18:55.000000 quool-5.2.0/quool/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23366 2024-05-22 04:18:55.000000 quool-5.2.0/quool/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-22 04:18:55.000000 quool-5.2.0/quool/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11403 2024-05-22 04:18:55.000000 quool-5.2.0/quool/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:19:20.148576 quool-5.2.0/quool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-22 04:19:20.000000 quool-5.2.0/quool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-22 04:19:20.000000 quool-5.2.0/quool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 04:19:20.000000 quool-5.2.0/quool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-22 04:19:20.000000 quool-5.2.0/quool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 04:19:20.000000 quool-5.2.0/quool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 04:19:20.148576 quool-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-22 04:18:55.000000 quool-5.2.0/setup.py
```

### Comparing `quool-5.1.0/LICENSE` & `quool-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quool-5.1.0/PKG-INFO` & `quool-5.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quool
-Version: 5.1.0
+Version: 5.2.0
 Summary: Quantitative Toolkit - a helper in quant developping
 Home-page: https://github.com/ppoak/quool
 Author: ppoak
 Author-email: ppoak@foxmail.com
 Keywords: quant,framework,finance
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `quool-5.1.0/README.md` & `quool-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `quool-5.1.0/quool/core.py` & `quool-5.2.0/quool/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         for frag in self.fragments:
             d = self._read_fragment(frag)
             d[list(column.keys())] = np.nan
             d = d.astype(column)
             d.to_parquet(self._fragment_path(frag))
     
     def delete(self, index: pd.Index):
-        related_fragment = self._related_frag(pd.DataFrame(index=index))
+        related_fragment = self._related_frag(pd.Series(np.ones(len(index)), index=index))
         for frag in related_fragment:
             df = self._read_fragment(frag)
             df = df.drop(index=index.intersection(df.index))
             df.to_parquet(self._fragment_path(frag))
 
     def remove(self, fragment: str | list = None):
         fragment = fragment or self.fragments
```

### Comparing `quool-5.1.0/quool/record.py` & `quool-5.2.0/quool/extension.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,315 +3,20 @@
 import random
 import requests
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from lxml import etree
 from pathlib import Path
-from .table import ItemTable
-from .util import parse_commastr
+from joblib import Parallel, delayed
+from .table import ItemTable, PanelTable
+from .util import parse_commastr, evaluate
 
 
-class RunRecorder(ItemTable):
-
-    def __init__(
-        self, 
-        uri: str | Path, 
-        model_path: str | Path,
-    ):
-        super().__init__(uri, True)
-        self._model_path = model_path
-    
-    @property
-    def spliter(self):
-        return pd.Grouper(leve=0, freq='D')
-
-    @property
-    def namer(self):
-        return lambda x: x.index[0].strftime(f"%Y-%m-%d")
-
-    def record(self, **kwargs):
-        rec = pd.DataFrame([kwargs], index=[pd.to_datetime('now')])
-        existed = rec[rec.columns.isin(self.columns)]
-        nonexisted = rec[~rec.columns.isin(self.columns)]
-        if not existed.empty:
-            self.update(rec)
-        if not nonexisted.empty:
-            self.add(rec)
-
-
-class TradeRecorder(ItemTable):
-
-    standard_columns = ["datetime", "code", "size", "price", "amount", "commission"]
-
-    def __init__(
-        self, 
-        uri: str | Path, 
-        principle: float = None, 
-        start: str | pd.Timestamp = None,
-    ):
-        super().__init__(uri, True)
-        if not self.fragments:
-            if principle is None or start is None:
-                raise ValueError("principle and start_date must be specified when initiating")
-            self.add(pd.DataFrame([{
-                "datetime": pd.to_datetime(start), 
-                "code": "cash", "size": float(principle), 
-                "price": 1.0, "amount": float(principle), "commission": 0.0
-            }], index=[pd.to_datetime('now')]))
-        
-        if not self.columns.isin(self.standard_columns).all():
-            raise ValueError("The table must have standard columns")
-    
-    @property
-    def spliter(self):
-        return pd.Grouper(key='datetime', freq='ME')
-
-    @property
-    def namer(self):
-        return lambda x: x['datetime'].iloc[0].strftime('%Y%m')
-    
-    def prune(self):
-        for frag in self.fragments:
-            self._fragment_path(frag).unlink()
-
-    def read(
-        self, 
-        field: str | list = None,
-        start: str | list = None, 
-        stop: str = None,
-        code: str | list = None,
-        filters: list = None,
-    ) -> pd.Series | pd.DataFrame:
-        field = parse_commastr(field)
-        code = parse_commastr(code)
-        start = pd.to_datetime(start if start is not None else 0)
-        stop = pd.to_datetime(stop if stop is not None else 'now')
-        filters = filters or []
-        if not isinstance(start, pd.DatetimeIndex):
-            filters += [
-                ("datetime", ">=", start),
-                ("datetime", "<=", stop)
-            ]
-            if code is not None:
-                filters.append(["code", "in", code])
-        else:
-            filters += [("datetime", "in", start)]
-            if code is not None:
-                filters.append(("code", "in", code))
-        
-        return pd.read_parquet(self.path, columns=field, filters=filters)
-
-    def trade(
-        self, 
-        date: str | pd.Timestamp,
-        code: str,
-        size: float = None,
-        price: float = None,
-        amount: float = None,
-        commission: float = 0,
-        **kwargs,
-    ):
-        if size is None and price is None and amount is None:
-            raise ValueError("two of size, price or amount must be specified")
-        size = size if size is not None else (amount / price)
-        price = price if price is not None else (amount / size)
-        amount = amount if amount is not None else (size * price)
-
-        trade = pd.DataFrame([{
-            "datetime": pd.to_datetime(date),
-            "code": code, "size": size,
-            "price": price, "amount": amount,
-            "commission": commission, **kwargs
-        }], index=[pd.to_datetime('now')])
-        if code != "cash":
-            cash = pd.DataFrame([{
-                "datetime": pd.to_datetime(date),
-                "code": "cash", "size": -size * price - commission,
-                "price": 1, "commission": 0,
-                "amount": -size * price - commission
-            }], index=[pd.to_datetime('now')])
-            trade = pd.concat([trade, cash], axis=0)
-        
-        if kwargs:
-            self.add(dict((k, type(v)) for k, v in kwargs.items()))
-        self.update(trade)
-
-    def peek(self, date: str | pd.Timestamp = None, price: pd.Series = None) -> pd.Series:
-        df = self.read(filters=[("datetime", "<=", pd.to_datetime(date or 'now'))])
-        df = df.groupby("code")[["size", "amount", "commission"]].sum()
-        df["cost"] = (df["amount"] / df["size"]).replace([-np.inf, np.inf], 0)
-        if price is None:
-            return df
-        price = price.copy()
-        price.loc["cash"] = 1
-        indexer = price.index.get_indexer_for(df.index)
-        df["price"] = price.iloc[indexer[indexer != -1]]
-        df["value"] = df["price"] * df["size"]
-        df['pnl'] = ((df['price'] - df['cost']) * df['size']).where(df['size'] != 0, -df['amount'])
-        return df
-        
-    def report(
-        self, 
-        price: pd.Series, 
-        code_level: int | str = 0,
-        date_level: int | str = 1,
-    ) -> pd.DataFrame:
-        data = self.read(["datetime", "code", "size", "amount", "commission"])
-        if isinstance(price, pd.DataFrame) and price.index.nlevels == 1:
-            code_level = code_level if not isinstance(code_level, int) else "code"
-            date_level = date_level if not isinstance(date_level, int) else "datetime"
-            price = price.stack().sort_index().to_frame("price")
-            price.index.names = [date_level, code_level]
-        price = price.squeeze().sort_index()
-        dates = price.index.get_level_values(date_level).unique()
-        dates = dates[dates >= data["datetime"].min()]
-
-        data = data.groupby(["code", "datetime"]).sum()
-        data = data.reindex(pd.MultiIndex.from_product(
-            [data.index.levels[0], dates], names=["code", "datetime"]))
-        cash = data.loc["cash", "amount"]
-        cash = cash.fillna(0).cumsum()
-
-        noncash = data.drop(labels="cash", axis=0)
-        noncash.index.names = price.index.names
-        price = price.loc[noncash.index.intersection(price.index)]
-        delta = (price * noncash["size"]).groupby(level=date_level).sum()
-        noncash = noncash.fillna(0).groupby(level=code_level, group_keys=False).cumsum()
-        market = (price * noncash["size"]).groupby(level=date_level).sum()
-        market = market.reindex(cash.index).fillna(0)
-        value = market + cash
-        turnover = (delta / value.shift(1)).fillna(0)
-
-        data = pd.concat([value, cash, turnover], axis=1, keys=["value", "cash", "turnover"])
-        return data
-
-    @staticmethod
-    def evaluate(
-        value: pd.Series, 
-        cash: pd.Series = None,
-        turnover: pd.Series = None,
-        benchmark: pd.Series = None,
-        image: str = None,
-        result: str = None,
-    ):
-        
-        cash = cash.squeeze() if isinstance(cash, (pd.Series, pd.DataFrame)) else \
-            pd.Series(np.zeros(value.shape[0]), index=value.index)
-        turnover = turnover.squeeze() if isinstance(turnover, (pd.Series, pd.DataFrame)) else \
-            pd.Series(np.zeros(value.shape[0]), index=value.index)
-        benchmark = benchmark if isinstance(benchmark, (pd.Series, pd.DataFrame)) else \
-            pd.Series(np.zeros(value.shape[0]), index=value.index)
-        benchmark = benchmark.loc[value.index]
-        net_value = value / value.iloc[0]
-        net_cash = cash / cash.iloc[0]
-        returns = value.pct_change(fill_method=None).fillna(0)
-        benchmark_returns = benchmark.pct_change(fill_method=None).fillna(0)
-        benchmark_returns = benchmark_returns if not benchmark_returns.isna().all() else pd.Series(np.zeros(benchmark_returns.shape[0]), index=benchmark.index)
-        drawdown = net_value / net_value.cummax() - 1
-
-        # evaluation indicators
-        evaluation = pd.Series(name='evaluation')
-        evaluation['total_return(%)'] = (net_value.iloc[-1] / net_value.iloc[0] - 1) * 100
-        evaluation['annual_return(%)'] = ((evaluation['total_return(%)'] / 100 + 1) ** (
-            365 / (value.index.max() - value.index.min()).days) - 1) * 100
-        evaluation['annual_volatility(%)'] = (returns.std() * np.sqrt(252)) * 100
-        down_volatility = (returns[returns < 0].std() * np.sqrt(252)) * 100
-        enddate = drawdown.idxmin()
-        startdate = drawdown.loc[:enddate][drawdown.loc[:enddate] == 0].index[-1]
-        evaluation['max_drawdown(%)'] = (-drawdown.min()) * 100
-        evaluation['max_drawdown_period(days)'] = enddate - startdate
-        evaluation['max_drawdown_start'] = startdate
-        evaluation['max_drawdown_stop'] = enddate
-        evaluation['daily_turnover(%)'] = turnover.mean() * 100
-        evaluation['sharpe_ratio'] = evaluation['annual_return(%)'] / evaluation['annual_volatility(%)'] \
-            if evaluation['annual_volatility(%)'] != 0 else np.nan
-        evaluation['sortino_ratio'] = evaluation['annual_return(%)'] / down_volatility \
-            if down_volatility != 0 else np.nan
-        evaluation['calmar_ratio'] = evaluation['annual_return(%)'] / evaluation['max_drawdown(%)'] \
-            if evaluation['max_drawdown(%)'] != 0 else np.nan
-
-        if not (benchmark==0).all():
-            exreturns = returns - benchmark_returns.loc[returns.index]
-            benchmark_volatility = (benchmark_returns.std() * np.sqrt(252)) * 100
-            exvalue = (1 + exreturns).cumprod()
-            cum_benchmark_return = (1 + benchmark_returns).cumprod()
-            exdrawdown = exvalue / exvalue.cummax() - 1
-            evaluation['total_exreturn(%)'] = (exvalue.iloc[-1] - exvalue.iloc[0]) * 100
-            evaluation['annual_exreturn(%)'] = ((evaluation['total_exreturn(%)'] / 100 + 1
-                ) ** (365 / (exvalue.index.max() - exvalue.index.min()).days) - 1) * 100
-            evaluation['annual_exvolatility(%)'] = (exreturns.std() * np.sqrt(252)) * 100
-            enddate = exdrawdown.idxmin()
-            startdate = exdrawdown.loc[:enddate][exdrawdown.loc[:enddate] == 0].index[-1]
-            evaluation['ext_max_drawdown(%)'] = (exdrawdown.min()) * 100
-            evaluation['ext_max_drawdown_period(days)'] = enddate - startdate
-            evaluation['ext_max_drawdown_start'] = startdate
-            evaluation['ext_max_drawdown_stop'] = enddate
-            evaluation['beta'] = returns.cov(benchmark_returns) / benchmark_returns.var()
-            evaluation['alpha(%)'] = (returns.mean() - (evaluation['beta'] * (benchmark_returns.mean()))) * 100
-            evaluation['treynor_ratio(%)'] = (evaluation['annual_exreturn(%)'] / evaluation['beta'])
-            evaluation['information_ratio'] = evaluation['annual_exreturn(%)'] / benchmark_volatility \
-                if benchmark_volatility != 0 else np.nan
-        else:
-            exvalue = net_value
-            exdrawdown = drawdown
-            cum_benchmark_return = pd.Series(np.ones(returns.shape[0]), index=returns.index)
-            
-        data = pd.concat([value, net_value, exvalue, net_cash, returns, cum_benchmark_return, drawdown, exdrawdown, turnover], 
-                axis=1, keys=['value', 'net_value', 'exvalue', 'net_cash', 'returns', 'benchmark', 'drawdown', 'exdrawdown', 'turnover'])
-        
-        if result is not None:
-            data.to_excel(result, sheet_name="performances")
-        
-        if image is not None:
-            fig, ax = plt.subplots(nrows=2, ncols=3, figsize=(20, 10))
-            plt.subplots_adjust(wspace=0.3, hspace=0.5)
-
-            ax00 = data["net_value"].plot(ax=ax[0,0], title="Fund Return", color=['#1C1C1C'], legend=True)
-            ax00.legend(loc='lower left')
-            ax00.set_ylabel("Cumulative Return")
-            ax00_twi = ax[0,0].twinx()
-            ax00_twi.fill_between(data.index, 0, data['drawdown'], color='#009100', alpha=0.3)
-            ax00_twi.set_ylabel("Drawdown")
-
-            if not (benchmark==0).all():
-                year = (data[['net_value', 'exvalue', 'benchmark']].resample('YE').last() - data[['net_value', 'exvalue', 'benchmark']].resample('YE').first())
-            else:
-                year = (data['net_value'].resample('YE').last() - data['net_value'].resample('YE').first())
-            month = (data['net_value'].resample('ME').last() - data['net_value'].resample('ME').first())
-            year.index = year.index.year
-            year.plot(ax=ax[0,1], kind='bar', title="Yearly Return", rot=45, colormap='Paired')
-            ax[0, 2].bar(month.index, month.values, width=20)
-            ax[0, 2].set_title("Monthly Return")
-
-            ax10 = data['exvalue'].plot(ax=ax[1,0], title='Extra Return', legend=True)
-            ax10.legend(loc='lower left')
-            ax10.set_ylabel("Cumulative Return")
-            ax10_twi = ax[1,0].twinx()
-            ax10_twi.fill_between(data.index, 0, data['exdrawdown'], color='#009100', alpha=0.3)
-            ax10_twi.set_ylabel("Drawdown")
-
-            data[['net_value', 'benchmark']].plot(ax=ax[1,1], title="Fund Return")
-
-            ax12 = data['net_cash'].plot(ax=ax[1,2], title="Turnover")
-            ax12.set_ylabel('net_cash')
-            ax12_twi = ax[1,2].twinx()
-            ax12_twi.set_ylabel('turnover')
-            ax12_twi.plot(data.index, data['turnover'], color='red')
-
-            fig.tight_layout()
-            if isinstance(image, (str, Path)):
-                fig.savefig(image)
-            else:
-                fig.show()
-
-        return evaluation
-
-
-class ProxyRecorder(ItemTable):
+class Proxy(ItemTable):
 
     headers = {"User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124S Safari/537.36"}
 
     def __init__(
         self, 
         uri: str | Path, 
         create: bool = False,
@@ -494,7 +199,427 @@
         
         if len(results):
             results = pd.concat(results, axis=1).T
             if self.fragments:
                 self.update(results)
             else:
                 self.add(results)
+
+
+class Broker(ItemTable):
+
+    def __init__(
+        self, 
+        uri: str | Path, 
+        principle: float = 1_000_000.00,
+        start: str | pd.Timestamp = None,
+    ):
+        super().__init__(uri, True)
+        if not self.fragments:
+            if principle is None or start is None:
+                raise ValueError("principle and start must be specified when initiating")
+            self.add({
+                "datetime": "datetime64[ns]",
+                "code": "str",
+                "size": "int",
+                "price": "float",
+                "amount": "float",
+                "commission": "float",
+            })
+            init = pd.DataFrame([{
+                "datetime": pd.to_datetime(start), 
+                "code": "cash", "size": float(principle), 
+                "price": 1.0, "amount": float(principle), "commission": 0.0
+            }], index=[pd.to_datetime('now')])
+            self.update(init)
+    
+    @property
+    def spliter(self):
+        return pd.Grouper(key='datetime', freq='ME')
+
+    @property
+    def namer(self):
+        return lambda x: x['datetime'].iloc[0].strftime('%Y%m')
+
+    def read(
+        self, 
+        column: str | list = None, 
+        start: str | list = None, 
+        stop: str = None, 
+        code: str | list[str] = None,
+        filters: list[list[tuple]] = None,
+    ):
+        filters = filters or []
+        if code is not None:
+            filters += [("code", "in", parse_commastr(code))]
+        return super().read(column, start, stop, "datetime", filters)
+
+    def prune(self):
+        for frag in self.fragments:
+            self._fragment_path(frag).unlink()
+        
+    def trade(
+        self, 
+        date: str | pd.Timestamp,
+        code: str,
+        size: float = None,
+        price: float = None,
+        amount: float = None,
+        commission: float = 0,
+        **kwargs,
+    ):
+        if size is None and price is None and amount is None:
+            raise ValueError("two of size, price or amount must be specified")
+        size = size if size is not None else (amount / price)
+        price = price if price is not None else (amount / size)
+        amount = amount if amount is not None else (size * price)
+
+        trade = pd.DataFrame([{
+            "datetime": pd.to_datetime(date),
+            "code": code, "size": size,
+            "price": price, "amount": amount,
+            "commission": commission, **kwargs
+        }], index=[pd.to_datetime('now')])
+        if code != "cash":
+            cash = pd.DataFrame([{
+                "datetime": pd.to_datetime(date),
+                "code": "cash", "size": -size * price - commission,
+                "price": 1, "commission": 0,
+                "amount": -size * price - commission
+            }], index=[pd.to_datetime('now')])
+            trade = pd.concat([trade, cash], axis=0)
+        
+        if kwargs:
+            self.add(dict((k, type(v)) for k, v in kwargs.items()))
+        self.update(trade)
+
+    def peek(self, date: str | pd.Timestamp = None, price: pd.Series = None) -> pd.Series:
+        df = self.read(filters=[("datetime", "<=", pd.to_datetime(date or 'now'))])
+        df = df.groupby("code")[["size", "amount", "commission"]].sum()
+        df["cost"] = (df["amount"] / df["size"]).replace([-np.inf, np.inf], 0)
+        if price is None:
+            return df
+        price = price.copy()
+        price.loc["cash"] = 1
+        indexer = price.index.get_indexer_for(df.index)
+        df["price"] = price.iloc[indexer[indexer != -1]]
+        df["value"] = df["price"] * df["size"]
+        df['pnl'] = ((df['price'] - df['cost']) * df['size']).where(df['size'] != 0, -df['amount'])
+        return df
+        
+    def report(
+        self, 
+        price: pd.Series, 
+        benchmark: pd.Series = None,
+        code_level: int | str = 0,
+        date_level: int | str = 1,
+        image: str | bool = True,
+        result: str = None,
+    ) -> pd.DataFrame:
+        data = self.read(["datetime", "code", "size", "amount", "commission"])
+        if isinstance(price, pd.DataFrame) and price.index.nlevels == 1:
+            code_level = code_level if not isinstance(code_level, int) else "code"
+            date_level = date_level if not isinstance(date_level, int) else "datetime"
+            price = price.stack().sort_index().to_frame("price")
+            price.index.names = [date_level, code_level]
+        price = price.squeeze().sort_index()
+        dates = price.index.get_level_values(date_level).unique()
+        dates = dates[dates >= data["datetime"].min()]
+
+        data = data.groupby(["code", "datetime"]).sum()
+        data = data.reindex(pd.MultiIndex.from_product(
+            [data.index.levels[0], dates], names=["code", "datetime"]))
+        cash = data.loc["cash", "amount"]
+        cash = cash.fillna(0).cumsum()
+
+        noncash = data.drop(labels="cash", axis=0)
+        noncash.index.names = price.index.names
+        price = price.loc[noncash.index.intersection(price.index)]
+        delta = (price * noncash["size"]).groupby(level=date_level).sum()
+        noncash = noncash.fillna(0).groupby(level=code_level, group_keys=False).cumsum()
+        market = (price * noncash["size"]).groupby(level=date_level).sum()
+        market = market.reindex(cash.index).fillna(0)
+        value = market + cash
+        turnover = (delta / value.shift(1)).fillna(0)
+
+        data = pd.concat([value, cash, turnover], axis=1, keys=["value", "cash", "turnover"])
+        if image or result:
+            return evaluate(
+                data["value"], 
+                data["cash"],
+                data["turnover"],
+                benchmark=benchmark,
+                image=image,
+                result=result
+            )
+        return data
+
+class Factor(PanelTable):
+
+    def read(
+        self, 
+        field: str | list = None, 
+        code: str | list = None, 
+        start: str | list = None, 
+        stop: str = None, 
+        processor: list = None,
+    ) -> pd.Series | pd.DataFrame:
+        processor = processor or []
+        if not isinstance(processor, list):
+            processor = [processor]
+        
+        df = super().read(field, code, start, stop)
+        
+        if df.columns.size == 1:
+            df = df.squeeze().unstack(level=self._code_level)
+        
+        for proc in processor:
+            kwargs = {}
+            if isinstance(proc, tuple):
+                proc, kwargs = proc
+            df = proc(df, **kwargs)
+        return df.dropna(axis=0, how='all')
+        
+    def get_future(
+        self, 
+        ptype: str = "volume_weighted_price",
+        period: int = 1, 
+        start: str | pd.Timestamp = None,
+        stop: str | pd.Timestamp = None,
+    ):
+        if stop is not None:
+            stop = self.get_trading_days_rollback(stop, -period - 1)
+        price = self.read(ptype, start=start, stop=stop)
+        future = price.shift(-1 - period) / price.shift(-1) - 1
+        return future.dropna(axis=0, how='all').squeeze()
+
+    def get_trading_days(
+        self,
+        start: str | pd.Timestamp = None,
+        stop: str | pd.Timestamp = None,
+    ):
+        frag = self._read_fragment(self.fragments[0])
+        field = frag.columns[0]
+        start = start or frag.index.get_level_values(self._date_level).min()
+        code = frag.index.get_level_values(self._code_level).min()
+        dates = super().read(field, code=code, start=start, stop=stop
+            ).droplevel(self._code_level).index
+        return dates
+    
+    def get_trading_days_rollback(
+        self, 
+        date: str | pd.Timestamp = None, 
+        rollback: int = 1
+    ):
+        date = pd.to_datetime(date or 'now')
+        if rollback >= 0:
+            trading_days = self.get_trading_days(start=None, stop=date)
+            rollback = trading_days[trading_days <= date][-rollback - 1]
+        else:
+            trading_days = self.get_trading_days(start=date, stop=None)
+            rollback = trading_days[min(len(trading_days) - 1, -rollback)]
+        return rollback
+    
+    def save(
+        self,
+        df: pd.DataFrame | pd.Series, 
+        name: str = None, 
+    ):
+        code_level = self.get_levelname(self._code_level)
+        date_level = self.get_levelname(self._date_level)
+        code_level = 'order_book_id' if isinstance(code_level, int) else code_level
+        date_level = 'date' if isinstance(date_level, int) else date_level
+        if isinstance(df, pd.DataFrame) and df.index.nlevels == 1:
+            df = df.stack(future_stack=True).swaplevel()
+            df.index.names = [code_level, date_level]
+        
+        if isinstance(df, pd.Series):
+            if name is None:
+                raise ValueError('name cannot be None')
+            df.index.names = [code_level, date_level]
+            df = df.to_frame(name)
+        
+        add_data = df[df.columns[~df.columns.isin(self.columns)]]
+        if not add_data.empty:
+            self.add(add_data.dtypes)
+        self.update(df)
+    
+    def perform_crosssection(
+        self, name: str, 
+        date: str | pd.Timestamp,
+        *,
+        processor: list = None,
+        period: int = 1,
+        ptype: str = "volume_weighted_price",
+        image: str | bool = True, 
+        result: str = None
+    ):
+        future = self.get_future(ptype, period, date, date)
+        factor = self.read(field=name, start=future.name, stop=future.name, processor=processor)
+        data = pd.concat([factor.squeeze(), future], axis=1, keys=[name, future.name])
+        if image is not None:
+            pd.plotting.scatter_matrix(data, figsize=(20, 20), hist_kwds={'bins': 100})
+            
+            plt.tight_layout()
+            if isinstance(image, (str, Path)):
+                plt.savefig(image)
+            else:
+                plt.show()
+                
+        if result is not None:
+            data.to_excel(result)
+
+    def perform_inforcoef(
+        self, name: str, 
+        *,
+        period: int = 1,
+        start: str = None,
+        stop: str = None,
+        ptype: str = "volume_weighted_price",
+        processor: list = None,
+        rolling: int = 20, 
+        method: str = 'pearson', 
+        image: str | bool = True, 
+        result: str = None
+    ):
+        future = self.get_future(ptype, period, start, stop)
+        factor = self.read(field=name, start=future.index, processor=processor)
+        inforcoef = factor.corrwith(future, axis=1, method=method).dropna()
+        inforcoef.name = f"infocoef"
+
+        if image is not None:
+            fig, ax = plt.subplots(1, 1, figsize=(20, 10))
+            inforcoef.plot(ax=ax, label='infor-coef', alpha=0.7, title=f'{name} Information Coef')
+            inforcoef.rolling(rolling).mean().plot(linestyle='--', ax=ax, label='trend')
+            inforcoef.cumsum().plot(linestyle='-.', secondary_y=True, ax=ax, label='cumm-infor-coef')
+            pd.Series(np.zeros(inforcoef.shape[0]), index=inforcoef.index).plot(color='grey', ax=ax, alpha=0.5)
+            ax.legend()
+            fig.tight_layout()
+            if not isinstance(image, bool):
+                fig.savefig(image)
+            else:
+                fig.show()
+        
+        if result is not None:
+            inforcoef.to_excel(result)
+        return inforcoef
+    
+    def perform_grouping(
+        self, 
+        name: str, 
+        period: int = 1,
+        start: str = None,
+        stop: str = None,
+        processor: list = None,
+        ptype: str = "volume_weighted_price",
+        ngroup: int = 5, 
+        commission: float = 0.002, 
+        image: str | bool = True, 
+        result: str = None
+    ):
+        future = self.get_future(ptype, period, start, stop)
+        factor = self.read(field=name, start=future.index, processor=processor)
+        # ngroup test
+        try:
+            groups = factor.apply(lambda x: pd.qcut(x, q=ngroup, labels=False), axis=1) + 1
+        except:
+            for date in factor.index:
+                try:
+                    pd.qcut(factor.loc[date], q=ngroup, labels=False)
+                except:
+                    raise ValueError(f"on date {date}, grouping failed")
+        
+        def _grouping(x):
+            group = groups.where(groups == x)
+            weight = (group / group).fillna(0)
+            weight = weight.div(weight.sum(axis=1), axis=0)
+            delta = weight.diff(periods=period).fillna(0)
+            turnover = delta.abs().sum(axis=1) / 2 / period
+            ret = (future * weight).sum(axis=1).shift(1) / period
+            ret -= commission * turnover
+            ret = ret.fillna(0)
+            val = (ret + 1).cumprod()
+            return {
+                'evaluation': evaluate(val, turnover=turnover, image=False),
+                'value': val, 'turnover': turnover,
+            }
+            
+        ngroup_result = Parallel(n_jobs=1, backend='loky')(
+            delayed(_grouping)(i) for i in range(1, ngroup + 1))
+        ngroup_evaluation = pd.concat([res['evaluation'] for res in ngroup_result], 
+            axis=1, keys=range(1, ngroup + 1)).add_prefix('group')
+        ngroup_value = pd.concat([res['value'] for res in ngroup_result], 
+            axis=1, keys=range(1, ngroup + 1)).add_prefix('group')
+        ngroup_turnover = pd.concat([res['turnover'] for res in ngroup_result], 
+            axis=1, keys=range(1, ngroup + 1)).add_prefix('group')
+        ngroup_returns = ngroup_value.pct_change().fillna(0)
+        longshort_returns = ngroup_returns[f"group{ngroup}"] - ngroup_returns["group1"]
+        longshort_value = (longshort_returns + 1).cumprod()
+        longshort_evaluation = evaluate(longshort_value, image=False)
+        
+        # naming
+        longshort_evaluation.name = "longshort"
+        longshort_value.name = "longshort value"
+
+        if image is not None:
+            fig, ax = plt.subplots(nrows=1, ncols=1, figsize=(20, 10))
+            longshort_value.plot(ax=ax, linestyle='--')
+            ngroup_value.plot(ax=ax, alpha=0.8)
+            ngroup_turnover.plot(ax=ax, secondary_y=True, alpha=0.2)
+            fig.tight_layout()
+            if isinstance(image, (str, Path)):
+                fig.savefig(image)
+            else:
+                fig.show()            
+        
+        if result is not None:
+            with pd.ExcelWriter(result) as writer:
+                ngroup_evaluation.to_excel(writer, sheet_name="ngroup_evaluation")
+                longshort_evaluation.to_excel(writer, sheet_name="longshort_evaluation")
+                ngroup_value.to_excel(writer, sheet_name="ngroup_value")
+                ngroup_turnover.to_excel(writer, sheet_name="ngroup_turnover")
+                longshort_value.to_excel(writer, sheet_name="longshort_value")
+        
+        return pd.concat([ngroup_evaluation, longshort_evaluation], axis=1)
+                
+    def perform_topk(
+        self, 
+        name: str, 
+        period: int = 1,
+        start: str = None,
+        stop: str = None,
+        ptype: str = "volume_weighted_price",
+        processor: list = None,
+        topk: int = 100, 
+        commission: float = 0.002, 
+        image: str | bool = True, 
+        result: str = None
+    ):
+        future = self.get_future(ptype, period, start, stop)
+        factor = self.read(field=name, start=future.index, processor=processor)
+        topks = factor.rank(ascending=False, axis=1) < topk
+        topks = factor.where(topks)
+        topks = (topks / topks).div(topks.count(axis=1), axis=0).fillna(0)
+        turnover = topks.diff().fillna(0).abs().sum(axis=1) / 2 / period
+        ret = (topks * future).sum(axis=1).shift(1).fillna(0) - turnover * commission
+        ret = ret.fillna(0) / period
+        val = (1 + ret).cumprod()
+        eva = evaluate(val, turnover=turnover, image=False)
+
+        val.name = "value"
+        turnover.name = "turnover"
+        eva.name = "evaluation"
+
+        if image is not None:
+            fig, ax = plt.subplots(nrows=1, ncols=1, figsize=(20, 10))
+            val.plot(ax=ax, title="Top K")
+            turnover.plot(ax=ax, secondary_y=True, alpha=0.5)
+            fig.tight_layout()
+            if not isinstance(image, bool):
+                fig.savefig(image)
+            else:
+                fig.show()
+
+        if result is not None:
+            pd.concat([eva, val, turnover], axis=1).to_excel(result)
+
+        return eva
```

### Comparing `quool-5.1.0/quool/table.py` & `quool-5.2.0/quool/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 class ItemTable(Table):
 
     def read(
         self,
         column: str | list = None,
         start: str | list = None,
         stop: str = None,
+        datecol: str = None,
         filters: list[list[tuple]] = None,
     ):
         filters = filters or []
-        index_name = self.get_levelname(0)
-        index_name = '__index_level_0__' if isinstance(index_name, int) else index_name
+        if datecol is None:
+            datecol = self.get_levelname(0)
+            datecol = '__index_level_0__' if isinstance(datecol, int) else datecol
 
-        if isinstance(start, list):
-            filters.append((index_name, "in", start))
-        elif isinstance(start, str):
-            filters.append((index_name, ">=", start))
+        if isinstance(start, (list, pd.DatetimeIndex)):
+            filters.append((datecol, "in", pd.to_datetime(start)))
+        elif isinstance(start, (str, pd.Timestamp)):
+            filters.append((datecol, ">=", pd.to_datetime(start)))
         if isinstance(stop, str) and not isinstance(start, list):
-            filters.append((index_name, "<=", stop))
+            filters.append((datecol, "<=", pd.to_datetime(stop)))
         
         if not len(filters):
             filters = None
         
         return super().read(parse_commastr(column), filters)
```

### Comparing `quool-5.1.0/quool.egg-info/PKG-INFO` & `quool-5.2.0/quool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quool
-Version: 5.1.0
+Version: 5.2.0
 Summary: Quantitative Toolkit - a helper in quant developping
 Home-page: https://github.com/ppoak/quool
 Author: ppoak
 Author-email: ppoak@foxmail.com
 Keywords: quant,framework,finance
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `quool-5.1.0/setup.py` & `quool-5.2.0/setup.py`

 * *Files identical despite different names*

