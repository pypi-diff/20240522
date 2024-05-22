# Comparing `tmp/nadl-1.3.0.tar.gz` & `tmp/nadl-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.3.0.tar", last modified: Thu May 16 22:59:49 2024, max compression
+gzip compressed data, was "nadl-1.4.0.tar", last modified: Tue May 21 15:38:56 2024, max compression
```

## Comparing `nadl-1.3.0.tar` & `nadl-1.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2275 2024-05-16 22:59:49.513755 nadl-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.3.0/readme.org
--rw-r--r--   0        0        0     1784 2024-05-16 22:59:08.461595 nadl-1.3.0/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.3.0/src/nadl/blocks.py
--rw-r--r--   0        0        0     5343 2024-05-14 05:05:57.551156 nadl-1.3.0/src/nadl/data.py
--rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.3.0/src/nadl/images.py
--rw-r--r--   0        0        0     3170 2024-04-22 06:27:49.753850 nadl-1.3.0/src/nadl/keys.py
--rw-r--r--   0        0        0     3986 2024-05-14 05:17:02.160133 nadl-1.3.0/src/nadl/loops.py
--rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.3.0/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.3.0/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.3.0/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.3.0/src/nadl/py.typed
--rw-r--r--   0        0        0     3884 2024-05-15 03:21:02.151713 nadl-1.3.0/src/nadl/states.py
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.3.0/src/nadl/transformers.py
--rw-r--r--   0        0        0     2363 2024-05-14 05:16:59.307787 nadl-1.3.0/src/nadl/utils.py
--rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 nadl-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2275 2024-05-21 15:38:56.528277 nadl-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.4.0/readme.org
+-rw-r--r--   0        0        0     1784 2024-05-21 15:34:55.693364 nadl-1.4.0/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.4.0/src/nadl/blocks.py
+-rw-r--r--   0        0        0     5133 2024-05-21 15:34:33.076254 nadl-1.4.0/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.4.0/src/nadl/images.py
+-rw-r--r--   0        0        0     3483 2024-05-18 03:07:59.101302 nadl-1.4.0/src/nadl/keys.py
+-rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.4.0/src/nadl/loops.py
+-rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.4.0/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.4.0/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.4.0/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.4.0/src/nadl/py.typed
+-rw-r--r--   0        0        0     3884 2024-05-15 03:21:02.151713 nadl-1.4.0/src/nadl/states.py
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.4.0/src/nadl/transformers.py
+-rw-r--r--   0        0        0     2363 2024-05-14 05:16:59.307787 nadl-1.4.0/src/nadl/utils.py
+-rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 nadl-1.4.0/PKG-INFO
```

### Comparing `nadl-1.3.0/pyproject.toml` & `nadl-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,26 @@
     "optax>=0.2.2",
     "equinox>=0.11.4",
     "beartype>=0.18.5",
     "scikit-image>=0.23.2",
     "orbax-checkpoint>=0.5.11",
 ]
 requires-python = ">=3.12"
