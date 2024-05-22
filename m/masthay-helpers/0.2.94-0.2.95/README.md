# Comparing `tmp/masthay_helpers-0.2.94-py3-none-macosx_11_0_arm64.whl.zip` & `tmp/masthay_helpers-0.2.95-py3-none-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18448 bytes, number of entries: 12
--rw-r--r--  2.0 unx      308 b- defN 24-Mar-17 04:31 mh/__init__.py
--rw-r--r--  2.0 unx    18370 b- defN 24-Mar-17 04:31 mh/core.py
--rw-r--r--  2.0 unx     4133 b- defN 24-Mar-17 04:31 mh/core_legacy.py
--rw-r--r--  2.0 unx       51 b- defN 24-Mar-17 04:31 mh/errors.py
--rw-r--r--  2.0 unx     3780 b- defN 24-Mar-17 04:31 mh/import_env.py
--rw-r--r--  2.0 unx     7394 b- defN 24-Mar-17 04:31 mh/jupyter.py
--rw-r--r--  2.0 unx    13973 b- defN 24-Mar-17 04:31 mh/typlotlib.py
--rw-r--r--  2.0 unx     4450 b- defN 24-Mar-17 04:31 mh/typlotlib_legacy.py
--rw-r--r--  2.0 unx     1361 b- defN 24-Mar-17 04:32 masthay_helpers-0.2.94.dist-info/METADATA
--rw-r--r--  2.0 unx      106 b- defN 24-Mar-17 04:32 masthay_helpers-0.2.94.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 24-Mar-17 04:32 masthay_helpers-0.2.94.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      908 b- defN 24-Mar-17 04:32 masthay_helpers-0.2.94.dist-info/RECORD
-12 files, 54837 bytes uncompressed, 16948 bytes compressed:  69.1%
+Zip file size: 20048 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      308 b- defN 24-May-22 04:26 mh/__init__.py
+-rw-r--r--  2.0 unx    23317 b- defN 24-May-22 04:26 mh/core.py
+-rw-r--r--  2.0 unx     4133 b- defN 24-May-22 04:26 mh/core_legacy.py
+-rw-r--r--  2.0 unx       51 b- defN 24-May-22 04:26 mh/errors.py
+-rw-r--r--  2.0 unx     4232 b- defN 24-May-22 04:26 mh/import_env.py
+-rw-r--r--  2.0 unx     7394 b- defN 24-May-22 04:26 mh/jupyter.py
+-rw-r--r--  2.0 unx    14178 b- defN 24-May-22 04:26 mh/typlotlib.py
+-rw-r--r--  2.0 unx     4450 b- defN 24-May-22 04:26 mh/typlotlib_legacy.py
+-rw-r--r--  2.0 unx     1361 b- defN 24-May-22 04:26 masthay_helpers-0.2.95.dist-info/METADATA
+-rw-r--r--  2.0 unx      106 b- defN 24-May-22 04:26 masthay_helpers-0.2.95.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 24-May-22 04:26 masthay_helpers-0.2.95.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      908 b- defN 24-May-22 04:26 masthay_helpers-0.2.95.dist-info/RECORD
+12 files, 60441 bytes uncompressed, 18548 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: mh/typlotlib.py
 Comment: 
 
 Filename: mh/typlotlib_legacy.py
 Comment: 
 
-Filename: masthay_helpers-0.2.94.dist-info/METADATA
+Filename: masthay_helpers-0.2.95.dist-info/METADATA
 Comment: 
 
-Filename: masthay_helpers-0.2.94.dist-info/WHEEL
+Filename: masthay_helpers-0.2.95.dist-info/WHEEL
 Comment: 
 
-Filename: masthay_helpers-0.2.94.dist-info/top_level.txt
+Filename: masthay_helpers-0.2.95.dist-info/top_level.txt
 Comment: 
 
-Filename: masthay_helpers-0.2.94.dist-info/RECORD
+Filename: masthay_helpers-0.2.95.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mh/core.py

