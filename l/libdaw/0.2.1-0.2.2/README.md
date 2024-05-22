# Comparing `tmp/libdaw-0.2.1.tar.gz` & `tmp/libdaw-0.2.2.tar.gz`

## Comparing `libdaw-0.2.1.tar` & `libdaw-0.2.2.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0     1001      127      427 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/Cargo.toml
--rw-r--r--   0     1001      127     1589 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/lib.rs
--rw-r--r--   0     1001      127      281 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/metronome/parse.rs
--rw-r--r--   0     1001      127     9873 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/metronome.rs
--rw-r--r--   0     1001      127      531 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes/add.rs
--rw-r--r--   0     1001      127      870 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes/constant_value.rs
--rw-r--r--   0     1001      127     1987 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes/delay.rs
--rw-r--r--   0     1001      127     2253 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes/detune.rs
--rw-r--r--   0     1001      127     4867 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes/envelope.rs
--rw-r--r--   0     1001      127      806 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes/gain.rs
--rw-r--r--   0     1001      127     1045 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes/graph/error.rs
--rw-r--r--   0     1001      127    17261 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes/graph.rs
--rw-r--r--   0     1001      127     6778 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes/instrument.rs
--rw-r--r--   0     1001      127     1195 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes/multi_frequency.rs
--rw-r--r--   0     1001      127      564 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes/multiply.rs
--rw-r--r--   0     1001      127      462 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes/passthrough.rs
--rw-r--r--   0     1001      127     1783 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes/sawtooth_oscillator.rs
--rw-r--r--   0     1001      127     1688 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes/sine_oscillator.rs
--rw-r--r--   0     1001      127     2172 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes/square_oscillator.rs
--rw-r--r--   0     1001      127     1806 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes/triangle_oscillator.rs
--rw-r--r--   0     1001      127      802 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/nodes.rs
--rw-r--r--   0     1001      127      965 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/chord/parse.rs
--rw-r--r--   0     1001      127     3007 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/chord.rs
--rw-r--r--   0     1001      127      440 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/inversion/parse.rs
--rw-r--r--   0     1001      127      763 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/inversion.rs
--rw-r--r--   0     1001      127     1197 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/item/parse.rs
--rw-r--r--   0     1001      127     5787 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/item.rs
--rw-r--r--   0     1001      127      897 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/note/parse.rs
--rw-r--r--   0     1001      127     4136 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/note.rs
--rw-r--r--   0     1001      127      689 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/overlapped/parse.rs
--rw-r--r--   0     1001      127     2134 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/overlapped.rs
--rw-r--r--   0     1001      127      798 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/pitch/parse.rs
--rw-r--r--   0     1001      127     1872 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/pitch.rs
--rw-r--r--   0     1001      127     1583 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/resolve_state.rs
--rw-r--r--   0     1001      127      329 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/rest/parse.rs
--rw-r--r--   0     1001      127     1104 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/rest.rs
--rw-r--r--   0     1001      127      679 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/scale/parse.rs
--rw-r--r--   0     1001      127     1110 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/scale.rs
--rw-r--r--   0     1001      127      679 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/sequence/parse.rs
--rw-r--r--   0     1001      127     2707 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/sequence.rs
--rw-r--r--   0     1001      127      575 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/step/parse.rs
--rw-r--r--   0     1001      127     2155 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation/step.rs
--rw-r--r--   0     1001      127      387 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/notation.rs
--rw-r--r--   0     1001      127     1566 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/parse.rs
--rw-r--r--   0     1001      127     2192 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/pitch/parse.rs
--rw-r--r--   0     1001      127     6415 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/pitch.rs
--rw-r--r--   0     1001      127     1726 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/stream/iter.rs
--rw-r--r--   0     1001      127     5784 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/stream.rs
--rw-r--r--   0     1001      127     1622 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/sync.rs
--rw-r--r--   0     1001      127     2361 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/time/duration.rs
--rw-r--r--   0     1001      127     2115 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/time/time.rs
--rw-r--r--   0     1001      127     3185 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/time/timestamp.rs
--rw-r--r--   0     1001      127      172 2024-05-21 22:17:43.000000 libdaw-0.2.1/libdaw/src/time.rs
--rw-r--r--   0     1001      127       95 2024-05-21 22:17:43.000000 libdaw-0.2.1/README.md
--rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 libdaw-0.2.1/python-libdaw/Cargo.toml
--rw-r--r--   0     1001      127     3526 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/.gitignore
--rw-r--r--   0     1001      127        6 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/doc/.gitignore
--rw-r--r--   0     1001      127      638 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/doc/Makefile
--rw-r--r--   0     1001      127      804 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/doc/make.bat
--rw-r--r--   0     1001      127      967 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/doc/source/conf.py
--rw-r--r--   0     1001      127      445 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/doc/source/index.rst
--rw-r--r--   0     1001      127      166 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/doc/source/libdaw/metronome.rst
--rw-r--r--   0     1001      127      180 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/doc/source/libdaw/nodes/envelope.rst
--rw-r--r--   0     1001      127      173 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/doc/source/libdaw/nodes/graph.rst
--rw-r--r--   0     1001      127      187 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/doc/source/libdaw/nodes/instrument.rst
--rw-r--r--   0     1001      127      200 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/doc/source/libdaw/nodes.rst
--rw-r--r--   0     1001      127      112 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/doc/source/libdaw/notation.rst
--rw-r--r--   0     1001      127      153 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/doc/source/libdaw/pitch.rst
--rw-r--r--   0     1001      127      152 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/doc/source/libdaw/time.rst
--rw-r--r--   0     1001      127      211 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/doc/source/libdaw.rst
--rw-r--r--   0     1001      127     1780 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/examples/1564.py
--rw-r--r--   0     1001      127     1662 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/examples/blues.py
--rwxr-xr-x   0     1001      127     1689 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/examples/instrument-test.py
--rw-r--r--   0     1001      127     1489 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/examples/pachelbel-canon-progression.py
--rw-r--r--   0     1001      127     1580 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/examples/round.py
--rw-r--r--   0     1001      127     1526 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/examples/scale-inversion-notation.py
--rw-r--r--   0     1001      127     1482 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/examples/simple-notation.py
--rw-r--r--   0     1001      127     1389 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/examples/simple-scale-notation.py
--rw-r--r--   0     1001      127      169 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/python/libdaw/__init__.py
--rw-r--r--   0     1001      127      980 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/python/libdaw/__init__.pyi
--rw-r--r--   0     1001      127     1588 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/python/libdaw/metronome.pyi
--rw-r--r--   0     1001      127     2528 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/python/libdaw/nodes/__init__.pyi
--rw-r--r--   0     1001      127      173 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/python/libdaw/nodes/envelope.pyi
--rw-r--r--   0     1001      127       23 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/python/libdaw/nodes/graph.pyi
--rw-r--r--   0     1001      127      151 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/python/libdaw/nodes/instrument.pyi
--rw-r--r--   0     1001      127     6173 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/python/libdaw/notation.pyi
--rw-r--r--   0     1001      127     1061 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/python/libdaw/pitch.pyi
--rw-r--r--   0     1001      127        0 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/python/libdaw/py.typed
--rw-r--r--   0     1001      127     1497 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/python/libdaw/time.pyi
--rw-r--r--   0     1001      127      491 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/frequency_node.rs
--rw-r--r--   0     1001      127     3052 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/lib.rs
--rw-r--r--   0     1001      127     4670 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/metronome.rs
--rw-r--r--   0     1001      127     1029 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/node.rs
--rw-r--r--   0     1001      127      514 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/nodes/add.rs
--rw-r--r--   0     1001      127      580 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/nodes/constant_value.rs
--rw-r--r--   0     1001      127      586 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/nodes/delay.rs
--rw-r--r--   0     1001      127      845 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/nodes/detune.rs
--rw-r--r--   0     1001      127     1868 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/nodes/envelope.rs
--rw-r--r--   0     1001      127      644 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/nodes/gain.rs
--rw-r--r--   0     1001      127     4554 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/nodes/graph.rs
--rw-r--r--   0     1001      127     2715 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/nodes/instrument.rs
--rw-r--r--   0     1001      127      672 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/nodes/multi_frequency.rs
--rw-r--r--   0     1001      127      534 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/nodes/multiply.rs
--rw-r--r--   0     1001      127      489 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/nodes/passthrough.rs
--rw-r--r--   0     1001      127      756 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/nodes/sawtooth_oscillator.rs
--rw-r--r--   0     1001      127      705 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/nodes/sine_oscillator.rs
--rw-r--r--   0     1001      127      748 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/nodes/square_oscillator.rs
--rw-r--r--   0     1001      127      756 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/nodes/triangle_oscillator.rs
--rw-r--r--   0     1001      127     1787 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/nodes.rs
--rw-r--r--   0     1001      127     6257 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/notation/chord.rs
--rw-r--r--   0     1001      127     1472 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/notation/inversion.rs
--rw-r--r--   0     1001      127     4459 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/notation/item.rs
--rw-r--r--   0     1001      127     1982 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/notation/note/note_pitch.rs
--rw-r--r--   0     1001      127     3895 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/notation/note.rs
--rw-r--r--   0     1001      127     5383 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/notation/overlapped.rs
--rw-r--r--   0     1001      127     2936 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/notation/pitch.rs
--rw-r--r--   0     1001      127     1561 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/notation/rest.rs
--rw-r--r--   0     1001      127     4458 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/notation/scale.rs
--rw-r--r--   0     1001      127     5218 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/notation/sequence.rs
--rw-r--r--   0     1001      127     1983 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/notation/step.rs
--rw-r--r--   0     1001      127      926 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/notation.rs
--rw-r--r--   0     1001      127     5708 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/pitch/pitch.rs
--rw-r--r--   0     1001      127     3014 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/pitch.rs
--rw-r--r--   0     1001      127     2178 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/play.rs
--rw-r--r--   0     1001      127     2658 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/stream.rs
--rw-r--r--   0     1001      127     5689 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/src/time.rs
--rw-r--r--   0     1001      127        0 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/test/__init__.py
--rw-r--r--   0     1001      127      471 2024-05-21 22:17:43.000000 libdaw-0.2.1/python-libdaw/test/test_pitch.py
--rw-r--r--   0     1001      127    30727 2024-05-21 22:17:49.000000 libdaw-0.2.1/Cargo.lock
--rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 libdaw-0.2.1/Cargo.toml
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 libdaw-0.2.1/pyproject.toml
--rw-r--r--   0     1001      127     6173 2024-05-21 22:17:43.000000 libdaw-0.2.1/python/libdaw/notation.pyi
--rw-r--r--   0     1001      127      169 2024-05-21 22:17:43.000000 libdaw-0.2.1/python/libdaw/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-21 22:17:43.000000 libdaw-0.2.1/python/libdaw/py.typed
--rw-r--r--   0     1001      127     1061 2024-05-21 22:17:43.000000 libdaw-0.2.1/python/libdaw/pitch.pyi
--rw-r--r--   0     1001      127     1497 2024-05-21 22:17:43.000000 libdaw-0.2.1/python/libdaw/time.pyi
--rw-r--r--   0     1001      127      980 2024-05-21 22:17:43.000000 libdaw-0.2.1/python/libdaw/__init__.pyi
--rw-r--r--   0     1001      127     1588 2024-05-21 22:17:43.000000 libdaw-0.2.1/python/libdaw/metronome.pyi
--rw-r--r--   0     1001      127      151 2024-05-21 22:17:43.000000 libdaw-0.2.1/python/libdaw/nodes/instrument.pyi
--rw-r--r--   0     1001      127       23 2024-05-21 22:17:43.000000 libdaw-0.2.1/python/libdaw/nodes/graph.pyi
--rw-r--r--   0     1001      127      173 2024-05-21 22:17:43.000000 libdaw-0.2.1/python/libdaw/nodes/envelope.pyi
--rw-r--r--   0     1001      127     2528 2024-05-21 22:17:43.000000 libdaw-0.2.1/python/libdaw/nodes/__init__.pyi
--rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 libdaw-0.2.1/PKG-INFO
+-rw-r--r--   0     1001      127      427 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/Cargo.toml
+-rw-r--r--   0     1001      127     1589 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/lib.rs
+-rw-r--r--   0     1001      127      281 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/metronome/parse.rs
+-rw-r--r--   0     1001      127     9873 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/metronome.rs
+-rw-r--r--   0     1001      127      531 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes/add.rs
+-rw-r--r--   0     1001      127      870 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes/constant_value.rs
+-rw-r--r--   0     1001      127     1987 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes/delay.rs
+-rw-r--r--   0     1001      127     2253 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes/detune.rs
+-rw-r--r--   0     1001      127     4867 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes/envelope.rs
+-rw-r--r--   0     1001      127      806 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes/gain.rs
+-rw-r--r--   0     1001      127     1045 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes/graph/error.rs
+-rw-r--r--   0     1001      127    17261 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes/graph.rs
+-rw-r--r--   0     1001      127     6778 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes/instrument.rs
+-rw-r--r--   0     1001      127     1195 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes/multi_frequency.rs
+-rw-r--r--   0     1001      127      564 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes/multiply.rs
+-rw-r--r--   0     1001      127      462 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes/passthrough.rs
+-rw-r--r--   0     1001      127     1783 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes/sawtooth_oscillator.rs
+-rw-r--r--   0     1001      127     1688 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes/sine_oscillator.rs
+-rw-r--r--   0     1001      127     2172 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes/square_oscillator.rs
+-rw-r--r--   0     1001      127     1806 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes/triangle_oscillator.rs
+-rw-r--r--   0     1001      127      802 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/nodes.rs
+-rw-r--r--   0     1001      127      965 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/chord/parse.rs
+-rw-r--r--   0     1001      127     3007 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/chord.rs
+-rw-r--r--   0     1001      127      440 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/inversion/parse.rs
+-rw-r--r--   0     1001      127      763 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/inversion.rs
+-rw-r--r--   0     1001      127     1197 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/item/parse.rs
+-rw-r--r--   0     1001      127     5787 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/item.rs
+-rw-r--r--   0     1001      127      897 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/note/parse.rs
+-rw-r--r--   0     1001      127     4136 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/note.rs
+-rw-r--r--   0     1001      127      689 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/overlapped/parse.rs
+-rw-r--r--   0     1001      127     2134 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/overlapped.rs
+-rw-r--r--   0     1001      127      798 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/pitch/parse.rs
+-rw-r--r--   0     1001      127     1872 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/pitch.rs
+-rw-r--r--   0     1001      127     1583 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/resolve_state.rs
+-rw-r--r--   0     1001      127      329 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/rest/parse.rs
+-rw-r--r--   0     1001      127     1104 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/rest.rs
+-rw-r--r--   0     1001      127      679 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/scale/parse.rs
+-rw-r--r--   0     1001      127     1110 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/scale.rs
+-rw-r--r--   0     1001      127      679 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/sequence/parse.rs
+-rw-r--r--   0     1001      127     2707 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/sequence.rs
+-rw-r--r--   0     1001      127      575 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/step/parse.rs
+-rw-r--r--   0     1001      127     2155 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation/step.rs
+-rw-r--r--   0     1001      127      387 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/notation.rs
+-rw-r--r--   0     1001      127     1566 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/parse.rs
+-rw-r--r--   0     1001      127     2192 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/pitch/parse.rs
+-rw-r--r--   0     1001      127     6415 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/pitch.rs
+-rw-r--r--   0     1001      127     1726 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/stream/iter.rs
+-rw-r--r--   0     1001      127     5784 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/stream.rs
+-rw-r--r--   0     1001      127     1622 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/sync.rs
+-rw-r--r--   0     1001      127     2361 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/time/duration.rs
+-rw-r--r--   0     1001      127     2115 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/time/time.rs
+-rw-r--r--   0     1001      127     3185 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/time/timestamp.rs
+-rw-r--r--   0     1001      127      172 2024-05-22 01:31:38.000000 libdaw-0.2.2/libdaw/src/time.rs
+-rw-r--r--   0     1001      127       95 2024-05-22 01:31:38.000000 libdaw-0.2.2/README.md
+-rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 libdaw-0.2.2/python-libdaw/Cargo.toml
+-rw-r--r--   0     1001      127     3526 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/.gitignore
+-rw-r--r--   0     1001      127        6 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/doc/.gitignore
+-rw-r--r--   0     1001      127      638 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/doc/Makefile
+-rw-r--r--   0     1001      127      804 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/doc/make.bat
+-rw-r--r--   0     1001      127      967 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/doc/source/conf.py
+-rw-r--r--   0     1001      127      445 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/doc/source/index.rst
+-rw-r--r--   0     1001      127      166 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/doc/source/libdaw/metronome.rst
+-rw-r--r--   0     1001      127      180 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/doc/source/libdaw/nodes/envelope.rst
+-rw-r--r--   0     1001      127      173 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/doc/source/libdaw/nodes/graph.rst
+-rw-r--r--   0     1001      127      187 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/doc/source/libdaw/nodes/instrument.rst
+-rw-r--r--   0     1001      127      200 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/doc/source/libdaw/nodes.rst
+-rw-r--r--   0     1001      127      112 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/doc/source/libdaw/notation.rst
+-rw-r--r--   0     1001      127      153 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/doc/source/libdaw/pitch.rst
+-rw-r--r--   0     1001      127      152 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/doc/source/libdaw/time.rst
+-rw-r--r--   0     1001      127      211 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/doc/source/libdaw.rst
+-rw-r--r--   0     1001      127     1780 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/examples/1564.py
+-rw-r--r--   0     1001      127     1662 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/examples/blues.py
+-rwxr-xr-x   0     1001      127     1689 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/examples/instrument-test.py
+-rw-r--r--   0     1001      127     1489 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/examples/pachelbel-canon-progression.py
+-rw-r--r--   0     1001      127     1576 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/examples/round.py
+-rw-r--r--   0     1001      127     1526 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/examples/scale-inversion-notation.py
+-rw-r--r--   0     1001      127     1482 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/examples/simple-notation.py
+-rw-r--r--   0     1001      127     1389 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/examples/simple-scale-notation.py
+-rw-r--r--   0     1001      127      169 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/python/libdaw/__init__.py
+-rw-r--r--   0     1001      127      980 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/python/libdaw/__init__.pyi
+-rw-r--r--   0     1001      127     1588 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/python/libdaw/metronome.pyi
+-rw-r--r--   0     1001      127     2528 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/python/libdaw/nodes/__init__.pyi
+-rw-r--r--   0     1001      127      173 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/python/libdaw/nodes/envelope.pyi
+-rw-r--r--   0     1001      127       23 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/python/libdaw/nodes/graph.pyi
+-rw-r--r--   0     1001      127      151 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/python/libdaw/nodes/instrument.pyi
+-rw-r--r--   0     1001      127     6173 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/python/libdaw/notation.pyi
+-rw-r--r--   0     1001      127     1061 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/python/libdaw/pitch.pyi
+-rw-r--r--   0     1001      127        0 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/python/libdaw/py.typed
+-rw-r--r--   0     1001      127     1497 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/python/libdaw/time.pyi
+-rw-r--r--   0     1001      127      491 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/frequency_node.rs
+-rw-r--r--   0     1001      127     3052 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/lib.rs
+-rw-r--r--   0     1001      127     4670 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/metronome.rs
+-rw-r--r--   0     1001      127     1029 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/node.rs
+-rw-r--r--   0     1001      127      514 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/nodes/add.rs
+-rw-r--r--   0     1001      127      580 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/nodes/constant_value.rs
+-rw-r--r--   0     1001      127      586 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/nodes/delay.rs
+-rw-r--r--   0     1001      127      845 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/nodes/detune.rs
+-rw-r--r--   0     1001      127     1868 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/nodes/envelope.rs
+-rw-r--r--   0     1001      127      644 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/nodes/gain.rs
+-rw-r--r--   0     1001      127     4554 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/nodes/graph.rs
+-rw-r--r--   0     1001      127     2715 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/nodes/instrument.rs
+-rw-r--r--   0     1001      127      672 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/nodes/multi_frequency.rs
+-rw-r--r--   0     1001      127      534 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/nodes/multiply.rs
+-rw-r--r--   0     1001      127      489 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/nodes/passthrough.rs
+-rw-r--r--   0     1001      127      756 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/nodes/sawtooth_oscillator.rs
+-rw-r--r--   0     1001      127      705 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/nodes/sine_oscillator.rs
+-rw-r--r--   0     1001      127      748 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/nodes/square_oscillator.rs
+-rw-r--r--   0     1001      127      756 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/nodes/triangle_oscillator.rs
+-rw-r--r--   0     1001      127     1787 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/nodes.rs
+-rw-r--r--   0     1001      127     6257 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/notation/chord.rs
+-rw-r--r--   0     1001      127     1472 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/notation/inversion.rs
+-rw-r--r--   0     1001      127     4459 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/notation/item.rs
+-rw-r--r--   0     1001      127     1982 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/notation/note/note_pitch.rs
+-rw-r--r--   0     1001      127     3895 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/notation/note.rs
+-rw-r--r--   0     1001      127     5383 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/notation/overlapped.rs
+-rw-r--r--   0     1001      127     2936 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/notation/pitch.rs
+-rw-r--r--   0     1001      127     1561 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/notation/rest.rs
+-rw-r--r--   0     1001      127     4458 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/notation/scale.rs
+-rw-r--r--   0     1001      127     5218 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/notation/sequence.rs
+-rw-r--r--   0     1001      127     1983 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/notation/step.rs
+-rw-r--r--   0     1001      127      926 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/notation.rs
+-rw-r--r--   0     1001      127     5708 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/pitch/pitch.rs
+-rw-r--r--   0     1001      127     3014 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/pitch.rs
+-rw-r--r--   0     1001      127     2178 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/play.rs
+-rw-r--r--   0     1001      127     2658 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/stream.rs
+-rw-r--r--   0     1001      127     5689 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/src/time.rs
+-rw-r--r--   0     1001      127        0 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/test/__init__.py
+-rw-r--r--   0     1001      127      471 2024-05-22 01:31:38.000000 libdaw-0.2.2/python-libdaw/test/test_pitch.py
+-rw-r--r--   0     1001      127    30727 2024-05-22 01:31:38.000000 libdaw-0.2.2/Cargo.lock
+-rw-r--r--   0        0        0      237 1970-01-01 00:00:00.000000 libdaw-0.2.2/Cargo.toml
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 libdaw-0.2.2/pyproject.toml
+-rw-r--r--   0     1001      127     6173 2024-05-22 01:31:38.000000 libdaw-0.2.2/python/libdaw/notation.pyi
+-rw-r--r--   0     1001      127      169 2024-05-22 01:31:38.000000 libdaw-0.2.2/python/libdaw/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-22 01:31:38.000000 libdaw-0.2.2/python/libdaw/py.typed
+-rw-r--r--   0     1001      127     1061 2024-05-22 01:31:38.000000 libdaw-0.2.2/python/libdaw/pitch.pyi
+-rw-r--r--   0     1001      127     1497 2024-05-22 01:31:38.000000 libdaw-0.2.2/python/libdaw/time.pyi
+-rw-r--r--   0     1001      127      980 2024-05-22 01:31:38.000000 libdaw-0.2.2/python/libdaw/__init__.pyi
+-rw-r--r--   0     1001      127     1588 2024-05-22 01:31:38.000000 libdaw-0.2.2/python/libdaw/metronome.pyi
+-rw-r--r--   0     1001      127      151 2024-05-22 01:31:38.000000 libdaw-0.2.2/python/libdaw/nodes/instrument.pyi
+-rw-r--r--   0     1001      127       23 2024-05-22 01:31:38.000000 libdaw-0.2.2/python/libdaw/nodes/graph.pyi
+-rw-r--r--   0     1001      127      173 2024-05-22 01:31:38.000000 libdaw-0.2.2/python/libdaw/nodes/envelope.pyi
+-rw-r--r--   0     1001      127     2528 2024-05-22 01:31:38.000000 libdaw-0.2.2/python/libdaw/nodes/__init__.pyi
+-rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 libdaw-0.2.2/PKG-INFO
```

### Comparing `libdaw-0.2.1/libdaw/src/lib.rs` & `libdaw-0.2.2/libdaw/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/metronome.rs` & `libdaw-0.2.2/libdaw/src/metronome.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/nodes/add.rs` & `libdaw-0.2.2/libdaw/src/nodes/add.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/nodes/constant_value.rs` & `libdaw-0.2.2/libdaw/src/nodes/constant_value.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/nodes/delay.rs` & `libdaw-0.2.2/libdaw/src/nodes/delay.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/nodes/detune.rs` & `libdaw-0.2.2/libdaw/src/nodes/detune.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/nodes/envelope.rs` & `libdaw-0.2.2/libdaw/src/nodes/envelope.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/nodes/gain.rs` & `libdaw-0.2.2/libdaw/src/nodes/gain.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/nodes/graph/error.rs` & `libdaw-0.2.2/libdaw/src/nodes/graph/error.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/nodes/graph.rs` & `libdaw-0.2.2/libdaw/src/nodes/graph.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/nodes/instrument.rs` & `libdaw-0.2.2/libdaw/src/nodes/instrument.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/nodes/multi_frequency.rs` & `libdaw-0.2.2/libdaw/src/nodes/multi_frequency.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/nodes/multiply.rs` & `libdaw-0.2.2/libdaw/src/nodes/multiply.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/nodes/sawtooth_oscillator.rs` & `libdaw-0.2.2/libdaw/src/nodes/sawtooth_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/nodes/sine_oscillator.rs` & `libdaw-0.2.2/libdaw/src/nodes/sine_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/nodes/square_oscillator.rs` & `libdaw-0.2.2/libdaw/src/nodes/square_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/nodes/triangle_oscillator.rs` & `libdaw-0.2.2/libdaw/src/nodes/triangle_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/nodes.rs` & `libdaw-0.2.2/libdaw/src/nodes.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/chord/parse.rs` & `libdaw-0.2.2/libdaw/src/notation/chord/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/chord.rs` & `libdaw-0.2.2/libdaw/src/notation/chord.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/inversion.rs` & `libdaw-0.2.2/libdaw/src/notation/inversion.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/item/parse.rs` & `libdaw-0.2.2/libdaw/src/notation/item/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/item.rs` & `libdaw-0.2.2/libdaw/src/notation/item.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/note/parse.rs` & `libdaw-0.2.2/libdaw/src/notation/note/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/note.rs` & `libdaw-0.2.2/libdaw/src/notation/note.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/overlapped/parse.rs` & `libdaw-0.2.2/libdaw/src/notation/overlapped/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/overlapped.rs` & `libdaw-0.2.2/libdaw/src/notation/overlapped.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/pitch/parse.rs` & `libdaw-0.2.2/libdaw/src/notation/pitch/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/pitch.rs` & `libdaw-0.2.2/libdaw/src/notation/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/resolve_state.rs` & `libdaw-0.2.2/libdaw/src/notation/resolve_state.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/rest.rs` & `libdaw-0.2.2/libdaw/src/notation/rest.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/scale/parse.rs` & `libdaw-0.2.2/libdaw/src/notation/scale/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/scale.rs` & `libdaw-0.2.2/libdaw/src/notation/scale.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/sequence/parse.rs` & `libdaw-0.2.2/libdaw/src/notation/sequence/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/sequence.rs` & `libdaw-0.2.2/libdaw/src/notation/sequence.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/step/parse.rs` & `libdaw-0.2.2/libdaw/src/notation/step/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/notation/step.rs` & `libdaw-0.2.2/libdaw/src/notation/step.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/parse.rs` & `libdaw-0.2.2/libdaw/src/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/pitch/parse.rs` & `libdaw-0.2.2/libdaw/src/pitch/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/pitch.rs` & `libdaw-0.2.2/libdaw/src/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/stream/iter.rs` & `libdaw-0.2.2/libdaw/src/stream/iter.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/stream.rs` & `libdaw-0.2.2/libdaw/src/stream.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/sync.rs` & `libdaw-0.2.2/libdaw/src/sync.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/time/duration.rs` & `libdaw-0.2.2/libdaw/src/time/duration.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/time/time.rs` & `libdaw-0.2.2/libdaw/src/time/time.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/libdaw/src/time/timestamp.rs` & `libdaw-0.2.2/libdaw/src/time/timestamp.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/.github/workflows/CI.yml` & `libdaw-0.2.2/python-libdaw/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/.gitignore` & `libdaw-0.2.2/python-libdaw/.gitignore`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/doc/Makefile` & `libdaw-0.2.2/python-libdaw/doc/Makefile`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/doc/make.bat` & `libdaw-0.2.2/python-libdaw/doc/make.bat`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/doc/source/conf.py` & `libdaw-0.2.2/python-libdaw/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/examples/1564.py` & `libdaw-0.2.2/python-libdaw/examples/1564.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/examples/blues.py` & `libdaw-0.2.2/python-libdaw/examples/blues.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/examples/instrument-test.py` & `libdaw-0.2.2/python-libdaw/examples/instrument-test.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/examples/pachelbel-canon-progression.py` & `libdaw-0.2.2/python-libdaw/examples/pachelbel-canon-progression.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/examples/round.py` & `libdaw-0.2.2/python-libdaw/examples/round.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #import copy
 
 if TYPE_CHECKING:
     pass
 
 sequence = loads('''+(
 @(ab4 bb c db eb f g)
-% 5
 1,1 1 1 2 1 1 5,2
 6,1 5 6 7 1,2 1
 1,1 1 1 2 1 1 5,2
 6,1 5 6 7 1,2 1
 5+,1 4 3 2 3 2 1,2
 6,1 5 6 7 1,2 1
 5,1 5 6 7 1 1 2,2
```