-version = "1.3.0"
+version = "1.4.0"
 
 [project.readme]
 content-type = "text/plain"
 file = "readme.org"
 
 [project.license]
 text = "GPLv3"
 
 [project.optional-dependencies]
 doc = [
-    "mkdocs-material>=9.5.22",
+    "mkdocs-material>=9.5.24",
     "mkdocs>=1.6.0",
     "mike>=2.1.1",
     "mkdocstrings[python]>=0.25.1",
 ]
 
 [build-system]
 requires = [
```

### Comparing `nadl-1.3.0/readme.org` & `nadl-1.4.0/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.3.0/src/nadl/__init__.py` & `nadl-1.4.0/src/nadl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 from .states import BaseTrainState, state_fn
 from .utils import (
     classit,
     rle,
     rle_array,
 )
 
-__version__ = "1.3.0"
+__version__ = "1.4.0"
 
 __all__ = [
   "PG",
   "SCALER",
   "BaseTrainState",
   "DState",
   "IdxDataloader",
```

### Comparing `nadl-1.3.0/src/nadl/blocks.py` & `nadl-1.4.0/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.3.0/src/nadl/data.py` & `nadl-1.4.0/src/nadl/data.py`

 * *Files 23% similar despite different names*

```diff
@@ -36,153 +36,142 @@
 """
 
 from collections.abc import Callable, Iterator
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
-from equinox import tree_at
+from equinox import field, tree_at
+
+from typing import NamedTuple
 
 from .keys import Keys
-from .loops import PG
+from .loops import PG, RESC, PGThread
 
 
-class DState[T](eqx.Module):
+class DState[T](NamedTuple):
   """Dataloader state."""
 
   xs: T
-  pad: int | None = None
-  epoch: int | None = None
-  step: int | None = None
+  pad: jax.Array
+  shape: tuple[int, ...]
+  epoch: jax.Array = field(default_factory=lambda: jnp.array(0))
+  step: jax.Array = field(default_factory=lambda: jnp.array(0))
   name: str | None = None
 
 
 class IdxDataloader[T](eqx.Module):
-  """Simple index dataloader.
-
-  Provide indexes only dataloader for dataset.
-  """
+  """Simple index dataloader."""
 
   length: int
-  key: Keys
-  batch_size: int = 1
-  shuffle: bool = False
-  drop_last: bool = False
-  auto_pad: bool = True
-  transform: Callable[[jax.Array], T] | None = None
+  pad: int
+  batch_size: int
+  drop_num: int = 0
+  transform: Callable[[jax.Array], T] = eqx.field(static=True, init=False)
 
   def __init__(
     self,
     length: int,
-    batch_size: int = 1,
-    shuffle: bool = False,
+    batch_size: int,
     drop_last: bool = False,
-    auto_pad: bool = False,
-    key: jax.Array | None = None,
-    transform: Callable[[jax.Array], T] | None = None,
+    transform: Callable[[jax.Array], T] = lambda x: x,
   ) -> None:
     """Initiate the dataloader."""
     self.length = length
-    self.batch_size = batch_size
-    self.shuffle = shuffle
-    self.drop_last = drop_last
-    self.auto_pad = auto_pad
-    self.key = Keys.from_int_or_key(key or 42)
-    self.transform = transform
 
-  def __call__(self, ki: int) -> Iterator[DState[T]]:
-    """Get the indexes."""
-    idxes = (
-      jax.random.permutation(self.key(ki)[1], self.length)
-      if self.shuffle
-      else jnp.arange(self.length)
-    )
-    length = (
-      self.length if not self.drop_last else self.length - self.length % self.batch_size
-    )
+    if drop_last:
+      self.drop_num = self.length % batch_size
 
-    pad = (
-      (self.batch_size - r) % self.batch_size if (r := length % self.batch_size) else 0
-    )
-    pad = pad if pad != self.batch_size else 0
+    length = length if not drop_last else length - length % batch_size
+    pad = (batch_size - r) % batch_size if (r := length % batch_size) else 0
+    self.pad = pad = pad if pad != batch_size else 0
 
-    # use -1 as padding placeholder
-    idxes = jnp.r_[idxes, jnp.full(pad, -1, idxes.dtype)]
+    self.batch_size = batch_size
+    self.transform = transform
 
-    idxes = idxes[: length + pad].reshape(-1, self.batch_size)
+  @eqx.filter_jit
+  def __call__(self, key: jax.Array | None = None) -> DState[T]:
+    """Get the indexes."""
+    if key is None:
+      idxes = jnp.arange(self.length)
+    else:
+      idxes = jax.random.permutation(key, self.length)
+    length = self.length if not self.drop_num else self.length - self.drop_num
 
-    for i in idxes:
-      ii = i
-      if pad and not self.auto_pad and (ii == -1).any():
-        ii = ii[ii != -1]
-      xs = self.transform(ii) if self.transform else ii
-      yield DState(xs, pad if ((ii == -1).any() and self.auto_pad) else None)
-
-  def __len__(self) -> int:
-    """Length."""
-    if self.drop_last:
-      return self.length // self.batch_size
-    return (self.length + self.batch_size - 1) // self.batch_size
+    idxes = jnp.r_[idxes, jnp.full(self.pad, -1, idxes.dtype)]
+    idxes = idxes[: length + self.pad].reshape(-1, self.batch_size)
+    return DState(self.transform(idxes), jnp.where(idxes == -1, 1, 0), idxes.shape)
 
 
 def es_loop[T](
   loader: IdxDataloader[T],
   pg: PG,
+  keys: Keys | None = None,
   epochs: int = 2,
   start_epoch: int = 1,
   prefix: str = "L",
   es: str = "E",
   ss: str = "S",
 ) -> Iterator[DState[T]]:
   """Simple epoch loop."""
   es, ss = f"{prefix}-{es}", f"{prefix}-{ss}"
+  assert epochs > 0, "Epochs should be greater than 0."
   if epochs > 1:
     if es in pg.tasks:
       pg.pg.reset(pg.tasks[es])
     else:
       pg.add_task(es, total=epochs, res="")
     pg.advance(pg.tasks[es], start_epoch - 1)
 
+  vdl = eqx.filter_jit(eqx.filter_vmap(loader, axis_size=1))
+  if keys:
+    keys.reverse(epochs)
+  ds: DState[T] = vdl() if keys is None else vdl(keys(jnp.arange(epochs)))
+  ds = tree_at(lambda d: d.name, ds, prefix, is_leaf=lambda x: x is None)
+
   if ss in pg.tasks:
     pg.pg.reset(pg.tasks[ss])
   else:
-    pg.add_task(ss, total=len(loader) * epochs, res="")
-  pg.advance(pg.tasks[ss], (start_step := max((start_epoch - 1), 0) * len(loader)))
+    pg.add_task(ss, total=ds.shape[0] * epochs, res="")
+  pg.advance(pg.tasks[ss], (start_step := max((start_epoch - 1), 0) * ds.shape[0]))
 
-  for i in range(start_epoch, epochs + 1):
-    for ii, ds in enumerate(loader(i), start_step):
-      yield tree_at(
-        lambda x: (x.epoch, x.step, x.name),
-        ds,
-        (i, (i - 1) * len(loader) + ii + 1, prefix),
-        is_leaf=lambda x: x is None,
-      )
-      pg.advance(pg.tasks[ss])
-    if epochs > 1:
-      pg.advance(pg.tasks[es])
+  @eqx.filter_jit
+  def _select(ds: DState[T], i: jax.Array, ii: jax.Array) -> DState[T]:
+    return tree_at(
+      lambda x: (x.epoch, x.step),
+      jax.tree.map(lambda x: x[i, ii] if isinstance(x, jax.Array) else x, ds),
+      (i, i * ds.shape[0] + ii),
+    )
+
+  with PGThread(pg.pg, pg.tasks[ss]) as pts, PGThread(pg.pg, pg.tasks[es]) as pte:
+    for i in jnp.arange(start_epoch, epochs + 1):
+      # nds = loader(keys and keys(i) or None)
+      for ii in jnp.arange(start_step, ds.shape[0]):
+        yield _select(ds, i, ii)
+        pts.completed += 1
+      if epochs > 1:
+        pte.completed += 1
 
 
 def __test() -> None:
   """Test."""
-  pg = PG.init_progress()
+  pg = PG.init_progress(extra_columns=(RESC,))
+  keys = Keys.from_int_or_key(42)
   with pg:
     pg.console.print("Drop Last: False, Auto Pad: True")
-    dl = IdxDataloader(10, 3, shuffle=True, drop_last=False, auto_pad=True)
-    for i in es_loop(dl, pg, prefix="DFAT"):
-      pg.update_res("DFAT-S", {"epoch": i.epoch, "step": i.step, "name": i.name})
-      pg.console.print(i, i.xs)
-    pg.console.print("Drop Last: False, Auto Pad: False")
-    dl = IdxDataloader(10, 3, shuffle=True, drop_last=False, auto_pad=False)
-    for i in es_loop(dl, pg, prefix="DFAF"):
-      pg.console.print(i, i.xs)
-    pg.console.print("Drop Last: True, Auto Pad: False")
-    dl = IdxDataloader(10, 3, shuffle=False, drop_last=True, auto_pad=False)
-    for i in es_loop(dl, pg, prefix="DTAF"):
-      pg.console.print(i, i.xs)
+    dl = IdxDataloader(10, 3, drop_last=False)
+
+    for i in es_loop(dl, pg, epochs=2, prefix="DFAT"):
+      pg.update_res(
+        "DFAT-S", {"epoch": i.epoch.item(), "step": i.step.item(), "name": i.name}
+      )
+      pg.console.print(i)
+      continue
+    pg.console.print(i)
     pg.console.print("Drop Last: True, Auto Pad: True")
-    dl = IdxDataloader(10, 3, shuffle=False, drop_last=True, auto_pad=True)
-    for i in es_loop(dl, pg, prefix="DTAT"):
-      pg.console.print(i, i.xs)
+    dl = IdxDataloader(10, 3, drop_last=True)
+    for i in es_loop(dl, pg, keys, prefix="DTAT"):
+      pg.console.print(i)
 
 
 if __name__ == "__main__":
   __test()
```

### Comparing `nadl-1.3.0/src/nadl/images.py` & `nadl-1.4.0/src/nadl/images.py`

 * *Files identical despite different names*

### Comparing `nadl-1.3.0/src/nadl/loops.py` & `nadl-1.4.0/src/nadl/states.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,145 +22,123 @@
     |  ___|______( (____|______|______|______|____
     |  ______|____\_|______|______|______|______|_
     |  ___|______|______|______|______|______|____
     |  ______|______|______|______|______|______|_
     |  ___|______|______|______|______|______|____
 
 author   : Nasy https://nasy.moe
-date     : Nov 30, 2023
+date     : May 14, 2024
 email    : Nasy <nasyxx+python@gmail.com>
-filename : loops.py
+filename : states.py
 project  : nadl
 license  : GPL-3.0+
 
-Train Eval Loops
+States
 """
 
-from collections.abc import Hashable, Mapping
+from __future__ import annotations
 
-from equinox import Module
+import shutil
+from abc import abstractmethod
 
-from types import TracebackType
-from typing import Any, Self
+import equinox as eqx
+import optax
+import orbax.checkpoint as ocp
 
-from rich.console import Console
-from rich.progress import (
-  BarColumn,
-  Progress,
-  ProgressColumn,
-  TaskID,
-  TextColumn,
-  TimeElapsedColumn,
-  TimeRemainingColumn,
-)
-from rich.theme import Theme
-
-from .utils import pformat
-
-DEF_LIGHT_THEME = Theme({
-  "bar.back": "#50616D",
-  "bar.complete": "#D3CBAF",
-  "bar.finished": "#b49b7f",
-})
-
-
-class PG(Module):
-  """Progress."""
-
-  pg: Progress
-  console: Console
-  tasks: dict[Hashable, TaskID]
+from typing import TYPE_CHECKING, cast
 
-  @classmethod
-  def init_progress(
-    cls: type[Self],
-    pg: Progress | None = None,
-    console: Console | None = None,
-    total: bool = True,
-    bar_width: int | None = 20,
-    extra_columns: tuple[ProgressColumn, ...] = (),
-    show_progress: bool = True,
-    theme: Theme | None = None,
-  ) -> Self:
-    """Init progress bar."""
-    if console is None:
-      console = Console(theme=theme or DEF_LIGHT_THEME)
-    if pg is None:
-      pg = Progress(
-        TextColumn(
-          "{task.description}" + " - {task.completed}/{task.total}" if total else ""
-        ),
-        TimeRemainingColumn(),
-        TimeElapsedColumn(),
-        BarColumn(bar_width),
-        TextColumn("{task.fields[res]}"),
-        console=console,
-        disable=not show_progress,
-      )
-    pg.columns += extra_columns
-    return cls(pg, console, {})
-
-  def add_columns(self, columns: tuple[ProgressColumn, ...]) -> Self:
-    """Add columns."""
-    self.pg.columns += columns
-    return self
-
-  def add_task(
-    self,
-    description: str,
-    start: bool = True,
-    total: float | None = 100,
-    completed: int = 0,
-    visible: bool = True,
-    **fileds: Any,  # noqa: ANN401
-  ) -> TaskID:
-    """Add task."""
-    task = self.pg.add_task(
-      description,
-      start=start,
-      total=total,
-      completed=completed,
-      visible=visible,
-      **fileds,
-    )
-    self.tasks[description] = task
-    return task
+if TYPE_CHECKING:
+  from collections.abc import Callable
+  from pathlib import Path
 
-  def advance(self, task: TaskID, advance: float = 1) -> None:
-    """Advance task."""
-    self.pg.advance(task, advance=advance)
-
-  def __enter__(self) -> Progress:
-    """Enter."""
-    return self.pg.__enter__()
-
-  def __exit__(
-    self,
-    exc_type: type[BaseException] | None,
-    exc_val: BaseException | None,
-    exc_tb: TracebackType | None,
-  ) -> None:
-    """Exit."""
-    self.pg.__exit__(exc_type, exc_val, exc_tb)
+  import jax
 
-  def update_res(
-    self, name: str, updates: Mapping[str, float | int | str | None]
-  ) -> None:
-    """Update res."""
-    if name in self.tasks:
-      self.pg.update(self.tasks[name], res=pformat(updates))
+  from jaxtyping import PyTree
 
+  from rich.console import Console
 
-def test() -> None:
-  """Test progress."""
-  import time  # noqa: PLC0415
 
-  pg = PG.init_progress()
-  with pg:
-    t0 = pg.add_task("Task 0", total=100)
-    for _i in range(100):
-      pg.advance(t0)
-      time.sleep(0.5)
+class BaseTrainState[T](eqx.Module):
+  """Train state."""
 
+  model: eqx.Module
+  tx: optax.GradientTransformation
+  opt_state: optax.OptState
+  loss: jax.Array
+  step: jax.Array
+  conf: T | None = None
+
+  @classmethod
+  @abstractmethod
+  def create[**P](
+    cls: type[BaseTrainState[T]], *args: P.args, **kwds: P.kwargs
+  ) -> BaseTrainState[T]:
+    """Create state."""
+    raise NotImplementedError
+
+  def apply_grads(self, loss: jax.Array, grads: eqx.Module) -> BaseTrainState[T]:
+    """Apply gradients."""
+    updates, opt_state = self.tx.update(
+      cast(optax.Updates, grads), self.opt_state, params=cast(optax.Params, self.model)
+    )
+    model = eqx.apply_updates(self.model, updates)
+    return eqx.tree_at(
+      lambda x: (x.model, x.opt_state, x.loss, x.step),
+      self,
+      (model, opt_state, loss, self.step + 1),
+    )
+
+
+def state_fn(
+  rpath: Path,
+  console: Console | None = None,
+  keeps: int = 5,
+  clean: bool = False,
+  item_names: tuple[str, ...] | None = None,
+  item_handlers: dict | None = None,
+  best_fn: Callable[[PyTree], float] | None = None,
+) -> tuple[
+  ocp.CheckpointManager, Callable[[int, BaseTrainState, dict[str, float] | None], None]
+]:
+  """Get states manager."""
+  match (item_names, item_handlers):
+    case (None, None):
+      item_names = ("state", "extra_metadata")
+      item_handlers = {
+        "state": ocp.StandardCheckpointHandler(),
+        "extra_metadata": ocp.JsonCheckpointHandler(),
+      }
+    case _ if item_names and item_handlers:
+      for i in item_names:
+        assert i in item_handlers, f"Item {i} not in item_handlers."
+    case _:
+      raise ValueError("item_names and item_handlers should be both None or not None.")
+
+  if console:
+    console.log(f"Checkpoint path at {rpath}")
+  if rpath.exists() and clean:
+    if console:
+      console.log("Cleaning up checkpoint...")
+    shutil.rmtree(rpath)
+
+  mngr = ocp.CheckpointManager(
+    rpath,
+    options=ocp.CheckpointManagerOptions(
+      max_to_keep=keeps, save_interval_steps=1, best_fn=best_fn
+    ),
+    item_names=item_names,
+    item_handlers=item_handlers,
+  )
+
+  def save(
+    step: int, state: BaseTrainState, metadata: dict[str, float] | None = None
+  ) -> None:
+    """Save state."""
+    mngr.save(
+      step,
+      args=ocp.args.Composite(
+        state=ocp.args.StandardSave(state),  # type: ignore
+        extra_metadata=ocp.args.JsonSave(metadata or {}),  # type: ignore
+      ),
+    )
 
-if __name__ == "__main__":
-  test()
+  return mngr, save
```

### Comparing `nadl-1.3.0/src/nadl/metrics.py` & `nadl-1.4.0/src/nadl/metrics.py`

 * *Files identical despite different names*

### Comparing `nadl-1.3.0/src/nadl/nets.py` & `nadl-1.4.0/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.3.0/src/nadl/preprocessing.py` & `nadl-1.4.0/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.3.0/src/nadl/transformers.py` & `nadl-1.4.0/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.3.0/src/nadl/utils.py` & `nadl-1.4.0/src/nadl/utils.py`

 * *Files identical despite different names*

### Comparing `nadl-1.3.0/PKG-INFO` & `nadl-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.3.0
+Version: 1.4.0
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
 Requires-Python: >=3.12
 Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
 Requires-Dist: jaxtyping>=0.2.28
 Requires-Dist: optax>=0.2.2
 Requires-Dist: equinox>=0.11.4
 Requires-Dist: beartype>=0.18.5
 Requires-Dist: scikit-image>=0.23.2
 Requires-Dist: orbax-checkpoint>=0.5.11
-Requires-Dist: mkdocs-material>=9.5.22; extra == "doc"
+Requires-Dist: mkdocs-material>=9.5.24; extra == "doc"
 Requires-Dist: mkdocs>=1.6.0; extra == "doc"
 Requires-Dist: mike>=2.1.1; extra == "doc"
 Requires-Dist: mkdocstrings[python]>=0.25.1; extra == "doc"
 Provides-Extra: doc
 Description-Content-Type: text/plain
 
 #+options: ':nil *:t -:t ::t <:t H:3 \n:nil ^:{} arch:headline
```