```diff
@@ -1,16 +1,35 @@
 import copy
 import importlib
 import inspect
 import os
+import random
 import sys
+from functools import wraps
+
 import hydra
+import yaml
+from hydra import compose, initialize
 from omegaconf import OmegaConf
-from functools import wraps
-import random
+
+
+def dict_dump(d):
+    def sdict(input_dict):
+        """
+        Recursively convert all values in the dictionary to strings, ensuring proper serialization without
+        including unwanted Python object references in the YAML output.
+        """
+        if isinstance(input_dict, dict) or isinstance(input_dict, DotDict):
+            return {str(k): sdict(v) for k, v in input_dict.items()}
+        elif isinstance(input_dict, list):
+            return [sdict(element) for element in input_dict]
+        else:
+            return str(input_dict)
+
+    return yaml.dump(sdict(d))
 
 
 class DotDict:
     def __init__(self, d=None, self_ref_resolve=False, deep=False):
         if d is None:
             d = {}
         if deep:
@@ -52,14 +71,17 @@
         return self.deep_get(k)
 
     def __setattr__(self, k, v):
         if isinstance(v, dict):
             v = DotDict(v)
         self.__dict__[k] = v
 
+    def __iter__(self):
+        return iter(self.__dict__)
+
     def getd(self, k, v):
         return self.__dict__.get(k, v)
 
     def setdefault(self, k, v):
         self.__dict__.setdefault(k, v)
 
     def keys(self):
@@ -71,15 +93,15 @@
     def values(self):
         return self.__dict__.values()
 
     def update(self, d):
         self.__dict__.update(DotDict.get_dict(d))
 
     def str(self):
-        return str(self.__dict__)
+        return dict_dump(self.__dict__)
 
     def dict(self):
         return self.__dict__
 
     def __str__(self):
         return self.str()
 
@@ -144,28 +166,26 @@
                         try:
                             if 'eval(' in v:
                                 d[k] = eval(v[5:-1], gbl, lcl)
                             elif 'self.' in v:
                                 d[k] = eval(v, gbl, lcl)
 
                         except AttributeError:
-
                             msg = (
                                 f"Could not resolve self reference for {k}={v}"
                                 f"\ngiven below\n\n{self}"
                             )
                             if not relax:
                                 raise AttributeError(msg)
                             else:
                                 UserWarning(msg)
                         except TypeError as e:
                             msg = str(e)
                             final_msg = (
-                                f'Error evaluating {v} of type {type(v)}'
-                                f'\n{msg}'
+                                f'Error evaluating {v} of type {type(v)}\n{msg}'
                             )
                             raise RuntimeError(final_msg)
             passes += 1
         if passes == max_passes:
             msg = f"Max passes ({max_passes}) reached. self_ref_resolve failed."
             if not relax:
                 raise ValueError(msg)
@@ -225,14 +245,50 @@
         valid_keys = set(inspect.signature(func).parameters.keys())
         filtered_kwargs = {k: v for k, v in kwargs.items() if k in valid_keys}
         return func(*args, **filtered_kwargs)
 
     return wrapper
 
 
+def colorize_yaml(lines, depth_color_map, value_color, max_length=160):
+    from rich.text import Text
+
+    colored_lines = Text()
+    for line in lines:
+        if len(line) > max_length:
+            line = line[:max_length] + '...'
+        # Detect the indentation level
+        stripped_line = line.lstrip()
+        indent_level = (len(line) - len(stripped_line)) // 2
+
+        # Determine the color based on the indentation level
+        color = depth_color_map.get(indent_level, 'white')
+
+        # Apply the color to the line without changing the indentation
+        if ':' in stripped_line:  # Key-value pair
+            key, value = stripped_line.split(':', 1)
+            colored_lines.append(
+                ' ' * (indent_level * 2)
+            )  # Preserve indentation
+            colored_lines.append(key + ': ', style=color)
+            colored_lines.append(value.strip(), style=value_color)
+        elif stripped_line.startswith('-'):  # List item
+            colored_lines.append(
+                ' ' * (indent_level * 2)
+            )  # Preserve indentation
+            colored_lines.append(stripped_line, style=value_color)
+        else:  # Handle keys without a value
+            colored_lines.append(
+                ' ' * (indent_level * 2)
+            )  # Preserve indentation
+            colored_lines.append(stripped_line, style=color)
+        colored_lines.append('\n')
+    return colored_lines
+
+
 def convert_dictconfig(obj, self_ref_resolve=False):
     return DotDict(
         OmegaConf.to_container(obj, resolve=True),
         self_ref_resolve=self_ref_resolve,
     )
 
 
@@ -264,15 +320,15 @@
     src = src.view(*expand_shape)
 
     # Expand to match target_shape
     return src.expand(target_shape)
 
 
 def dyn_import(*, path, mod, func=None):
-    if '.' in mod:
+    if '.' in mod or path.lower()[-4:] in ['null', 'none']:
         obj = importlib.import_module(mod)
     else:
         if not path.startswith('/'):
             path = os.path.join(os.getcwd(), path)
         if not path.endswith('.py'):
             path = os.path.join(path, f'{mod}.py')
 
@@ -291,26 +347,27 @@
 ) -> DotDict:
     cfg = OmegaConf.load(os.path.join(config_path, config_name))
     return OmegaConf.to_container(cfg, resolve=True)
 
 
 def exec_imports(d: DotDict, *, root=None, delim='|', import_key='^^'):
     q = [('', d)]
-    root = root or os.getcwd()
+    root = os.getcwd() if root is None else root
     while q:
         prefix, curr = q.pop(0)
         for k, v in curr.items():
             if isinstance(v, DotDict) or isinstance(v, dict):
                 q.append((f'{prefix}.{k}' if prefix else k, v))
             elif isinstance(v, str) and v.startswith(import_key):
                 lcl_root = os.path.join(root, *prefix.split('.'))
                 full_key = f'{prefix}.{k}' if prefix else k
                 d[full_key] = cfg_import(
                     v[len(import_key) :], root=lcl_root, delim=delim
                 )
+
     return d
 
 
 def flip_dict(d):
     try:
         u = {}
         for outer_key, inner_dict in d.items():
@@ -439,14 +496,16 @@
 
     return generated_slices
 
 
 def rich_tensor(
     tensor, *, name='Tensor', filename=None, max_width=None, strip=True, sep=','
 ):
+    import torch
+
     stats = dict(dtype=tensor.dtype, shape=tensor.shape)
     if tensor.dtype == torch.bool:
         return str(stats)
     elif tensor.dtype in [
         torch.int8,
         torch.int16,
         torch.int32,
@@ -492,14 +551,55 @@
                 [sep.join(e.split(sep)[1:]) for e in csv_str.split('\n')]
             )
         with open(df_filename, 'w') as f:
             f.write(csv_str)
 
 
 def torch_stats(report=None, black_formattable=True):
+    """
+    Calculate statistics of a torch tensor.
+
+    Args:
+        report (list or str, optional): Specifies which statistics to include in the report.
+            If not provided, only the shape of the tensor will be included.
+            Defaults to None.
+            Available options:
+                - 'shape': Shape of the tensor
+                - 'device': Device of the tensor
+                - 'dtype': Data type of the tensor
+                - 'mean': Mean value of the tensor
+                - 'variance': Variance of the tensor
+                - 'median': Median value of the tensor
+                - 'min': Minimum value of the tensor
+                - 'max': Maximum value of the tensor
+                - 'stddev': Standard deviation of the tensor
+                - 'RMS': Root mean square of the tensor
+                - 'L2': L2 norm of the tensor
+
+        black_formattable (bool, optional): Specifies whether to format the output using black.
+            If True, the output will be formatted using black_str function.
+            If False, the output will be a plain string.
+            Defaults to True.
+
+    Returns:
+        function: A helper function that calculates the requested statistics of a torch tensor.
+
+    Raises:
+        ModuleNotFoundError: If the torch module is not found, it raises an error with installation instructions.
+
+    Example:
+        >>> import torch
+        >>> stats = torch_stats(['shape', 'mean', 'min'])
+        >>> tensor = torch.tensor([1, 2, 3, 4, 5])
+        >>> print(stats(tensor))
+        shape: torch.Size([5])
+        mean: 3.0
+        min: 1
+    """
+
     try:
         import torch
 
         all = [
             'shape',
             'dtype',
             'mean',
@@ -508,23 +608,25 @@
             'min',
             'max',
             'stddev',
             'RMS',
             'L2',
         ]
         if not report:
-            report = ['shape']
+            report = ['shape', 'device', 'dtype']
         if report in ['all', ['all']]:
             report = all
         report = set(report)
 
         def helper(x):
             stats = {}
             if 'shape' in report:
                 stats['shape'] = x.shape
+            if 'device' in report:
+                stats['device'] = x.device
             if 'dtype' in report:
                 stats['dtype'] = x.dtype
             if 'mean' in report:
                 stats['mean'] = torch.mean(x).item()
             if 'variance' in report:
                 stats['variance'] = torch.var(x).item()
             if 'median' in report:
@@ -568,19 +670,61 @@
                 if type(s) == str and s.startswith('<') and s.endswith('>'):
                     curr[k] = f'"{s}"'
             return curr
 
         s = black.format_str(str(stringify(d)), mode=black.FileMode())
         return s
     except ModuleNotFoundError as e:
-        msg = f'{e}\nIn order to use black_str, you need to install black formatter'
+        msg = (
+            f'{e}\nIn order to use black_str, you need to install black'
+            ' formatter'
+        )
         msg = f'{msg} with "pip install black"'
         raise ModuleNotFoundError(msg)
 
 
+def set_print_options(
+    *,
+    precision=None,
+    threshold=None,
+    edgeitems=None,
+    linewidth=None,
+    profile=None,
+    sci_mode=None,
+    callback=None,
+):
+    try:
+        import torch
+
+        torch.set_printoptions(
+            precision=precision,
+            threshold=threshold,
+            edgeitems=edgeitems,
+            linewidth=linewidth,
+            profile=profile,
+            sci_mode=sci_mode,
+            callback=callback,
+        )
+    except TypeError:
+        print(
+            'Ignoring callback and using standard torch print options.\n'
+            'Modify your local pytorch distribution according to the following'
+            ' link to use callback.\n'
+            '    https://github.com/tmasthay/Experiments/tree/main/custom_torch_print'
+        )
+        torch.set_printoptions(
+            precision=precision,
+            threshold=threshold,
+            edgeitems=edgeitems,
+            linewidth=linewidth,
+            profile=profile,
+            sci_mode=sci_mode,
+        )
+
+
 def yamlfy(c: DotDict, lcls, gbls) -> str:
     try:
         import yaml
 
         u = eval(black_str(c), lcls, gbls)
 
         def helper(d):
```

