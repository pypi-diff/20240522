# Comparing `tmp/meeko-0.6.0a2.tar.gz` & `tmp/meeko-0.6.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meeko-0.6.0a2.tar", last modified: Thu Nov 30 18:06:09 2023, max compression
+gzip compressed data, was "meeko-0.6.0a3.tar", last modified: Fri Feb  2 07:35:44 2024, max compression
```

## Comparing `meeko-0.6.0a2.tar` & `meeko-0.6.0a3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 18:06:09.698564 meeko-0.6.0a2/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2023-11-30 18:05:58.000000 meeko-0.6.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14128 2023-11-30 18:06:09.698564 meeko-0.6.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12840 2023-11-30 18:05:58.000000 meeko-0.6.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 18:06:09.690564 meeko-0.6.0a2/meeko/
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 18:06:09.690564 meeko-0.6.0a2/meeko/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/analysis/fingerprint_interactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11922 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/analysis/interactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13820 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/atomtyper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/bondtyper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9317 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/covalentbuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 18:06:09.694564 meeko-0.6.0a2/meeko/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/data/atomtypes.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/data/flexres_templates.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 18:06:09.694564 meeko-0.6.0a2/meeko/data/params/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/data/params/ad4_desolv_param.json
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/data/params/ad4_desolv_volume.json
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/data/params/ad4_types.json
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/data/params/ad4_vdw.json
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/data/params/example_offatom_charge.json
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/data/params/vina_params.json
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/data/pi_non_aromatic.txt
--rw-r--r--   0 runner    (1001) docker     (127)   181255 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/data/prot_res_params.json
--rw-r--r--   0 runner    (1001) docker     (127)   205550 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/data/residue_params.json
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/data/waterfield.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/espalomatyper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/flexibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/gridbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    14776 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/hydrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    45546 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/linked_rdkit_chorizo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10722 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/macrocycle.py
--rw-r--r--   0 runner    (1001) docker     (127)    32118 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/molecule_pdbqt.py
--rw-r--r--   0 runner    (1001) docker     (127)    46812 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/molsetup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10383 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/openff_xml_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    16917 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/preparation.py
--rw-r--r--   0 runner    (1001) docker     (127)    20781 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/rdkit_mol_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     8486 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/reactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    20165 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/receptor_pdbqt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 18:06:09.694564 meeko-0.6.0a2/meeko/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/utils/autodock4_atom_types_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/utils/covalent_radius_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    14425 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/utils/geomutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/utils/obutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/utils/pdbutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/utils/rdkitutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13324 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/utils/van_der_waals_radius_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    26244 2023-11-30 18:05:58.000000 meeko-0.6.0a2/meeko/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 18:06:09.698564 meeko-0.6.0a2/meeko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14128 2023-11-30 18:06:09.000000 meeko-0.6.0a2/meeko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2023-11-30 18:06:09.000000 meeko-0.6.0a2/meeko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 18:06:09.000000 meeko-0.6.0a2/meeko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 18:06:09.000000 meeko-0.6.0a2/meeko.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-30 18:06:09.000000 meeko-0.6.0a2/meeko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-30 18:06:09.000000 meeko-0.6.0a2/meeko.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 18:06:09.694564 meeko-0.6.0a2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5385 2023-11-30 18:05:58.000000 meeko-0.6.0a2/scripts/mk_export.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-11-30 18:05:58.000000 meeko-0.6.0a2/scripts/mk_get_openff_epsilon_sigma.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18592 2023-11-30 18:05:58.000000 meeko-0.6.0a2/scripts/mk_prepare_ligand.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24606 2023-11-30 18:05:58.000000 meeko-0.6.0a2/scripts/mk_prepare_receptor.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-30 18:06:09.698564 meeko-0.6.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2023-11-30 18:05:58.000000 meeko-0.6.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 18:06:09.698564 meeko-0.6.0a2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2023-11-30 18:05:58.000000 meeko-0.6.0a2/test/test-oids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 07:35:44.195423 meeko-0.6.0a3/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-02-02 07:35:36.000000 meeko-0.6.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14393 2024-02-02 07:35:44.195423 meeko-0.6.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-02-02 07:35:36.000000 meeko-0.6.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 07:35:44.191423 meeko-0.6.0a3/meeko/
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 07:35:44.191423 meeko-0.6.0a3/meeko/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/analysis/fingerprint_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11922 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/analysis/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13820 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/atomtyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/bondtyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9317 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/covalentbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 07:35:44.191423 meeko-0.6.0a3/meeko/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/data/atomtypes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/data/flexres_templates.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 07:35:44.195423 meeko-0.6.0a3/meeko/data/params/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/data/params/ad4_desolv_param.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/data/params/ad4_desolv_volume.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/data/params/ad4_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/data/params/ad4_vdw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/data/params/example_offatom_charge.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/data/params/vina_params.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/data/pi_non_aromatic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   191805 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/data/prot_res_params.json
+-rw-r--r--   0 runner    (1001) docker     (127)   205550 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/data/residue_params.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/data/waterfield.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/espalomatyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/flexibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/gridbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/hydrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47693 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/linked_rdkit_chorizo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/macrocycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32118 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/molecule_pdbqt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46913 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/molsetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10383 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/openff_xml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17027 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/preparation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20857 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/rdkit_mol_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/reactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20087 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/receptor_pdbqt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 07:35:44.195423 meeko-0.6.0a3/meeko/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/utils/autodock4_atom_types_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/utils/covalent_radius_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14425 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/utils/geomutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/utils/obutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/utils/pdbutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/utils/rdkitutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/utils/van_der_waals_radius_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26116 2024-02-02 07:35:37.000000 meeko-0.6.0a3/meeko/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 07:35:44.195423 meeko-0.6.0a3/meeko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14393 2024-02-02 07:35:44.000000 meeko-0.6.0a3/meeko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-02-02 07:35:44.000000 meeko-0.6.0a3/meeko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 07:35:44.000000 meeko-0.6.0a3/meeko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 07:35:44.000000 meeko-0.6.0a3/meeko.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-02 07:35:44.000000 meeko-0.6.0a3/meeko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-02 07:35:44.000000 meeko-0.6.0a3/meeko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 07:35:44.195423 meeko-0.6.0a3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5385 2024-02-02 07:35:37.000000 meeko-0.6.0a3/scripts/mk_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-02 07:35:37.000000 meeko-0.6.0a3/scripts/mk_get_openff_epsilon_sigma.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18592 2024-02-02 07:35:37.000000 meeko-0.6.0a3/scripts/mk_prepare_ligand.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26233 2024-02-02 07:35:37.000000 meeko-0.6.0a3/scripts/mk_prepare_receptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 07:35:44.195423 meeko-0.6.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-02-02 07:35:37.000000 meeko-0.6.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 07:35:44.195423 meeko-0.6.0a3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-02 07:35:37.000000 meeko-0.6.0a3/test/test-oids.py
```

### Comparing `meeko-0.6.0a2/LICENSE` & `meeko-0.6.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/PKG-INFO` & `meeko-0.6.0a3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meeko
-Version: 0.6.0a2
+Version: 0.6.0a3
 Summary: Python package for preparing small molecule for docking
 Home-page: https://github.com/ccsb-scripps/meeko
 Author: Forli Lab
 Author-email: forli@scripps.edu
 License: LGPL-2.1
 Keywords: molecular modeling,drug design,docking,autodock
 Classifier: Environment :: Console
