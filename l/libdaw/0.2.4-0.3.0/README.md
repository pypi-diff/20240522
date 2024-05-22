# Comparing `tmp/libdaw-0.2.4.tar.gz` & `tmp/libdaw-0.3.0.tar.gz`

## Comparing `libdaw-0.2.4.tar` & `libdaw-0.3.0.tar`

### file list

```diff
@@ -1,146 +1,149 @@
--rw-r--r--   0     1001      127      427 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/Cargo.toml
--rw-r--r--   0     1001      127     1589 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/lib.rs
--rw-r--r--   0     1001      127      281 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/metronome/parse.rs
--rw-r--r--   0     1001      127     9873 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/metronome.rs
--rw-r--r--   0     1001      127      531 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes/add.rs
--rw-r--r--   0     1001      127      870 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes/constant_value.rs
--rw-r--r--   0     1001      127     1987 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes/delay.rs
--rw-r--r--   0     1001      127     2253 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes/detune.rs
--rw-r--r--   0     1001      127     4867 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes/envelope.rs
--rw-r--r--   0     1001      127      806 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes/gain.rs
--rw-r--r--   0     1001      127     1045 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes/graph/error.rs
--rw-r--r--   0     1001      127    17261 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes/graph.rs
--rw-r--r--   0     1001      127     6778 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes/instrument.rs
--rw-r--r--   0     1001      127     1195 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes/multi_frequency.rs
--rw-r--r--   0     1001      127      564 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes/multiply.rs
--rw-r--r--   0     1001      127      462 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes/passthrough.rs
--rw-r--r--   0     1001      127     1783 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes/sawtooth_oscillator.rs
--rw-r--r--   0     1001      127     1688 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes/sine_oscillator.rs
--rw-r--r--   0     1001      127     2172 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes/square_oscillator.rs
--rw-r--r--   0     1001      127     1806 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes/triangle_oscillator.rs
--rw-r--r--   0     1001      127      802 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/nodes.rs
--rw-r--r--   0     1001      127      965 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/chord/parse.rs
--rw-r--r--   0     1001      127     3007 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/chord.rs
--rw-r--r--   0     1001      127      440 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/inversion/parse.rs
--rw-r--r--   0     1001      127      763 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/inversion.rs
--rw-r--r--   0     1001      127     1197 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/item/parse.rs
--rw-r--r--   0     1001      127     5787 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/item.rs
--rw-r--r--   0     1001      127      897 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/note/parse.rs
--rw-r--r--   0     1001      127     4136 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/note.rs
--rw-r--r--   0     1001      127      689 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/overlapped/parse.rs
--rw-r--r--   0     1001      127     2134 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/overlapped.rs
--rw-r--r--   0     1001      127      798 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/pitch/parse.rs
--rw-r--r--   0     1001      127     1872 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/pitch.rs
--rw-r--r--   0     1001      127     1583 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/resolve_state.rs
--rw-r--r--   0     1001      127      329 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/rest/parse.rs
--rw-r--r--   0     1001      127     1104 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/rest.rs
--rw-r--r--   0     1001      127      679 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/scale/parse.rs
--rw-r--r--   0     1001      127     1110 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/scale.rs
--rw-r--r--   0     1001      127      679 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/sequence/parse.rs
--rw-r--r--   0     1001      127     2707 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/sequence.rs
--rw-r--r--   0     1001      127      575 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/step/parse.rs
--rw-r--r--   0     1001      127     2155 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation/step.rs
--rw-r--r--   0     1001      127      387 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/notation.rs
--rw-r--r--   0     1001      127     1566 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/parse.rs
--rw-r--r--   0     1001      127     2192 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/pitch/parse.rs
--rw-r--r--   0     1001      127     6415 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/pitch.rs
--rw-r--r--   0     1001      127     1726 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/stream/iter.rs
--rw-r--r--   0     1001      127     5784 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/stream.rs
--rw-r--r--   0     1001      127     1622 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/sync.rs
--rw-r--r--   0     1001      127     2361 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/time/duration.rs
--rw-r--r--   0     1001      127     2115 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/time/time.rs
--rw-r--r--   0     1001      127     3185 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/time/timestamp.rs
--rw-r--r--   0     1001      127      172 2024-05-22 02:50:26.000000 libdaw-0.2.4/libdaw/src/time.rs
--rw-r--r--   0     1001      127      101 2024-05-22 02:50:26.000000 libdaw-0.2.4/README.md
--rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 libdaw-0.2.4/python-libdaw/Cargo.toml
--rw-r--r--   0     1001      127     3526 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/.gitignore
--rw-r--r--   0     1001      127      131 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/README.md
--rw-r--r--   0     1001      127        6 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/docs/.gitignore
--rw-r--r--   0     1001      127      638 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/docs/Makefile
--rw-r--r--   0     1001      127      804 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/docs/make.bat
--rw-r--r--   0     1001      127       20 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/docs/requirements.txt
--rw-r--r--   0     1001      127      977 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/docs/source/conf.py
--rw-r--r--   0     1001      127      445 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/docs/source/index.rst
--rw-r--r--   0     1001      127      166 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/docs/source/libdaw/metronome.rst
--rw-r--r--   0     1001      127      180 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/docs/source/libdaw/nodes/envelope.rst
--rw-r--r--   0     1001      127      173 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/docs/source/libdaw/nodes/graph.rst
--rw-r--r--   0     1001      127      187 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/docs/source/libdaw/nodes/instrument.rst
--rw-r--r--   0     1001      127      200 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/docs/source/libdaw/nodes.rst
--rw-r--r--   0     1001      127      112 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/docs/source/libdaw/notation.rst
--rw-r--r--   0     1001      127      153 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/docs/source/libdaw/pitch.rst
--rw-r--r--   0     1001      127      152 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/docs/source/libdaw/time.rst
--rw-r--r--   0     1001      127      211 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/docs/source/libdaw.rst
--rw-r--r--   0     1001      127     1780 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/examples/1564.py
--rw-r--r--   0     1001      127     1662 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/examples/blues.py
--rwxr-xr-x   0     1001      127     1689 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/examples/instrument-test.py
--rw-r--r--   0     1001      127     1489 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/examples/pachelbel-canon-progression.py
--rw-r--r--   0     1001      127     1576 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/examples/round.py
--rw-r--r--   0     1001      127     1526 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/examples/scale-inversion-notation.py
--rw-r--r--   0     1001      127     1482 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/examples/simple-notation.py
--rw-r--r--   0     1001      127     1389 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/examples/simple-scale-notation.py
--rw-r--r--   0     1001      127      169 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/python/libdaw/__init__.py
--rw-r--r--   0     1001      127      980 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/python/libdaw/__init__.pyi
--rw-r--r--   0     1001      127     1588 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/python/libdaw/metronome.pyi
--rw-r--r--   0     1001      127     2528 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/python/libdaw/nodes/__init__.pyi
--rw-r--r--   0     1001      127      173 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/python/libdaw/nodes/envelope.pyi
--rw-r--r--   0     1001      127       23 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/python/libdaw/nodes/graph.pyi
--rw-r--r--   0     1001      127      151 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/python/libdaw/nodes/instrument.pyi
--rw-r--r--   0     1001      127     6173 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/python/libdaw/notation.pyi
--rw-r--r--   0     1001      127     1061 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/python/libdaw/pitch.pyi
--rw-r--r--   0     1001      127        0 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/python/libdaw/py.typed
--rw-r--r--   0     1001      127     1497 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/python/libdaw/time.pyi
--rw-r--r--   0     1001      127      491 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/frequency_node.rs
--rw-r--r--   0     1001      127     3052 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/lib.rs
--rw-r--r--   0     1001      127     4670 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/metronome.rs
--rw-r--r--   0     1001      127     1029 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/node.rs
--rw-r--r--   0     1001      127      514 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/nodes/add.rs
--rw-r--r--   0     1001      127      580 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/nodes/constant_value.rs
--rw-r--r--   0     1001      127      586 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/nodes/delay.rs
--rw-r--r--   0     1001      127      845 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/nodes/detune.rs
--rw-r--r--   0     1001      127     1868 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/nodes/envelope.rs
--rw-r--r--   0     1001      127      644 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/nodes/gain.rs
--rw-r--r--   0     1001      127     4554 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/nodes/graph.rs
--rw-r--r--   0     1001      127     2715 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/nodes/instrument.rs
--rw-r--r--   0     1001      127      672 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/nodes/multi_frequency.rs
--rw-r--r--   0     1001      127      534 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/nodes/multiply.rs
--rw-r--r--   0     1001      127      489 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/nodes/passthrough.rs
--rw-r--r--   0     1001      127      756 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/nodes/sawtooth_oscillator.rs
--rw-r--r--   0     1001      127      705 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/nodes/sine_oscillator.rs
--rw-r--r--   0     1001      127      748 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/nodes/square_oscillator.rs
--rw-r--r--   0     1001      127      756 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/nodes/triangle_oscillator.rs
--rw-r--r--   0     1001      127     1787 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/nodes.rs
--rw-r--r--   0     1001      127     6257 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/notation/chord.rs
--rw-r--r--   0     1001      127     1472 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/notation/inversion.rs
--rw-r--r--   0     1001      127     4459 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/notation/item.rs
--rw-r--r--   0     1001      127     1982 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/notation/note/note_pitch.rs
--rw-r--r--   0     1001      127     3895 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/notation/note.rs
--rw-r--r--   0     1001      127     5383 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/notation/overlapped.rs
--rw-r--r--   0     1001      127     2936 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/notation/pitch.rs
--rw-r--r--   0     1001      127     1561 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/notation/rest.rs
--rw-r--r--   0     1001      127     4458 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/notation/scale.rs
--rw-r--r--   0     1001      127     5218 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/notation/sequence.rs
--rw-r--r--   0     1001      127     1983 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/notation/step.rs
--rw-r--r--   0     1001      127      926 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/notation.rs
--rw-r--r--   0     1001      127     5708 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/pitch/pitch.rs
--rw-r--r--   0     1001      127     3014 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/pitch.rs
--rw-r--r--   0     1001      127     2178 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/play.rs
--rw-r--r--   0     1001      127     2658 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/stream.rs
--rw-r--r--   0     1001      127     5689 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/src/time.rs
--rw-r--r--   0     1001      127        0 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/test/__init__.py
--rw-r--r--   0     1001      127      471 2024-05-22 02:50:26.000000 libdaw-0.2.4/python-libdaw/test/test_pitch.py
--rw-r--r--   0     1001      127    30727 2024-05-22 02:50:31.000000 libdaw-0.2.4/Cargo.lock
--rw-r--r--   0        0        0      237 1970-01-01 00:00:00.000000 libdaw-0.2.4/Cargo.toml
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 libdaw-0.2.4/pyproject.toml
--rw-r--r--   0     1001      127     6173 2024-05-22 02:50:26.000000 libdaw-0.2.4/python/libdaw/notation.pyi
--rw-r--r--   0     1001      127      169 2024-05-22 02:50:26.000000 libdaw-0.2.4/python/libdaw/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-22 02:50:26.000000 libdaw-0.2.4/python/libdaw/py.typed
--rw-r--r--   0     1001      127     1061 2024-05-22 02:50:26.000000 libdaw-0.2.4/python/libdaw/pitch.pyi
--rw-r--r--   0     1001      127     1497 2024-05-22 02:50:26.000000 libdaw-0.2.4/python/libdaw/time.pyi
--rw-r--r--   0     1001      127      980 2024-05-22 02:50:26.000000 libdaw-0.2.4/python/libdaw/__init__.pyi
--rw-r--r--   0     1001      127     1588 2024-05-22 02:50:26.000000 libdaw-0.2.4/python/libdaw/metronome.pyi
--rw-r--r--   0     1001      127      151 2024-05-22 02:50:26.000000 libdaw-0.2.4/python/libdaw/nodes/instrument.pyi
--rw-r--r--   0     1001      127       23 2024-05-22 02:50:26.000000 libdaw-0.2.4/python/libdaw/nodes/graph.pyi
--rw-r--r--   0     1001      127      173 2024-05-22 02:50:26.000000 libdaw-0.2.4/python/libdaw/nodes/envelope.pyi
--rw-r--r--   0     1001      127     2528 2024-05-22 02:50:26.000000 libdaw-0.2.4/python/libdaw/nodes/__init__.pyi
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 libdaw-0.2.4/PKG-INFO
+-rw-r--r--   0     1001      127      427 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/Cargo.toml
+-rw-r--r--   0     1001      127     1589 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/lib.rs
+-rw-r--r--   0     1001      127      281 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/metronome/parse.rs
+-rw-r--r--   0     1001      127     9873 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/metronome.rs
+-rw-r--r--   0     1001      127      531 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes/add.rs
+-rw-r--r--   0     1001      127      870 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes/constant_value.rs
+-rw-r--r--   0     1001      127     1987 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes/delay.rs
+-rw-r--r--   0     1001      127     2253 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes/detune.rs
+-rw-r--r--   0     1001      127     4867 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes/envelope.rs
+-rw-r--r--   0     1001      127      806 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes/gain.rs
+-rw-r--r--   0     1001      127     1045 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes/graph/error.rs
+-rw-r--r--   0     1001      127    17261 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes/graph.rs
+-rw-r--r--   0     1001      127     6778 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes/instrument.rs
+-rw-r--r--   0     1001      127     1195 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes/multi_frequency.rs
+-rw-r--r--   0     1001      127      564 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes/multiply.rs
+-rw-r--r--   0     1001      127      462 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes/passthrough.rs
+-rw-r--r--   0     1001      127     1783 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes/sawtooth_oscillator.rs
+-rw-r--r--   0     1001      127     1688 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes/sine_oscillator.rs
+-rw-r--r--   0     1001      127     2172 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes/square_oscillator.rs
+-rw-r--r--   0     1001      127     1806 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes/triangle_oscillator.rs
+-rw-r--r--   0     1001      127      802 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/nodes.rs
+-rw-r--r--   0     1001      127      965 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/chord/parse.rs
+-rw-r--r--   0     1001      127     3007 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/chord.rs
+-rw-r--r--   0     1001      127      429 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/inversion/parse.rs
+-rw-r--r--   0     1001      127      763 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/inversion.rs
+-rw-r--r--   0     1001      127     1320 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/item/parse.rs
+-rw-r--r--   0     1001      127     6057 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/item.rs
+-rw-r--r--   0     1001      127      897 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/note/parse.rs
+-rw-r--r--   0     1001      127     4136 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/note.rs
+-rw-r--r--   0     1001      127      689 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/overlapped/parse.rs
+-rw-r--r--   0     1001      127     2134 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/overlapped.rs
+-rw-r--r--   0     1001      127      798 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/pitch/parse.rs
+-rw-r--r--   0     1001      127     1872 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/pitch.rs
+-rw-r--r--   0     1001      127     1553 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/resolve_state.rs
+-rw-r--r--   0     1001      127      329 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/rest/parse.rs
+-rw-r--r--   0     1001      127     1104 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/rest.rs
+-rw-r--r--   0     1001      127      679 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/scale/parse.rs
+-rw-r--r--   0     1001      127     1104 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/scale.rs
+-rw-r--r--   0     1001      127      679 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/sequence/parse.rs
+-rw-r--r--   0     1001      127     2707 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/sequence.rs
+-rw-r--r--   0     1001      127     1565 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/set/parse.rs
+-rw-r--r--   0     1001      127     1308 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/set.rs
+-rw-r--r--   0     1001      127      553 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/step/parse.rs
+-rw-r--r--   0     1001      127     2158 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation/step.rs
+-rw-r--r--   0     1001      127      414 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/notation.rs
+-rw-r--r--   0     1001      127     1576 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/parse.rs
+-rw-r--r--   0     1001      127     2192 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/pitch/parse.rs
+-rw-r--r--   0     1001      127     6415 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/pitch.rs
+-rw-r--r--   0     1001      127     1726 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/stream/iter.rs
+-rw-r--r--   0     1001      127     5784 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/stream.rs
+-rw-r--r--   0     1001      127     1622 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/sync.rs
+-rw-r--r--   0     1001      127     2361 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/time/duration.rs
+-rw-r--r--   0     1001      127     2115 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/time/time.rs
+-rw-r--r--   0     1001      127     3185 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/time/timestamp.rs
+-rw-r--r--   0     1001      127      172 2024-05-22 04:28:10.000000 libdaw-0.3.0/libdaw/src/time.rs
+-rw-r--r--   0     1001      127      101 2024-05-22 04:28:10.000000 libdaw-0.3.0/README.md
+-rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 libdaw-0.3.0/python-libdaw/Cargo.toml
+-rw-r--r--   0     1001      127     3526 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/.gitignore
+-rw-r--r--   0     1001      127      131 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/README.md
+-rw-r--r--   0     1001      127        6 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/docs/.gitignore
+-rw-r--r--   0     1001      127      638 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/docs/Makefile
+-rw-r--r--   0     1001      127      804 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/docs/make.bat
+-rw-r--r--   0     1001      127       20 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/docs/requirements.txt
+-rw-r--r--   0     1001      127      977 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/docs/source/conf.py
+-rw-r--r--   0     1001      127      445 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/docs/source/index.rst
+-rw-r--r--   0     1001      127      166 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/docs/source/libdaw/metronome.rst
+-rw-r--r--   0     1001      127      180 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/docs/source/libdaw/nodes/envelope.rst
+-rw-r--r--   0     1001      127      173 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/docs/source/libdaw/nodes/graph.rst
+-rw-r--r--   0     1001      127      187 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/docs/source/libdaw/nodes/instrument.rst
+-rw-r--r--   0     1001      127      200 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/docs/source/libdaw/nodes.rst
+-rw-r--r--   0     1001      127      112 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/docs/source/libdaw/notation.rst
+-rw-r--r--   0     1001      127      153 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/docs/source/libdaw/pitch.rst
+-rw-r--r--   0     1001      127      152 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/docs/source/libdaw/time.rst
+-rw-r--r--   0     1001      127      211 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/docs/source/libdaw.rst
+-rw-r--r--   0     1001      127     1780 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/examples/1564.py
+-rw-r--r--   0     1001      127     1662 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/examples/blues.py
+-rwxr-xr-x   0     1001      127     1689 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/examples/instrument-test.py
+-rw-r--r--   0     1001      127     1475 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/examples/pachelbel-canon-progression.py
+-rw-r--r--   0     1001      127     1576 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/examples/round.py
+-rw-r--r--   0     1001      127     1526 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/examples/scale-inversion-notation.py
+-rw-r--r--   0     1001      127     1482 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/examples/simple-notation.py
+-rw-r--r--   0     1001      127     1389 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/examples/simple-scale-notation.py
+-rw-r--r--   0     1001      127      169 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/python/libdaw/__init__.py
+-rw-r--r--   0     1001      127      980 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/python/libdaw/__init__.pyi
+-rw-r--r--   0     1001      127     1588 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/python/libdaw/metronome.pyi
+-rw-r--r--   0     1001      127     2528 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/python/libdaw/nodes/__init__.pyi
+-rw-r--r--   0     1001      127      173 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/python/libdaw/nodes/envelope.pyi
+-rw-r--r--   0     1001      127       23 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/python/libdaw/nodes/graph.pyi
+-rw-r--r--   0     1001      127      151 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/python/libdaw/nodes/instrument.pyi
+-rw-r--r--   0     1001      127     6622 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/python/libdaw/notation.pyi
+-rw-r--r--   0     1001      127     1061 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/python/libdaw/pitch.pyi
+-rw-r--r--   0     1001      127        0 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/python/libdaw/py.typed
+-rw-r--r--   0     1001      127     1497 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/python/libdaw/time.pyi
+-rw-r--r--   0     1001      127      491 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/frequency_node.rs
+-rw-r--r--   0     1001      127     3052 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/lib.rs
+-rw-r--r--   0     1001      127     4670 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/metronome.rs
+-rw-r--r--   0     1001      127     1029 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/node.rs
+-rw-r--r--   0     1001      127      514 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/nodes/add.rs
+-rw-r--r--   0     1001      127      580 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/nodes/constant_value.rs
+-rw-r--r--   0     1001      127      586 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/nodes/delay.rs
+-rw-r--r--   0     1001      127      845 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/nodes/detune.rs
+-rw-r--r--   0     1001      127     1868 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/nodes/envelope.rs
+-rw-r--r--   0     1001      127      644 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/nodes/gain.rs
+-rw-r--r--   0     1001      127     4554 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/nodes/graph.rs
+-rw-r--r--   0     1001      127     2715 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/nodes/instrument.rs
+-rw-r--r--   0     1001      127      672 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/nodes/multi_frequency.rs
+-rw-r--r--   0     1001      127      534 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/nodes/multiply.rs
+-rw-r--r--   0     1001      127      489 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/nodes/passthrough.rs
+-rw-r--r--   0     1001      127      756 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/nodes/sawtooth_oscillator.rs
+-rw-r--r--   0     1001      127      705 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/nodes/sine_oscillator.rs
+-rw-r--r--   0     1001      127      748 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/nodes/square_oscillator.rs
+-rw-r--r--   0     1001      127      756 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/nodes/triangle_oscillator.rs
+-rw-r--r--   0     1001      127     1787 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/nodes.rs
+-rw-r--r--   0     1001      127     6257 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/notation/chord.rs
+-rw-r--r--   0     1001      127     1472 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/notation/inversion.rs
+-rw-r--r--   0     1001      127     4835 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/notation/item.rs
+-rw-r--r--   0     1001      127     1982 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/notation/note/note_pitch.rs
+-rw-r--r--   0     1001      127     3871 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/notation/note.rs
+-rw-r--r--   0     1001      127     5383 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/notation/overlapped.rs
+-rw-r--r--   0     1001      127     2936 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/notation/pitch.rs
+-rw-r--r--   0     1001      127     1561 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/notation/rest.rs
+-rw-r--r--   0     1001      127     4458 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/notation/scale.rs
+-rw-r--r--   0     1001      127     5218 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/notation/sequence.rs
+-rw-r--r--   0     1001      127     2667 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/notation/set.rs
+-rw-r--r--   0     1001      127     1983 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/notation/step.rs
+-rw-r--r--   0     1001      127      985 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/notation.rs
+-rw-r--r--   0     1001      127     5708 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/pitch/pitch.rs
+-rw-r--r--   0     1001      127     3014 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/pitch.rs
+-rw-r--r--   0     1001      127     2178 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/play.rs
+-rw-r--r--   0     1001      127     2658 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/stream.rs
+-rw-r--r--   0     1001      127     5689 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/src/time.rs
+-rw-r--r--   0     1001      127        0 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/test/__init__.py
+-rw-r--r--   0     1001      127      471 2024-05-22 04:28:10.000000 libdaw-0.3.0/python-libdaw/test/test_pitch.py
+-rw-r--r--   0     1001      127    30727 2024-05-22 04:28:10.000000 libdaw-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0      237 1970-01-01 00:00:00.000000 libdaw-0.3.0/Cargo.toml
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 libdaw-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      127     6622 2024-05-22 04:28:10.000000 libdaw-0.3.0/python/libdaw/notation.pyi
+-rw-r--r--   0     1001      127      169 2024-05-22 04:28:10.000000 libdaw-0.3.0/python/libdaw/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-22 04:28:10.000000 libdaw-0.3.0/python/libdaw/py.typed
+-rw-r--r--   0     1001      127     1061 2024-05-22 04:28:10.000000 libdaw-0.3.0/python/libdaw/pitch.pyi
+-rw-r--r--   0     1001      127     1497 2024-05-22 04:28:10.000000 libdaw-0.3.0/python/libdaw/time.pyi
+-rw-r--r--   0     1001      127      980 2024-05-22 04:28:10.000000 libdaw-0.3.0/python/libdaw/__init__.pyi
+-rw-r--r--   0     1001      127     1588 2024-05-22 04:28:10.000000 libdaw-0.3.0/python/libdaw/metronome.pyi
+-rw-r--r--   0     1001      127      151 2024-05-22 04:28:10.000000 libdaw-0.3.0/python/libdaw/nodes/instrument.pyi
+-rw-r--r--   0     1001      127       23 2024-05-22 04:28:10.000000 libdaw-0.3.0/python/libdaw/nodes/graph.pyi
+-rw-r--r--   0     1001      127      173 2024-05-22 04:28:10.000000 libdaw-0.3.0/python/libdaw/nodes/envelope.pyi
+-rw-r--r--   0     1001      127     2528 2024-05-22 04:28:10.000000 libdaw-0.3.0/python/libdaw/nodes/__init__.pyi
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 libdaw-0.3.0/PKG-INFO
```