## mh/import_env.py

```diff
@@ -17,14 +17,18 @@
 
 def get_local_name(s, ext=".py"):
     u = s if "/" not in s else s.split("/")[-1]
     u = u.replace(ext + "x", "")
     return u.replace(ext, "")
 
 
+def get_tracked_files():
+    return set(sco('git ls-files | grep ".py$" | grep -v "__init__.py" | xargs -I {} readlink -f {}', True))
+
+
 def get_subfolders(path, **kw):
     omissions = kw.get("omissions", [])
     inclusions = kw.get("inclusions", None)
     local = kw.get("local", True)
     ext = kw.get("ext", ".py")
     depth = kw.get("depth", 1)
     omissions = [path + "/%s" % e if "/" not in e else e for e in omissions]
@@ -43,53 +47,59 @@
             e
             for e in u
             if not e.split("/")[-1].startswith("__")
             and not e.split("/")[-1].startswith(".")
         ]
     except:
         u = []
+    # if only_tracked:
+    #     input(u)
+    #     input(get_tracked_files())
+    #     u = [d for d in u if d in get_tracked_files()]
     if len(omissions) > 0 or inclusions != None:
         if inclusions != None:
             [omissions.append(e) for e in u if e not in inclusions]
         u = [e for e in u if e not in omissions]
     if local:
         u = [get_local_name(e, ext) for e in u]
     return u
 
 
-def get_local_modules(path, **kw):
+def get_local_modules(path, *, only_tracked=False, **kw):
     local = kw.get("local", True)
     ext = kw.get("ext", ".py")
     res = sco(
         r'find %s -mindepth 1 -maxdepth 1 -type f -name "*%s"' % (path, ext)
     )
     res2 = sco(
         r'find %s -mindepth 1 -maxdepth 1 -type f -name "*%sx"' % (path, ext)
     )
     [res.append(e) for e in res2]
+    if only_tracked:
+        res = [f for f in res if f in get_tracked_files()]
     res = [
         e
         for e in res
         if not (
             e.split("/")[-1].startswith(".") or e.split("/")[-1].startswith("_")
         )
     ]
     if local:
         res = [get_local_name(e) for e in res]
     return res
 
 
-def init_modules(path, **kw):
+def init_modules(path, *, only_tracked=False, **kw):
     root = kw.get("root", False)
     unload = kw.get("unload", False)
     if root:
         local_modules = []
     else:
-        local_modules = get_local_modules(path, **kw)
-    subfolders = get_subfolders(path, **kw)
+        local_modules = get_local_modules(path, only_tracked=only_tracked, **kw)
+    subfolders = get_subfolders(path, only_tracked=only_tracked, **kw)
     [local_modules.append(e) for e in subfolders]
     s = "__all__ = [\n"
     for e in local_modules:
         s += '    "%s",\n' % e
     if s == "__all__ = [\n":
         s += "]\n"
     else:
```