### Comparing `libdaw-0.2.1/python-libdaw/examples/scale-inversion-notation.py` & `libdaw-0.2.2/python-libdaw/examples/scale-inversion-notation.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/examples/simple-notation.py` & `libdaw-0.2.2/python-libdaw/examples/simple-notation.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/examples/simple-scale-notation.py` & `libdaw-0.2.2/python-libdaw/examples/simple-scale-notation.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/python/libdaw/__init__.pyi` & `libdaw-0.2.2/python-libdaw/python/libdaw/__init__.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/python/libdaw/metronome.pyi` & `libdaw-0.2.2/python-libdaw/python/libdaw/metronome.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/python/libdaw/nodes/__init__.pyi` & `libdaw-0.2.2/python-libdaw/python/libdaw/nodes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/python/libdaw/notation.pyi` & `libdaw-0.2.2/python-libdaw/python/libdaw/notation.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/python/libdaw/pitch.pyi` & `libdaw-0.2.2/python-libdaw/python/libdaw/pitch.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/python/libdaw/time.pyi` & `libdaw-0.2.2/python-libdaw/python/libdaw/time.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/lib.rs` & `libdaw-0.2.2/python-libdaw/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/metronome.rs` & `libdaw-0.2.2/python-libdaw/src/metronome.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/node.rs` & `libdaw-0.2.2/python-libdaw/src/node.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/nodes/add.rs` & `libdaw-0.2.2/python-libdaw/src/nodes/add.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/nodes/constant_value.rs` & `libdaw-0.2.2/python-libdaw/src/nodes/constant_value.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/nodes/delay.rs` & `libdaw-0.2.2/python-libdaw/src/nodes/delay.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/nodes/detune.rs` & `libdaw-0.2.2/python-libdaw/src/nodes/detune.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/nodes/envelope.rs` & `libdaw-0.2.2/python-libdaw/src/nodes/envelope.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/nodes/gain.rs` & `libdaw-0.2.2/python-libdaw/src/nodes/gain.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/nodes/graph.rs` & `libdaw-0.2.2/python-libdaw/src/nodes/graph.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/nodes/instrument.rs` & `libdaw-0.2.2/python-libdaw/src/nodes/instrument.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/nodes/multi_frequency.rs` & `libdaw-0.2.2/python-libdaw/src/nodes/multi_frequency.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/nodes/multiply.rs` & `libdaw-0.2.2/python-libdaw/src/nodes/multiply.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/nodes/sawtooth_oscillator.rs` & `libdaw-0.2.2/python-libdaw/src/nodes/sawtooth_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/nodes/sine_oscillator.rs` & `libdaw-0.2.2/python-libdaw/src/nodes/sine_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/nodes/square_oscillator.rs` & `libdaw-0.2.2/python-libdaw/src/nodes/square_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/nodes/triangle_oscillator.rs` & `libdaw-0.2.2/python-libdaw/src/nodes/triangle_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/nodes.rs` & `libdaw-0.2.2/python-libdaw/src/nodes.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/notation/chord.rs` & `libdaw-0.2.2/python-libdaw/src/notation/chord.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/notation/inversion.rs` & `libdaw-0.2.2/python-libdaw/src/notation/inversion.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/notation/item.rs` & `libdaw-0.2.2/python-libdaw/src/notation/item.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/notation/note/note_pitch.rs` & `libdaw-0.2.2/python-libdaw/src/notation/note/note_pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/notation/note.rs` & `libdaw-0.2.2/python-libdaw/src/notation/note.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/notation/overlapped.rs` & `libdaw-0.2.2/python-libdaw/src/notation/overlapped.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/notation/pitch.rs` & `libdaw-0.2.2/python-libdaw/src/notation/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/notation/rest.rs` & `libdaw-0.2.2/python-libdaw/src/notation/rest.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/notation/scale.rs` & `libdaw-0.2.2/python-libdaw/src/notation/scale.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/notation/sequence.rs` & `libdaw-0.2.2/python-libdaw/src/notation/sequence.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/notation/step.rs` & `libdaw-0.2.2/python-libdaw/src/notation/step.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/notation.rs` & `libdaw-0.2.2/python-libdaw/src/notation.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/pitch/pitch.rs` & `libdaw-0.2.2/python-libdaw/src/pitch/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/pitch.rs` & `libdaw-0.2.2/python-libdaw/src/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/play.rs` & `libdaw-0.2.2/python-libdaw/src/play.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/stream.rs` & `libdaw-0.2.2/python-libdaw/src/stream.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python-libdaw/src/time.rs` & `libdaw-0.2.2/python-libdaw/src/time.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/Cargo.lock` & `libdaw-0.2.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
 name = "libc"
 version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libdaw"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "nohash-hasher",
  "nom",
  "ordered-float",
 ]
 
 [[package]]
@@ -665,15 +665,15 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "python-libdaw"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "libdaw",
  "nohash-hasher",
  "pyo3",
  "rodio",
 ]
```

### Comparing `libdaw-0.2.1/python/libdaw/notation.pyi` & `libdaw-0.2.2/python/libdaw/notation.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python/libdaw/pitch.pyi` & `libdaw-0.2.2/python/libdaw/pitch.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python/libdaw/time.pyi` & `libdaw-0.2.2/python/libdaw/time.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python/libdaw/__init__.pyi` & `libdaw-0.2.2/python/libdaw/__init__.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python/libdaw/metronome.pyi` & `libdaw-0.2.2/python/libdaw/metronome.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.1/python/libdaw/nodes/__init__.pyi` & `libdaw-0.2.2/python/libdaw/nodes/__init__.pyi`

 * *Files identical despite different names*