@@ -29,15 +29,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.18
 
 # Meeko: preparation of small molecules for AutoDock
 
 [![API stability](https://img.shields.io/badge/stable%20API-no-orange)](https://shields.io/)
-[![PyPI version fury.io](https://img.shields.io/badge/version-0.6.0--alpha.2-green.svg)](https://pypi.python.org/pypi/ansicolortags/)
+[![PyPI version fury.io](https://img.shields.io/badge/version-0.6.0--alpha.3-green.svg)](https://pypi.python.org/pypi/ansicolortags/)
 
 Meeko reads an RDKit molecule object and writes a PDBQT string (or file)
 for [AutoDock-Vina](https://github.com/ccsb-scripps/AutoDock-Vina)
 and [AutoDock-GPU](https://github.com/ccsb-scripps/AutoDock-GPU).
 It converts the docking output to RDKit molecules and
 SD files, without loss of bond orders.
 
@@ -63,15 +63,15 @@
 and RDKit issues
 [1755](https://github.com/rdkit/rdkit/issues/1755) and
 [917](https://github.com/rdkit/rdkit/issues/917). So, what could go wrong?
 For example, reading Mol2 files from ZINC
 [led to incorrect net charge of some molecules.](https://github.com/forlilab/Meeko/issues/63)
 
 
-## v0.6.0-alpha.2
+## v0.6.0-alpha.3
 
 This release aims to distribute an enhanced `mk_prepare_receptor.py`.
 Some features are still being developed, hence the `-alpha` suffix in the version.
 Reactive docking is not working in v0.6.0-alpha, but should be restored soon.
 Documentation is also work in progress.
 
 
@@ -306,14 +306,19 @@
     --receptor protein.pdb\
     --rec_residue ":CYS:6"\
     --tether_smarts "NC(=O)C(O)(C)SCC"\
     --tether_smarts_indices 9 8\
     -o prepared.pdbqt
 ```
 
+Prody is required for preparing ligands as flexible sidechains.
+Often, `pip install prody` suffices to install Prody in the currently
+active virtual environment (e.g., conda). For more detailed installation
+instructions visit http://prody.csb.pitt.edu/downloads/.
+
 ## Reactive Docking
 
 ### 1. Prepare protein with waterkit
 Follow `wk_prepare_receptor.py` instructions and run with `--pdb`.
 The goal of this step is to perform essential fixes to the protein
 (such as missing atoms), to add hydrogens, and to follow the Amber
 naming scheme for atoms and residues, e.g., `HIE` or `HID`
```

### Comparing `meeko-0.6.0a2/README.md` & `meeko-0.6.0a3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Meeko: preparation of small molecules for AutoDock
 
 [![API stability](https://img.shields.io/badge/stable%20API-no-orange)](https://shields.io/)
-[![PyPI version fury.io](https://img.shields.io/badge/version-0.6.0--alpha.2-green.svg)](https://pypi.python.org/pypi/ansicolortags/)
+[![PyPI version fury.io](https://img.shields.io/badge/version-0.6.0--alpha.3-green.svg)](https://pypi.python.org/pypi/ansicolortags/)
 
 Meeko reads an RDKit molecule object and writes a PDBQT string (or file)
 for [AutoDock-Vina](https://github.com/ccsb-scripps/AutoDock-Vina)
 and [AutoDock-GPU](https://github.com/ccsb-scripps/AutoDock-GPU).
 It converts the docking output to RDKit molecules and
 SD files, without loss of bond orders.
 
@@ -31,15 +31,15 @@
 and RDKit issues
 [1755](https://github.com/rdkit/rdkit/issues/1755) and
 [917](https://github.com/rdkit/rdkit/issues/917). So, what could go wrong?
 For example, reading Mol2 files from ZINC
 [led to incorrect net charge of some molecules.](https://github.com/forlilab/Meeko/issues/63)
 
 
-## v0.6.0-alpha.2
+## v0.6.0-alpha.3
 
 This release aims to distribute an enhanced `mk_prepare_receptor.py`.
 Some features are still being developed, hence the `-alpha` suffix in the version.
 Reactive docking is not working in v0.6.0-alpha, but should be restored soon.
 Documentation is also work in progress.
 
 
@@ -274,14 +274,19 @@
     --receptor protein.pdb\
     --rec_residue ":CYS:6"\
     --tether_smarts "NC(=O)C(O)(C)SCC"\
     --tether_smarts_indices 9 8\
     -o prepared.pdbqt
 ```
 
+Prody is required for preparing ligands as flexible sidechains.
+Often, `pip install prody` suffices to install Prody in the currently
+active virtual environment (e.g., conda). For more detailed installation
+instructions visit http://prody.csb.pitt.edu/downloads/.
+
 ## Reactive Docking
 
 ### 1. Prepare protein with waterkit
 Follow `wk_prepare_receptor.py` instructions and run with `--pdb`.
 The goal of this step is to perform essential fixes to the protein
 (such as missing atoms), to add hydrogens, and to follow the Amber
 naming scheme for atoms and residues, e.g., `HIE` or `HID`
```

### Comparing `meeko-0.6.0a2/meeko/__init__.py` & `meeko-0.6.0a3/meeko/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
 # Meeko
 #
 
-__version__ = "0.6.0-alpha.2"
+__version__ = "0.6.0-alpha.3"
 
 try:
     import openbabel
 except ImportError:
     _has_openbabel = False
 else:
     _has_openbabel = True
```

### Comparing `meeko-0.6.0a2/meeko/analysis/fingerprint_interactions.py` & `meeko-0.6.0a3/meeko/analysis/fingerprint_interactions.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/analysis/interactions.py` & `meeko-0.6.0a3/meeko/analysis/interactions.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/atomtyper.py` & `meeko-0.6.0a3/meeko/atomtyper.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/bondtyper.py` & `meeko-0.6.0a3/meeko/bondtyper.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/covalentbuilder.py` & `meeko-0.6.0a3/meeko/covalentbuilder.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/data/atomtypes.txt` & `meeko-0.6.0a3/meeko/data/atomtypes.txt`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/data/flexres_templates.json` & `meeko-0.6.0a3/meeko/data/flexres_templates.json`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/data/params/ad4_desolv_param.json` & `meeko-0.6.0a3/meeko/data/params/ad4_desolv_param.json`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/data/params/ad4_desolv_volume.json` & `meeko-0.6.0a3/meeko/data/params/ad4_desolv_volume.json`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/data/params/ad4_types.json` & `meeko-0.6.0a3/meeko/data/params/ad4_types.json`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/data/params/ad4_vdw.json` & `meeko-0.6.0a3/meeko/data/params/ad4_vdw.json`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/data/params/vina_params.json` & `meeko-0.6.0a3/meeko/data/params/vina_params.json`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/data/pi_non_aromatic.txt` & `meeko-0.6.0a3/meeko/data/pi_non_aromatic.txt`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/data/prot_res_params.json` & `meeko-0.6.0a3/meeko/data/prot_res_params.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9183429118773947%*

 * *Differences: {"'ACE'": "{'atom_ignore': [False, False, False, True, True, True], 'charge': [0.196, -0.3, 0.104, "*

 * *          "0.0, 0.0, 0.0], delete: ['gasteiger']}",*

 * * "'ALA'": "{'atom_ignore': [False, False, False, True, False, False, False, True, True, True], "*

 * *          "'charge': [0.243, -0.272, 0.168, 0.0, -0.344, 0.164, 0.041, 0.0, 0.0, 0.0], delete: "*

 * *          "['gasteiger']}",*

 * * "'ARG'": "{'atom_ignore': [False, False, False, True, False, False, False, True, True, False, "*

 * *          'True, True, False, True, True […]*

```diff
@@ -44,14 +44,22 @@
             33.5103,
             17.1573,
             33.5103,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            true,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CH3",
             "H1",
             "H2",
             "H3"
@@ -85,15 +93,15 @@
                 4
             ],
             [
                 2,
                 5
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.196,
             -0.3,
             0.104,
             0.0,
             0.0,
             0.0
         ],
@@ -200,14 +208,26 @@
             22.4493,
             0.0,
             33.5103,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -266,15 +286,15 @@
                 8
             ],
             [
                 6,
                 9
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.243,
             -0.272,
             0.168,
             0.0,
             -0.344,
             0.164,
             0.041,
@@ -485,14 +505,40 @@
             22.4493,
             0.0,
             0.0,
             22.4493,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -635,15 +681,15 @@
                 22
             ],
             [
                 21,
                 23
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.242,
             -0.273,
             0.171,
             0.0,
             -0.344,
             0.164,
             0.038,
@@ -858,14 +904,29 @@
             0.0,
             0.0,
             33.5103,
             17.1573,
             17.1573,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -942,15 +1003,15 @@
                 11
             ],
             [
                 11,
                 12
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.242,
             -0.273,
             0.182,
             0.0,
             -0.342,
             0.164,
             0.157,
@@ -1116,14 +1177,30 @@
             0.0,
             33.5103,
             17.1573,
             22.4493,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -1206,15 +1283,15 @@
                 12
             ],
             [
                 11,
                 13
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.242,
             -0.273,
             0.18,
             0.0,
             -0.342,
             0.164,
             0.134,
@@ -1373,14 +1450,28 @@
             33.5103,
             0.0,
             0.0,
             33.5103,
             17.1573,
             17.1573
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -1451,15 +1542,15 @@
                 10
             ],
             [
                 9,
                 11
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.242,
             -0.273,
             0.176,
             0.0,
             -0.343,
             0.164,
             0.087,
@@ -1602,14 +1693,27 @@
             22.4493,
             0.0,
             33.5103,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            true
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -1673,15 +1777,15 @@
                 9
             ],
             [
                 7,
                 10
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.532,
             0.066,
             -0.531,
             0.129,
             0.0,
             -0.339,
             0.169,
@@ -1903,14 +2007,41 @@
             22.4493,
             0.0,
             0.0,
             22.4493,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -2058,15 +2189,15 @@
                 23
             ],
             [
                 22,
                 24
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.541,
             0.065,
             -0.541,
             0.13,
             0.0,
             -0.344,
             0.166,
@@ -2292,14 +2423,30 @@
             0.0,
             0.0,
             33.5103,
             17.1573,
             17.1573,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -2381,15 +2528,15 @@
                 12
             ],
             [
                 12,
                 13
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.539,
             0.065,
             -0.538,
             0.141,
             0.0,
             -0.342,
             0.167,
@@ -2566,14 +2713,31 @@
             0.0,
             33.5103,
             17.1573,
             22.4493,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -2661,15 +2825,15 @@
                 13
             ],
             [
                 12,
                 14
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.538,
             0.065,
             -0.538,
             0.14,
             0.0,
             -0.342,
             0.167,
@@ -2839,14 +3003,29 @@
             33.5103,
             0.0,
             0.0,
             33.5103,
             17.1573,
             17.1573
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -2922,15 +3101,15 @@
                 11
             ],
             [
                 10,
                 12
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.538,
             0.065,
             -0.538,
             0.135,
             0.0,
             -0.342,
             0.167,
@@ -3078,14 +3257,27 @@
             22.4493,
             0.0,
             33.5103,
             0.0,
             0.0,
             33.5103
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -3149,15 +3341,15 @@
                 9
             ],
             [
                 7,
                 10
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.537,
             0.063,
             -0.537,
             0.106,
             0.0,
             -0.343,
             0.167,
@@ -3301,14 +3493,28 @@
             0.0,
             33.5103,
             0.0,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -3378,15 +3584,15 @@
                 10
             ],
             [
                 10,
                 11
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.534,
             0.067,
             -0.534,
             0.14,
             0.0,
             -0.338,
             0.168,
@@ -3529,14 +3735,27 @@
             22.4493,
             0.0,
             33.5103,
             0.0,
             0.0,
             33.5103
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -3601,15 +3820,15 @@
                 9
             ],
             [
                 7,
                 10
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.533,
             0.067,
             -0.533,
             0.143,
             0.0,
             -0.338,
             0.168,
@@ -3783,14 +4002,33 @@
             0.0,
             0.0,
             33.5103,
             17.1573,
             17.1573,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -3890,15 +4128,15 @@
                 15
             ],
             [
                 15,
                 16
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.539,
             0.065,
             -0.54,
             0.13,
             0.0,
             -0.342,
             0.167,
@@ -4108,14 +4346,34 @@
             0.0,
             33.5103,
             17.1573,
             22.4493,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -4221,15 +4479,15 @@
                 16
             ],
             [
                 15,
                 17
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.539,
             0.065,
             -0.539,
             0.13,
             0.0,
             -0.342,
             0.167,
@@ -4432,14 +4690,32 @@
             33.5103,
             0.0,
             0.0,
             33.5103,
             17.1573,
             17.1573
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -4533,15 +4809,15 @@
                 14
             ],
             [
                 13,
                 15
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.538,
             0.065,
             -0.538,
             0.13,
             0.0,
             -0.342,
             0.167,
@@ -4686,14 +4962,24 @@
             17.1573,
             33.5103,
             0.0,
             22.4493,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            true
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA2",
             "N",
@@ -4739,15 +5025,15 @@
                 6
             ],
             [
                 3,
                 7
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.532,
             0.063,
             -0.531,
             0.173,
             0.0,
             -0.341,
             0.168,
@@ -4912,14 +5198,34 @@
             0.0,
             33.5103,
             0.0,
             22.4493,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            true
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -5029,15 +5335,15 @@
                 17
             ],
             [
                 16,
                 10
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.538,
             0.065,
             -0.537,
             0.136,
             0.0,
             -0.342,
             0.167,
@@ -5252,14 +5558,34 @@
             33.5103,
             0.0,
             22.4493,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -5369,15 +5695,15 @@
                 17
             ],
             [
                 16,
                 10
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.538,
             0.065,
             -0.537,
             0.136,
             0.0,
             -0.342,
             0.167,
@@ -5598,14 +5924,35 @@
             33.5103,
             0.0,
             22.4493,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -5721,15 +6068,15 @@
                 18
             ],
             [
                 17,
                 10
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.541,
             0.065,
             -0.541,
             0.138,
             0.0,
             -0.343,
             0.166,
@@ -5961,14 +6308,36 @@
             0.0,
             0.0,
             33.5103,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            false,
+            true,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            true
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -6086,15 +6455,15 @@
                 18
             ],
             [
                 16,
                 19
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.531,
             0.066,
             -0.531,
             0.135,
             0.0,
             -0.338,
             0.169,
@@ -6331,14 +6700,36 @@
             0.0,
             0.0,
             33.5103,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            false,
+            true,
+            true,
+            true,
+            false,
+            true,
+            true,
+            true
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -6456,15 +6847,15 @@
                 18
             ],
             [
                 16,
                 19
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.532,
             0.066,
             -0.531,
             0.132,
             0.0,
             -0.338,
             0.169,
@@ -6713,14 +7104,38 @@
             33.5103,
             0.0,
             0.0,
             22.4493,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -6850,15 +7265,15 @@
                 20
             ],
             [
                 19,
                 21
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.536,
             0.065,
             -0.537,
             0.131,
             0.0,
             -0.34,
             0.168,
@@ -7123,14 +7538,39 @@
             0.0,
             0.0,
             22.4493,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -7266,15 +7706,15 @@
                 21
             ],
             [
                 19,
                 22
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.539,
             0.065,
             -0.538,
             0.13,
             0.0,
             -0.343,
             0.167,
@@ -7514,14 +7954,34 @@
             0.0,
             33.5103,
             33.5103,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            true,
+            true,
+            true
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -7627,15 +8087,15 @@
                 16
             ],
             [
                 14,
                 17
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.535,
             0.066,
             -0.535,
             0.132,
             0.0,
             -0.339,
             0.168,
@@ -7868,14 +8328,37 @@
             33.5103,
             0.0,
             33.5103,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            true,
+            false,
+            true,
+            false,
+            true,
+            false,
+            true,
+            false,
+            true
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -8003,15 +8486,15 @@
                 20
             ],
             [
                 19,
                 10
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.532,
             0.066,
             -0.532,
             0.136,
             0.0,
             -0.338,
             0.169,
@@ -8223,14 +8706,31 @@
             33.5103,
             0.0,
             0.0,
             33.5103,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -8322,15 +8822,15 @@
                 14
             ],
             [
                 12,
                 5
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.53,
             0.066,
             -0.53,
             0.135,
             0.0,
             -0.324,
             0.034,
@@ -8494,14 +8994,28 @@
             0.0,
             33.5103,
             0.0,
             0.0,
             17.1573,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -8571,15 +9085,15 @@
                 10
             ],
             [
                 10,
                 11
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.536,
             0.067,
             -0.535,
             0.156,
             0.0,
             -0.339,
             0.168,
@@ -8746,14 +9260,31 @@
             33.5103,
             0.0,
             0.0,
             0.0,
             17.1573,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            false,
+            true,
+            true,
+            true,
+            false,
+            false
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -8841,15 +9372,15 @@
                 13
             ],
             [
                 13,
                 14
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.536,
             0.067,
             -0.536,
             0.159,
             0.0,
             -0.339,
             0.168,
@@ -9091,14 +9622,41 @@
             33.5103,
             0.0,
             33.5103,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            true,
+            false,
+            true,
+            false,
+            true
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -9254,15 +9812,15 @@
                 10
             ],
             [
                 23,
                 15
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.536,
             0.065,
             -0.536,
             0.135,
             0.0,
             -0.341,
             0.167,
@@ -9536,14 +10094,38 @@
             17.1573,
             0.0,
             33.5103,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            true,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            true
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -9677,15 +10259,15 @@
                 21
             ],
             [
                 20,
                 10
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.537,
             0.065,
             -0.538,
             0.135,
             0.0,
             -0.341,
             0.167,
@@ -9914,14 +10496,33 @@
             0.0,
             0.0,
             33.5103,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            false,
+            true,
+            true,
+            true,
+            false,
+            true,
+            true,
+            true
+        ],
         "atom_name": [
             "OXT",
             "C",
             "O",
             "CA",
             "HA",
             "N",
@@ -10021,15 +10622,15 @@
                 15
             ],
             [
                 13,
                 16
             ]
         ],
-        "gasteiger": [
+        "charge": [
             -0.531,
             0.066,
             -0.531,
             0.134,
             0.0,
             -0.338,
             0.169,
@@ -10191,14 +10792,26 @@
             22.4493,
             0.0,
             33.5103,
             0.0,
             0.0,
             33.5103
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -10257,15 +10870,15 @@
                 8
             ],
             [
                 6,
                 9
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.24,
             -0.273,
             0.147,
             0.0,
             -0.346,
             0.164,
             -0.144,
@@ -10398,14 +11011,27 @@
             0.0,
             33.5103,
             0.0,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -10470,15 +11096,15 @@
                 9
             ],
             [
                 9,
                 10
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.243,
             -0.272,
             0.181,
             0.0,
             -0.342,
             0.164,
             0.101,
@@ -10610,14 +11236,26 @@
             22.4493,
             0.0,
             33.5103,
             0.0,
             0.0,
             33.5103
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -10677,15 +11315,15 @@
                 8
             ],
             [
                 6,
                 9
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.244,
             -0.272,
             0.183,
             0.0,
             -0.343,
             0.164,
             0.116,
@@ -10848,14 +11486,32 @@
             0.0,
             0.0,
             33.5103,
             17.1573,
             17.1573,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -10950,15 +11606,15 @@
                 14
             ],
             [
                 14,
                 15
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.242,
             -0.273,
             0.171,
             0.0,
             -0.344,
             0.164,
             0.047,
@@ -11157,14 +11813,33 @@
             0.0,
             33.5103,
             17.1573,
             22.4493,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -11265,15 +11940,15 @@
                 15
             ],
             [
                 14,
                 16
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.242,
             -0.273,
             0.171,
             0.0,
             -0.343,
             0.164,
             0.045,
@@ -11465,14 +12140,31 @@
             33.5103,
             0.0,
             0.0,
             33.5103,
             17.1573,
             17.1573
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -11561,15 +12253,15 @@
                 13
             ],
             [
                 12,
                 14
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.242,
             -0.273,
             0.171,
             0.0,
             -0.344,
             0.164,
             0.041,
@@ -11703,14 +12395,23 @@
             17.1573,
             33.5103,
             0.0,
             22.4493,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA2",
             "N",
             "H",
@@ -11751,15 +12452,15 @@
                 5
             ],
             [
                 2,
                 6
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.239,
             -0.273,
             0.216,
             0.0,
             -0.346,
             0.164,
             0.0
@@ -11913,14 +12614,33 @@
             0.0,
             33.5103,
             0.0,
             22.4493,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -12025,15 +12745,15 @@
                 16
             ],
             [
                 15,
                 9
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.242,
             -0.272,
             0.177,
             0.0,
             -0.343,
             0.164,
             0.09,
@@ -12237,14 +12957,33 @@
             33.5103,
             0.0,
             22.4493,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -12349,15 +13088,15 @@
                 16
             ],
             [
                 15,
                 9
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.242,
             -0.272,
             0.177,
             0.0,
             -0.343,
             0.164,
             0.093,
@@ -12567,14 +13306,34 @@
             33.5103,
             0.0,
             22.4493,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -12685,15 +13444,15 @@
                 17
             ],
             [
                 16,
                 9
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.242,
             -0.273,
             0.179,
             0.0,
             -0.343,
             0.164,
             0.119,
@@ -12914,14 +13673,35 @@
             0.0,
             0.0,
             33.5103,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            false,
+            true,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -13034,15 +13814,15 @@
                 17
             ],
             [
                 15,
                 18
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.243,
             -0.272,
             0.174,
             0.0,
             -0.343,
             0.164,
             0.018,
@@ -13268,14 +14048,35 @@
             0.0,
             0.0,
             33.5103,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            false,
+            true,
+            true,
+            true,
+            false,
+            true,
+            true,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -13388,15 +14189,15 @@
                 17
             ],
             [
                 15,
                 18
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.243,
             -0.272,
             0.172,
             0.0,
             -0.345,
             0.165,
             0.038,
@@ -13634,14 +14435,37 @@
             33.5103,
             0.0,
             0.0,
             22.4493,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -13766,15 +14590,15 @@
                 19
             ],
             [
                 18,
                 20
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.243,
             -0.272,
             0.171,
             0.0,
             -0.344,
             0.164,
             0.035,
@@ -14028,14 +14852,38 @@
             0.0,
             0.0,
             22.4493,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -14166,15 +15014,15 @@
                 20
             ],
             [
                 18,
                 21
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.242,
             -0.273,
             0.171,
             0.0,
             -0.344,
             0.164,
             0.035,
@@ -14403,14 +15251,33 @@
             0.0,
             33.5103,
             33.5103,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            true,
+            true,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -14511,15 +15378,15 @@
                 15
             ],
             [
                 13,
                 16
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.242,
             -0.272,
             0.172,
             0.0,
             -0.344,
             0.164,
             0.046,
@@ -14627,21 +15494,24 @@
         ],
         "ad4_sol_par": [
             -0.0011
         ],
         "ad4_sol_vol": [
             1.56
         ],
+        "atom_ignore": [
+            false
+        ],
         "atom_name": [
             "OW"
         ],
         "atom_type": [
             "OA"
         ],
-        "gasteiger": [
+        "charge": [
             2.0
         ],
         "smiles": "[Mg]",
         "vina_acceptor": [
             false
         ],
         "vina_donor": [
@@ -14735,14 +15605,28 @@
             0.0,
             0.0,
             33.5103,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -14812,15 +15696,15 @@
                 10
             ],
             [
                 8,
                 11
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.271,
             -0.274,
             0.261,
             0.0,
             -0.356,
             0.338,
             0.338,
@@ -15053,14 +15937,42 @@
             22.4493,
             0.0,
             0.0,
             22.4493,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -15214,15 +16126,15 @@
                 24
             ],
             [
                 23,
                 25
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.274,
             -0.271,
             0.268,
             0.0,
             -0.349,
             0.342,
             0.342,
@@ -15459,14 +16371,31 @@
             0.0,
             0.0,
             33.5103,
             17.1573,
             17.1573,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -15554,15 +16483,15 @@
                 13
             ],
             [
                 13,
                 14
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.274,
             -0.272,
             0.278,
             0.0,
             -0.351,
             0.341,
             0.34,
@@ -15750,14 +16679,32 @@
             0.0,
             33.5103,
             17.1573,
             22.4493,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -15851,15 +16798,15 @@
                 14
             ],
             [
                 13,
                 15
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.274,
             -0.272,
             0.276,
             0.0,
             -0.352,
             0.34,
             0.34,
@@ -16040,14 +16987,30 @@
             33.5103,
             0.0,
             0.0,
             33.5103,
             17.1573,
             17.1573
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -16129,15 +17092,15 @@
                 12
             ],
             [
                 11,
                 13
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.274,
             -0.272,
             0.272,
             0.0,
             -0.352,
             0.34,
             0.34,
@@ -16296,14 +17259,28 @@
             0.0,
             0.0,
             33.5103,
             0.0,
             0.0,
             33.5103
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -16373,15 +17350,15 @@
                 10
             ],
             [
                 8,
                 11
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.271,
             -0.272,
             0.242,
             0.0,
             -0.355,
             0.339,
             0.339,
@@ -16536,14 +17513,29 @@
             0.0,
             33.5103,
             0.0,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -16619,15 +17611,15 @@
                 11
             ],
             [
                 11,
                 12
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.273,
             -0.273,
             0.275,
             0.0,
             -0.354,
             0.339,
             0.339,
@@ -16781,14 +17773,28 @@
             0.0,
             0.0,
             33.5103,
             0.0,
             0.0,
             33.5103
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -16859,15 +17865,15 @@
                 10
             ],
             [
                 8,
                 11
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.273,
             -0.273,
             0.275,
             0.0,
             -0.353,
             0.338,
             0.338,
@@ -17052,14 +18058,34 @@
             0.0,
             0.0,
             33.5103,
             17.1573,
             17.1573,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -17165,15 +18191,15 @@
                 16
             ],
             [
                 16,
                 17
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.273,
             -0.272,
             0.267,
             0.0,
             -0.351,
             0.34,
             0.34,
@@ -17394,14 +18420,35 @@
             0.0,
             33.5103,
             17.1573,
             22.4493,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -17513,15 +18560,15 @@
                 17
             ],
             [
                 16,
                 18
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.273,
             -0.272,
             0.267,
             0.0,
             -0.352,
             0.34,
             0.34,
@@ -17735,14 +18782,33 @@
             33.5103,
             0.0,
             0.0,
             33.5103,
             17.1573,
             17.1573
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -17842,15 +18908,15 @@
                 15
             ],
             [
                 14,
                 16
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.273,
             -0.272,
             0.267,
             0.0,
             -0.352,
             0.34,
             0.34,
@@ -18006,14 +19072,25 @@
             0.0,
             22.4493,
             0.0,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA2",
             "N",
             "H1",
@@ -18065,15 +19142,15 @@
                 7
             ],
             [
                 2,
                 8
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.268,
             -0.275,
             0.353,
             0.0,
             -0.357,
             0.337,
             0.337,
@@ -18249,14 +19326,35 @@
             0.0,
             33.5103,
             0.0,
             22.4493,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -18372,15 +19470,15 @@
                 18
             ],
             [
                 17,
                 11
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.274,
             -0.272,
             0.272,
             0.0,
             -0.352,
             0.34,
             0.34,
@@ -18606,14 +19704,35 @@
             33.5103,
             0.0,
             22.4493,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -18729,15 +19848,15 @@
                 18
             ],
             [
                 17,
                 11
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.274,
             -0.272,
             0.272,
             0.0,
             -0.352,
             0.34,
             0.34,
@@ -18969,14 +20088,36 @@
             33.5103,
             0.0,
             22.4493,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -19098,15 +20239,15 @@
                 19
             ],
             [
                 18,
                 11
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.275,
             -0.271,
             0.276,
             0.0,
             -0.351,
             0.341,
             0.341,
@@ -19349,14 +20490,37 @@
             0.0,
             0.0,
             33.5103,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            true,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -19480,15 +20644,15 @@
                 19
             ],
             [
                 17,
                 20
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.272,
             -0.274,
             0.267,
             0.0,
             -0.355,
             0.337,
             0.338,
@@ -19736,14 +20900,37 @@
             0.0,
             0.0,
             33.5103,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            false,
+            true,
+            true,
+            true,
+            false,
+            true,
+            true,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -19867,15 +21054,15 @@
                 19
             ],
             [
                 17,
                 20
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.271,
             -0.274,
             0.265,
             0.0,
             -0.355,
             0.338,
             0.338,
@@ -20135,14 +21322,39 @@
             33.5103,
             0.0,
             0.0,
             22.4493,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -20278,15 +21490,15 @@
                 21
             ],
             [
                 20,
                 22
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.272,
             -0.272,
             0.266,
             0.0,
             -0.353,
             0.339,
             0.339,
@@ -20562,14 +21774,40 @@
             0.0,
             0.0,
             22.4493,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -20711,15 +21949,15 @@
                 22
             ],
             [
                 20,
                 23
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.274,
             -0.271,
             0.267,
             0.0,
             -0.352,
             0.341,
             0.341,
@@ -20892,14 +22130,22 @@
             33.5103,
             0.0,
             0.0,
             0.0,
             22.4493,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            true,
+            true,
+            true,
+            false,
+            false
+        ],
         "atom_name": [
             "CH3",
             "HH31",
             "HH32",
             "HH33",
             "N",
             "H"
@@ -20933,15 +22179,15 @@
                 4
             ],
             [
                 4,
                 5
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.154,
             0.0,
             0.0,
             0.0,
             -0.33,
             0.176
         ],
@@ -21102,14 +22348,35 @@
             0.0,
             33.5103,
             33.5103,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            false,
+            true,
+            true,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -21221,15 +22488,15 @@
                 17
             ],
             [
                 15,
                 18
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.272,
             -0.273,
             0.266,
             0.0,
             -0.353,
             0.338,
             0.338,
@@ -21473,14 +22740,38 @@
             33.5103,
             0.0,
             33.5103,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            true,
+            false,
+            true,
+            false,
+            true,
+            false,
+            true,
+            false,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -21614,15 +22905,15 @@
                 21
             ],
             [
                 20,
                 11
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.272,
             -0.274,
             0.269,
             0.0,
             -0.355,
             0.338,
             0.338,
@@ -21845,14 +23136,32 @@
             33.5103,
             0.0,
             0.0,
             33.5103,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H2",
@@ -21950,15 +23259,15 @@
                 15
             ],
             [
                 13,
                 4
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.271,
             -0.274,
             0.266,
             0.0,
             -0.343,
             0.339,
             0.339,
@@ -22133,14 +23442,29 @@
             0.0,
             33.5103,
             0.0,
             0.0,
             17.1573,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -22216,15 +23540,15 @@
                 11
             ],
             [
                 11,
                 12
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.276,
             -0.272,
             0.291,
             0.0,
             -0.351,
             0.339,
             0.339,
@@ -22402,14 +23726,32 @@
             33.5103,
             0.0,
             0.0,
             0.0,
             17.1573,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            true,
+            true,
+            true,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -22503,15 +23845,15 @@
                 14
             ],
             [
                 14,
                 15
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.275,
             -0.272,
             0.294,
             0.0,
             -0.35,
             0.339,
             0.339,
@@ -22764,14 +24106,42 @@
             33.5103,
             0.0,
             33.5103,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            true,
+            false,
+            true,
+            false,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -22933,15 +24303,15 @@
                 11
             ],
             [
                 24,
                 16
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.273,
             -0.272,
             0.27,
             0.0,
             -0.353,
             0.339,
             0.339,
@@ -23226,14 +24596,39 @@
             17.1573,
             0.0,
             33.5103,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            true,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -23373,15 +24768,15 @@
                 22
             ],
             [
                 21,
                 11
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.274,
             -0.272,
             0.271,
             0.0,
             -0.352,
             0.34,
             0.34,
@@ -23621,14 +25016,34 @@
             0.0,
             0.0,
             33.5103,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            true,
+            true,
+            true,
+            false,
+            true,
+            true,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H1",
@@ -23734,15 +25149,15 @@
                 16
             ],
             [
                 14,
                 17
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.272,
             -0.274,
             0.267,
             0.0,
             -0.354,
             0.337,
             0.337,
@@ -23969,14 +25384,36 @@
             33.5103,
             0.0,
             33.5103,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            true,
+            false,
+            true,
+            false,
+            true,
+            false,
+            true,
+            false,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -24099,15 +25536,15 @@
                 19
             ],
             [
                 18,
                 9
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.243,
             -0.272,
             0.175,
             0.0,
             -0.343,
             0.164,
             0.07,
@@ -24308,14 +25745,30 @@
             33.5103,
             0.0,
             0.0,
             33.5103,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true,
+            false,
+            true,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "CB",
@@ -24402,15 +25855,15 @@
                 13
             ],
             [
                 11,
                 4
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.243,
             -0.271,
             0.175,
             0.0,
             -0.329,
             0.037,
             0.0,
@@ -24563,14 +26016,27 @@
             0.0,
             33.5103,
             0.0,
             0.0,
             17.1573,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -24635,15 +26101,15 @@
                 9
             ],
             [
                 9,
                 10
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.244,
             -0.272,
             0.197,
             0.0,
             -0.342,
             0.164,
             0.191,
@@ -24799,14 +26265,30 @@
             33.5103,
             0.0,
             0.0,
             0.0,
             17.1573,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            false,
+            true,
+            true,
+            true,
+            false,
+            false
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -24889,15 +26371,15 @@
                 12
             ],
             [
                 12,
                 13
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.245,
             -0.273,
             0.199,
             0.0,
             -0.341,
             0.164,
             0.143,
@@ -25147,14 +26629,40 @@
             33.5103,
             0.0,
             33.5103,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            true,
+            false,
+            true,
+            false,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -25305,15 +26813,15 @@
                 9
             ],
             [
                 22,
                 14
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.242,
             -0.272,
             0.175,
             0.0,
             -0.343,
             0.164,
             0.072,
@@ -25576,14 +27084,37 @@
             17.1573,
             0.0,
             33.5103,
             0.0,
             33.5103,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            true,
+            false,
+            false,
+            true,
+            false,
+            true,
+            false,
+            false,
+            false,
+            false,
+            true,
+            false,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -25712,15 +27243,15 @@
                 20
             ],
             [
                 19,
                 9
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.243,
             -0.272,
             0.175,
             0.0,
             -0.343,
             0.164,
             0.07,
@@ -25938,14 +27469,32 @@
             0.0,
             0.0,
             33.5103,
             0.0,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false,
+            true,
+            false,
+            false,
+            false,
+            true,
+            false,
+            true,
+            true,
+            true,
+            false,
+            true,
+            true,
+            true
+        ],
         "atom_name": [
             "C",
             "O",
             "CA",
             "HA",
             "N",
             "H",
@@ -26040,15 +27589,15 @@
                 14
             ],
             [
                 12,
                 15
             ]
         ],
-        "gasteiger": [
+        "charge": [
             0.243,
             -0.272,
             0.173,
             0.0,
             -0.343,
             0.164,
             0.015,
@@ -26163,25 +27712,30 @@
             0.00051
         ],
         "ad4_sol_vol": [
             17.1573,
             0.0,
             0.0
         ],
+        "atom_ignore": [
+            false,
+            false,
+            false
+        ],
         "atom_name": [
             "OW",
             "HW1",
             "HW2"
         ],
         "atom_type": [
             "OA",
             "HD",
             "HD"
         ],
-        "gasteiger": [
+        "charge": [
             -0.412,
             0.206,
             0.206
         ],
         "smiles": "O([H])[H]",
         "vina_acceptor": [
             true,
```

### Comparing `meeko-0.6.0a2/meeko/data/residue_params.json` & `meeko-0.6.0a3/meeko/data/residue_params.json`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/data/waterfield.txt` & `meeko-0.6.0a3/meeko/data/waterfield.txt`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/espalomatyper.py` & `meeko-0.6.0a3/meeko/espalomatyper.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/flexibility.py` & `meeko-0.6.0a3/meeko/flexibility.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/gridbox.py` & `meeko-0.6.0a3/meeko/gridbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -146,9 +146,15 @@
     center_y = (y_min + y_max) / 2.0
     center_z = (z_min + z_max) / 2.0
     size_x = x_max - x_min + 2 * padding
     size_y = y_max - y_min + 2 * padding
     size_z = z_max - z_min + 2 * padding
     return (center_x, center_y, center_z), (size_x, size_y, size_z)
 
+def box_to_vina_string(gridcenter, gridsizes):
+    dims = ['x', 'y', 'z']
+    centers_str = "\n".join([f"center_{d} = {gridcenter[i]}" for i, d in enumerate(dims)])
+    sizes_str = "\n".join([f"size_{d} = {gridsizes[i]}" for i, d in enumerate(dims)])
+    return centers_str + "\n" + sizes_str
+
 boron_silicon_atompar  = "atom_par Si     4.10  0.200  35.8235  -0.00143  0.0  0.0  0  -1  -1  6" + os_linesep
 boron_silicon_atompar += "atom_par B      3.84  0.155  29.6478  -0.00152  0.0  0.0  0  -1  -1  0" + os_linesep
```

### Comparing `meeko-0.6.0a2/meeko/hydrate.py` & `meeko-0.6.0a3/meeko/hydrate.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/linked_rdkit_chorizo.py` & `meeko-0.6.0a3/meeko/linked_rdkit_chorizo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,112 +1,123 @@
 import pathlib
 import json
 from rdkit import Chem
 from rdkit.Chem import rdFMCS
 from rdkit.Chem import rdChemReactions
 from rdkit.Chem.AllChem import EmbedMolecule, AssignBondOrdersFromTemplate
 from .writer import PDBQTWriterLegacy
-from .molsetup import RDKitMoleculeSetup
+from .molsetup import MoleculeSetup
 from .utils.rdkitutils import mini_periodic_table
 from .utils.rdkitutils import react_and_map
+from .utils.pdbutils import PDBAtomInfo
 
 import numpy as np
 
 pkg_dir = pathlib.Path(__file__).parents[0]
 with open(pkg_dir / "data" / "prot_res_params.json") as f:
     chorizo_params = json.load(f)
 
+
 def mapping_by_mcs(mol, ref):
-    mcs_result = rdFMCS.FindMCS([mol,ref], bondCompare=rdFMCS.BondCompare.CompareAny)
+    mcs_result = rdFMCS.FindMCS([mol, ref], bondCompare=rdFMCS.BondCompare.CompareAny)
     mcs_mol = Chem.MolFromSmarts(mcs_result.smartsString)
 
     mol_idxs = mol.GetSubstructMatch(mcs_mol)
     ref_idxs = ref.GetSubstructMatch(mcs_mol)
 
-    atom_map = {i:j for (i,j) in zip(mol_idxs, ref_idxs)}
+    atom_map = {i: j for (i, j) in zip(mol_idxs, ref_idxs)}
     return atom_map
 
+
 def reassign_formal_charge(mol, ref, mapping):
-    #TODO this could be optimized
-    #TODO ref charges could be precalculated to speed up large structures
+    # TODO this could be optimized
+    # TODO ref charges could be precalculated to speed up large structures
     mol_charged_atoms = []
     for idx, atom in enumerate(mol.GetAtoms()):
         if atom.GetFormalCharge() != 0:
             mol_charged_atoms.append(idx)
-            
+
     ref_charged_atoms = []
     for idx, atom in enumerate(ref.GetAtoms()):
         if atom.GetFormalCharge() != 0:
             ref_charged_atoms.append(idx)
-    
-    for (k,v) in mapping.items():
+
+    for (k, v) in mapping.items():
         if k in ref_charged_atoms or v in mol_charged_atoms:
             mol.GetAtomWithIdx(v).SetFormalCharge(ref.GetAtomWithIdx(k).GetFormalCharge())
 
     return mol
 
+
 def reassign_bond_orders(mol, ref, mapping):
-    #TODO this could be optimized
+    # TODO this could be optimized
     for i in mapping.keys():
         for ref_bond in ref.GetAtomWithIdx(i).GetBonds():
             j = ref_bond.GetOtherAtomIdx(i)
             if j in mapping.keys():
                 mol_bond = mol.GetBondBetweenAtoms(mapping[i], mapping[j])
                 mol_bond.SetBondType(ref_bond.GetBondType())
     return mol
 
+
 def h_coord_from_dipeptide(pdb1, pdb2):
-    mol = Chem.MolFromPDBBlock(pdb1+pdb2)
+    mol = Chem.MolFromPDBBlock(pdb1 + pdb2)
     if mol is None:
         print(pdb1)
         print(pdb2)
         raise RuntimeError
     mol_h = Chem.AddHs(mol, addCoords=True)
     ps = Chem.SmilesParserParams()
     ps.removeHs = False
-    template = Chem.MolFromSmiles('C(=O)C([H])N([H])C(=O)C([H])N',ps)
+    template = Chem.MolFromSmiles('C(=O)C([H])N([H])C(=O)C([H])N', ps)
     h_idx = 5
     atom_map = mapping_by_mcs(template, mol_h)
-    
+
     return mol_h.GetConformer().GetAtomPosition(atom_map[h_idx])
 
+
 def h_coord_random_n_terminal(mol, debug=False):
+    idx = mol.GetSubstructMatches(Chem.MolFromSmarts("[Nh1H2X3+0][CX4]"))
+    assert len(idx) == 1, f"expected 1 backbone match got {len(idx)}"
+    nitrogen = mol.GetAtomWithIdx(idx[0][0])
+    nitrogen.SetBoolProp("this_N", True)
     mol_no_h = Chem.RemoveHs(mol)
     for atom in mol_no_h.GetAtoms():
-        if atom.GetProp("atom_name") == "N":
+        if atom.HasProp("this_N") and atom.GetBoolProp("this_N"):
             bb_n_idx = atom.GetIdx()
     mol_h = Chem.AddHs(mol_no_h, addCoords=True)
-    #positions = mol_h.GetConformer().GetPositions()
+    # positions = mol_h.GetConformer().GetPositions()
     bb_n = mol_h.GetAtomWithIdx(bb_n_idx)
     for neighbor in bb_n.GetNeighbors():
         if neighbor.GetAtomicNum() == 1:
             return mol_h.GetConformer().GetAtomPosition(neighbor.GetIdx())
 
 
 def _snap_to_int(value, tolerance=0.12):
     for inc in [-1, 0, 1]:
         if abs(value - int(value) - inc) <= tolerance:
             return int(value) + inc
     return None
 
+
 def divide_int_gracefully(integer, weights, allow_equal_weights_to_differ=False):
     for weight in weights:
         if type(weight) not in [int, float] or weight < 0:
             raise ValueError("weights must be numeric and non-negative")
     if type(integer) != int:
         raise ValueError("integer must be integer")
     inv_total_weight = 1.0 / sum(weights)
-    shares = [w * inv_total_weight for w in weights] # normalize
+    shares = [w * inv_total_weight for w in weights]  # normalize
     result = [_snap_to_int(integer * s, tolerance=0.5) for s in shares]
     surplus = integer - sum(result)
     if surplus == 0:
         return result
     data = [(i, w) for (i, w) in enumerate(weights)]
     data = sorted(data, key=lambda x: x[1], reverse=True)
-    idxs = [i for (i, _) in data] 
+    idxs = [i for (i, _) in data]
     if allow_equal_weights_to_differ:
         groups = [1 for _ in weights]
     else:
         groups = []
         last_weight = None
         for i in idxs:
             if weights[i] == last_weight:
@@ -114,19 +125,19 @@
             else:
                 groups.append(1)
             last_weight = weights[i]
 
     # iterate over all possible combinations of groups
     # this is potentially very slow
     nr_groups = len(groups)
-    for j in range(1, 2**nr_groups):
+    for j in range(1, 2 ** nr_groups):
         n_changes = 0
         combo = []
         for grpidx in range(nr_groups):
-            is_changed = bool(j & 2**grpidx) 
+            is_changed = bool(j & 2 ** grpidx)
             combo.append(is_changed)
             n_changes += is_changed * groups[grpidx]
         if n_changes == abs(surplus):
             break
 
     # add or subtract 1 to distribute surplus
     increment = surplus / abs(surplus)
@@ -135,14 +146,15 @@
         if is_changed:
             for j in range(groups[i]):
                 result[idxs[index]] += increment
                 index += 1
 
     return result
 
+
 def rectify_charges(q_list, net_charge=None, decimals=3):
     """make them 3 decimals and sum to an integer"""
 
     fstr = "%%.%df" % decimals
     charges_dec = [float(fstr % q) for q in q_list]
 
     if net_charge is None:
@@ -151,26 +163,27 @@
             msg = "net charge could not be predicted from input q_list. (residual is beyond tolerance) "
             msg = "Please set the net_charge argument directly"
             raise RuntimeError(msg)
     elif type(net_charge) != int:
         raise TypeError("net charge must be an integer")
 
     surplus = net_charge - sum(charges_dec)
-    surplus_int = _snap_to_int(10**decimals * surplus)
+    surplus_int = _snap_to_int(10 ** decimals * surplus)
 
     if surplus_int == 0:
         return charges_dec
 
     weights = [abs(q) for q in q_list]
     surplus_int_splits = divide_int_gracefully(surplus_int, weights)
     for i, increment in enumerate(surplus_int_splits):
-        charges_dec[i] += 10**-decimals * increment
+        charges_dec[i] += 10 ** -decimals * increment
 
     return charges_dec
 
+
 class LinkedRDKitChorizo:
     """
     This is a class used to represent linked residues and associate them with RDKit and other information
     and there are most likely many more details that should be included in this little blurb.
 
     Attributes
     ----------
@@ -185,112 +198,116 @@
     rxn_nterm_pad: RDKit ChemicalReaction
 
     TODO: Organize the following in a way that makes sense
     residues: dict (string -> ChorizoResidue) #TODO: figure out exact SciPy standard for dictionary key/value notation
     termini: dict (string (representing residue id) -> string (representing what we want the capping to look like))
     deleted_residues: list (string) residue ids to be deleted
     mutate_res_dict: dict (string (representing starting residue id) -> string (representing the desired mutated id))
-    res_templates: dict (string -> rdkit.Chem.rdchem.Mol)
+    res_templates: dict (string -> dict (rdkit_mol and atom_data))
     ambiguous:
     disulfide_bridges:
     suggested_mutations:
     """
 
     cterm_pad_smiles = "CN"
     nterm_pad_smiles = "CC=O"
-    backbone_smarts = "[C:1](=[O:2])[C:3][N:4]" # TODO make sure it matches res only once
+    backbone_smarts = "[C:1](=[O:2])[C:3][N:4]"  # TODO make sure it matches res only once
     backbone = Chem.MolFromSmarts(backbone_smarts)
     backboneh = Chem.MolFromSmarts("[C:1](=[O:2])[C:3][N:4][#1]")
     nterm_pad_backbone_smarts_idxs = (0, 2, 1)
     cterm_pad_backbone_smarts_idxs = (2, 3)
     rxn_cterm_pad = rdChemReactions.ReactionFromSmarts(f"[N:5][C:6].{backbone_smarts}>>[C:6][N:5]{backbone_smarts}")
-    rxn_nterm_pad = rdChemReactions.ReactionFromSmarts(f"[C:5][C:6]=[O:7].{backbone_smarts}>>{backbone_smarts}[C:6](=[O:7])[C:5]")
-
+    rxn_nterm_pad = rdChemReactions.ReactionFromSmarts(
+        f"[C:5][C:6]=[O:7].{backbone_smarts}>>{backbone_smarts}[C:6](=[O:7])[C:5]")
 
-    def __init__(self, pdb_string, params=chorizo_params, mutate_res_dict=None, termini=None, deleted_residues=None, allow_bad_res=False):
+    def __init__(self, pdb_string, params=chorizo_params, mutate_res_dict=None, termini=None, deleted_residues=None,
+                 allow_bad_res=False, skip_auto_disulfide=False):
         suggested_mutations = {}
-        
+
         # Generates the residue representations based purely on the information in the pdb file to begin with.
         self.residues = self._pdb_to_resblocks(pdb_string)
         res_list = self.residues.keys()
-        
+
         # User-specified modifications to the residues, capping of terminal residues and marking residues 
         # as deleted.
         self.termini = self._check_termini(termini, res_list)
         if deleted_residues is None:
             deleted_residues = ()
         self._check_del_res(deleted_residues, self.residues)
         self.deleted_residues = deleted_residues
-        
+
         # User-specified mutations to the residues that we're tracking
         self.mutate_res_dict = mutate_res_dict
-        if mutate_res_dict is not None:
+        if mutate_res_dict is None:
+            mutate_res_dict = {}
+        else:
             self._rename_residues(mutate_res_dict)
 
         # Loads user specified parameters
         self.res_templates, self.ambiguous = self._load_params(params)
-        
+
         # Uses termini and user parameters to 
-        ambiguous_chosen = self.parameterize_residues(self.termini, self.ambiguous)
+        ambiguous_chosen = self.match_residues_templates(self.termini, self.ambiguous)
         suggested_mutations.update(ambiguous_chosen)
 
-        removed_residues = self.getIgnoredResidues()
+        removed_residues = self.get_ignored_residues()
         if len(removed_residues) > 0 and not allow_bad_res:
             for res in removed_residues:
                 suggested_mutations[res] = res
             print("The following mutations are suggested. For HIS, mutate to HID, HIE, or HIP.")
             print(json.dumps(suggested_mutations, indent=2))
             msg = "The following residues could not be processed:" + pathlib.os.linesep
             msg += self.print_residues_by_resname(removed_residues)
             raise RuntimeError(msg)
 
-        self.disulfide_bridges = self._find_disulfide_bridges()
+        if skip_auto_disulfide:
+            self.disulfide_bridges = []
+        else:
+            self.disulfide_bridges = self._find_disulfide_bridges()
         for cys_1, cys_2 in self.disulfide_bridges:
             chain_1, resname_1, resnum_1 = cys_1.split(":")
             chain_2, resname_2, resnum_2 = cys_2.split(":")
             if resname_1 != "CYX" or resname_2 != "CYX":
                 print(f"Likely disulfide bridge between {cys_1} and {cys_2}")
             if resname_1 != "CYX":
                 cyx_1 = f"{chain_1}:CYX:{resnum_1}"
                 suggested_mutations[cys_1] = cyx_1
                 if (cys_1 not in mutate_res_dict) and ((cys_2 not in mutate_res_dict) or resname_2 == "CYX"):
                     self._rename_residues({cys_1: cyx_1})
                     resmol = self.build_resmol(cyx_1, "CYX")
-                    if resmol is not None:
-                        self.residues[cyx_1].rdkit_mol = resmol
-                    else:
-                        self.residues[cyx_1].ignore_residue = True
+                    if resmol is None:
+                        raise RuntimeError("got resmol=None while converting {cys_1} to {cyx_1}")
+                    self.build_molsetup_wrap(cyx_1, "CYX", resmol)
             if resname_2 != "CYX":
                 cyx_2 = f"{chain_2}:CYX:{resnum_2}"
                 suggested_mutations[cys_2] = cyx_2
                 if (cys_2 not in mutate_res_dict) and ((cys_1 not in mutate_res_dict) or resname_1 == "CYX"):
                     self._rename_residues({cys_2: cyx_2})
                     resmol = self.build_resmol(cyx_2, "CYX")
-                    if resmol is not None:
-                        self.residues[cyx_2].rdkit_mol = resmol
-                    else:
-                        self.residues[cyx_2].ignore_residue = True
+                    if resmol is None:
+                        raise RuntimeError("got resmol=None while converting {cys_2} to {cyx_2}")
+                    self.build_molsetup_wrap(cyx_2, "CYX", resmol)
 
         """to_remove = []
         for res_id in self.getIgnoredResidues():
             i = self.res_list.index(res_id)
             to_remove.append(i)
         for i in sorted(to_remove, reverse=True):
             self.res_list.pop(i) """
         self.suggested_mutations = suggested_mutations
         return
 
     def _find_disulfide_bridges(self):
         cys_list = {}
-        cutoff = 2.5 # angstrom
+        cutoff = 2.5  # angstrom
         bridges = []
-        for res in self.residues:
-            if self.residues[res].ignore_residue: continue
+        for res in self.get_valid_residues():
             resname = res.split(":")[1]
-            if resname in ["CYS", "CYX", "CYM"]: # TODO move "protected resnames" next to residue params they are associated with
+            if resname in ["CYS", "CYX",
+                           "CYM"]:  # TODO move "protected resnames" next to residue params they are associated with
                 resmol = self.residues[res].rdkit_mol
                 molxyz = resmol.GetConformer().GetPositions()
                 s_xyz = None
                 for atom in resmol.GetAtoms():
                     if atom.GetAtomicNum() == 16:
                         s_xyz = molxyz[atom.GetIdx()]
                 for cys, other_s_xyz in cys_list.items():
@@ -329,20 +346,20 @@
             elif value.lower() in allowed_n:
                 output[resn] = "N"
             else:
                 raise ValueError("termini value was %s, expected %s or %s" % (value, allowed_c, allowed_n))
         return output
 
     def get_padded_mol(self, resn):
-        #TODO disulfides, ACE, NME
+        # TODO disulfides, ACE, NME
         # TODO double check next/previous res logic for "blunt" ending
         def _join(mol, pad_mol, pad_smarts_mol, rxn, is_res_atom, mapidx, adjacent_mol=None, pad_smarts_idxs=None):
             pad_matches = adjacent_mol.GetSubstructMatches(pad_smarts_mol)
             if len(pad_matches) != 1:
-                raise RuntimeError("expected 1 match but got %d" % (len(pad_matches)))
+                raise RuntimeError(f"expected 1 match but got {len(pad_matches)}, {resn=}")
             conformer = Chem.Conformer(pad_mol.GetNumAtoms())
             pad_mol.AddConformer(conformer)
             if adjacent_mol is not None:
                 for index, smarts_index in enumerate(pad_smarts_idxs):
                     adjacent_mol_index = pad_matches[0][smarts_index]
                     pos = adjacent_mol.GetConformer().GetAtomPosition(adjacent_mol_index)
                     pad_mol.GetConformer().SetAtomPosition(index, pos)
@@ -354,174 +371,177 @@
             index_map["atom_idx"] = index_map["atom_idx"][0][0]
             Chem.SanitizeMol(mol)
             new_is_res_atom = []
             new_mapidx = {}
             for atom in mol.GetAtoms():
                 index = atom.GetIdx()
                 reactant_idx = index_map["reactant_idx"][index]
-                if  reactant_idx == 0:
+                if reactant_idx == 0:
                     new_is_res_atom.append(False)
-                elif reactant_idx == 1: # mol is 2nd reactant (0-index)
-                    atom_idx = index_map["atom_idx"][index] 
+                elif reactant_idx == 1:  # mol is 2nd reactant (0-index)
+                    atom_idx = index_map["atom_idx"][index]
                     new_is_res_atom.append(is_res_atom[atom_idx])
                     if atom_idx in mapidx:
                         new_mapidx[index] = mapidx[atom_idx]
                 else:
                     raise RuntimeError("we have only two reactants, got %d ?" % reactant_idx)
             return mol, new_is_res_atom, new_mapidx
 
         mol = Chem.Mol(self.residues[resn].rdkit_mol)
         is_res_atom = [True for atom in mol.GetAtoms()]
         mapidx = {atom.GetIdx(): atom.GetIdx() for atom in mol.GetAtoms()}
-        if self.residues[resn].previous_id is not None and self.residues[self.residues[resn].previous_id].rdkit_mol is not None:
+        if self.residues[resn].previous_id is not None and self.residues[
+            self.residues[resn].previous_id].rdkit_mol is not None:
             prev_resn = self.residues[resn].previous_id
             prev_mol = self.residues[prev_resn].rdkit_mol
             nterm_pad = Chem.MolFromSmiles(self.nterm_pad_smiles)
             mol, is_res_atom, mapidx = _join(
-                    mol,
-                    nterm_pad,
-                    self.backbone,
-                    self.rxn_nterm_pad,
-                    is_res_atom,
-                    mapidx,
-                    prev_mol,
-                    self.nterm_pad_backbone_smarts_idxs)
-            
+                mol,
+                nterm_pad,
+                self.backbone,
+                self.rxn_nterm_pad,
+                is_res_atom,
+                mapidx,
+                prev_mol,
+                self.nterm_pad_backbone_smarts_idxs)
+
         if self.residues[resn].next_id is not None and self.residues[self.residues[resn].next_id].rdkit_mol is not None:
             next_resn = self.residues[resn].next_id
             next_mol = self.residues[next_resn].rdkit_mol
             cterm_pad = Chem.MolFromSmiles(self.cterm_pad_smiles)
             mol, is_res_atom, mapidx = _join(
-                    mol,
-                    cterm_pad,
-                    self.backbone,
-                    self.rxn_cterm_pad,
-                    is_res_atom,
-                    mapidx,
-                    next_mol, 
-                    self.cterm_pad_backbone_smarts_idxs)
+                mol,
+                cterm_pad,
+                self.backbone,
+                self.rxn_cterm_pad,
+                is_res_atom,
+                mapidx,
+                next_mol,
+                self.cterm_pad_backbone_smarts_idxs)
         n_atoms_before_addhs = mol.GetNumAtoms()
         mol = Chem.AddHs(mol)
         is_res_atom.extend([False] * (mol.GetNumAtoms() - n_atoms_before_addhs))
         return mol, is_res_atom, mapidx
 
+    @staticmethod
+    def expand_resid(resid_string):
+        chain, resnum = resid_string.strip().split(":")
+        if len(chain) > 1: raise ValueError(f"chain must be empty or single character, got {chain=}")
+        if len(resnum) == 0: raise ValueError(f"resnum can't be empty in {resid_string=}")
+        if resnum[-1].isalpha(): # PDB insertion code
+            insertion_code = resnum[-1]
+            resnum
+        return chain, resnum, icode
+
     def res_to_molsetup(self, res, mk_prep, is_protein_sidechain=False, cut_at_calpha=False):
         padded_mol, is_res_atom, mapidx = self.get_padded_mol(res)
         if is_protein_sidechain:
             bb_matches = padded_mol.GetSubstructMatches(self.backboneh)
             if len(bb_matches) != 1:
                 raise RuntimeError("expected 1 backbone match, got %d" % (len(bb_matches)))
             c_alpha = bb_matches[0][2]
         else:
             c_alpha = None
         molsetups = mk_prep.prepare(padded_mol, root_atom_index=c_alpha)
         if len(molsetups) > 1:
             raise NotImplementedError("multiple molsetups not yet implemented for flexres")
         molsetup = molsetups[0]
         molsetup.is_sidechain = is_protein_sidechain
-        ignored_in_molsetup = []
+        is_flexres_atom = []
         for atom_index in molsetup.atom_ignore:
             if atom_index < len(is_res_atom):
                 is_res = is_res_atom[atom_index] # Hs from Chem.AddHs beyond length of is_res_atom
             else:
                 is_res = False
-            ignore = not is_res
-            ignore |= is_protein_sidechain and cut_at_calpha and (
-                    (atom_index != c_alpha) and (atom_index in bb_matches[0]))
-            molsetup.atom_ignore[atom_index] |= ignore
-            if ignore and is_res:
-                ignored_in_molsetup.append(mapidx[atom_index])
+            molsetup.atom_ignore[atom_index] |= not is_res # ignore padding atoms
+            is_flex = is_protein_sidechain
+            if cut_at_calpha and (atom_index != c_alpha) and (atom_index in bb_matches[0]): # TODO bb pseudos
+                is_flex = False
+            is_flexres_atom.append(is_flex)
+
         # rectify charges to sum to integer (because of padding)
         net_charge = sum([atom.GetFormalCharge() for atom in self.residues[res].rdkit_mol.GetAtoms()])
         if mk_prep.charge_model == "zero":
             net_charge = 0
         not_ignored_idxs = []
         charges = []
-        for i, q in molsetup.charge.items(): # charge is ordered dict
-            if i in mapidx:
+        for i, q in molsetup.charge.items():  # charge is ordered dict
+            if i in mapidx: # TODO offsite not in mapidx
                 charges.append(q)
-                not_ignored_idxs.append(i) 
+                not_ignored_idxs.append(i)
         charges = rectify_charges(charges, net_charge, decimals=3)
+        chain, resname, resnum = res.split(":")
+        if self.residues[res].atom_names is None:
+            atom_names = ["" for _ in not_ignored_idxs]
+        else:
+            atom_names = self.residues[res].atom_names
         for i, j in enumerate(not_ignored_idxs):
             molsetup.charge[j] = charges[i]
-        return molsetup, mapidx, ignored_in_molsetup
-
+            atom_name = atom_names[mapidx[j]]
+            molsetup.pdbinfo[j] = PDBAtomInfo(atom_name, resname, int(resnum), chain)
+        return molsetup, mapidx, is_flexres_atom
 
     def flexibilize_protein_sidechain(self, res, mk_prep, cut_at_calpha=False):
-        molsetup, mapidx, ignored_in_molsetup = self.res_to_molsetup(res, mk_prep,
-                                                                  is_protein_sidechain=True,
-                                                                  cut_at_calpha=cut_at_calpha)
+        molsetup, mapidx, is_flexres_atom = self.res_to_molsetup(res, mk_prep,
+                                                                 is_protein_sidechain=True,
+                                                                 cut_at_calpha=cut_at_calpha)
         self.residues[res].molsetup = molsetup
         self.residues[res].molsetup_mapidx = mapidx
-        self.residues[res].molsetup_ignored = ignored_in_molsetup
+        self.residues[res].is_flexres_atom = is_flexres_atom
         self.residues[res].is_movable = True
         return
 
-    def add_molsetup_inflexible(self, res, mk_prep, cut_at_calpha=False):
-        molsetup, mapidx, ignored_in_molsetup = self.res_to_molsetup(res, mk_prep,
-                                                                  is_protein_sidechain=False,
-                                                                  cut_at_calpha=cut_at_calpha)  
-        self.residues[res].molsetup = molsetup
-        self.residues[res].molsetup_mapidx = mapidx
-        self.residues[res].molsetup_ignored = ignored_in_molsetup
-        self.residues[res].is_movable = False
-        return
-
     @staticmethod
     def print_residues_by_resname(removed_residues):
         by_resname = dict()
         for res_id in removed_residues:
             chain, resn, resi = res_id.split(":")
             by_resname.setdefault(resn, [])
             by_resname[resn].append(f"{chain}:{resi}")
         string = ""
         for resname, removed_res in by_resname.items():
             string += f"Resname: {resname}:" + pathlib.os.linesep
             string += " ".join(removed_res) + pathlib.os.linesep
         return string
 
-    @staticmethod 
+    @staticmethod
     def _load_params(params):
         undesired_props = ("bonds", "//", "bond_cut_atoms", "smiles")
-        
+
         ps = Chem.SmilesParserParams()
         ps.removeHs = False
 
         res_templates = {}
         for resn in params:
             if resn == "ambiguous": continue
-            resmol = Chem.MolFromSmiles(params[resn]['smiles'], ps)
-            # Using user provided parameters to assign properties to atoms.
-            for idx, atom in enumerate(resmol.GetAtoms()):
-                for propname in params[resn]:
-                    if propname in undesired_props:
-                        continue
-                    value = params[resn][propname][idx]
-                    if value is None:
-                        continue
-                    if type(value) == bool:
-                        atom.SetBoolProp(propname, value)
-                    elif type(value) == float:
-                        atom.SetDoubleProp(propname, value)
-                    elif type(value) == str:
-                        atom.SetProp(propname, value)
-                    else:
-                        raise RuntimeError("property type:", type(value), value, "propname:", propname, "resn:", resn)
-            res_templates[resn] = resmol
-        ambiguous = params["ambiguous"]
+            template = {}
+            atom_data = {}
+            atom_data_lengths = set() # to verify consistency
+            for propname in params[resn]:
+                if propname not in undesired_props:
+                    atom_data[propname] = params[resn][propname].copy()
+                    atom_data_lengths.add(len(atom_data[propname]))
+            rdkit_mol = Chem.MolFromSmiles(params[resn]['smiles'], ps)
+            assert len(atom_data_lengths) == 1, f"not all properties have same length for {resn=}"
+            assert list(atom_data_lengths)[0] == rdkit_mol.GetNumAtoms(), f"nr of atoms ({rdkit_mol.GetNumAtoms()}) and length of properties ({list(atom_data_lengths)[0]}) differs for {resn=}"
+
+            template["atom_data"] = atom_data
+            template["rdkit_mol"] = rdkit_mol
+            res_templates[resn] = template
+        ambiguous = {key: values.copy() for key, values in params["ambiguous"].items() if key != "//"}
         return res_templates, ambiguous
-    
+
     @staticmethod
     def _pdb_to_resblocks(pdb_string):
-        #TODO detect (and test distance) chain breaks
-        #TODO cyclic peptides nex res == None ?!
+        # TODO detect (and test distance) chain breaks
+        # TODO cyclic peptides nex res == None ?!
         residues = {}
         # Tracking the key and the value for the current dictionary pair being read in
-        current_res_id = None # the residue id we are tracking
-        current_res = None    # the ChorizoResidue object we are tracking
+        current_res_id = None  # the residue id we are tracking
+        current_res = None  # the ChorizoResidue object we are tracking
         for line in pdb_string.splitlines(True):
             if line.startswith('TER') and current_res is not None:
                 current_res.next_id = None
                 residues[current_res_id] = current_res
                 current_res = None
                 current_res_id = None
             if line.startswith('ATOM') or line.startswith('HETATM'):
@@ -534,30 +554,30 @@
                 if full_res_id == current_res_id:
                     current_res.pdb_text += line
                 else:
                     if current_res_id is not None:
                         last_resid = int(current_res_id.split(":")[2])
                         if resid - last_resid < 2:
                             current_res.next_id = full_res_id
-                        else: # chain break
+                        else:  # chain break
                             current_res.next_id = None
-                    
+
                     # Updates tracking to the new key-value pair we're dealing with
                     current_res = ChorizoResidue(full_res_id, line)
                     if current_res_id is not None and (resid - int(current_res_id.split(":")[2])) < 2:
                         current_res.previous_id = current_res_id
                     else:
                         current_res.previous_id = None
                     current_res_id = full_res_id
                     residues[current_res_id] = current_res
         if current_res is not None:
             current_res.next_id = None
             residues[current_res_id] = current_res
         return residues
-    
+
     def _rename_residues(self, mutate_dict):
         residue_order = list(self.residues.keys())
         for res in mutate_dict:
             old_resn = res.split(':')[1]
             new_resn = mutate_dict[res].split(':')[1]
             # Adds the previous residue as a new key in the dictionary
             self.residues[mutate_dict[res]] = self.residues.pop(res)
@@ -572,15 +592,15 @@
             next_res = self.residues[mutate_dict[res]].next_id
             if next_res:
                 self.residues[next_res].previous_id = mutate_dict[res]
 
             # tracks locations for reordering
             i = residue_order.index(res)
             residue_order[i] = mutate_dict[res]
-        
+
         # clears and recreates self.residues in the desired order. Fairly inefficient
         # but we should only be doing this once.
         for residue in residue_order:
             value = self.residues.pop(residue)
             self.residues[residue] = value
 
     @staticmethod
@@ -593,166 +613,193 @@
                 raise ValueError("Trying to C-term {res} but {next_res=} exists")
             resn = 'C' + resn
         elif termini.get(res, None) == "N":
             if (prev_res is not None) and (not residues[prev_res].user_deleted):
                 raise ValueError("Trying to N-term {res} but {prev_res=} exists")
             resn = 'N' + resn
         elif termini.get(res, None) is None:
-            resn = resn # wow, such assignment, very code
+            resn = resn  # wow, such assignment, very code
         else:
             # TODO verify sanity of termini earlier
             raise ValueError("termini must be either 'C' or 'N', not %s" % termini.get(res, None))
         return resn
 
-    def parameterize_residues(self, termini, ambiguous):
+    def match_residues_templates(self, termini, ambiguous):
         ambiguous_chosen = {}
         for res in self.residues:
+
             # skip deleted resides
             if self.residues[res].user_deleted:
                 continue
-            
+
             # if we can't generate an RDKit Mol for the residue, mark it as ignored and skip
-            pdbmol = Chem.MolFromPDBBlock(self.residues[res].pdb_text, removeHs=False)
+            pdbmol = Chem.MolFromPDBBlock(self.residues[res].pdb_text, removeHs=False) # TODO AltLoc ?
             if pdbmol is None:
                 self.residues[res].ignore_residue = True
                 continue
-            
+
             # Check if parameters are available for a residue
             chain, resn, resnum = res.split(':')
             if (resn not in self.res_templates) and (resn not in ambiguous):
-                #self.residues.pop(res)
+                # self.residues.pop(res)
                 self.residues[res].ignore_residue = True
                 continue
 
             if resn in ambiguous:
                 possible_resn = ambiguous[resn]
             else:
                 possible_resn = [resn]
 
-            #if resn == "HIS": print("HIS ambiguous:", possible_resn)
+            # if resn == "HIS": print("HIS ambiguous:", possible_resn)
 
             lowest_nr_missing = 9999999
             # loops through possible resmol generated for the residue based on number of atoms missing
             for resn in possible_resn:
 
-                resn = self.add_termini(resn, res, termini, self.residues) # prefix C or N if applicable
+                resn = self.add_termini(resn, res, termini, self.residues)  # prefix C or N if applicable
 
                 # TODO add to preprocessing to save time
                 # Create mol object and map between the pdb and residue template
-                resmol = Chem.Mol(self.res_templates[resn])
+                resmol = Chem.Mol(self.res_templates[resn]["rdkit_mol"])
                 n_atoms = len(resmol.GetAtoms())
                 atom_map = mapping_by_mcs(resmol, pdbmol)
                 nr_missing = n_atoms - len(atom_map)
                 if nr_missing < lowest_nr_missing:
                     best_resmol = resmol
                     lowest_nr_missing = nr_missing
                     best_n_atoms = n_atoms
                     best_resn = resn
-            resmol = best_resmol
             n_atoms = best_n_atoms
             resn = best_resn
-            #if len(possible_resn) > 1:
-            #    print("%9s" % res, "-->", resn, "...out of", possible_resn)
-            #    ambiguous_chosen[res] = f"{chain}:{resn}:{resnum}"
+            # TODO missing atoms from PDB? Extra PDB atoms OK currently?
+            if len(possible_resn) > 1:
+                ambiguous_chosen[res] = f"{chain}:{resn}:{resnum}"
 
             resmol = self.build_resmol(res, resn)
             if resmol is None:
                 self.residues[res].ignore_residue = True
             else:
-                self.residues[res].rdkit_mol = resmol
+                self.build_molsetup_wrap(res, resn, resmol)
+
         return ambiguous_chosen
 
+    def build_molsetup_wrap(self, res_id, resname, resmol):
+        self.residues[res_id].rdkit_mol = resmol
+        coords = resmol.GetConformer().GetPositions()
+        atom_data = self.res_templates[resname]["atom_data"]
+        if "atom_name" in atom_data:
+            self.residues[res_id].set_atom_names(atom_data["atom_name"])
+        chain, _, resnum = res_id.split(":")
+        atomic_nrs = [atom.GetAtomicNum() for atom in resmol.GetAtoms()]
+        molsetup, molsetup_mapidx, is_flexres_atom = self.build_molsetup(
+                coords, atom_data, chain, resname, int(resnum), atomic_nrs)
+        self.residues[res_id].molsetup = molsetup
+        self.residues[res_id].molsetup_mapidx = molsetup_mapidx
+        self.residues[res_id].is_flexres_atom = is_flexres_atom
+        return
+
+    @staticmethod
+    def build_molsetup(coords, atom_data, chain, resn, resnum, atomic_nrs):
+
+        n = set([len(coords)] + [len(values) for (key, values) in atom_data.items()])
+        if len(n) != 1:
+            raise ValueError(f"mismatch in lengths of coords or atom_data {n}")
+        n = n.pop()
+
+        molsetup = MoleculeSetup()
+        dedicated_attributes_in_molsetup = ("atom_type", "charge", "atom_ignore")
+
+        for key, values in atom_data.items():
+            if key in dedicated_attributes_in_molsetup:
+                d = getattr(molsetup, key)
+                for i in range(n):
+                    d[i] = values[i]
+            else:
+                molsetup.atom_params[key] = values.copy()
+
+        for i, xyz in enumerate(coords):
+            molsetup.coord[i] = xyz
+            if "atom_name" in molsetup.atom_params:
+                atom_name = molsetup.atom_params["atom_name"][i]
+            else:
+                atom_name = ""
+            molsetup.pdbinfo[i] = PDBAtomInfo(atom_name, resn, resnum, chain)
+            molsetup.element[i] = atomic_nrs[i]
+
+        molsetup_mapidx = {i: i for i in range(n)} # identity mapping (padded_mol == mol)
+        is_flexres_atom = [False for i in range(n)]
+            
+        return molsetup, molsetup_mapidx, is_flexres_atom
+
     def build_resmol(self, res, resn):
         # Transfer coordinates and info for any matched atoms
-        #TODO time these functions
-        #TODO maybe embed in preprocessing depending on time
-        #EmbedMolecule(resmol)
+        # TODO time these functions
+        # TODO maybe embed in preprocessing depending on time
+        # EmbedMolecule(resmol)
 
-        resmol = Chem.Mol(self.res_templates[resn])
+        resmol = Chem.Mol(self.res_templates[resn]["rdkit_mol"])
+        atom_data = self.res_templates[resn]["atom_data"]
         pdbmol = Chem.MolFromPDBBlock(self.residues[res].pdb_text, removeHs=False)
 
         atom_map = mapping_by_mcs(resmol, pdbmol)
-        #Chem.rdDepictor.Compute2DCoords(resmol)
         resmol.AddConformer(Chem.Conformer(resmol.GetNumAtoms()))
 
         resmol.GetConformer().Set3D(True)
         for idx, pdb_idx in atom_map.items():
-            pdb_atom = pdbmol.GetAtomWithIdx(pdb_idx)
             pdb_coord = pdbmol.GetConformer().GetAtomPosition(pdb_idx)
             resmol.GetConformer().SetAtomPosition(idx, pdb_coord)
 
-            resinfo = pdb_atom.GetPDBResidueInfo()
-            resmol.GetAtomWithIdx(idx).SetDoubleProp('occupancy', resinfo.GetOccupancy())
-            resmol.GetAtomWithIdx(idx).SetDoubleProp('temp_factor', resinfo.GetTempFactor())
-
-        missing_atoms = {resmol.GetAtomWithIdx(i).GetProp('atom_name'):i for i in range(resmol.GetNumAtoms()) if i not in atom_map.keys()}
+        missing_atoms = {atom_data["atom_name"][i]:i for i in range(resmol.GetNumAtoms()) if i not in atom_map.keys()}
 
         # Handle case of missing backbone amide H
         if 'H' in missing_atoms:
             prev_res = self.residues[res].previous_id
             if prev_res is not None:
-                h_pos = h_coord_from_dipeptide(self.residues[res].pdb_text, 
-                                                self.residues[prev_res].pdb_text)
+                h_pos = h_coord_from_dipeptide(self.residues[res].pdb_text,
+                                               self.residues[prev_res].pdb_text)
             else:
                 h_pos = h_coord_random_n_terminal(resmol)
             resmol.GetConformer().SetAtomPosition(missing_atoms['H'], h_pos)
             resmol.GetAtomWithIdx(missing_atoms['H']).SetBoolProp('computed', True)
             missing_atoms.pop('H')
-            
-        
+
         missing_atom_elements = set([atom[0] for atom in missing_atoms.keys()])
         if len(missing_atom_elements) > 0:
-            
             resmol_h = Chem.RemoveHs(resmol)
             resmol_h = Chem.AddHs(resmol_h, addCoords=True)
             h_map = mapping_by_mcs(resmol, resmol_h)
             for atom in list(missing_atoms.keys()):
                 if atom.startswith('H'):
                     h_idx = missing_atoms[atom]
-                    #TODO magic function from Diogo to add H atom
-                    #TODO bring in parameterless H atom for chain breaks
+                    # TODO magic function from Diogo to add H atom
+                    # TODO bring in parameterless H atom for chain breaks
                     resmol.GetConformer().SetAtomPosition(h_idx, resmol_h.GetConformer().GetAtomPosition(h_map[h_idx]))
                     resmol.GetAtomWithIdx(h_idx).SetBoolProp('computed', True)
                     missing_atoms.pop(atom)
-        # TODO missing atoms from PDB? Extra PDB atoms OK currently?
         if len(missing_atoms) > 0:
             err = f'Could not add {res=} {missing_atoms=}'
             print(err)
             resmol = None
         return resmol
 
-
     def mk_parameterize_all_residues(self, mk_prep):
         # TODO disulfide bridges are hard-coded, generalize branching maybe
-        for res in self.getAllValidResidues():
+        for res in self.get_valid_residues():
             """if self.residues[res].user_deleted or self.residues[res].ignore_residue:
                 continue"""
-            self.mk_parameterize_residue(self, res, mk_prep)
+            self.mk_parameterize_residue(res, mk_prep)
         return
 
 
     def mk_parameterize_residue(self, res, mk_prep): 
-        molsetup, mapidx, ignored_in_molsetup = self.res_to_molsetup(res, mk_prep)
-        resmol = self.residues[res].rdkit_mol
-        for molsetup_idx, resmol_idx in mapidx.items(): # ignoring pseudo atoms, rdkit atom props no good for pseudos
-            atom = resmol.GetAtomWithIdx(resmol_idx)
-            atom.SetDoubleProp("q", molsetup.charge[molsetup_idx])
-            atom.SetProp("atom_type", molsetup.atom_type[molsetup_idx])
-            #atom.SetProp("ignore", molsetup.atom_ignore[molsetup_idx])
-            for key, value_array in molsetup.atom_params.items():
-                value = value_array[molsetup_idx]
-                if type(value) == float:
-                    atom.SetDoubleProp(key, value)
-                elif type(value) == bool:
-                    atom.SetBoolProp(key, value)
-                else:
-                    atom.SetProp(key, value)
-        # consider deleting existing properties/parameters
+        molsetup, mapidx, is_flexres_atom = self.res_to_molsetup(res, mk_prep)
+        self.residues[res].molsetup = molsetup
+        self.residues[res].mapidx = mapidx
+        self.residues[res].is_flexres_atom = is_flexres_atom
         return
-                
 
     def to_pdb(self, use_modified_coords=False, modified_coords_index=0):
         pdbout = ""
         atom_count = 0
         icode = ""
         pdb_line = "{:6s}{:5d} {:^4s} {:3s} {:1s}{:4d}{:1s}   {:8.3f}{:8.3f}{:8.3f}                       {:2s} "
         pdb_line += pathlib.os.linesep
@@ -760,15 +807,15 @@
             if self.residues[res_id].user_deleted or self.residues[res_id].ignore_residue:
                 continue
             resmol = self.residues[res_id].rdkit_mol
             if use_modified_coords and self.residues[res_id].molsetup is not None:
                 molsetup = self.residues[res_id].molsetup
                 if len(molsetup.modified_atom_positions) <= modified_coords_index:
                     errmsg = "Requesting pose %d but only got %d in molsetup of %s" % (
-                            modified_coords_index, len(molsetup.modified_atom_positions), res_id)
+                        modified_coords_index, len(molsetup.modified_atom_positions), res_id)
                     raise RuntimeError(errmsg)
                 p = molsetup.modified_atom_positions[modified_coords_index]
                 modified_positions = molsetup.get_conformer_with_modified_positions(p).GetPositions()
                 positions = {}
                 for i, j in self.residues[res_id].molsetup_mapidx.items():
                     positions[j] = modified_positions[i]
             else:
@@ -779,139 +826,137 @@
 
             for (i, atom) in enumerate(resmol.GetAtoms()):
                 atom_count += 1
                 props = atom.GetPropsAsDict()
                 atom_name = props.get("atom_name", "")
                 x, y, z = positions[i]
                 element = mini_periodic_table[atom.GetAtomicNum()]
-                pdbout += pdb_line.format("ATOM", atom_count, atom_name, resname, chain, resnum, icode, x, y, z, element)
+                pdbout += pdb_line.format("ATOM", atom_count, atom_name, resname, chain, resnum, icode, x, y, z,
+                                          element)
         return pdbout
 
-    def export_static_atom_params(self, ignore_atom_types=("H",)):
+    def export_static_atom_params(self):
         atom_params = {}
         counter_atoms = 0
         coords = []
-        for res_id in self.residues:
-            if self.residues[res_id].user_deleted or self.residues[res_id].ignore_residue:
-                continue
-            resmol = self.residues[res_id].rdkit_mol
-            for atom in resmol.GetAtoms():
-                props = atom.GetPropsAsDict()
-                if len(ignore_atom_types) > 0 and props["atom_type"] in ignore_atom_types:
-                    continue
-                if (self.residues[res_id].molsetup):
-                    if atom.GetIdx() not in self.residues[res_id].molsetup_ignored:
-                        continue
-                for key, value in props.items():
-                    if key.startswith("_"):
-                        continue
-                    atom_params.setdefault(key, [None]*counter_atoms) # add new "column"
-                    atom_params[key].append(value)
-                counter_atoms += 1
-                for key in set(atom_params).difference(props): # <key> missing in <props>
-                    atom_params[key].append(None) # fill in incomplete "row"
-                coords.append(resmol.GetConformer().GetAtomPosition(atom.GetIdx()))
+        dedicated_attribute = ("charge", "atom_type") # molsetup has a dedicated attribute
+        for res_id in self.get_valid_residues():
+            molsetup = self.residues[res_id].molsetup
+            wanted_atom_indices = []
+            for i, ignore in molsetup.atom_ignore.items():
+                if not ignore and not self.residues[res_id].is_flexres_atom[i]:
+                    wanted_atom_indices.append(i)
+            for key, values in molsetup.atom_params.items():
+                atom_params.setdefault(key, [None]*counter_atoms) # add new "column"
+                for i in wanted_atom_indices:
+                    atom_params[key].append(values[i])
+            for key in dedicated_attribute:
+                atom_params.setdefault(key, [None]*counter_atoms) # add new "column"
+                values_dict = getattr(molsetup, key)
+                for i in wanted_atom_indices:
+                    atom_params[key].append(values_dict[i])
+            counter_atoms += len(wanted_atom_indices)
+            added_keys = set(molsetup.atom_params).union(dedicated_attribute)
+            for key in set(atom_params).difference(added_keys): # <key> missing in current molsetup
+                atom_params[key].extend([None] * len(wanted_atom_indices)) # fill in incomplete "row"
+            coords.extend(molsetup.coord[i])
         if hasattr(self, "param_rename"): # e.g. "gasteiger" -> "q"
             for key, new_key in self.param_rename.items():
                 atom_params[new_key] = atom_params.pop(key)
         return atom_params, coords
-    
+
     # The following functions return filtered dictionaries of residues based on the value of residue flags.
-    def getUserDeletedResidues(self):
-        return {k: v for k, v in self.residues.items() if v.user_deleted == True}
-        
-    def getNonUserDeletedResidues(self):
-        return {k: v for k, v in self.residues.items() if v.user_deleted == False}
-        
-    def getIgnoredResidues(self):
-        return {k: v for k, v in self.residues.items() if v.ignore_residue == True}
-        
-    def getNotIgnoredResidues(self):
-        return {k: v for k, v in self.residues.items() if v.ignore_residue == False}
-    
+    def get_user_deleted_residues(self):
+        return {k: v for k, v in self.residues.items() if v.user_deleted}
+
+    def get_non_user_deleted_residues(self):
+        return {k: v for k, v in self.residues.items() if not v.user_deleted}
+
+    def get_ignored_residues(self):
+        return {k: v for k, v in self.residues.items() if v.ignore_residue}
+
+    def get_not_ignored_residues(self):
+        return {k: v for k, v in self.residues.items() if not v.ignore_residue}
+
     # TODO: rename this
-    def getValidResidues(self):
-        return {k: v for k, v in self.residues.items() if v.ignore_residue == False and v.user_deleted == False}
+    def get_valid_residues(self):
+        return {k: v for k, v in self.residues.items() if v.is_valid_residue()}
 
 
 residues_rotamers = {"SER": [("C", "CA", "CB", "OG")],
                      "THR": [("C", "CA", "CB", "CG2")],
                      "CYS": [("C", "CA", "CB", "SG")],
                      "VAL": [("C", "CA", "CB", "CG1")],
-                     "HIS": [("C", "CA", "CB", "CG"), 
+                     "HIS": [("C", "CA", "CB", "CG"),
                              ("CA", "CB", "CG", "CD2")],
-                     "ASN": [("C", "CA", "CB", "CG"), 
+                     "ASN": [("C", "CA", "CB", "CG"),
                              ("CA", "CB", "CG", "ND2")],
                      "ASP": [("C", "CA", "CB", "CG"),
                              ("CA", "CB", "CG", "OD1")],
-                     "ILE": [("C", "CA", "CB", "CG2"), 
+                     "ILE": [("C", "CA", "CB", "CG2"),
                              ("CA", "CB", "CG2", "CD1")],
-                     "LEU": [("C", "CA", "CB", "CG"), 
+                     "LEU": [("C", "CA", "CB", "CG"),
                              ("CA", "CB", "CG", "CD1")],
-                     "PHE": [("C", "CA", "CB", "CG"), 
+                     "PHE": [("C", "CA", "CB", "CG"),
                              ("CA", "CB", "CG", "CD2")],
-                     "TYR": [("C", "CA", "CB", "CG"), 
+                     "TYR": [("C", "CA", "CB", "CG"),
                              ("CA", "CB", "CG", "CD2")],
-                     "TRP": [("C", "CA", "CB", "CG"), 
+                     "TRP": [("C", "CA", "CB", "CG"),
                              ("CA", "CB", "CG", "CD2")],
-                     "GLU": [("C", "CA", "CB", "CG"), 
-                             ("CA", "CB", "CG", "CD"), 
+                     "GLU": [("C", "CA", "CB", "CG"),
+                             ("CA", "CB", "CG", "CD"),
                              ("CB", "CG", "CD", "OE1")],
-                     "GLN": [("C", "CA", "CB", "CG"), 
-                             ("CA", "CB", "CG", "CD"), 
+                     "GLN": [("C", "CA", "CB", "CG"),
+                             ("CA", "CB", "CG", "CD"),
                              ("CB", "CG", "CD", "OE1")],
-                     "MET": [("C", "CA", "CB", "CG"), 
-                             ("CA", "CB", "CG", "SD"), 
+                     "MET": [("C", "CA", "CB", "CG"),
+                             ("CA", "CB", "CG", "SD"),
                              ("CB", "CG", "SD", "CE")],
-                     "ARG": [("C", "CA", "CB", "CG"), 
-                             ("CA", "CB", "CG", "CD"), 
+                     "ARG": [("C", "CA", "CB", "CG"),
+                             ("CA", "CB", "CG", "CD"),
                              ("CB", "CG", "CD", "NE"),
                              ("CG", "CD", "NE", "CZ")],
-                     "LYS": [("C", "CA", "CB", "CG"), 
-                             ("CA", "CB", "CG", "CD"), 
+                     "LYS": [("C", "CA", "CB", "CG"),
+                             ("CA", "CB", "CG", "CD"),
                              ("CB", "CG", "CD", "CE"),
                              ("CG", "CD", "CE", "NZ")]}
 
-
 rotamer_res_disambiguate = {}
 for primary_res, specific_res_list in chorizo_params["ambiguous"].items():
     for specific_res in specific_res_list:
         rotamer_res_disambiguate[specific_res] = primary_res
 
+
 def add_rotamers_to_chorizo_molsetups(rotamer_states_list, chorizo):
     no_resname_to_resname = {}
     for res_with_resname in chorizo.residues:
         chain, resname, resnum = res_with_resname.split(":")
         no_resname_key = f"{chain}:{resnum}"
         if no_resname_key in no_resname_to_resname:
             errmsg = "both %s and %s would be keyed by %s" % (
                 res_with_resname, no_resname_to_resname[no_resname_key], no_resname_key)
             raise RuntimeError(errmsg)
         no_resname_to_resname[no_resname_key] = res_with_resname
 
     state_indices_list = []
-    for state_dict in rotamer_states_list:
+    for state_index, state_dict in enumerate(rotamer_states_list):
+        print(f"adding rotamer state {state_index + 1}")
         state_indices = {}
         for res_no_resname, angles in state_dict.items():
             res_with_resname = no_resname_to_resname[res_no_resname]
-            if not "molsetup" in chorizo.residues[res_with_resname]:
+            if chorizo.residues[res_with_resname].molsetup is None:
                 raise RuntimeError("no molsetup for %s, can't add rotamers" % (res_with_resname))
-            # next block is inneficient for large rotamer_states_list
+            # next block is inefficient for large rotamer_states_list
             # refactored chorizos could help by having the following
             # data readily available
-            resmol = chorizo.residues[res_with_resname]["resmol"]
-            molsetup = chorizo.residues[res_with_resname]["molsetup"]
-            mapidx = chorizo.residues[res_with_resname]["molsetup_mapidx"]
-            mapidx_inv = {value: key for (key, value) in mapidx.items()}
+            molsetup = chorizo.residues[res_with_resname].molsetup
             name_to_molsetup_idx = {}
-            for atom in resmol.GetAtoms():
-                props = atom.GetPropsAsDict()
-                if "atom_name" in props:
-                    atom_name = props["atom_name"]
-                    name_to_molsetup_idx[atom_name] = mapidx_inv[atom.GetIdx()]
+            for atom_index, pdbinfo in molsetup.pdbinfo.items():
+                atom_name = pdbinfo.name 
+                name_to_molsetup_idx[atom_name] = atom_index
 
             resname = res_with_resname.split(":")[1]
             resname = rotamer_res_disambiguate.get(resname, resname)
 
             atom_names = residues_rotamers[resname]
             if len(atom_names) != len(angles):
                 raise RuntimeError(
@@ -925,14 +970,15 @@
             state_indices[res_with_resname] = len(molsetup.rotamers)
             molsetup.add_rotamer(atom_idxs, np.radians(angles))
 
         state_indices_list.append(state_indices)
 
     return state_indices_list
 
+
 class ChorizoResidue:
     """
     A class representing a single residue in the chain of chorizo residues
 
     Attributes
     ----------
     residue_id: string
@@ -945,57 +991,72 @@
     next_id: string or None
         the next residue in this chain
     
     rdkit_mol: rdkit.Chem.rdchem.Mol or None
         the rdkit Mol object generated from this residue
     molsetup: RDKitMoleculeSetup or None
         the RDKitMoleculeSetup object generated from this residue
-    molsetup_mapidx: or None
-        needs info
-    molsetup_ignored: List[] or None
-        needs info
+    molsetup_mapidx: dict() or None
+        atom index map between molsetup (keys) and rdkit_mol (values)
+    is_flexres_atom: List[] of booleans, or None
+        indicates whether each atom is part of the flexible sidechain
+
 
     ignore_residue: bool
         marks residues that formerly were part of the removed_residues structure,
         put on residues that are ignored due to being incomplete or incorrect
     is_movable: bool
         marks residues that are flexible
     user_deleted: bool
         marks residues that the user indicated should be deleted
 
     additional_connections: List[ResidueAdditionalConnection]
         connections to additional residues along the chain (there's probably
         more specific information about the nature of these connections that
         could be added here)
     """
+
     def __init__(self, residue_id, pdb_text, previous_id=None, next_id=None):
         self.residue_id = residue_id
         self.pdb_text = pdb_text
         self.previous_id = previous_id
         self.next_id = next_id
 
         self.rdkit_mol = None
+        self.atom_names = None # assumes same order and length as atoms in rdkit_mol
         self.molsetup = None
         self.molsetup_mapidx = None
-        self.molsetup_ignored = None # Check about these data types/Do we want the default to be None or empty
+        self.is_flexres_atom = None # Check about these data types/Do we want the default to be None or empty
 
         # flags
         self.ignore_residue = False
         self.is_movable = False
         self.user_deleted = False
 
         self.additional_connections = []
 
-    def toJson(self):
+    def set_atom_names(self, atom_names_list):
+        if self.rdkit_mol is None:
+            raise RuntimeError("can't set atom_names if rdkit_mol is not set yet")
+        if len(atom_names_list) != self.rdkit_mol.GetNumAtoms():
+            raise ValueError(f"{len(atom_names_list)=} differs from {self.rdkit_mol.GetNumAtoms()=}")
+        name_types = set([type(name) for name in atom_names_list])
+        if name_types != {str}:
+            raise ValueError(f"atom names must be str but {name_types=}")
+        self.atom_names = atom_names_list
+        return
+
+    def to_json(self):
         return json.dumps(self, default=lambda o: o.__dict__)
-    
-    def isValidResidue(self):
+
+    def is_valid_residue(self):
         """Returns true if the residue is not marked as deleted by a user and has not been marked as a residue to ignore"""
         return not self.ignore_residue and not self.user_deleted
 
+
 # This could be a named tuple or a dataclass as it stands, but that is dependent on the amount of custom behavior
 # we want to encode for these additional connections.
 class ResidueAdditionalConnection:
     """
     Represents additional connections & bonds from a residue
 
     Attributes
@@ -1003,14 +1064,15 @@
     connection_residue: string
         the id of the connected residue
     connection_atom: string
         the connected atom
     bond_order: string                    # SHOULD MAYBE NOT BE A STRING?
         the bond order of the connection
     """
+
     def __init__(self, residue, atom, bond_order):
         self.connection_residue = None
         self.connection_atom = None
         self.bond_order = None
 
-    def toJson(self):
+    def to_json(self):
         return json.dumps(self, default=lambda o: o.__dict__)
```

### Comparing `meeko-0.6.0a2/meeko/macrocycle.py` & `meeko-0.6.0a3/meeko/macrocycle.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/molecule_pdbqt.py` & `meeko-0.6.0a3/meeko/molecule_pdbqt.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/molsetup.py` & `meeko-0.6.0a3/meeko/molsetup.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             - data storage
             - SMARTS matcher for all atom typers
     """
 
     def __init__(self):
 
         self.atom_pseudo = []
-        self.coord = OrderedDict()  # FIXME all OrderedDict shuold be converted to lists?
+        self.coord = OrderedDict()  # FIXME all OrderedDict should be converted to lists?
         self.charge = OrderedDict()
         self.pdbinfo = OrderedDict()
         self.atom_type = OrderedDict()
         self.atom_params = {}
         self.dihedral_interactions = list()
         self.dihedral_partaking_atoms = dict()
         self.dihedral_labels = dict()
@@ -756,16 +756,16 @@
         is_set_list = [False] * self.mol.GetNumAtoms()
         for atom_index, new_position in new_atom_positions.items():
             new_conformer.SetAtomPosition(atom_index, new_position)
             is_set_list[atom_index] = True
         new_mol.RemoveAllConformers()
         new_mol.AddConformer(new_conformer, assignId=True)
         for atom_index, is_set in enumerate(is_set_list):
-            if not is_set and new_mol.GetAtomWithIdx(atom_idx).GetAtomicNum() == 1:
-                neighbors = new_mol.GetAtomWithIdx(atom_idx).GetNeighbors()
+            if not is_set and new_mol.GetAtomWithIdx(atom_index).GetAtomicNum() == 1:
+                neighbors = new_mol.GetAtomWithIdx(atom_index).GetNeighbors()
                 if len(neighbors) != 1:
                     raise RuntimeError("Expected H to have one neighbors")
                 Chem.SetTerminalAtomCoords(new_mol, atom_index, neighbors[0].GetIdx())
         return new_conformer
 
     def get_mol_with_modified_positions(self, new_atom_positions_list=None):
         if new_atom_positions_list is None:
@@ -872,15 +872,15 @@
                 matches = []
                 for i, sibling_isotope in enumerate(sibling_isotopes):
                     for hidx in hidxs[len(matches):]:
                         if mol_noH.GetAtomWithIdx(hidx).GetIsotope() == sibling_isotope:
                             matches.append(i)
                             break
                 if len(matches) != len(hidxs):
-                    raise RuntimeError("Number of matched isotopes %d differs from query Hs: %d" % (len(matched), len(hidxs)))
+                    raise RuntimeError("Number of matched isotopes %d differs from query Hs: %d" % (len(matches), len(hidxs)))
                 for hidx, i in zip(hidxs, matches):
                     noH_to_H[hidx] = siblings_of_h[sortidx[i]].GetIdx()
             else:
                 raise RuntimeError("nr of Hs in mol_noH bonded to an atom exceeds nr of Hs in mol_no_ignore")
 
         smiles = Chem.MolToSmiles(mol_noH)
         order_string = mol_noH.GetProp("_smilesAtomOutputOrder")
@@ -1106,20 +1106,22 @@
 
         # if we are here, we didn't match
         new_row_index = len(self.params)
         self.params.append(new_row)
         return new_row_index
 
 
-    def add_molsetup(self, molsetup, add_atomic_nr=False, add_atom_type=False):
+    def add_molsetup(self, molsetup, atom_params=None, add_atomic_nr=False, add_atom_type=False):
         if "q" in molsetup.atom_params or "atom_type" in molsetup.atom_params:
             msg = '"q" and "atom_type" found in molsetup.atom_params'
             msg += ' but are hard-coded to store molsetup.charge and'
             msg += ' molsetup.atom_type in the internal data structure'
             raise RuntimeError(msg)
+        if atom_params is None:
+            atom_params = molsetup.atom_params
         param_idxs = []
         for atom_index, ignore in molsetup.atom_ignore.items():
             if ignore:
                 param_idx = None
             else:
                 p = {k: v[atom_index] for (k, v) in molsetup.atom_params.items()}
                 if add_atomic_nr:
```

### Comparing `meeko-0.6.0a2/meeko/openff_xml_parser.py` & `meeko-0.6.0a3/meeko/openff_xml_parser.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/preparation.py` & `meeko-0.6.0a3/meeko/preparation.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,16 @@
 
         self.atom_params = self.get_atom_params(
                 input_atom_params,
                 load_atom_params,
                 add_atom_types,
                 self.packaged_params)
 
+        if load_offatom_params is not None:
+            raise NotImplementedError("load_offatom_params not implemented")
         self.load_offatom_params = load_offatom_params
         
         allowed_charge_models = ["espaloma", "gasteiger", "zero"]
         if charge_model not in allowed_charge_models:
             raise ValueError("unrecognized charge_model: %s, allowed options are: %s" % (charge_model, allowed_charge_models))
 
         self.charge_model = charge_model
@@ -125,16 +127,27 @@
 
         self._bond_typer = BondTyperLegacy()
         self._macrocycle_typer = FlexMacrocycle(
                 self.min_ring_size, self.max_ring_size, self.double_bond_penalty)
         self._flex_builder = FlexibilityBuilder()
         self._water_builder = HydrateMoleculeLegacy()
         self._classes_setup = {Chem.rdchem.Mol: RDKitMoleculeSetup}
+        
+        if input_offatom_params is None:
+            self.offatom_params = {}
+        else:
+            self.offatom_params = input_offatom_params
+
+        if _has_openbabel:
+            self._classes_setup[ob.OBMol] = OBMoleculeSetup
+        if keep_chorded_rings and keep_equivalent_rings==False:
+            warnings.warn("keep_equivalent_rings=False ignored because keep_chorded_rings=True", RuntimeWarning)
+        if (reactive_smarts is None) != (reactive_smarts_idx is None):
+            raise ValueError("reactive_smarts and reactive_smarts_idx require each other")
 
-        self.offatom_params = {}
 
     @staticmethod
     def get_atom_params(input_atom_params, load_atom_params, add_atom_types, packaged_params):
         atom_params = {}
         if type(load_atom_params) == str:
             load_atom_params = [load_atom_params]
         elif load_atom_params is None:
@@ -207,25 +220,14 @@
                 ###     msg += "A total of %d types were found in atom_params:" % (len(types)) + os.linesep
                 ###     msg += str(types) + os.linesep
                 ###     raise ValueError(msg)
                 ### 
                 ### #for value in atom_params:
                     
 
-        self.offatom_params = offatom_params
-        self.charge_model = charge_model
-        self.dihedral_params = dihedral_params
-
-
-        if _has_openbabel:
-            self._classes_setup[ob.OBMol] = OBMoleculeSetup
-        if keep_chorded_rings and keep_equivalent_rings==False:
-            warnings.warn("keep_equivalent_rings=False ignored because keep_chorded_rings=True", RuntimeWarning)
-        if (reactive_smarts is None) != (reactive_smarts_idx is None):
-            raise ValueError("reactive_smarts and reactive_smarts_idx require each other")
 
     @property
     def setup(self):
         msg = "MoleculePreparation.setup is deprecated in Meeko v0.5."
         msg += " MoleculePreparation.prepare() returns a list of MoleculeSetup instances."
         warnings.warn(msg, DeprecationWarning)
         return self.deprecated_setup_access
```

### Comparing `meeko-0.6.0a2/meeko/rdkit_mol_create.py` & `meeko-0.6.0a3/meeko/rdkit_mol_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,21 +363,23 @@
             returns None if input is empty list or all molecules are None
         """
         combined_mol = None
         props = {}
         for mol in mol_list:
             if mol is None:
                 continue
-            data = json.loads(mol.GetProp("meeko"))
-            clean_extend(props, data)
+            if mol.HasProp("meeko"):
+                data = json.loads(mol.GetProp("meeko"))
+                clean_extend(props, data)
             if combined_mol is None: # first iteration
                 combined_mol = mol
             else:
                 combined_mol = Chem.CombineMols(combined_mol, mol)
-        combined_mol.SetProp("meeko", json.dumps(props))
+        if len(props) > 0:
+            combined_mol.SetProp("meeko", json.dumps(props))
         return combined_mol
 
     @classmethod
     def _verify_flexres(cls):
         for resname in cls.flexres:
             atom_names_in_smiles_order = cls.flexres[resname]["atom_names_in_smiles_order"]
             h_to_parent_index = cls.flexres[resname]["h_to_parent_index"]
```

### Comparing `meeko-0.6.0a2/meeko/reactive.py` & `meeko-0.6.0a3/meeko/reactive.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/receptor_pdbqt.py` & `meeko-0.6.0a3/meeko/receptor_pdbqt.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,15 +347,14 @@
                     two_bond_away.add(j)
         names_1bond = [atom_names[i] for i in one_bond_away]
         names_2bond = [atom_names[i] for i in two_bond_away]
         new_pdbqt_str = ""
         for i, line in enumerate(pdbqtstr.split(os_linesep)[:-1]):
             if line.startswith("ATOM") or line.startswith("HETATM"):
                 name = line[12:16].strip()
-                print(name, "<<<") # TODO need proper atom names from chorizo
                 atype = line[77:].strip()
                 if name == reactive_name:
                     new_type = prefix_atype + get_reactive_atype(atype, 1)
                 elif name in names_1bond:
                     new_type = prefix_atype + get_reactive_atype(atype, 2)
                 elif name in names_2bond:
                     new_type = prefix_atype + get_reactive_atype(atype, 3)
```

### Comparing `meeko-0.6.0a2/meeko/utils/autodock4_atom_types_elements.py` & `meeko-0.6.0a3/meeko/utils/autodock4_atom_types_elements.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/utils/covalent_radius_table.py` & `meeko-0.6.0a3/meeko/utils/covalent_radius_table.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/utils/geomutils.py` & `meeko-0.6.0a3/meeko/utils/geomutils.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/utils/obutils.py` & `meeko-0.6.0a3/meeko/utils/obutils.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/utils/rdkitutils.py` & `meeko-0.6.0a3/meeko/utils/rdkitutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 
 from collections import namedtuple
 PDBAtomInfo = namedtuple('PDBAtomInfo', "name resName resNum chain")
 
 def getPdbInfoNoNull(atom):
     """extract information for populating an ATOM/HETATM line
     in the PDB"""
-    # res = atom.GetResidue()
-    minfo = atom.GetMonomerInfo()
+    minfo = atom.GetMonomerInfo() # same as GetPDBResidueInfo
     if minfo is None:
         atomic_number = atom.GetAtomicNum()
         if atomic_number == 0:
             name = '%-2s' % '*'
         else:
             name = '%-2s' % mini_periodic_table[atomic_number]
         chain = ' '
```

### Comparing `meeko-0.6.0a2/meeko/utils/utils.py` & `meeko-0.6.0a3/meeko/utils/utils.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/utils/van_der_waals_radius_table.py` & `meeko-0.6.0a3/meeko/utils/van_der_waals_radius_table.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/meeko/writer.py` & `meeko-0.6.0a3/meeko/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,52 +411,50 @@
                 success = False
 
         return success, error_msg
 
 
     @classmethod
     def write_string_from_linked_rdkit_chorizo(cls, chorizo):
-        rigid_pdbqt_string, flex_pdbqt_dict = cls.write_string_flexdict_from_linked_rdkit_chorizo(chorizo)
+        rigid_pdbqt_string, flex_pdbqt_dict = cls.write_from_linked_rdkit_chorizo(chorizo)
         flex_pdbqt_string = ""
         for res_id, pdbqt_string in flex_pdbqt_dict.items():
             flex_pdbqt_string += pdbqt_string
         return rigid_pdbqt_string, flex_pdbqt_string
 
 
     @classmethod
     def write_from_linked_rdkit_chorizo(cls, chorizo):
         rigid_pdbqt_string = ""
         flex_pdbqt_dict = {}
         atom_count = 0
         flex_atom_count = 0
-        for res_id in chorizo.getValidResidues():
-            resmol = chorizo.residues[res_id].rdkit_mol
-            positions = resmol.GetConformer().GetPositions()
+        for res_id in chorizo.get_valid_residues():
+            molsetup = chorizo.residues[res_id].molsetup
             chain, resname, resnum = res_id.split(":")
             resnum = int(resnum)
             molsetup_mapidx = {} if chorizo.residues[res_id].molsetup_mapidx is None else chorizo.residues[res_id].molsetup_mapidx
-            molsetup_ignored = () if chorizo.residues[res_id].molsetup_ignored is None else chorizo.residues[res_id].molsetup_ignored
-            flexres_idxs = [j for (i, j) in molsetup_mapidx.items() if j not in molsetup_ignored]
-            for atom in resmol.GetAtoms():
-                if atom.GetIdx() in flexres_idxs:
+            is_flexres_atom = chorizo.residues[res_id].is_flexres_atom
+            for i, atom_ignore in molsetup.atom_ignore.items():
+                if atom_ignore or is_flexres_atom[i]:
                     continue
-                props = atom.GetPropsAsDict()
-                atom_type = props["atom_type"]
-                if atom_type == "H": # TODO read ignore flag in molsetup
-                    continue
-                coord = positions[atom.GetIdx()]
-                atom_name = props.get("atom_name", "")
-                charge = props["gasteiger"]
+                atom_type = molsetup.atom_type[i]
+                coord = molsetup.coord[i]
+                atom_name = molsetup.pdbinfo[i].name
+                charge = molsetup.charge[i]
                 atom_count += 1
                 rigid_pdbqt_string += cls._make_pdbqt_line(
                     atom_count, atom_name, resname, chain, resnum, coord, charge, atom_type) + linesep
-            if chorizo.residues[res_id].molsetup:
+            if chorizo.residues[res_id].is_movable:
                 chain, resname, resnum = res_id.split(":")
                 molsetup = chorizo.residues[res_id].molsetup
+                original_ignore = molsetup.atom_ignore.copy()
+                molsetup.atom_ignore = {i: ig or not is_flexres_atom[i] for (i, ig) in molsetup.atom_ignore.items()}
                 this_flex_pdbqt, ok, err = PDBQTWriterLegacy.write_string(molsetup, remove_smiles=True)
+                molsetup.atom_ignore = original_ignore
                 if not ok:
                     raise RuntimeError(err)
                 this_flex_pdbqt, flex_atom_count = cls.adapt_pdbqt_for_autodock4_flexres(
                     this_flex_pdbqt, 
                     resname,
                     chain,
                     resnum,
```

### Comparing `meeko-0.6.0a2/meeko.egg-info/PKG-INFO` & `meeko-0.6.0a3/meeko.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meeko
-Version: 0.6.0a2
+Version: 0.6.0a3
 Summary: Python package for preparing small molecule for docking
 Home-page: https://github.com/ccsb-scripps/meeko
 Author: Forli Lab
 Author-email: forli@scripps.edu
 License: LGPL-2.1
 Keywords: molecular modeling,drug design,docking,autodock
 Classifier: Environment :: Console
@@ -29,15 +29,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.18
 
 # Meeko: preparation of small molecules for AutoDock
 
 [![API stability](https://img.shields.io/badge/stable%20API-no-orange)](https://shields.io/)
-[![PyPI version fury.io](https://img.shields.io/badge/version-0.6.0--alpha.2-green.svg)](https://pypi.python.org/pypi/ansicolortags/)
+[![PyPI version fury.io](https://img.shields.io/badge/version-0.6.0--alpha.3-green.svg)](https://pypi.python.org/pypi/ansicolortags/)
 
 Meeko reads an RDKit molecule object and writes a PDBQT string (or file)
 for [AutoDock-Vina](https://github.com/ccsb-scripps/AutoDock-Vina)
 and [AutoDock-GPU](https://github.com/ccsb-scripps/AutoDock-GPU).
 It converts the docking output to RDKit molecules and
 SD files, without loss of bond orders.
 
@@ -63,15 +63,15 @@
 and RDKit issues
 [1755](https://github.com/rdkit/rdkit/issues/1755) and
 [917](https://github.com/rdkit/rdkit/issues/917). So, what could go wrong?
 For example, reading Mol2 files from ZINC
 [led to incorrect net charge of some molecules.](https://github.com/forlilab/Meeko/issues/63)
 
 
-## v0.6.0-alpha.2
+## v0.6.0-alpha.3
 
 This release aims to distribute an enhanced `mk_prepare_receptor.py`.
 Some features are still being developed, hence the `-alpha` suffix in the version.
 Reactive docking is not working in v0.6.0-alpha, but should be restored soon.
 Documentation is also work in progress.
 
 
@@ -306,14 +306,19 @@
     --receptor protein.pdb\
     --rec_residue ":CYS:6"\
     --tether_smarts "NC(=O)C(O)(C)SCC"\
     --tether_smarts_indices 9 8\
     -o prepared.pdbqt
 ```
 
+Prody is required for preparing ligands as flexible sidechains.
+Often, `pip install prody` suffices to install Prody in the currently
+active virtual environment (e.g., conda). For more detailed installation
+instructions visit http://prody.csb.pitt.edu/downloads/.
+
 ## Reactive Docking
 
 ### 1. Prepare protein with waterkit
 Follow `wk_prepare_receptor.py` instructions and run with `--pdb`.
 The goal of this step is to perform essential fixes to the protein
 (such as missing atoms), to add hydrogens, and to follow the Amber
 naming scheme for atoms and residues, e.g., `HIE` or `HID`
```

### Comparing `meeko-0.6.0a2/meeko.egg-info/SOURCES.txt` & `meeko-0.6.0a3/meeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/scripts/mk_export.py` & `meeko-0.6.0a3/scripts/mk_export.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/scripts/mk_prepare_ligand.py` & `meeko-0.6.0a3/scripts/mk_prepare_ligand.py`

 * *Files identical despite different names*

### Comparing `meeko-0.6.0a2/scripts/mk_prepare_receptor.py` & `meeko-0.6.0a3/scripts/mk_prepare_receptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import json
 import math
 from os import linesep as os_linesep
 import pathlib
 import pickle
 import sys
 
+import numpy as np
 
 from meeko import PDBQTReceptor
 from meeko import PDBQTMolecule
 from meeko import RDKitMolCreate
 from meeko import MoleculePreparation
 from meeko import MoleculeSetup
 from meeko import PDBQTWriterLegacy
@@ -138,70 +139,86 @@
     config_group.add_argument(      '--termini',
                                   help="e.g. '{\"A:GLY:350\":\"C-term\"}'")
     config_group.add_argument(      '--del_res', help="e.g. '[\"A:GLY:350\", \"B:ALA:17\"]'")
     config_group.add_argument(      '--chorizo_config', help="[.json]")
     config_group.add_argument(      '--mk_config', help="[.json]")
     config_group.add_argument(      '--allow_bad_res', action="store_true",
                                                  help="delete residues with missing atoms instead of raising error")
+    config_group.add_argument(      '--skip_auto_disulfide', action="store_true")
     config_group.add_argument('-f', '--flexres', action="append", default=[],
                         help="repeat flag for each residue, e.g: -f \" :LYS:42\" -f \"B:TYR:23\" and keep space for empty chain")
 
     box_group = parser.add_argument_group("Size and center of grid box")
     #box_group.add_argument('-b', '--gridbox_filename', help="set grid box size and center using a Vina configuration file")
     box_group.add_argument('--skip_gpf', help="do not write a GPF file for autogrid", action="store_true")
     box_group.add_argument('--box_size', help="size of grid box (x, y, z) in Angstrom", nargs=3, type=float)
     box_group.add_argument('--box_center', help="center of grid box (x, y, z) in Angstrom", nargs=3, type=float)
-    box_group.add_argument('--box_center_on_reactive_res', help="project center of grid box along CA-CB bond 5 A away from CB", action="store_true")
+    box_group.add_argument('--box_center_off_reactive_res', help="project grid box center along CA-CB bond 5 A away from CB", action="store_true")
     box_group.add_argument('--ligand', help="Reference ligand file path: .sdf, .mol, .mol2, .pdb, and .pdbqt files accepted")
     box_group.add_argument('--padding', help="padding around reference ligand [A]", type=float)
 
 
-    #reactive_group = parser.add_argument_group("Reactive")
-    #reactive_group.add_argument('-r', '--reactive_flexres', action="append", default=[],
-    #                    help="same as --flexres but for reactive residues (max 8)")
-    #reactive_group.add_argument('-g', '--reactive_name', action="append", default=[],
-    #                    help="set name of reactive atom of a residue type, e.g: -g 'TRP:NE1'. Overridden by --reactive_name_specific")
-    #reactive_group.add_argument('-s', '--reactive_name_specific', action="append", default=[],
-    #                    help="set name of reactive atom for an individual residue, e.g: -s 'A:HIE:42:NE2'. Residue will be reactive.")
-
-    #reactive_group.add_argument('--r_eq_12', default=1.8, type=float, help="r_eq for reactive atoms (1-2 interaction)")
-    #reactive_group.add_argument('--eps_12', default=2.5, type=float, help="epsilon for reactive atoms (1-2 interaction)")
-    #reactive_group.add_argument('--r_eq_13_scaling', default=0.5, type=float, help="r_eq scaling for 1-3 interaction across reactive atoms")
-    #reactive_group.add_argument('--r_eq_14_scaling', default=0.5, type=float, help="r_eq scaling for 1-4 interaction across reactive atoms")
+    reactive_group = parser.add_argument_group("Reactive")
+    reactive_group.add_argument('-r', '--reactive_flexres', action="append", default=[],
+                        help="same as --flexres but for reactive residues (max 8)")
+    reactive_group.add_argument('-g', '--reactive_name', action="append", default=[],
+                        help="set name of reactive atom of a residue type, e.g: -g 'TRP:NE1'. Overridden by --reactive_name_specific")
+    reactive_group.add_argument('-s', '--reactive_name_specific', action="append", default=[],
+                        help="set name of reactive atom for an individual residue, e.g: -s 'A:HIE:42:NE2'. Residue will be reactive.")
+
+    reactive_group.add_argument('--r_eq_12', default=1.8, type=float, help="r_eq for reactive atoms (1-2 interaction)")
+    reactive_group.add_argument('--eps_12', default=2.5, type=float, help="epsilon for reactive atoms (1-2 interaction)")
+    reactive_group.add_argument('--r_eq_13_scaling', default=0.5, type=float, help="r_eq scaling for 1-3 interaction across reactive atoms")
+    reactive_group.add_argument('--r_eq_14_scaling', default=0.5, type=float, help="r_eq scaling for 1-4 interaction across reactive atoms")
     args = parser.parse_args()
 
     #if (args.pdb is None) == (args.pdbqt is None):
         #msg = "need either --pdb or --pdbqt"
     if args.pdb is None:
         msg = "need --pdb"
         print("Command line error: " + msg, file=sys.stderr)
         sys.exit(2)
-    if (args.box_center is not None) and args.box_center_on_reactive_res:
-        msg = "can't use both --box_center and --box_center_on_reactive_res"
+    if (args.box_center is not None) and args.box_center_off_reactive_res:
+        msg = "can't use both --box_center and --box_center_off_reactive_res"
         print("Command line error: " + msg, file=sys.stderr)
         sys.exit(2)
-    got_center = (args.box_center is not None) or args.box_center_on_reactive_res or (args.ligand is not None)
+    if (args.padding is None) != (args.ligand is None):
+        print("--padding and --ligand must be used together", file=sys.stderr)
+        sys.exit(2)
+    nr_boxcenter_specs = 0
+    nr_boxcenter_specs += int(args.box_center is not None)
+    nr_boxcenter_specs += int(args.box_center_off_reactive_res)
+    nr_boxcenter_specs += int(args.ligand is not None)
+    if nr_boxcenter_specs > 1:
+        msg = "box center can't be specified in more than once."
+        msg += "use one of the following three options:" + os_linesep
+        msg += "  1) --box_center" + os_linesep
+        msg += "  2) --box_center_off_reactive_res" + os_linesep
+        msg += "  3) both --ligand and --padding in combination" + os_linesep
+        print(msg, file=sys.stderr)
+        sys.exit(42)
     if not args.skip_gpf:
-        if not got_center:
-            msg  = "missing center or size of grid box to write .gpf file for autogrid4" + os_linesep
-            msg += "use --box_size and either --box_center or --box_center_on_reactive_res" + os_linesep
+        if nr_boxcenter_specs < 1:
+            msg  = "missing center of grid box to write .gpf file for autogrid4" + os_linesep
+            msg += "use --box_size and either --box_center or --box_center_off_reactive_res" + os_linesep
             msg += "or --ligand and --padding" + os_linesep
-            msg += "Exactly one reactive residue required for --box_center_on_reactive_res" + os_linesep
+            msg += "Exactly one reactive residue required for --box_center_off_reactive_res" + os_linesep
             msg += "If a GPF file is not needed (e.g. docking with Vina scoring function) use option --skip_gpf"
             print("Command line error: " + msg, file=sys.stderr)
             sys.exit(2)
         if (args.box_size is None) and (args.padding is None):
-            msg  = "grid box information is needed to dock with the AD4 scoring function." + os_linesep
+            msg  = "grid box size is missing to dock with the AD4 scoring function." + os_linesep
+            msg += "use either --box_size or both --ligand and --padding" + os_linesep
             msg += "The grid box center and size will be used to write a GPF file for autogrid" + os_linesep
             msg += "If a GPF file is not needed (e.g. docking with Vina scoring function) use option --skip_gpf"
             print("Command line error: " + msg, file=sys.stderr)
             sys.exit(2)
 
-    if (args.box_center is not None) + (args.ligand is not None) + args.box_center_on_reactive_res > 1:
-        msg = "--box_center, --box_center_on_reactive_res, and --ligand are mutually exclusive options"
+    if (args.box_center is not None) + (args.ligand is not None) + args.box_center_off_reactive_res > 1:
+        msg = "--box_center, --box_center_off_reactive_res, and --ligand are mutually exclusive options"
         print("Command line error: " + msg, file=sys.stderr)
         sys.exit(2)
 
     return args
 
 args = get_args()
 
@@ -223,39 +240,39 @@
 ###         print("Error in parsing --reactive_name argument" + os_linesep, file=sys.stderr)
 ###         print(err, file=sys.stderr)
 ###         sys.exit(2)
 
 reactive_flexres = {}
 all_ok = True
 all_err = ""
-### for resid_string in args.reactive_flexres:
-###     res_id, ok, err = parse_residue_string(resid_string)
-###     if ok:
-###         resname = res_id[1]
-###         if resname in reactive_atom:
-###             reactive_flexres[res_id] = reactive_atom[resname]
-###         else:
-###             all_ok = False
-###             all_err += "no default reactive name for %s, " % resname
-###             all_err += "use --reactive_name or --reactive_name_specific" + os_linesep
-###     all_ok &= ok
-###     all_err += err
+for resid_string in args.reactive_flexres:
+    res_id, ok, err = parse_residue_string(resid_string)
+    if ok:
+        resname = res_id[1]
+        if resname in reactive_atom:
+            reactive_flexres[res_id] = reactive_atom[resname]
+        else:
+            all_ok = False
+            all_err += "no default reactive name for %s, " % resname
+            all_err += "use --reactive_name or --reactive_name_specific" + os_linesep
+    all_ok &= ok
+    all_err += err
 
-### for string in args.reactive_name_specific:
-###     out, ok, err = parse_residue_string_and_name(string)
-###     if ok:
-###         # override name if res_id was also passed to --reactive_flexres
-###         reactive_flexres[out["res_id"]] = out["name"]
-###     all_ok &= ok
-###     all_err += err
-
-### if len(reactive_flexres) > 8:
-###     msg = "got %d reactive_flexres but maximum is 8." % (len(args.reactive_flexres))
-###     print("Command line error: " + msg, file=sys.stderr)
-###     sys.exit(2)
+for string in args.reactive_name_specific:
+    out, ok, err = parse_residue_string_and_name(string)
+    if ok:
+        # override name if res_id was also passed to --reactive_flexres
+        reactive_flexres[out["res_id"]] = out["name"]
+    all_ok &= ok
+    all_err += err
+
+if len(reactive_flexres) > 8:
+    msg = "got %d reactive_flexres but maximum is 8." % (len(args.reactive_flexres))
+    print("Command line error: " + msg, file=sys.stderr)
+    sys.exit(2)
 
 all_flexres = set()
 for resid_string in args.flexres:
     res_id, ok, err = parse_residue_string(resid_string)
     all_ok &= ok
     all_err += err
     if ok:
@@ -283,15 +300,15 @@
         if is_react:
             react_atom = reactive_flexres[res_id]
         else:
             react_atom = ""
         print(string % (chain, resname, resnum, is_react, react_atom))
     print()
 
-if len(reactive_flexres) != 1 and args.box_center_on_reactive_res:
+if len(reactive_flexres) != 1 and args.box_center_off_reactive_res:
     msg = "--box_center_on-reactive_res can be used only with one reactive" + os_linesep
     msg += "residue, but %d reactive residues are set" % len(reactive_flexres)
     print("Command line error:" + msg, file=sys.stderr)
     sys.exit(2)
 
 if args.pdb is not None:
     mutate_res_dict = {}
@@ -309,15 +326,15 @@
     if args.termini is not None:
         termini.update(json.loads(args.termini))
     if args.del_res is not None:
         del_res.update(json.loads(args.del_res))
     with open(args.pdb) as f:
         pdb_string = f.read()
     chorizo = LinkedRDKitChorizo(pdb_string, mutate_res_dict=mutate_res_dict, termini=termini, deleted_residues=del_res,
-                                 allow_bad_res=args.allow_bad_res)
+                                 allow_bad_res=args.allow_bad_res, skip_auto_disulfide=args.skip_auto_disulfide)
     if args.mk_config is not None:
         with open(args.mk_config) as f:
             mk_config = json.load(f)
         mk_prep = MoleculePreparation.from_config(mk_config)
         chorizo.mk_parameterize_all_residues(mk_prep)
     else:
         mk_prep = MoleculePreparation()
@@ -331,18 +348,19 @@
         with open(args.chorizo_pickle, "wb") as f:
             pickle.dump(chorizo, f)
 
     suggested_config = {}
     if len(chorizo.suggested_mutations):
         suggested_config["mutate_res_dict"] = chorizo.suggested_mutations.copy()
 
-    if len(chorizo.getIgnoredResidues()) > 0:
-        print("Automatically deleted %d residues" % len(chorizo.removed_residues))
-        print(json.dumps(chorizo.removed_residues, indent=4))
-        suggested_config["del_res"] = chorizo.removed_residues.copy()
+    if len(chorizo.get_ignored_residues()) > 0:
+        removed_residues = chorizo.get_ignored_residues()
+        print("Automatically deleted %d residues" % len(removed_residues))
+        print(json.dumps(list(removed_residues.keys()), indent=4))
+        suggested_config["deleted_residues"] = removed_residues.copy()
 
     #rigid_pdbqt, ok, err = PDBQTWriterLegacy.write_string_static_molsetup(molsetup)
     #ok, err = receptor.assign_types_charges()
     #check(ok, err)
 #else:
 #    receptor = PDBQTReceptor(args.pdbqt)
 #    pdbqt, ok, err = receptor.write_pdbqt_string(flexres=all_flexres)
@@ -361,14 +379,15 @@
 written_files_log = {"filename": [], "description": []}
 
 if len(all_flexres) == 0:
     box_center = args.box_center
     rigid_fn = str(outpath.with_suffix(".pdbqt"))
     flex_fn = None
 else:
+    print(f"{reactive_flexres=}")
     all_flex_pdbqt = ""
     reactive_flexres_count = 0
     for res_id, flexres_pdbqt in pdbqt["flex"].items():
         res_id = tuple(res_id.split(":"))
         res_id = res_id[:2] + (int(res_id[2]),)
         if res_id in reactive_flexres:
             reactive_flexres_count += 1
@@ -395,53 +414,60 @@
     f.write(pdbqt["rigid"])
 
 if len(suggested_config):
     suggested_fn = str(outpath.with_suffix("")) + "_suggested-config.json"
     written_files_log["filename"].append(suggested_fn)
     written_files_log["description"].append("log of automated decisions for user inspection")
     with open(suggested_fn, "w") as f:
-        json.dump(suggested_config, f)
+        print(suggested_config)
+        json.dump(list(suggested_config.keys()), f)
 
 # GPF for autogrid4
 if not args.skip_gpf:
     if args.box_center is not None:
         box_center = args.box_center
         box_size = args.box_size
-    elif args.box_center_on_reactive_res:
+    elif args.box_center_off_reactive_res:
         # we have only one reactive residue and will set the box center
         # to be 5 Angstromg away from CB along the CA->CB vector
-        idxs = receptor.atom_idxs_by_res[list(reactive_flexres.keys())[0]]
-        ca = None
-        cb = None
-        for atom in receptor.atoms(idxs):
-            if atom["name"] == "CA":
-                ca = atom["xyz"]
-            if atom["name"] == "CB":
-                cb = atom["xyz"]
-        if ca is None or cb is None:
-            check(success=False, error_msg="could not find CA or CB in %s" % reactive_flexres[0])
-        v = (cb - ca)
-        v /= math.sqrt(v[0]**2 + v[1]**2 + v[2]**2) + 1e-8
-        box_center = ca + 5 * v
+        box_centers = []
+        for res_id_tuple in reactive_flexres.keys():
+            res_id = f"{res_id_tuple[0]}:{res_id_tuple[1]}:{res_id_tuple[2]}"
+            molsetup = chorizo.residues[res_id].molsetup
+            calpha_idx = [i for i, pdbinfo in molsetup.pdbinfo.items() if pdbinfo.name == "CA"]
+            cbeta_idx = [i for i, pdbinfo in molsetup.pdbinfo.items() if pdbinfo.name == "CB"]
+            if len(calpha_idx) != 1:
+                check(success=False, error_msg=f"found {len(calpha_idx)} CA in {res_id} but expected 1")
+            if len(cbeta_idx) != 1:
+                check(success=False, error_msg=f"found {len(cbeta_idx)} CB in {res_id} but expected 1")
+            calpha_idx = calpha_idx[0]
+            cbeta_idx = cbeta_idx[0]
+            ca = molsetup.coord[calpha_idx]
+            cb = molsetup.coord[cbeta_idx]
+            v = (cb - ca)
+            v /= math.sqrt(v[0]**2 + v[1]**2 + v[2]**2) + 1e-8
+            box_center = ca + 5 * v
+            box_centers.append(box_center)
+        box_center = np.mean(box_centers, 0)
         box_size = args.box_size
     elif args.ligand is not None:
         ft = pathlib.Path(args.ligand).suffix
         suppliers = {
             ".pdb": Chem.MolFromPDBFile,
             ".mol": Chem.MolFromMolFile,
             ".mol2": Chem.MolFromMol2File,
             ".sdf": Chem.SDMolSupplier,
             ".pdbqt": None
         }
         if ft not in suppliers.keys():
             check(success=False, error_msg=f"Given --ligand file type {ft} not readable!")
         elif ft != ".sdf" and ft != ".pdbqt":
-            ligmol = suppliers[ft](args.ligand)
+            ligmol = suppliers[ft](args.ligand, removeHs=False, sanitize=False)
         elif ft == ".sdf":
-            ligmol = suppliers[ft](args.ligand)[0]  # assume we only want first molecule in file
+            ligmol = suppliers[ft](args.ligand, removeHs=False, sanitize=False)[0]  # assume we only want first molecule in file
         else:  # .pdbqt
             ligmol = RDKitMolCreate.from_pdbqt_mol(PDBQTMolecule.from_file(args.ligand))[0]  # assume we only want first molecule in file
         
         box_center, box_size = gridbox.calc_box(ligmol.GetConformer().GetPositions(), args.padding)
     else:
         print("Error: No box center specified.", file=sys.stderr)
         sys.exit(2)
@@ -460,100 +486,108 @@
     written_files_log["filename"].append(str(gpf_fn))
     written_files_log["description"].append("autogrid input file")
     with open(gpf_fn, "w") as f:
         f.write(gpf_string)
 
     # write a PDB for the box
     box_fn = str(gpf_fn) + ".pdb"
+    vinabox_fn = str(gpf_fn) + ".vinabox"
     written_files_log["filename"].append(box_fn)
     written_files_log["description"].append("PDB file to visualize the grid box")
     with open(box_fn, "w") as f:
         f.write(gridbox.box_to_pdb_string(box_center, npts))
 
+    # write gridbox vina format
+    box_vina_fn = str(pathlib.Path(rigid_fn).with_suffix(".box.txt"))
+    written_files_log["filename"].append(box_vina_fn)
+    written_files_log["description"].append("Vina-style box dimension file")
+    with open(box_vina_fn, "w") as f:
+        f.write(gridbox.box_to_vina_string(box_center, box_size))
+    
     # check all flexres are inside the box
     if len(reactive_flexres) > 0:
         any_outside = False
         for res_id, res in chorizo.residues.items():
             if not res.is_movable:
                 continue
             for index, coord in res.molsetup.coord.items():
-                if index in res.molsetup_ignored:
+                if not res.is_flexres_atom[index]:
                     continue
-                if gridbox.is_point_outside_box(atom["xyz"], box_center, npts):
+                if gridbox.is_point_outside_box(coord, box_center, npts):
                     print("WARNING: Flexible residue outside box." + os_linesep, file=sys.stderr)
                     print("WARNING: Strongly recommended to use a box that encompasses flexible residues." + os_linesep, file=sys.stderr)
                     break # only need to warn once
 
-### # configuration info for AutoDock-GPU reactive docking
-### if len(reactive_flexres) > 0:
-###     any_lig_reac_types = []
-###     for order in (1, 2, 3):
-###         for t in any_lig_base_types:
-###             any_lig_reac_types.append(reactive_typer.get_reactive_atype(t, order))
-### 
-###     rec_reac_types = []
-###     for line in all_flex_pdbqt.split(os_linesep):
-###         if line.startswith("ATOM") or line.startswith("HETATM"):
-###             atype = line[77:].strip()
-###             basetype, _ = reactive_typer.get_basetype_and_order(atype)
-###             if basetype is not None: # is None if not reactive
-###                 rec_reac_types.append(line[77:].strip())
-### 
-###     derivtypes, modpairs, collisions = get_reactive_config(
-###                                     any_lig_reac_types,
-###                                     rec_reac_types,
-###                                     args.eps_12,
-###                                     args.r_eq_12,
-###                                     args.r_eq_13_scaling,
-###                                     args.r_eq_14_scaling)
-### 
-###     if len(collisions) > 0:
-###         collision_str = ""
-###         for t1, t2 in collisions:
-###             collision_str += "%3s %3s" % (t1, t2) + os_linesep
-###         collision_fn = str(outpath.with_suffix(".atype_collisions"))
-###         written_files_log["filename"].append(collision_fn)
-###         written_files_log["description"].append("type pairs (n=%d) that may lead to intra-molecular reactions" % len(collisions))
-###         with open(collision_fn, "w") as f:
-###             f.write(collision_str)
-### 
-###     # The maps block is to tell AutoDock-GPU the base types for the reactive types.
-###     # This could be done with -T/--derivtypes, but putting derivtypes and intnbp
-###     # lines in a single configuration file simplifies the command line call.
-###     map_block = ""
-###     map_prefix = pathlib.Path(rigid_fn).with_suffix("").name
-###     all_types = []
-###     for basetype, reactypes in derivtypes.items():
-###         all_types.append(basetype)
-###         map_block += "map %s.%s.map" % (map_prefix, basetype) + os_linesep
-###         for reactype in reactypes:
-###             all_types.append(reactype)
-###             map_block += "map %s.%s.map" % (map_prefix, basetype) + os_linesep
-###     config = "ligand_types " + " ".join(all_types) + os_linesep
-###     config += "fld %s.maps.fld" % map_prefix + os_linesep
-###     config += map_block
-### 
-###     # in modpairs (dict): types are keys, parameters are values
-###     # now we will write a configuration file with nbp keywords
-###     # that AD-GPU reads using the --import_dpf flag
-###     # nbp stands for "non-bonded potential" or "non-bonded pairwise"
-###     line = "intnbp_r_eps %8.6f %8.6f %3d %3d %4s %4s" + os_linesep
-###     nbp_count = 0
-###     for (t1, t2), param in modpairs.items():
-###         config += line % (param["r_eq"], param["eps"], param["n"], param["m"], t1, t2)
-###         nbp_count += 1
-###     config_fn = str(outpath.with_suffix(".reactive_config"))
-###     written_files_log["filename"].append(config_fn)
-###     written_files_log["description"].append("reactive parameters for AutoDock-GPU")
-###     with open(config_fn, "w") as f:
-###         f.write(config)
-###     print()
-###     print("For reactive docking, pass the configuration file to AutoDock-GPU:")
-###     print("    autodock_gpu -C 1 --import_dpf %s --flexres %s -L <ligand_filename>" % (config_fn, flex_fn))
-###     print()
+# configuration info for AutoDock-GPU reactive docking
+if len(reactive_flexres) > 0:
+    any_lig_reac_types = []
+    for order in (1, 2, 3):
+        for t in any_lig_base_types:
+            any_lig_reac_types.append(reactive_typer.get_reactive_atype(t, order))
+
+    rec_reac_types = []
+    for line in all_flex_pdbqt.split(os_linesep):
+        if line.startswith("ATOM") or line.startswith("HETATM"):
+            atype = line[77:].strip()
+            basetype, _ = reactive_typer.get_basetype_and_order(atype)
+            if basetype is not None: # is None if not reactive
+                rec_reac_types.append(line[77:].strip())
+
+    derivtypes, modpairs, collisions = get_reactive_config(
+                                    any_lig_reac_types,
+                                    rec_reac_types,
+                                    args.eps_12,
+                                    args.r_eq_12,
+                                    args.r_eq_13_scaling,
+                                    args.r_eq_14_scaling)
+
+    if len(collisions) > 0:
+        collision_str = ""
+        for t1, t2 in collisions:
+            collision_str += "%3s %3s" % (t1, t2) + os_linesep
+        collision_fn = str(outpath.with_suffix(".atype_collisions"))
+        written_files_log["filename"].append(collision_fn)
+        written_files_log["description"].append("type pairs (n=%d) that may lead to intra-molecular reactions" % len(collisions))
+        with open(collision_fn, "w") as f:
+            f.write(collision_str)
+
+    # The maps block is to tell AutoDock-GPU the base types for the reactive types.
+    # This could be done with -T/--derivtypes, but putting derivtypes and intnbp
+    # lines in a single configuration file simplifies the command line call.
+    map_block = ""
+    map_prefix = pathlib.Path(rigid_fn).with_suffix("").name
+    all_types = []
+    for basetype, reactypes in derivtypes.items():
+        all_types.append(basetype)
+        map_block += "map %s.%s.map" % (map_prefix, basetype) + os_linesep
+        for reactype in reactypes:
+            all_types.append(reactype)
+            map_block += "map %s.%s.map" % (map_prefix, basetype) + os_linesep
+    config = "ligand_types " + " ".join(all_types) + os_linesep
+    config += "fld %s.maps.fld" % map_prefix + os_linesep
+    config += map_block
+
+    # in modpairs (dict): types are keys, parameters are values
+    # now we will write a configuration file with nbp keywords
+    # that AD-GPU reads using the --import_dpf flag
+    # nbp stands for "non-bonded potential" or "non-bonded pairwise"
+    line = "intnbp_r_eps %8.6f %8.6f %3d %3d %4s %4s" + os_linesep
+    nbp_count = 0
+    for (t1, t2), param in modpairs.items():
+        config += line % (param["r_eq"], param["eps"], param["n"], param["m"], t1, t2)
+        nbp_count += 1
+    config_fn = str(outpath.with_suffix(".reactive_config"))
+    written_files_log["filename"].append(config_fn)
+    written_files_log["description"].append("reactive parameters for AutoDock-GPU")
+    with open(config_fn, "w") as f:
+        f.write(config)
+    print()
+    print("For reactive docking, pass the configuration file to AutoDock-GPU:")
+    print("    autodock_gpu -C 1 --import_dpf %s --flexres %s -L <ligand_filename>" % (config_fn, flex_fn))
+    print()
 
 print()
 print("Files written:")
 longest_fn = max([len(fn) for fn in written_files_log["filename"]])
 line = "%%%ds <-- " % longest_fn + "%s"
 for fn, desc in zip(written_files_log["filename"], written_files_log["description"]):
     print(line % (fn, desc))
```

### Comparing `meeko-0.6.0a2/setup.py` & `meeko-0.6.0a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             matches.append(os.path.join(root, filename))
 
     return matches
 
 
 setup(
     name="meeko",
-    version='0.6.0-alpha.2',
+    version='0.6.0-alpha.3',
     author="Forli Lab",
     author_email="forli@scripps.edu",
     url="https://github.com/ccsb-scripps/meeko",
     description='Python package for preparing small molecule for docking',
     long_description=open(os.path.join(base_dir, 'README.md')).read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `meeko-0.6.0a2/test/test-oids.py` & `meeko-0.6.0a3/test/test-oids.py`

 * *Files identical despite different names*