## mh/typlotlib.py

```diff
@@ -178,40 +178,43 @@
     framer: PlotTypes.PlotHandler = None,
     **kw,
 ):
     frames = []
 
     from time import time
 
+    print('Plotting frames...', flush=True, end='')
+    start_time = time()
     if framer is None:
 
         def default_frame_handler(*, data, idx, fig, axes, **kw2):
             fig.canvas.draw()
             frame = Image.frombytes(
                 'RGB', fig.canvas.get_width_height(), fig.canvas.tostring_rgb()
             )
             return frame
 
         frame_handler = default_frame_handler
 
     curr_kw = kw
     for idx, plot_frame in iter:
-        iter_time = time()
+        # iter_time = time()
         curr_kw = plotter(data=data, idx=idx, fig=fig, axes=axes, **curr_kw)
         curr_kw = curr_kw if curr_kw is not None else kw
         if plot_frame:
             frames.append(
                 frame_handler(data=data, idx=idx, fig=fig, axes=axes, **kw)
             )
-        iter_time = time() - iter_time
-        print(
-            f'idx={idx} took {iter_time:.2f} seconds:'
-            f' len(frames)=={len(frames)}',
-            flush=True,
-        )
+        # iter_time = time() - iter_time
+        # print(
+        #     f'idx={idx} took {iter_time:.2f} seconds:'
+        #     f' len(frames)=={len(frames)}',
+        #     flush=True,
+        # )
+    print(f'done in {time() - start_time:.2f} seconds.', flush=True)
 
     return frames
 
 
 def save_frames(
     frames, *, path, movie_format='gif', duration=100, verbose=False, loop=0
 ):
@@ -437,14 +440,15 @@
     idx=None,
     xlabel=("", ""),
     ylabel=("", ""),
     title=("", ""),
     ind_var=None,
     xlim=None,
     ylim=None,
+    **other_opts,
 ):
     specs = cfg.plts[name]
     lyr = specs[layer]
     opts = lyr.get('opts', {})
 
     if lyr.get('filt', None) is not None:
         if lyr.filt == 'transpose':
@@ -470,17 +474,17 @@
         callback = plt.bar
     else:
         raise ValueError(f'Unknown plot_type: {specs.type}')
 
     idx = slice(None) if idx in [None, 'all', ':'] else idx
     data_slice = data[idx]
     if ind_var is not None:
-        callback(ind_var, data_slice, **opts)
+        callback(ind_var, data_slice, **opts, **other_opts)
     else:
-        callback(data_slice, **opts)
+        callback(data_slice, **opts, **other_opts)
 
     if lyr.get('xlabel', None) is not None:
         plt.xlabel(f"{xlabel[0]}{lyr.xlabel}{xlabel[1]}")
     if lyr.get('ylabel', None) is not None:
         plt.ylabel(f"{ylabel[0]}{lyr.ylabel}{ylabel[1]}")
     if ylim not in [None, 'dynamic']:
         plt.ylim(ylim)
```