### Comparing `libdaw-0.2.4/libdaw/src/lib.rs` & `libdaw-0.3.0/libdaw/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/metronome.rs` & `libdaw-0.3.0/libdaw/src/metronome.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/nodes/add.rs` & `libdaw-0.3.0/libdaw/src/nodes/add.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/nodes/constant_value.rs` & `libdaw-0.3.0/libdaw/src/nodes/constant_value.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/nodes/delay.rs` & `libdaw-0.3.0/libdaw/src/nodes/delay.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/nodes/detune.rs` & `libdaw-0.3.0/libdaw/src/nodes/detune.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/nodes/envelope.rs` & `libdaw-0.3.0/libdaw/src/nodes/envelope.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/nodes/gain.rs` & `libdaw-0.3.0/libdaw/src/nodes/gain.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/nodes/graph/error.rs` & `libdaw-0.3.0/libdaw/src/nodes/graph/error.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/nodes/graph.rs` & `libdaw-0.3.0/libdaw/src/nodes/graph.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/nodes/instrument.rs` & `libdaw-0.3.0/libdaw/src/nodes/instrument.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/nodes/multi_frequency.rs` & `libdaw-0.3.0/libdaw/src/nodes/multi_frequency.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/nodes/multiply.rs` & `libdaw-0.3.0/libdaw/src/nodes/multiply.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/nodes/sawtooth_oscillator.rs` & `libdaw-0.3.0/libdaw/src/nodes/sawtooth_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/nodes/sine_oscillator.rs` & `libdaw-0.3.0/libdaw/src/nodes/sine_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/nodes/square_oscillator.rs` & `libdaw-0.3.0/libdaw/src/nodes/square_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/nodes/triangle_oscillator.rs` & `libdaw-0.3.0/libdaw/src/nodes/triangle_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/nodes.rs` & `libdaw-0.3.0/libdaw/src/nodes.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/notation/chord/parse.rs` & `libdaw-0.3.0/libdaw/src/notation/chord/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/notation/chord.rs` & `libdaw-0.3.0/libdaw/src/notation/chord.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/notation/inversion.rs` & `libdaw-0.3.0/libdaw/src/notation/inversion.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/notation/item/parse.rs` & `libdaw-0.3.0/libdaw/src/notation/item/parse.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-use super::{Chord, Inversion, Item, Note, Overlapped, Rest, Scale, Sequence};
+use super::{Chord, Inversion, Item, Note, Overlapped, Rest, Scale, Sequence, Set};
 use crate::parse::IResult;
 use nom::{branch::alt, combinator::map, error::context};
 use std::sync::{Arc, Mutex};
 
 pub fn item(input: &str) -> IResult<&str, Item> {
     alt((
+        map(context("Set", Set::parse), move |chord| {
+            Item::Set(Arc::new(Mutex::new(chord)))
+        }),
         map(context("Chord", Chord::parse), move |chord| {
             Item::Chord(Arc::new(Mutex::new(chord)))
         }),
         map(
             context("Overlapped", Overlapped::parse),
             move |overlapped| Item::Overlapped(Arc::new(Mutex::new(overlapped))),
         ),
```

### Comparing `libdaw-0.2.4/libdaw/src/notation/item.rs` & `libdaw-0.3.0/libdaw/src/notation/item.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mod parse;
 
 use super::{
-    resolve_state::ResolveState, Chord, Inversion, Note, Overlapped, Rest, Scale, Sequence,
+    resolve_state::ResolveState, Chord, Inversion, Note, Overlapped, Rest, Scale, Sequence, Set,
 };
 use crate::{
     metronome::{Beat, Metronome},
     nodes::instrument::Tone,
     parse::IResult,
     pitch::PitchStandard,
 };
@@ -21,28 +21,30 @@
     Note(Arc<Mutex<Note>>),
     Chord(Arc<Mutex<Chord>>),
     Rest(Arc<Mutex<Rest>>),
     Overlapped(Arc<Mutex<Overlapped>>),
     Sequence(Arc<Mutex<Sequence>>),
     Scale(Arc<Mutex<Scale>>),
     Inversion(Arc<Mutex<Inversion>>),
+    Set(Arc<Mutex<Set>>),
 }
 
 impl fmt::Debug for Item {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         match self {
             Item::Note(note) => fmt::Debug::fmt(&note.lock().expect("poisoned"), f),
             Item::Chord(chord) => fmt::Debug::fmt(&chord.lock().expect("poisoned"), f),
             Item::Rest(rest) => fmt::Debug::fmt(&rest.lock().expect("poisoned"), f),
             Item::Overlapped(overlapped) => {
                 fmt::Debug::fmt(&overlapped.lock().expect("poisoned"), f)
             }
             Item::Sequence(sequence) => fmt::Debug::fmt(&sequence.lock().expect("poisoned"), f),
             Item::Scale(scale) => fmt::Debug::fmt(&scale.lock().expect("poisoned"), f),
             Item::Inversion(inversion) => fmt::Debug::fmt(&inversion.lock().expect("poisoned"), f),
+            Item::Set(set) => fmt::Debug::fmt(&set.lock().expect("poisoned"), f),
         }
     }
 }
 
 impl Item {
     /// Resolve all the section's notes to playable instrument tones.
     /// The offset is the beat offset.
@@ -78,15 +80,17 @@
             }
             Item::Sequence(sequence) => Box::new(sequence.lock().expect("poisoned").inner_tones(
                 offset,
                 metronome,
                 pitch_standard,
                 state.clone(),
             )),
-            Item::Scale(_) | Item::Inversion(_) | Item::Rest(_) => Box::new(std::iter::empty()),
+            Item::Scale(_) | Item::Inversion(_) | Item::Rest(_) | Item::Set(_) => {
+                Box::new(std::iter::empty())
+            }
         }
     }
     pub fn tones<S>(
         &self,
         offset: Beat,
         metronome: &Metronome,
         pitch_standard: &S,
@@ -105,25 +109,26 @@
             Item::Overlapped(overlapped) => {
                 overlapped.lock().expect("poisoned").inner_length(state)
             }
             Item::Sequence(sequence) => sequence
                 .lock()
                 .expect("poisoned")
                 .inner_length(state.clone()),
-            Item::Scale(_) | Item::Inversion(_) => Beat::ZERO,
+            Item::Scale(_) | Item::Inversion(_) | Item::Set(_) => Beat::ZERO,
         }
     }
 
     pub(super) fn update_state(&self, state: &mut ResolveState) {
         match self {
             Item::Note(note) => note.lock().expect("poisoned").update_state(state),
             Item::Chord(chord) => chord.lock().expect("poisoned").update_state(state),
             Item::Rest(rest) => rest.lock().expect("poisoned").update_state(state),
             Item::Scale(scale) => scale.lock().expect("poisoned").update_state(state),
             Item::Inversion(inversion) => inversion.lock().expect("poisoned").update_state(state),
+            Item::Set(set) => set.lock().expect("poisoned").update_state(state),
             Item::Overlapped(_) | Item::Sequence(_) => (),
         }
     }
 
     pub(super) fn inner_duration(&self, state: &ResolveState) -> Beat {
         match self {
             Item::Note(note) => note.lock().expect("poisoned").inner_duration(state),
@@ -132,15 +137,15 @@
             Item::Overlapped(overlapped) => {
                 overlapped.lock().expect("poisoned").inner_duration(state)
             }
             Item::Sequence(sequence) => sequence
                 .lock()
                 .expect("poisoned")
                 .inner_duration(state.clone()),
-            Item::Scale(_) | Item::Inversion(_) => Beat::ZERO,
+            Item::Scale(_) | Item::Inversion(_) | Item::Set(_) => Beat::ZERO,
         }
     }
     pub fn length(&self) -> Beat {
         self.inner_length(&Default::default())
     }
     pub fn duration(&self) -> Beat {
         self.inner_duration(&Default::default())
```

### Comparing `libdaw-0.2.4/libdaw/src/notation/note/parse.rs` & `libdaw-0.3.0/libdaw/src/notation/note/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/notation/note.rs` & `libdaw-0.3.0/libdaw/src/notation/note.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/notation/overlapped/parse.rs` & `libdaw-0.3.0/libdaw/src/notation/overlapped/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/notation/overlapped.rs` & `libdaw-0.3.0/libdaw/src/notation/overlapped.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/notation/pitch/parse.rs` & `libdaw-0.3.0/libdaw/src/notation/pitch/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/notation/pitch.rs` & `libdaw-0.3.0/libdaw/src/notation/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/notation/resolve_state.rs` & `libdaw-0.3.0/libdaw/src/notation/resolve_state.rs`

 * *Files 9% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
     /// The scale for scale-inversion notation.
     pub scale: Vec<Pitch>,
 
     /// The current scale inversion.
     pub inversion: i64,
 
-    /// Previous used scale step, post-inversion and zero-basing.
-    pub scale_step: usize,
+    /// Previous used scale step, post-inversion.
+    pub step: i64,
 
     /// Previous used scale octave.
     pub scale_octave: i8,
 }
 
 impl Default for ResolveState {
     fn default() -> Self {
@@ -53,12 +53,12 @@
                     name,
                     adjustment: 0.0,
                 })),
                 octave: 4,
             })
             .collect(),
             inversion: 0,
-            scale_step: 0,
+            step: 1,
             scale_octave: 0,
         }
     }
 }
```

### Comparing `libdaw-0.2.4/libdaw/src/notation/rest.rs` & `libdaw-0.3.0/libdaw/src/notation/rest.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/notation/scale/parse.rs` & `libdaw-0.3.0/libdaw/src/notation/scale/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/notation/scale.rs` & `libdaw-0.3.0/libdaw/src/notation/scale.rs`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         let mut running_state = state.clone();
         for pitch in &self.pitches {
             let absolute = pitch.absolute(&running_state);
             scale.push(absolute.clone());
             running_state.pitch = absolute;
         }
         state.scale = scale;
-        state.scale_step = 0;
+        state.step = 0;
         state.inversion = 0;
         state.scale_octave = 0;
     }
 }
 
 impl FromStr for Scale {
     type Err = String;
```

### Comparing `libdaw-0.2.4/libdaw/src/notation/sequence/parse.rs` & `libdaw-0.3.0/libdaw/src/notation/sequence/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/notation/sequence.rs` & `libdaw-0.3.0/libdaw/src/notation/sequence.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/notation/step/parse.rs` & `libdaw-0.3.0/libdaw/src/notation/step/parse.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 use super::Step;
 use crate::parse::{numeric_adjustment, octave_shift, IResult};
-use nom::{
-    character::complete::i64,
-    combinator::{map_res, opt},
-};
+use nom::{character::complete::i64, combinator::opt};
 
 pub fn step(input: &str) -> IResult<&str, Step> {
     let (input, step) = i64(input)?;
     let (input, numeric_adjustment) = opt(numeric_adjustment)(input)?;
     let (input, octave_shift) = opt(octave_shift)(input)?;
     Ok((
         input,
```

### Comparing `libdaw-0.2.4/libdaw/src/notation/step.rs` & `libdaw-0.3.0/libdaw/src/notation/step.rs`

 * *Files 15% similar despite different names*

```diff
@@ -31,29 +31,28 @@
             octave: scale_pitch.octave.saturating_add(scale_octave),
         }
     }
 
     pub(super) fn scale_octave(&self, state: &ResolveState) -> i8 {
         let half_scale = state.scale.len() / 2;
         let step = (self.step - 1 + state.inversion).rem_euclid(state.scale.len() as i64) as usize;
-        let state_step = state.scale_step % state.scale.len();
+        let state_step = (state.step - 1).rem_euclid(state.scale.len() as i64) as usize;
         let relative_shift = if state_step + half_scale < step {
             -1
         } else if step + half_scale < state_step {
             1
         } else {
             0
         };
         relative_shift + self.octave_shift + state.scale_octave
     }
     pub(super) fn update_state(&self, state: &mut ResolveState) {
-        let scale_step =
-            (self.step - 1 + state.inversion).rem_euclid(state.scale.len() as i64) as usize;
+        let scale_step = (self.step - 1 + state.inversion).rem_euclid(state.scale.len() as i64) + 1;
         let scale_octave = self.scale_octave(state);
-        state.scale_step = scale_step;
+        state.step = scale_step;
         state.scale_octave = scale_octave;
     }
 }
 impl FromStr for Step {
     type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
```

### Comparing `libdaw-0.2.4/libdaw/src/parse.rs` & `libdaw-0.3.0/libdaw/src/parse.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 //! Common parsers and types for parsers.
 
 use nom::{
     branch::alt,
     bytes::complete::tag,
     character::complete::char,
-    combinator::{map_res, opt},
+    combinator::{cut, map_res, opt},
     error::VerboseError,
     multi::many1_count,
     number::complete::double,
 };
 
 pub type IResult<I, O> = nom::IResult<I, O, VerboseError<I>>;
 
 pub fn denominator(input: &str) -> IResult<&str, f64> {
     let (input, _) = tag("/")(input)?;
-    let (input, denominator) = double(input)?;
+    let (input, denominator) = cut(double)(input)?;
     Ok((input, denominator))
 }
 
 /// A floating point number, optionally divided by another floating point number.
 pub fn number(input: &str) -> IResult<&str, f64> {
     let (input, numerator) = double(input)?;
     let (input, denominator) = opt(denominator)(input)?;
```

### Comparing `libdaw-0.2.4/libdaw/src/pitch/parse.rs` & `libdaw-0.3.0/libdaw/src/pitch/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/pitch.rs` & `libdaw-0.3.0/libdaw/src/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/stream/iter.rs` & `libdaw-0.3.0/libdaw/src/stream/iter.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/stream.rs` & `libdaw-0.3.0/libdaw/src/stream.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/sync.rs` & `libdaw-0.3.0/libdaw/src/sync.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/time/duration.rs` & `libdaw-0.3.0/libdaw/src/time/duration.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/time/time.rs` & `libdaw-0.3.0/libdaw/src/time/time.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/libdaw/src/time/timestamp.rs` & `libdaw-0.3.0/libdaw/src/time/timestamp.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/.github/workflows/CI.yml` & `libdaw-0.3.0/python-libdaw/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/.gitignore` & `libdaw-0.3.0/python-libdaw/.gitignore`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/docs/Makefile` & `libdaw-0.3.0/python-libdaw/docs/Makefile`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/docs/make.bat` & `libdaw-0.3.0/python-libdaw/docs/make.bat`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/docs/source/conf.py` & `libdaw-0.3.0/python-libdaw/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/examples/1564.py` & `libdaw-0.3.0/python-libdaw/examples/1564.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/examples/blues.py` & `libdaw-0.3.0/python-libdaw/examples/blues.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/examples/instrument-test.py` & `libdaw-0.3.0/python-libdaw/examples/instrument-test.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/examples/pachelbel-canon-progression.py` & `libdaw-0.3.0/python-libdaw/examples/pachelbel-canon-progression.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from libdaw import play
 from libdaw.metronome import Metronome, TempoInstruction, Beat, BeatsPerMinute
 from libdaw.nodes.envelope import Point
 from libdaw.nodes import Instrument, Graph, Gain, SquareOscillator
-from libdaw.notation import Chord, Note, Sequence, Inversion, Step
+from libdaw.notation import Chord, Sequence, Inversion, Set, Step
 from libdaw.time import Time
 
 #import copy
 
 if TYPE_CHECKING:
     pass
 
-chord = Chord.loads('=(1 3 5),1')
+chord = Chord.loads('=(1 3 5)')
 sequence = Sequence()
 
 for progression_chord in [1, 5, 6, 3, 4, 1, 4, 5]:
     sequence.append(Inversion(progression_chord - 1))
-    sequence.append(Note(Step(0), length=Beat(0)))
+    sequence.append(Set(pitch=Step(1)))
     sequence.append(chord)
 
 assert isinstance(sequence, Sequence)
     
 metronome = Metronome()
 metronome.add_tempo_instruction(TempoInstruction(beat=Beat(0), tempo=BeatsPerMinute(60)))
```

### Comparing `libdaw-0.2.4/python-libdaw/examples/round.py` & `libdaw-0.3.0/python-libdaw/examples/round.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/examples/scale-inversion-notation.py` & `libdaw-0.3.0/python-libdaw/examples/scale-inversion-notation.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/examples/simple-notation.py` & `libdaw-0.3.0/python-libdaw/examples/simple-notation.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/examples/simple-scale-notation.py` & `libdaw-0.3.0/python-libdaw/examples/simple-scale-notation.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/python/libdaw/__init__.pyi` & `libdaw-0.3.0/python-libdaw/python/libdaw/__init__.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/python/libdaw/metronome.pyi` & `libdaw-0.3.0/python-libdaw/python/libdaw/metronome.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/python/libdaw/nodes/__init__.pyi` & `libdaw-0.3.0/python-libdaw/python/libdaw/nodes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/python/libdaw/notation.pyi` & `libdaw-0.3.0/python-libdaw/python/libdaw/notation.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import abc
 from typing import Self
 from libdaw.metronome import Beat, Metronome
 from libdaw.nodes.instrument import Tone
 from libdaw.pitch import A440, PitchStandard, PitchClass
 
-type _Item = Chord | Note | Rest | Overlapped | Sequence | Inversion | Scale
+type _Item = Chord | Note | Rest | Overlapped | Sequence | Inversion | Scale | Set
 type _NotePitch = Step | Pitch
 
 class _ChordIterator:
     def __iter__(self) -> Self: ...
     def __next__(self) -> _NotePitch: ...
 
 class _ScaleIterator:
@@ -201,8 +201,26 @@
     def loads(source: str) -> Inversion: ...
 
     @property
     def inversion(self) -> int: ...
     @inversion.setter
     def inversion(self, value: int): ...
 
+class Set:
+    def __new__(
+        cls: type,
+        pitch: _NotePitch | None = None,
+        length: Beat | None = None,
+    ): ...
+    @staticmethod
+    def loads(source: str) -> Set: ...
+
+    @property
+    def pitch(self) -> _NotePitch | None: ...
+    @pitch.setter
+    def pitch(self, value: _NotePitch | None): ...
+    @property
+    def length(self) -> Beat | None: ...
+    @length.setter
+    def length(self, value: Beat | None): ...
+
 def loads(source: str) -> _Item: ...
```

### Comparing `libdaw-0.2.4/python-libdaw/python/libdaw/pitch.pyi` & `libdaw-0.3.0/python-libdaw/python/libdaw/pitch.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/python/libdaw/time.pyi` & `libdaw-0.3.0/python-libdaw/python/libdaw/time.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/lib.rs` & `libdaw-0.3.0/python-libdaw/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/metronome.rs` & `libdaw-0.3.0/python-libdaw/src/metronome.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/node.rs` & `libdaw-0.3.0/python-libdaw/src/node.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/nodes/add.rs` & `libdaw-0.3.0/python-libdaw/src/nodes/add.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/nodes/constant_value.rs` & `libdaw-0.3.0/python-libdaw/src/nodes/constant_value.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/nodes/delay.rs` & `libdaw-0.3.0/python-libdaw/src/nodes/delay.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/nodes/detune.rs` & `libdaw-0.3.0/python-libdaw/src/nodes/detune.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/nodes/envelope.rs` & `libdaw-0.3.0/python-libdaw/src/nodes/envelope.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/nodes/gain.rs` & `libdaw-0.3.0/python-libdaw/src/nodes/gain.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/nodes/graph.rs` & `libdaw-0.3.0/python-libdaw/src/nodes/graph.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/nodes/instrument.rs` & `libdaw-0.3.0/python-libdaw/src/nodes/instrument.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/nodes/multi_frequency.rs` & `libdaw-0.3.0/python-libdaw/src/nodes/multi_frequency.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/nodes/multiply.rs` & `libdaw-0.3.0/python-libdaw/src/nodes/multiply.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/nodes/sawtooth_oscillator.rs` & `libdaw-0.3.0/python-libdaw/src/nodes/sawtooth_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/nodes/sine_oscillator.rs` & `libdaw-0.3.0/python-libdaw/src/nodes/sine_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/nodes/square_oscillator.rs` & `libdaw-0.3.0/python-libdaw/src/nodes/square_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/nodes/triangle_oscillator.rs` & `libdaw-0.3.0/python-libdaw/src/nodes/triangle_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/nodes.rs` & `libdaw-0.3.0/python-libdaw/src/nodes.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/notation/chord.rs` & `libdaw-0.3.0/python-libdaw/src/notation/chord.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/notation/inversion.rs` & `libdaw-0.3.0/python-libdaw/src/notation/inversion.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/notation/item.rs` & `libdaw-0.3.0/python-libdaw/src/notation/item.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use super::{Chord, Inversion, Note, Overlapped, Rest, Scale, Sequence};
+use super::{Chord, Inversion, Note, Overlapped, Rest, Scale, Sequence, Set};
 use crate::Result;
 use libdaw::notation::Item as DawItem;
 use pyo3::{
     exceptions::PyTypeError, pyfunction, types::PyAnyMethods as _, AsPyPointer, Bound,
     FromPyObject, IntoPy, Py, PyAny, PyResult, Python,
 };
 
@@ -12,28 +12,30 @@
     Note(Py<Note>),
     Chord(Py<Chord>),
     Rest(Py<Rest>),
     Overlapped(Py<Overlapped>),
     Sequence(Py<Sequence>),
     Scale(Py<Scale>),
     Inversion(Py<Inversion>),
+    Set(Py<Set>),
 }
 
 impl Item {
     pub fn from_inner(py: Python<'_>, inner: DawItem) -> Self {
         match inner {
             DawItem::Note(note) => Self::Note(Note::from_inner(py, note)),
             DawItem::Chord(chord) => Self::Chord(Chord::from_inner(py, chord)),
             DawItem::Rest(rest) => Self::Rest(Rest::from_inner(py, rest)),
             DawItem::Overlapped(overlapped) => {
                 Self::Overlapped(Overlapped::from_inner(py, overlapped))
             }
             DawItem::Sequence(sequence) => Self::Sequence(Sequence::from_inner(py, sequence)),
             DawItem::Scale(scale) => Self::Scale(Scale::from_inner(py, scale)),
             DawItem::Inversion(inversion) => Self::Inversion(Inversion::from_inner(py, inversion)),
+            DawItem::Set(set) => Self::Set(Set::from_inner(py, set)),
         }
     }
     pub fn as_inner(&self, py: Python<'_>) -> DawItem {
         match self {
             Item::Note(note) => DawItem::Note(note.bind_borrowed(py).borrow().inner.clone()),
             Item::Chord(chord) => DawItem::Chord(chord.bind_borrowed(py).borrow().inner.clone()),
             Item::Rest(rest) => DawItem::Rest(rest.bind_borrowed(py).borrow().inner.clone()),
@@ -43,14 +45,15 @@
             Item::Sequence(sequence) => {
                 DawItem::Sequence(sequence.bind_borrowed(py).borrow().inner.clone())
             }
             Item::Scale(scale) => DawItem::Scale(scale.bind_borrowed(py).borrow().inner.clone()),
             Item::Inversion(inversion) => {
                 DawItem::Inversion(inversion.bind_borrowed(py).borrow().inner.clone())
             }
+            Item::Set(set) => DawItem::Set(set.bind_borrowed(py).borrow().inner.clone()),
         }
     }
 }
 
 impl<'py> FromPyObject<'py> for Item {
     fn extract_bound(value: &Bound<'py, PyAny>) -> PyResult<Self> {
         Ok(if let Ok(note) = value.downcast::<Note>() {
@@ -63,14 +66,16 @@
             Self::Overlapped(overlapped.clone().unbind())
         } else if let Ok(sequence) = value.downcast::<Sequence>() {
             Self::Sequence(sequence.clone().unbind())
         } else if let Ok(scale) = value.downcast::<Scale>() {
             Self::Scale(scale.clone().unbind())
         } else if let Ok(inversion) = value.downcast::<Inversion>() {
             Self::Inversion(inversion.clone().unbind())
+        } else if let Ok(set) = value.downcast::<Set>() {
+            Self::Set(set.clone().unbind())
         } else {
             return Err(PyTypeError::new_err("Item was invalid type"));
         })
     }
 }
 
 impl IntoPy<Py<PyAny>> for Item {
@@ -79,28 +84,30 @@
             Item::Note(note) => note.into_py(py),
             Item::Chord(chord) => chord.into_py(py),
             Item::Rest(rest) => rest.into_py(py),
             Item::Overlapped(overlapped) => overlapped.into_py(py),
             Item::Sequence(sequence) => sequence.into_py(py),
             Item::Scale(scale) => scale.into_py(py),
             Item::Inversion(inversion) => inversion.into_py(py),
+            Item::Set(set) => set.into_py(py),
         }
     }
 }
 
 unsafe impl AsPyPointer for Item {
     fn as_ptr(&self) -> *mut pyo3::ffi::PyObject {
         match self {
             Item::Note(note) => note.as_ptr(),
             Item::Chord(chord) => chord.as_ptr(),
             Item::Rest(rest) => rest.as_ptr(),
             Item::Overlapped(overlapped) => overlapped.as_ptr(),
             Item::Sequence(sequence) => sequence.as_ptr(),
             Item::Scale(scale) => scale.as_ptr(),
             Item::Inversion(inversion) => inversion.as_ptr(),
+            Item::Set(set) => set.as_ptr(),
         }
     }
 }
 
 #[pyfunction]
 pub fn loads(py: Python<'_>, source: &str) -> Result<Item> {
     let item: DawItem = source.parse()?;
```

### Comparing `libdaw-0.2.4/python-libdaw/src/notation/note/note_pitch.rs` & `libdaw-0.3.0/python-libdaw/src/notation/note/note_pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/notation/note.rs` & `libdaw-0.3.0/python-libdaw/src/notation/note.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 use crate::{
     metronome::{Beat, MaybeMetronome},
     nodes::instrument::Tone,
     pitch::MaybePitchStandard,
 };
 use libdaw::{metronome::Beat as DawBeat, notation::Note as DawNote};
-use pyo3::{pyclass, pymethods, IntoPy as _, Py, PyResult, PyTraverseError, PyVisit, Python};
+use pyo3::{pyclass, pymethods, IntoPy as _, Py, PyTraverseError, PyVisit, Python};
 use std::{
     ops::Deref,
     sync::{Arc, Mutex},
 };
 
 #[pyclass(module = "libdaw.notation")]
 #[derive(Debug, Clone)]
@@ -42,23 +42,23 @@
 impl Note {
     #[new]
     pub fn new(
         py: Python<'_>,
         pitch: NotePitch,
         length: Option<Beat>,
         duration: Option<Beat>,
-    ) -> PyResult<Self> {
-        Ok(Self {
+    ) -> Self {
+        Self {
             inner: Arc::new(Mutex::new(DawNote {
                 pitch: pitch.as_inner(py),
                 length: length.map(|beat| beat.0),
                 duration: duration.map(|beat| beat.0),
             })),
             pitch: Some(pitch),
-        })
+        }
     }
 
     #[staticmethod]
     pub fn loads(py: Python<'_>, source: String) -> crate::Result<Py<Self>> {
         Ok(Self::from_inner(py, Arc::new(Mutex::new(source.parse()?))))
     }
```

### Comparing `libdaw-0.2.4/python-libdaw/src/notation/overlapped.rs` & `libdaw-0.3.0/python-libdaw/src/notation/overlapped.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/notation/pitch.rs` & `libdaw-0.3.0/python-libdaw/src/notation/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/notation/rest.rs` & `libdaw-0.3.0/python-libdaw/src/notation/rest.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/notation/scale.rs` & `libdaw-0.3.0/python-libdaw/src/notation/scale.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/notation/sequence.rs` & `libdaw-0.3.0/python-libdaw/src/notation/sequence.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/notation/step.rs` & `libdaw-0.3.0/python-libdaw/src/notation/step.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/notation.rs` & `libdaw-0.3.0/python-libdaw/src/notation.rs`

 * *Files 16% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 mod item;
 mod note;
 mod overlapped;
 mod pitch;
 mod rest;
 mod scale;
 mod sequence;
+mod set;
 mod step;
 
 pub use chord::Chord;
 pub use inversion::Inversion;
 pub use item::Item;
 pub use note::{Note, NotePitch};
 pub use overlapped::Overlapped;
 pub use pitch::Pitch;
 pub use rest::Rest;
 pub use scale::Scale;
 pub use sequence::Sequence;
+pub use set::Set;
 pub use step::Step;
 
 use pyo3::{
     types::{PyModule, PyModuleMethods as _},
     wrap_pyfunction, Bound, PyResult,
 };
 
@@ -31,10 +33,11 @@
     module.add_class::<Inversion>()?;
     module.add_class::<Note>()?;
     module.add_class::<Overlapped>()?;
     module.add_class::<Pitch>()?;
     module.add_class::<Rest>()?;
     module.add_class::<Scale>()?;
     module.add_class::<Sequence>()?;
+    module.add_class::<Set>()?;
     module.add_class::<Step>()?;
     Ok(())
 }
```

### Comparing `libdaw-0.2.4/python-libdaw/src/pitch/pitch.rs` & `libdaw-0.3.0/python-libdaw/src/pitch/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/pitch.rs` & `libdaw-0.3.0/python-libdaw/src/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/play.rs` & `libdaw-0.3.0/python-libdaw/src/play.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/stream.rs` & `libdaw-0.3.0/python-libdaw/src/stream.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python-libdaw/src/time.rs` & `libdaw-0.3.0/python-libdaw/src/time.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/Cargo.lock` & `libdaw-0.3.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
 name = "libc"
 version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libdaw"
-version = "0.2.4"
+version = "0.3.0"
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
-version = "0.2.4"
+version = "0.3.0"
 dependencies = [
  "libdaw",
  "nohash-hasher",
  "pyo3",
  "rodio",
 ]
```

### Comparing `libdaw-0.2.4/pyproject.toml` & `libdaw-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python/libdaw/notation.pyi` & `libdaw-0.3.0/python/libdaw/notation.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import abc
 from typing import Self
 from libdaw.metronome import Beat, Metronome
 from libdaw.nodes.instrument import Tone
 from libdaw.pitch import A440, PitchStandard, PitchClass
 
-type _Item = Chord | Note | Rest | Overlapped | Sequence | Inversion | Scale
+type _Item = Chord | Note | Rest | Overlapped | Sequence | Inversion | Scale | Set
 type _NotePitch = Step | Pitch
 
 class _ChordIterator:
     def __iter__(self) -> Self: ...
     def __next__(self) -> _NotePitch: ...
 
 class _ScaleIterator:
@@ -201,8 +201,26 @@
     def loads(source: str) -> Inversion: ...
 
     @property
     def inversion(self) -> int: ...
     @inversion.setter
     def inversion(self, value: int): ...
 
+class Set:
+    def __new__(
+        cls: type,
+        pitch: _NotePitch | None = None,
+        length: Beat | None = None,
+    ): ...
+    @staticmethod
+    def loads(source: str) -> Set: ...
+
+    @property
+    def pitch(self) -> _NotePitch | None: ...
+    @pitch.setter
+    def pitch(self, value: _NotePitch | None): ...
+    @property
+    def length(self) -> Beat | None: ...
+    @length.setter
+    def length(self, value: Beat | None): ...
+
 def loads(source: str) -> _Item: ...
```

### Comparing `libdaw-0.2.4/python/libdaw/pitch.pyi` & `libdaw-0.3.0/python/libdaw/pitch.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python/libdaw/time.pyi` & `libdaw-0.3.0/python/libdaw/time.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python/libdaw/__init__.pyi` & `libdaw-0.3.0/python/libdaw/__init__.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python/libdaw/metronome.pyi` & `libdaw-0.3.0/python/libdaw/metronome.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/python/libdaw/nodes/__init__.pyi` & `libdaw-0.3.0/python/libdaw/nodes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.2.4/PKG-INFO` & `libdaw-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: libdaw
-Version: 0.2.4
+Version: 0.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 License: MPL 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