## Comparing `masthay_helpers-0.2.94.dist-info/METADATA` & `masthay_helpers-0.2.95.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masthay-helpers
-Version: 0.2.94
+Version: 0.2.95
 Summary: Helper functions for repetitive and useful tasks
 Author: Tyler Masthay
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

## Comparing `masthay_helpers-0.2.94.dist-info/RECORD` & `masthay_helpers-0.2.95.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 mh/__init__.py,sha256=8aCfNWpIjiYHXdBDiQ1csfwvTLV4M6AzsGX4Zyls8Fc,308
-mh/core.py,sha256=osmlMWmR5Wc9FdG3AUyU_biPbGipcO2UU32Y87wenDU,18370
+mh/core.py,sha256=oGumbHI_QU6vd1BNGbHZOopWFr6UG9ZGwlhx8wBZnqw,23317
 mh/core_legacy.py,sha256=M6HI-k50OIZ5-je6PtSgxK5ax2psD0TPDJfq7_25MXY,4133
 mh/errors.py,sha256=jDpCLCSGEcRCNJCxCdMZx_hr3__V8m8g5vGg88zamh4,51
-mh/import_env.py,sha256=tSB7UCA4owYvqjET897tz0P85-etjVeIqmPJLmwrEeU,3780
+mh/import_env.py,sha256=ycv0sIvYrJReJgSRm6qF28EsQ06PNj3BBAhiErWcN4U,4232
 mh/jupyter.py,sha256=tWsOPBQUaVNjvJn0HIfnsTyY4NrG4qhvLL7XH3SBPQ4,7394
-mh/typlotlib.py,sha256=wewCHj89oH_MAQOn2pgoMtPExN7yaduDQWzu5MDiWgs,13973
+mh/typlotlib.py,sha256=KaANXD9xLuEnkUEuCqp2odb10JEKNfDmKvwL1LMoR6U,14178
 mh/typlotlib_legacy.py,sha256=4tCla5R4ryQB81YqzUfGzryOwKP898hkK0reQCgNDmE,4450
-masthay_helpers-0.2.94.dist-info/METADATA,sha256=llIb1t1oLY7JPlPjQmqW9yFHVToRwrMu2y7bL_H_jLQ,1361
-masthay_helpers-0.2.94.dist-info/WHEEL,sha256=S7b8YYk-yJ5La3yIsS368T2_Hd_9s929Seaql3JcY7Q,106
-masthay_helpers-0.2.94.dist-info/top_level.txt,sha256=8Pn8eTSlPGDH3Lgl_pW5A8ch7lAIInNkhVBsc7ro8pM,3
-masthay_helpers-0.2.94.dist-info/RECORD,,
+masthay_helpers-0.2.95.dist-info/METADATA,sha256=_PVGMKsJdZs9UqA6kcp0mq60IU_O-mvTmhNDebx0AF4,1361
+masthay_helpers-0.2.95.dist-info/WHEEL,sha256=S7b8YYk-yJ5La3yIsS368T2_Hd_9s929Seaql3JcY7Q,106
+masthay_helpers-0.2.95.dist-info/top_level.txt,sha256=8Pn8eTSlPGDH3Lgl_pW5A8ch7lAIInNkhVBsc7ro8pM,3
+masthay_helpers-0.2.95.dist-info/RECORD,,
```

