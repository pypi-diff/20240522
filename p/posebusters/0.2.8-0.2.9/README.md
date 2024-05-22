# Comparing `tmp/posebusters-0.2.8.tar.gz` & `tmp/posebusters-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posebusters-0.2.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "posebusters-0.2.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `posebusters-0.2.8.tar` & `posebusters-0.2.9.tar`

### file list

```diff
@@ -1,166 +1,166 @@
--rw-r--r--   0        0        0      630 2023-11-21 22:22:52.666324 posebusters-0.2.8/.github/workflows/publishing.yml
--rw-r--r--   0        0        0     2144 2023-11-21 22:22:52.666324 posebusters-0.2.8/.github/workflows/security.yml
--rw-r--r--   0        0        0     1420 2023-11-21 22:22:52.666324 posebusters-0.2.8/.github/workflows/testing.yml
--rw-r--r--   0        0        0      947 2023-11-21 22:22:52.666324 posebusters-0.2.8/.github/workflows/validation.yml
--rw-r--r--   0        0        0     1879 2023-11-21 22:22:52.666324 posebusters-0.2.8/.gitignore
--rw-r--r--   0        0        0     2541 2023-11-21 22:22:52.666324 posebusters-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     7606 2023-11-21 22:22:52.666324 posebusters-0.2.8/.vscode/launch.json
--rw-r--r--   0        0        0     1099 2023-11-21 22:22:52.666324 posebusters-0.2.8/.vscode/settings.json
--rw-r--r--   0        0        0     1527 2023-11-21 22:22:52.666324 posebusters-0.2.8/LICENSE
--rw-r--r--   0        0        0     2441 2023-11-21 22:22:52.666324 posebusters-0.2.8/README.md
--rw-r--r--   0        0        0      638 2023-11-21 22:22:52.666324 posebusters-0.2.8/docs/Makefile
--rw-r--r--   0        0        0      804 2023-11-21 22:22:52.666324 posebusters-0.2.8/docs/make.bat
--rw-r--r--   0        0        0       98 2023-11-21 22:22:52.666324 posebusters-0.2.8/docs/requirements.txt
--rw-r--r--   0        0        0    58908 2023-11-21 22:22:52.666324 posebusters-0.2.8/docs/source/_static/logo_banner.png
--rwxr-xr-x   0        0        0    41654 2023-11-21 22:22:52.666324 posebusters-0.2.8/docs/source/_static/logo_square.png
--rw-r--r--   0        0        0     1992 2023-11-21 22:22:52.666324 posebusters-0.2.8/docs/source/api.rst
--rw-r--r--   0        0        0    46247 2023-11-21 22:22:52.666324 posebusters-0.2.8/docs/source/api_notebook.ipynb
--rw-r--r--   0        0        0     8645 2023-11-21 22:22:52.666324 posebusters-0.2.8/docs/source/checks.rst
--rw-r--r--   0        0        0     2868 2023-11-21 22:22:52.666324 posebusters-0.2.8/docs/source/cli.rst
--rw-r--r--   0        0        0     3061 2023-11-21 22:22:52.666324 posebusters-0.2.8/docs/source/conf.py
--rw-r--r--   0        0        0   122628 2023-11-21 22:22:52.670323 posebusters-0.2.8/docs/source/images/crystal_astex_1hww.png
--rw-r--r--   0        0        0    94435 2023-11-21 22:22:52.670323 posebusters-0.2.8/docs/source/images/crystal_astex_1k3u.png
--rw-r--r--   0        0        0    83738 2023-11-21 22:22:52.670323 posebusters-0.2.8/docs/source/images/crystal_astex_1s19.png
--rw-r--r--   0        0        0    84467 2023-11-21 22:22:52.670323 posebusters-0.2.8/docs/source/images/crystal_astex_1s3v.png
--rw-r--r--   0        0        0    92271 2023-11-21 22:22:52.670323 posebusters-0.2.8/docs/source/images/crystal_astex_1t9b.png
--rw-r--r--   0        0        0   153904 2023-11-21 22:22:52.670323 posebusters-0.2.8/docs/source/images/crystal_astex_1tt1.png
--rw-r--r--   0        0        0    67540 2023-11-21 22:22:52.670323 posebusters-0.2.8/docs/source/images/crystal_astex_1tz8.png
--rw-r--r--   0        0        0   110315 2023-11-21 22:22:52.670323 posebusters-0.2.8/docs/source/images/crystal_fragalysis_NSP14-x1316.png
--rw-r--r--   0        0        0   112813 2023-11-21 22:22:52.674324 posebusters-0.2.8/docs/source/images/deepdock_astex_1t9b.png
--rw-r--r--   0        0        0    67522 2023-11-21 22:22:52.674324 posebusters-0.2.8/docs/source/images/diffdock_astex_1s19.png
--rw-r--r--   0        0        0   136262 2023-11-21 22:22:52.674324 posebusters-0.2.8/docs/source/images/diffdock_astex_1tt1.png
--rw-r--r--   0        0        0    67077 2023-11-21 22:22:52.674324 posebusters-0.2.8/docs/source/images/equibind_astex_1tz8.png
--rw-r--r--   0        0        0    98366 2023-11-21 22:22:52.674324 posebusters-0.2.8/docs/source/images/tankbind_astex_1hww.png
--rw-r--r--   0        0        0    92996 2023-11-21 22:22:52.674324 posebusters-0.2.8/docs/source/images/tankbind_astex_1s3v.png
--rw-r--r--   0        0        0    74604 2023-11-21 22:22:52.674324 posebusters-0.2.8/docs/source/images/unimol_astex_1k3u.png
--rw-r--r--   0        0        0    77966 2023-11-21 22:22:52.674324 posebusters-0.2.8/docs/source/images/unimol_fragalysis_NSP14-x1316.png
--rw-r--r--   0        0        0     7107 2023-11-21 22:22:52.674324 posebusters-0.2.8/docs/source/index.rst
--rw-r--r--   0        0        0     1678 2023-11-21 22:22:52.674324 posebusters-0.2.8/docs/source/inputs/1ia1/1ia1_ligand.sdf
--rw-r--r--   0        0        0     3366 2023-11-21 22:22:52.674324 posebusters-0.2.8/docs/source/inputs/1ia1/1ia1_ligands.sdf
--rw-r--r--   0        0        0   259057 2023-11-21 22:22:52.678324 posebusters-0.2.8/docs/source/inputs/1ia1/1ia1_protein_one_lig_removed.pdb
--rw-r--r--   0        0        0     1154 2023-11-21 22:22:52.678324 posebusters-0.2.8/docs/source/inputs/1of6/1of6_ligand.sdf
--rw-r--r--   0        0        0     9272 2023-11-21 22:22:52.678324 posebusters-0.2.8/docs/source/inputs/1of6/1of6_ligands.sdf
--rw-r--r--   0        0        0  1652386 2023-11-21 22:22:52.686324 posebusters-0.2.8/docs/source/inputs/1of6/1of6_protein_one_lig_removed.pdb
--rw-r--r--   0        0        0     2342 2023-11-21 22:22:52.686324 posebusters-0.2.8/docs/source/inputs/1s3v/1s3v_ligand.sdf
--rw-r--r--   0        0        0     2347 2023-11-21 22:22:52.686324 posebusters-0.2.8/docs/source/inputs/1s3v/1s3v_ligands.sdf
--rw-r--r--   0        0        0   118807 2023-11-21 22:22:52.686324 posebusters-0.2.8/docs/source/inputs/1s3v/1s3v_protein_one_lig_removed.pdb
--rw-r--r--   0        0        0     1416 2023-11-21 22:22:52.686324 posebusters-0.2.8/docs/source/inputs/1uou/1uou_ligand.sdf
--rw-r--r--   0        0        0     1421 2023-11-21 22:22:52.686324 posebusters-0.2.8/docs/source/inputs/1uou/1uou_ligands.sdf
--rw-r--r--   0        0        0   253660 2023-11-21 22:22:52.686324 posebusters-0.2.8/docs/source/inputs/1uou/1uou_protein_one_lig_removed.pdb
--rw-r--r--   0        0        0     1689 2023-11-21 22:22:52.686324 posebusters-0.2.8/docs/source/inputs/crystal_ligand.sdf
--rw-r--r--   0        0        0     3388 2023-11-21 22:22:52.686324 posebusters-0.2.8/docs/source/inputs/generated_ligands.sdf
--rw-r--r--   0        0        0     6717 2023-11-21 22:22:52.686324 posebusters-0.2.8/docs/source/inputs/generated_molecules.sdf
--rw-r--r--   0        0        0      376 2023-11-21 22:22:52.686324 posebusters-0.2.8/docs/source/inputs/molecule_table.csv
--rw-r--r--   0        0        0   252714 2023-11-21 22:22:52.686324 posebusters-0.2.8/docs/source/inputs/protein.pdb
--rw-r--r--   0        0        0     1690 2023-11-21 22:22:52.686324 posebusters-0.2.8/docs/source/inputs/redocked_ligand.sdf
--rw-r--r--   0        0        0      946 2023-11-21 22:22:52.686324 posebusters-0.2.8/posebusters/__init__.py
--rw-r--r--   0        0        0      183 2023-11-21 22:22:52.686324 posebusters-0.2.8/posebusters/__main__.py
--rw-r--r--   0        0        0     6194 2023-11-21 22:22:52.686324 posebusters-0.2.8/posebusters/cli.py
--rw-r--r--   0        0        0     7204 2023-11-21 22:22:52.686324 posebusters-0.2.8/posebusters/config/dock.yml
--rw-r--r--   0        0        0     3350 2023-11-21 22:22:52.686324 posebusters-0.2.8/posebusters/config/mol.yml
--rw-r--r--   0        0        0     8015 2023-11-21 22:22:52.686324 posebusters-0.2.8/posebusters/config/redock.yml
--rw-r--r--   0        0        0      147 2023-11-21 22:22:52.686324 posebusters-0.2.8/posebusters/datasets/__init__.py
--rw-r--r--   0        0        0      688 2023-11-21 22:22:52.686324 posebusters-0.2.8/posebusters/datasets/load_datasets.py
--rw-r--r--   0        0        0      424 2023-11-21 22:22:52.686324 posebusters-0.2.8/posebusters/datasets/pdb.csv
--rw-r--r--   0        0        0     1678 2023-11-21 22:22:52.686324 posebusters-0.2.8/posebusters/datasets/pdb/1ia1/1ia1_ligand.sdf
--rw-r--r--   0        0        0     3366 2023-11-21 22:22:52.686324 posebusters-0.2.8/posebusters/datasets/pdb/1ia1/1ia1_ligands.sdf
--rw-r--r--   0        0        0   265544 2023-11-21 22:22:52.690324 posebusters-0.2.8/posebusters/datasets/pdb/1ia1/1ia1_protein_one_lig_removed.pdb
--rw-r--r--   0        0        0     1154 2023-11-21 22:22:52.690324 posebusters-0.2.8/posebusters/datasets/pdb/1of6/1of6_ligand.sdf
--rw-r--r--   0        0        0     9272 2023-11-21 22:22:52.690324 posebusters-0.2.8/posebusters/datasets/pdb/1of6/1of6_ligands.sdf
--rw-r--r--   0        0        0  1694211 2023-11-21 22:22:52.690324 posebusters-0.2.8/posebusters/datasets/pdb/1of6/1of6_protein_one_lig_removed.pdb
--rw-r--r--   0        0        0     2342 2023-11-21 22:22:52.690324 posebusters-0.2.8/posebusters/datasets/pdb/1s3v/1s3v_ligand.sdf
--rw-r--r--   0        0        0     2347 2023-11-21 22:22:52.690324 posebusters-0.2.8/posebusters/datasets/pdb/1s3v/1s3v_ligands.sdf
--rw-r--r--   0        0        0   121812 2023-11-21 22:22:52.690324 posebusters-0.2.8/posebusters/datasets/pdb/1s3v/1s3v_protein_one_lig_removed.pdb
--rw-r--r--   0        0        0     1416 2023-11-21 22:22:52.690324 posebusters-0.2.8/posebusters/datasets/pdb/1uou/1uou_ligand.sdf
--rw-r--r--   0        0        0     1421 2023-11-21 22:22:52.690324 posebusters-0.2.8/posebusters/datasets/pdb/1uou/1uou_ligands.sdf
--rw-r--r--   0        0        0   260079 2023-11-21 22:22:52.690324 posebusters-0.2.8/posebusters/datasets/pdb/1uou/1uou_protein_one_lig_removed.pdb
--rw-r--r--   0        0        0       45 2023-11-21 22:22:52.690324 posebusters-0.2.8/posebusters/modules/__init__.py
--rw-r--r--   0        0        0     9830 2023-11-21 22:22:52.690324 posebusters-0.2.8/posebusters/modules/distance_geometry.py
--rw-r--r--   0        0        0     5243 2023-11-21 22:22:52.690324 posebusters-0.2.8/posebusters/modules/energy_ratio.py
--rw-r--r--   0        0        0     3187 2023-11-21 22:22:52.690324 posebusters-0.2.8/posebusters/modules/flatness.py
--rw-r--r--   0        0        0     6044 2023-11-21 22:22:52.694324 posebusters-0.2.8/posebusters/modules/identity.py
--rw-r--r--   0        0        0     5177 2023-11-21 22:22:52.694324 posebusters-0.2.8/posebusters/modules/intermolecular_distance.py
--rw-r--r--   0        0        0      792 2023-11-21 22:22:52.694324 posebusters-0.2.8/posebusters/modules/loading.py
--rw-r--r--   0        0        0     6830 2023-11-21 22:22:52.694324 posebusters-0.2.8/posebusters/modules/rmsd.py
--rw-r--r--   0        0        0     1294 2023-11-21 22:22:52.694324 posebusters-0.2.8/posebusters/modules/sanity.py
--rw-r--r--   0        0        0     2713 2023-11-21 22:22:52.694324 posebusters-0.2.8/posebusters/modules/volume_overlap.py
--rw-r--r--   0        0        0     9135 2023-11-21 22:22:52.694324 posebusters-0.2.8/posebusters/posebusters.py
--rw-r--r--   0        0        0       58 2023-11-21 22:22:52.694324 posebusters-0.2.8/posebusters/tools/__init__.py
--rw-r--r--   0        0        0     1426 2023-11-21 22:22:52.694324 posebusters-0.2.8/posebusters/tools/formatting.py
--rw-r--r--   0        0        0     6123 2023-11-21 22:22:52.694324 posebusters-0.2.8/posebusters/tools/loading.py
--rw-r--r--   0        0        0     1165 2023-11-21 22:22:52.694324 posebusters-0.2.8/posebusters/tools/logging.py
--rw-r--r--   0        0        0     6993 2023-11-21 22:22:52.694324 posebusters-0.2.8/posebusters/tools/molecules.py
--rw-r--r--   0        0        0      516 2023-11-21 22:22:52.694324 posebusters-0.2.8/posebusters/tools/parallel.py
--rw-r--r--   0        0        0     2367 2023-11-21 22:22:52.694324 posebusters-0.2.8/posebusters/tools/protein.py
--rw-r--r--   0        0        0     1122 2023-11-21 22:22:52.694324 posebusters-0.2.8/posebusters/tools/stats.py
--rw-r--r--   0        0        0     2229 2023-11-21 22:22:52.694324 posebusters-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-21 22:22:52.694324 posebusters-0.2.8/tests/__init__.py
--rw-r--r--   0        0        0     4724 2023-11-21 22:22:52.694324 posebusters-0.2.8/tests/conftest.py
--rw-r--r--   0        0        0   705759 2023-11-21 22:22:52.694324 posebusters-0.2.8/tests/conftest/1G9V_RQ3/1G9V_RQ3_gold_redock.sdf
--rw-r--r--   0        0        0     2179 2023-11-21 22:22:52.694324 posebusters-0.2.8/tests/conftest/1G9V_RQ3/1G9V_RQ3_ligand.sdf
--rw-r--r--   0        0        0     4069 2023-11-21 22:22:52.694324 posebusters-0.2.8/tests/conftest/1G9V_RQ3/1G9V_RQ3_ligand_start_conf.sdf
--rw-r--r--   0        0        0     4358 2023-11-21 22:22:52.694324 posebusters-0.2.8/tests/conftest/1G9V_RQ3/1G9V_RQ3_ligands.sdf
--rw-r--r--   0        0        0   374213 2023-11-21 22:22:52.698324 posebusters-0.2.8/tests/conftest/1G9V_RQ3/1G9V_RQ3_protein.pdb
--rw-r--r--   0        0        0     1694 2023-11-21 22:22:52.698324 posebusters-0.2.8/tests/conftest/1IA1_TQ3/1IA1_TQ3_ligand.sdf
--rw-r--r--   0        0        0     2671 2023-11-21 22:22:52.698324 posebusters-0.2.8/tests/conftest/1IA1_TQ3/1IA1_TQ3_ligand_start_conf.sdf
--rw-r--r--   0        0        0     3388 2023-11-21 22:22:52.698324 posebusters-0.2.8/tests/conftest/1IA1_TQ3/1IA1_TQ3_ligands.sdf
--rw-r--r--   0        0        0   269862 2023-11-21 22:22:52.698324 posebusters-0.2.8/tests/conftest/1IA1_TQ3/1IA1_TQ3_no_ligand_no_solvent.pdb
--rw-r--r--   0        0        0   268852 2023-11-21 22:22:52.698324 posebusters-0.2.8/tests/conftest/1IA1_TQ3/1IA1_TQ3_no_ligand_no_solvent_no_inorganic.pdb
--rw-r--r--   0        0        0   258884 2023-11-21 22:22:52.698324 posebusters-0.2.8/tests/conftest/1IA1_TQ3/1IA1_TQ3_no_ligand_no_solvent_no_inorganic_no_cofactors.pdb
--rw-r--r--   0        0        0     1342 2023-11-21 22:22:52.698324 posebusters-0.2.8/tests/conftest/1MMV_3AR/1MMV_3AR_crystal.sdf
--rw-r--r--   0        0        0     1327 2023-11-21 22:22:52.698324 posebusters-0.2.8/tests/conftest/1MMV_3AR/1MMV_3AR_tankbind.sdf
--rw-r--r--   0        0        0     1171 2023-11-21 22:22:52.698324 posebusters-0.2.8/tests/conftest/1OF6_DTY/1OF6_DTY_crystal.sdf
--rw-r--r--   0        0        0    28966 2023-11-21 22:22:52.698324 posebusters-0.2.8/tests/conftest/1OF6_DTY/1OF6_DTY_vina.sdf
--rw-r--r--   0        0        0     1795 2023-11-21 22:22:52.698324 posebusters-0.2.8/tests/conftest/1Q1G_MTI/1Q1G_MTI_crystal.sdf
--rw-r--r--   0        0        0     1781 2023-11-21 22:22:52.698324 posebusters-0.2.8/tests/conftest/1Q1G_MTI/1Q1G_MTI_tankbind.sdf
--rw-r--r--   0        0        0     1018 2023-11-21 22:22:52.698324 posebusters-0.2.8/tests/conftest/1W1P_GIO/1W1P_GIO_ligand.sdf
--rw-r--r--   0        0        0     1828 2023-11-21 22:22:52.698324 posebusters-0.2.8/tests/conftest/1W1P_GIO/1W1P_GIO_ligand_start_conf.sdf
--rw-r--r--   0        0        0     2036 2023-11-21 22:22:52.698324 posebusters-0.2.8/tests/conftest/1W1P_GIO/1W1P_GIO_ligands.sdf
--rw-r--r--   0        0        0   650319 2023-11-21 22:22:52.702324 posebusters-0.2.8/tests/conftest/1W1P_GIO/1W1P_GIO_protein.pdb
--rw-r--r--   0        0        0     1678 2023-11-21 22:22:52.702324 posebusters-0.2.8/tests/conftest/1ia1/1ia1_ligand.sdf
--rw-r--r--   0        0        0     3366 2023-11-21 22:22:52.702324 posebusters-0.2.8/tests/conftest/1ia1/1ia1_ligands.sdf
--rw-r--r--   0        0        0   265544 2023-11-21 22:22:52.702324 posebusters-0.2.8/tests/conftest/1ia1/1ia1_protein_one_lig_removed.pdb
--rw-r--r--   0        0        0     1154 2023-11-21 22:22:52.702324 posebusters-0.2.8/tests/conftest/1of6/1of6_ligand.sdf
--rw-r--r--   0        0        0     9272 2023-11-21 22:22:52.702324 posebusters-0.2.8/tests/conftest/1of6/1of6_ligands.sdf
--rw-r--r--   0        0        0  1694211 2023-11-21 22:22:52.706324 posebusters-0.2.8/tests/conftest/1of6/1of6_protein_one_lig_removed.pdb
--rw-r--r--   0        0        0     2342 2023-11-21 22:22:52.706324 posebusters-0.2.8/tests/conftest/1s3v/1s3v_ligand.sdf
--rw-r--r--   0        0        0     2347 2023-11-21 22:22:52.706324 posebusters-0.2.8/tests/conftest/1s3v/1s3v_ligands.sdf
--rw-r--r--   0        0        0   121812 2023-11-21 22:22:52.706324 posebusters-0.2.8/tests/conftest/1s3v/1s3v_protein_one_lig_removed.pdb
--rw-r--r--   0        0        0     1416 2023-11-21 22:22:52.706324 posebusters-0.2.8/tests/conftest/1uou/1uou_ligand.sdf
--rw-r--r--   0        0        0     1421 2023-11-21 22:22:52.706324 posebusters-0.2.8/tests/conftest/1uou/1uou_ligands.sdf
--rw-r--r--   0        0        0   260079 2023-11-21 22:22:52.706324 posebusters-0.2.8/tests/conftest/1uou/1uou_protein_one_lig_removed.pdb
--rw-r--r--   0        0        0     3645 2023-11-21 22:22:52.706324 posebusters-0.2.8/tests/conftest/6YR2_T1C/6YR2_T1C_crystal.sdf
--rw-r--r--   0        0        0     3628 2023-11-21 22:22:52.706324 posebusters-0.2.8/tests/conftest/6YR2_T1C/6YR2_T1C_tankbind.sdf
--rw-r--r--   0        0        0      838 2023-11-21 22:22:52.706324 posebusters-0.2.8/tests/conftest/7CNQ_G8X/7CNQ_G8X_ligand.sdf
--rw-r--r--   0        0        0  1329827 2023-11-21 22:22:52.710324 posebusters-0.2.8/tests/conftest/7CNQ_G8X/7CNQ_G8X_protein.pdb
--rw-r--r--   0        0        0      742 2023-11-21 22:22:52.710324 posebusters-0.2.8/tests/conftest/7ECR_SIN/7ECR_SIN_ligand.sdf
--rw-r--r--   0        0        0   867187 2023-11-21 22:22:52.714324 posebusters-0.2.8/tests/conftest/7ECR_SIN/7ECR_SIN_protein.pdb
--rw-r--r--   0        0        0      991 2023-11-21 22:22:52.714324 posebusters-0.2.8/tests/conftest/7ZTL_BCN/7ZTL_BCN_ligand.sdf
--rw-r--r--   0        0        0      991 2023-11-21 22:22:52.714324 posebusters-0.2.8/tests/conftest/7ZTL_BCN/7ZTL_BCN_ligands.sdf
--rw-r--r--   0        0        0   189935 2023-11-21 22:22:52.714324 posebusters-0.2.8/tests/conftest/7ZTL_BCN/7ZTL_BCN_protein.pdb
--rw-r--r--   0        0        0     2270 2023-11-21 22:22:52.714324 posebusters-0.2.8/tests/conftest/mol_1a30_clash_2.sdf
--rw-r--r--   0        0        0     2270 2023-11-21 22:22:52.714324 posebusters-0.2.8/tests/conftest/mol_1a30_clash_3.sdf
--rw-r--r--   0        0        0     5041 2023-11-21 22:22:52.714324 posebusters-0.2.8/tests/conftest/mol_1a30_ligand.mol2
--rw-r--r--   0        0        0     2604 2023-11-21 22:22:52.714324 posebusters-0.2.8/tests/conftest/mol_2bm2_ligand.sdf
--rw-r--r--   0        0        0   613807 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/conftest/mol_2bm2_protein_one_ligand_removed.pdb
--rw-r--r--   0        0        0     2652 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/conftest/mol_CGB.sdf
--rw-r--r--   0        0        0     2604 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/conftest/mol_PM2.sdf
--rw-r--r--   0        0        0     2163 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/conftest/mol_RQ3_x00.sdf
--rw-r--r--   0        0        0     2163 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/conftest/mol_RQ3_x01.sdf
--rw-r--r--   0        0        0     2163 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/conftest/mol_RQ3_x10.sdf
--rw-r--r--   0        0        0      160 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/conftest/mol_calcium.sdf
--rw-r--r--   0        0        0     6253 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/conftest/mol_cholesterol.sdf
--rw-r--r--   0        0        0      556 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/conftest/sample_bust_docks_table.csv
--rw-r--r--   0        0        0      178 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/conftest/sample_bust_mols_table.csv
--rw-r--r--   0        0        0      161 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/conftest/single_hydrogen.sdf
--rw-r--r--   0        0        0     1301 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/test_cli.py
--rw-r--r--   0        0        0      812 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/test_modules/test_distance_geometry.py
--rw-r--r--   0        0        0      597 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/test_modules/test_energy_ratio.py
--rw-r--r--   0        0        0     1405 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/test_modules/test_flatness.py
--rw-r--r--   0        0        0     2966 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/test_modules/test_identity.py
--rw-r--r--   0        0        0      675 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/test_modules/test_intermolecular_distance.py
--rw-r--r--   0        0        0     1924 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/test_modules/test_rmsd.py
--rw-r--r--   0        0        0     1191 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/test_modules/test_sanity.py
--rw-r--r--   0        0        0     2778 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/test_modules/test_volume_overlap.py
--rw-r--r--   0        0        0     2698 2023-11-21 22:22:52.718324 posebusters-0.2.8/tests/test_posebusters.py
--rw-r--r--   0        0        0     4159 1970-01-01 00:00:00.000000 posebusters-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      630 2023-12-08 20:39:23.353460 posebusters-0.2.9/.github/workflows/publishing.yml
+-rw-r--r--   0        0        0     2144 2023-12-08 20:39:23.353460 posebusters-0.2.9/.github/workflows/security.yml
+-rw-r--r--   0        0        0     1420 2023-12-08 20:39:23.353460 posebusters-0.2.9/.github/workflows/testing.yml
+-rw-r--r--   0        0        0      947 2023-12-08 20:39:23.353460 posebusters-0.2.9/.github/workflows/validation.yml
+-rw-r--r--   0        0        0     1886 2023-12-08 20:39:23.353460 posebusters-0.2.9/.gitignore
+-rw-r--r--   0        0        0     2541 2023-12-08 20:39:23.353460 posebusters-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     7606 2023-12-08 20:39:23.353460 posebusters-0.2.9/.vscode/launch.json
+-rw-r--r--   0        0        0     1099 2023-12-08 20:39:23.353460 posebusters-0.2.9/.vscode/settings.json
+-rw-r--r--   0        0        0     1527 2023-12-08 20:39:23.353460 posebusters-0.2.9/LICENSE
+-rw-r--r--   0        0        0     2441 2023-12-08 20:39:23.353460 posebusters-0.2.9/README.md
+-rw-r--r--   0        0        0      638 2023-12-08 20:39:23.353460 posebusters-0.2.9/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-12-08 20:39:23.353460 posebusters-0.2.9/docs/make.bat
+-rw-r--r--   0        0        0       98 2023-12-08 20:39:23.353460 posebusters-0.2.9/docs/requirements.txt
+-rw-r--r--   0        0        0    58908 2023-12-08 20:39:23.353460 posebusters-0.2.9/docs/source/_static/logo_banner.png
+-rwxr-xr-x   0        0        0    41654 2023-12-08 20:39:23.353460 posebusters-0.2.9/docs/source/_static/logo_square.png
+-rw-r--r--   0        0        0     1992 2023-12-08 20:39:23.353460 posebusters-0.2.9/docs/source/api.rst
+-rw-r--r--   0        0        0    46247 2023-12-08 20:39:23.353460 posebusters-0.2.9/docs/source/api_notebook.ipynb
+-rw-r--r--   0        0        0     8645 2023-12-08 20:39:23.353460 posebusters-0.2.9/docs/source/checks.rst
+-rw-r--r--   0        0        0     2868 2023-12-08 20:39:23.353460 posebusters-0.2.9/docs/source/cli.rst
+-rw-r--r--   0        0        0     3061 2023-12-08 20:39:23.353460 posebusters-0.2.9/docs/source/conf.py
+-rw-r--r--   0        0        0   122628 2023-12-08 20:39:23.357460 posebusters-0.2.9/docs/source/images/crystal_astex_1hww.png
+-rw-r--r--   0        0        0    94435 2023-12-08 20:39:23.357460 posebusters-0.2.9/docs/source/images/crystal_astex_1k3u.png
+-rw-r--r--   0        0        0    83738 2023-12-08 20:39:23.357460 posebusters-0.2.9/docs/source/images/crystal_astex_1s19.png
+-rw-r--r--   0        0        0    84467 2023-12-08 20:39:23.357460 posebusters-0.2.9/docs/source/images/crystal_astex_1s3v.png
+-rw-r--r--   0        0        0    92271 2023-12-08 20:39:23.357460 posebusters-0.2.9/docs/source/images/crystal_astex_1t9b.png
+-rw-r--r--   0        0        0   153904 2023-12-08 20:39:23.357460 posebusters-0.2.9/docs/source/images/crystal_astex_1tt1.png
+-rw-r--r--   0        0        0    67540 2023-12-08 20:39:23.357460 posebusters-0.2.9/docs/source/images/crystal_astex_1tz8.png
+-rw-r--r--   0        0        0   110315 2023-12-08 20:39:23.357460 posebusters-0.2.9/docs/source/images/crystal_fragalysis_NSP14-x1316.png
+-rw-r--r--   0        0        0   112813 2023-12-08 20:39:23.357460 posebusters-0.2.9/docs/source/images/deepdock_astex_1t9b.png
+-rw-r--r--   0        0        0    67522 2023-12-08 20:39:23.361460 posebusters-0.2.9/docs/source/images/diffdock_astex_1s19.png
+-rw-r--r--   0        0        0   136262 2023-12-08 20:39:23.361460 posebusters-0.2.9/docs/source/images/diffdock_astex_1tt1.png
+-rw-r--r--   0        0        0    67077 2023-12-08 20:39:23.361460 posebusters-0.2.9/docs/source/images/equibind_astex_1tz8.png
+-rw-r--r--   0        0        0    98366 2023-12-08 20:39:23.361460 posebusters-0.2.9/docs/source/images/tankbind_astex_1hww.png
+-rw-r--r--   0        0        0    92996 2023-12-08 20:39:23.361460 posebusters-0.2.9/docs/source/images/tankbind_astex_1s3v.png
+-rw-r--r--   0        0        0    74604 2023-12-08 20:39:23.361460 posebusters-0.2.9/docs/source/images/unimol_astex_1k3u.png
+-rw-r--r--   0        0        0    77966 2023-12-08 20:39:23.361460 posebusters-0.2.9/docs/source/images/unimol_fragalysis_NSP14-x1316.png
+-rw-r--r--   0        0        0     7107 2023-12-08 20:39:23.361460 posebusters-0.2.9/docs/source/index.rst
+-rw-r--r--   0        0        0     1678 2023-12-08 20:39:23.361460 posebusters-0.2.9/docs/source/inputs/1ia1/1ia1_ligand.sdf
+-rw-r--r--   0        0        0     3366 2023-12-08 20:39:23.361460 posebusters-0.2.9/docs/source/inputs/1ia1/1ia1_ligands.sdf
+-rw-r--r--   0        0        0   259057 2023-12-08 20:39:23.365460 posebusters-0.2.9/docs/source/inputs/1ia1/1ia1_protein_one_lig_removed.pdb
+-rw-r--r--   0        0        0     1154 2023-12-08 20:39:23.365460 posebusters-0.2.9/docs/source/inputs/1of6/1of6_ligand.sdf
+-rw-r--r--   0        0        0     9272 2023-12-08 20:39:23.365460 posebusters-0.2.9/docs/source/inputs/1of6/1of6_ligands.sdf
+-rw-r--r--   0        0        0  1652386 2023-12-08 20:39:23.373460 posebusters-0.2.9/docs/source/inputs/1of6/1of6_protein_one_lig_removed.pdb
+-rw-r--r--   0        0        0     2342 2023-12-08 20:39:23.373460 posebusters-0.2.9/docs/source/inputs/1s3v/1s3v_ligand.sdf
+-rw-r--r--   0        0        0     2347 2023-12-08 20:39:23.373460 posebusters-0.2.9/docs/source/inputs/1s3v/1s3v_ligands.sdf
+-rw-r--r--   0        0        0   118807 2023-12-08 20:39:23.373460 posebusters-0.2.9/docs/source/inputs/1s3v/1s3v_protein_one_lig_removed.pdb
+-rw-r--r--   0        0        0     1416 2023-12-08 20:39:23.373460 posebusters-0.2.9/docs/source/inputs/1uou/1uou_ligand.sdf
+-rw-r--r--   0        0        0     1421 2023-12-08 20:39:23.373460 posebusters-0.2.9/docs/source/inputs/1uou/1uou_ligands.sdf
+-rw-r--r--   0        0        0   253660 2023-12-08 20:39:23.373460 posebusters-0.2.9/docs/source/inputs/1uou/1uou_protein_one_lig_removed.pdb
+-rw-r--r--   0        0        0     1689 2023-12-08 20:39:23.373460 posebusters-0.2.9/docs/source/inputs/crystal_ligand.sdf
+-rw-r--r--   0        0        0     3388 2023-12-08 20:39:23.373460 posebusters-0.2.9/docs/source/inputs/generated_ligands.sdf
+-rw-r--r--   0        0        0     6717 2023-12-08 20:39:23.373460 posebusters-0.2.9/docs/source/inputs/generated_molecules.sdf
+-rw-r--r--   0        0        0      376 2023-12-08 20:39:23.373460 posebusters-0.2.9/docs/source/inputs/molecule_table.csv
+-rw-r--r--   0        0        0   252714 2023-12-08 20:39:23.373460 posebusters-0.2.9/docs/source/inputs/protein.pdb
+-rw-r--r--   0        0        0     1690 2023-12-08 20:39:23.373460 posebusters-0.2.9/docs/source/inputs/redocked_ligand.sdf
+-rw-r--r--   0        0        0      946 2023-12-08 20:39:23.373460 posebusters-0.2.9/posebusters/__init__.py
+-rw-r--r--   0        0        0      183 2023-12-08 20:39:23.373460 posebusters-0.2.9/posebusters/__main__.py
+-rw-r--r--   0        0        0     6312 2023-12-08 20:39:23.373460 posebusters-0.2.9/posebusters/cli.py
+-rw-r--r--   0        0        0     7204 2023-12-08 20:39:23.373460 posebusters-0.2.9/posebusters/config/dock.yml
+-rw-r--r--   0        0        0     3350 2023-12-08 20:39:23.373460 posebusters-0.2.9/posebusters/config/mol.yml
+-rw-r--r--   0        0        0     8015 2023-12-08 20:39:23.373460 posebusters-0.2.9/posebusters/config/redock.yml
+-rw-r--r--   0        0        0      147 2023-12-08 20:39:23.373460 posebusters-0.2.9/posebusters/datasets/__init__.py
+-rw-r--r--   0        0        0      688 2023-12-08 20:39:23.373460 posebusters-0.2.9/posebusters/datasets/load_datasets.py
+-rw-r--r--   0        0        0      424 2023-12-08 20:39:23.373460 posebusters-0.2.9/posebusters/datasets/pdb.csv
+-rw-r--r--   0        0        0     1678 2023-12-08 20:39:23.373460 posebusters-0.2.9/posebusters/datasets/pdb/1ia1/1ia1_ligand.sdf
+-rw-r--r--   0        0        0     3366 2023-12-08 20:39:23.373460 posebusters-0.2.9/posebusters/datasets/pdb/1ia1/1ia1_ligands.sdf
+-rw-r--r--   0        0        0   265544 2023-12-08 20:39:23.373460 posebusters-0.2.9/posebusters/datasets/pdb/1ia1/1ia1_protein_one_lig_removed.pdb
+-rw-r--r--   0        0        0     1154 2023-12-08 20:39:23.373460 posebusters-0.2.9/posebusters/datasets/pdb/1of6/1of6_ligand.sdf
+-rw-r--r--   0        0        0     9272 2023-12-08 20:39:23.373460 posebusters-0.2.9/posebusters/datasets/pdb/1of6/1of6_ligands.sdf
+-rw-r--r--   0        0        0  1694211 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/datasets/pdb/1of6/1of6_protein_one_lig_removed.pdb
+-rw-r--r--   0        0        0     2342 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/datasets/pdb/1s3v/1s3v_ligand.sdf
+-rw-r--r--   0        0        0     2347 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/datasets/pdb/1s3v/1s3v_ligands.sdf
+-rw-r--r--   0        0        0   121812 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/datasets/pdb/1s3v/1s3v_protein_one_lig_removed.pdb
+-rw-r--r--   0        0        0     1416 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/datasets/pdb/1uou/1uou_ligand.sdf
+-rw-r--r--   0        0        0     1421 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/datasets/pdb/1uou/1uou_ligands.sdf
+-rw-r--r--   0        0        0   260079 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/datasets/pdb/1uou/1uou_protein_one_lig_removed.pdb
+-rw-r--r--   0        0        0       45 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/modules/__init__.py
+-rw-r--r--   0        0        0     9830 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/modules/distance_geometry.py
+-rw-r--r--   0        0        0     5243 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/modules/energy_ratio.py
+-rw-r--r--   0        0        0     3187 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/modules/flatness.py
+-rw-r--r--   0        0        0     6044 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/modules/identity.py
+-rw-r--r--   0        0        0     5177 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/modules/intermolecular_distance.py
+-rw-r--r--   0        0        0      792 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/modules/loading.py
+-rw-r--r--   0        0        0     6830 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/modules/rmsd.py
+-rw-r--r--   0        0        0     1294 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/modules/sanity.py
+-rw-r--r--   0        0        0     2713 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/modules/volume_overlap.py
+-rw-r--r--   0        0        0     9135 2023-12-08 20:39:23.377460 posebusters-0.2.9/posebusters/posebusters.py
+-rw-r--r--   0        0        0       58 2023-12-08 20:39:23.381460 posebusters-0.2.9/posebusters/tools/__init__.py
+-rw-r--r--   0        0        0     1426 2023-12-08 20:39:23.381460 posebusters-0.2.9/posebusters/tools/formatting.py
+-rw-r--r--   0        0        0     6123 2023-12-08 20:39:23.381460 posebusters-0.2.9/posebusters/tools/loading.py
+-rw-r--r--   0        0        0     1165 2023-12-08 20:39:23.381460 posebusters-0.2.9/posebusters/tools/logging.py
+-rw-r--r--   0        0        0     6993 2023-12-08 20:39:23.381460 posebusters-0.2.9/posebusters/tools/molecules.py
+-rw-r--r--   0        0        0      516 2023-12-08 20:39:23.381460 posebusters-0.2.9/posebusters/tools/parallel.py
+-rw-r--r--   0        0        0     2367 2023-12-08 20:39:23.381460 posebusters-0.2.9/posebusters/tools/protein.py
+-rw-r--r--   0        0        0     1122 2023-12-08 20:39:23.381460 posebusters-0.2.9/posebusters/tools/stats.py
+-rw-r--r--   0        0        0     2229 2023-12-08 20:39:23.381460 posebusters-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-08 20:39:23.381460 posebusters-0.2.9/tests/__init__.py
+-rw-r--r--   0        0        0     4724 2023-12-08 20:39:23.381460 posebusters-0.2.9/tests/conftest.py
+-rw-r--r--   0        0        0   705759 2023-12-08 20:39:23.381460 posebusters-0.2.9/tests/conftest/1G9V_RQ3/1G9V_RQ3_gold_redock.sdf
+-rw-r--r--   0        0        0     2179 2023-12-08 20:39:23.381460 posebusters-0.2.9/tests/conftest/1G9V_RQ3/1G9V_RQ3_ligand.sdf
+-rw-r--r--   0        0        0     4069 2023-12-08 20:39:23.381460 posebusters-0.2.9/tests/conftest/1G9V_RQ3/1G9V_RQ3_ligand_start_conf.sdf
+-rw-r--r--   0        0        0     4358 2023-12-08 20:39:23.381460 posebusters-0.2.9/tests/conftest/1G9V_RQ3/1G9V_RQ3_ligands.sdf
+-rw-r--r--   0        0        0   374213 2023-12-08 20:39:23.385460 posebusters-0.2.9/tests/conftest/1G9V_RQ3/1G9V_RQ3_protein.pdb
+-rw-r--r--   0        0        0     1694 2023-12-08 20:39:23.385460 posebusters-0.2.9/tests/conftest/1IA1_TQ3/1IA1_TQ3_ligand.sdf
+-rw-r--r--   0        0        0     2671 2023-12-08 20:39:23.385460 posebusters-0.2.9/tests/conftest/1IA1_TQ3/1IA1_TQ3_ligand_start_conf.sdf
+-rw-r--r--   0        0        0     3388 2023-12-08 20:39:23.385460 posebusters-0.2.9/tests/conftest/1IA1_TQ3/1IA1_TQ3_ligands.sdf
+-rw-r--r--   0        0        0   269862 2023-12-08 20:39:23.385460 posebusters-0.2.9/tests/conftest/1IA1_TQ3/1IA1_TQ3_no_ligand_no_solvent.pdb
+-rw-r--r--   0        0        0   268852 2023-12-08 20:39:23.385460 posebusters-0.2.9/tests/conftest/1IA1_TQ3/1IA1_TQ3_no_ligand_no_solvent_no_inorganic.pdb
+-rw-r--r--   0        0        0   258884 2023-12-08 20:39:23.385460 posebusters-0.2.9/tests/conftest/1IA1_TQ3/1IA1_TQ3_no_ligand_no_solvent_no_inorganic_no_cofactors.pdb
+-rw-r--r--   0        0        0     1342 2023-12-08 20:39:23.385460 posebusters-0.2.9/tests/conftest/1MMV_3AR/1MMV_3AR_crystal.sdf
+-rw-r--r--   0        0        0     1327 2023-12-08 20:39:23.385460 posebusters-0.2.9/tests/conftest/1MMV_3AR/1MMV_3AR_tankbind.sdf
+-rw-r--r--   0        0        0     1171 2023-12-08 20:39:23.385460 posebusters-0.2.9/tests/conftest/1OF6_DTY/1OF6_DTY_crystal.sdf
+-rw-r--r--   0        0        0    28966 2023-12-08 20:39:23.385460 posebusters-0.2.9/tests/conftest/1OF6_DTY/1OF6_DTY_vina.sdf
+-rw-r--r--   0        0        0     1795 2023-12-08 20:39:23.385460 posebusters-0.2.9/tests/conftest/1Q1G_MTI/1Q1G_MTI_crystal.sdf
+-rw-r--r--   0        0        0     1781 2023-12-08 20:39:23.385460 posebusters-0.2.9/tests/conftest/1Q1G_MTI/1Q1G_MTI_tankbind.sdf
+-rw-r--r--   0        0        0     1018 2023-12-08 20:39:23.385460 posebusters-0.2.9/tests/conftest/1W1P_GIO/1W1P_GIO_ligand.sdf
+-rw-r--r--   0        0        0     1828 2023-12-08 20:39:23.385460 posebusters-0.2.9/tests/conftest/1W1P_GIO/1W1P_GIO_ligand_start_conf.sdf
+-rw-r--r--   0        0        0     2036 2023-12-08 20:39:23.385460 posebusters-0.2.9/tests/conftest/1W1P_GIO/1W1P_GIO_ligands.sdf
+-rw-r--r--   0        0        0   650319 2023-12-08 20:39:23.389460 posebusters-0.2.9/tests/conftest/1W1P_GIO/1W1P_GIO_protein.pdb
+-rw-r--r--   0        0        0     1678 2023-12-08 20:39:23.389460 posebusters-0.2.9/tests/conftest/1ia1/1ia1_ligand.sdf
+-rw-r--r--   0        0        0     3366 2023-12-08 20:39:23.389460 posebusters-0.2.9/tests/conftest/1ia1/1ia1_ligands.sdf
+-rw-r--r--   0        0        0   265544 2023-12-08 20:39:23.389460 posebusters-0.2.9/tests/conftest/1ia1/1ia1_protein_one_lig_removed.pdb
+-rw-r--r--   0        0        0     1154 2023-12-08 20:39:23.389460 posebusters-0.2.9/tests/conftest/1of6/1of6_ligand.sdf
+-rw-r--r--   0        0        0     9272 2023-12-08 20:39:23.389460 posebusters-0.2.9/tests/conftest/1of6/1of6_ligands.sdf
+-rw-r--r--   0        0        0  1694211 2023-12-08 20:39:23.389460 posebusters-0.2.9/tests/conftest/1of6/1of6_protein_one_lig_removed.pdb
+-rw-r--r--   0        0        0     2342 2023-12-08 20:39:23.389460 posebusters-0.2.9/tests/conftest/1s3v/1s3v_ligand.sdf
+-rw-r--r--   0        0        0     2347 2023-12-08 20:39:23.389460 posebusters-0.2.9/tests/conftest/1s3v/1s3v_ligands.sdf
+-rw-r--r--   0        0        0   121812 2023-12-08 20:39:23.393460 posebusters-0.2.9/tests/conftest/1s3v/1s3v_protein_one_lig_removed.pdb
+-rw-r--r--   0        0        0     1416 2023-12-08 20:39:23.393460 posebusters-0.2.9/tests/conftest/1uou/1uou_ligand.sdf
+-rw-r--r--   0        0        0     1421 2023-12-08 20:39:23.393460 posebusters-0.2.9/tests/conftest/1uou/1uou_ligands.sdf
+-rw-r--r--   0        0        0   260079 2023-12-08 20:39:23.393460 posebusters-0.2.9/tests/conftest/1uou/1uou_protein_one_lig_removed.pdb
+-rw-r--r--   0        0        0     3645 2023-12-08 20:39:23.393460 posebusters-0.2.9/tests/conftest/6YR2_T1C/6YR2_T1C_crystal.sdf
+-rw-r--r--   0        0        0     3628 2023-12-08 20:39:23.393460 posebusters-0.2.9/tests/conftest/6YR2_T1C/6YR2_T1C_tankbind.sdf
+-rw-r--r--   0        0        0      838 2023-12-08 20:39:23.393460 posebusters-0.2.9/tests/conftest/7CNQ_G8X/7CNQ_G8X_ligand.sdf
+-rw-r--r--   0        0        0  1329827 2023-12-08 20:39:23.397460 posebusters-0.2.9/tests/conftest/7CNQ_G8X/7CNQ_G8X_protein.pdb
+-rw-r--r--   0        0        0      742 2023-12-08 20:39:23.397460 posebusters-0.2.9/tests/conftest/7ECR_SIN/7ECR_SIN_ligand.sdf
+-rw-r--r--   0        0        0   867187 2023-12-08 20:39:23.401460 posebusters-0.2.9/tests/conftest/7ECR_SIN/7ECR_SIN_protein.pdb
+-rw-r--r--   0        0        0      991 2023-12-08 20:39:23.401460 posebusters-0.2.9/tests/conftest/7ZTL_BCN/7ZTL_BCN_ligand.sdf
+-rw-r--r--   0        0        0      991 2023-12-08 20:39:23.401460 posebusters-0.2.9/tests/conftest/7ZTL_BCN/7ZTL_BCN_ligands.sdf
+-rw-r--r--   0        0        0   189935 2023-12-08 20:39:23.401460 posebusters-0.2.9/tests/conftest/7ZTL_BCN/7ZTL_BCN_protein.pdb
+-rw-r--r--   0        0        0     2270 2023-12-08 20:39:23.401460 posebusters-0.2.9/tests/conftest/mol_1a30_clash_2.sdf
+-rw-r--r--   0        0        0     2270 2023-12-08 20:39:23.401460 posebusters-0.2.9/tests/conftest/mol_1a30_clash_3.sdf
+-rw-r--r--   0        0        0     5041 2023-12-08 20:39:23.401460 posebusters-0.2.9/tests/conftest/mol_1a30_ligand.mol2
+-rw-r--r--   0        0        0     2604 2023-12-08 20:39:23.401460 posebusters-0.2.9/tests/conftest/mol_2bm2_ligand.sdf
+-rw-r--r--   0        0        0   613807 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/conftest/mol_2bm2_protein_one_ligand_removed.pdb
+-rw-r--r--   0        0        0     2652 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/conftest/mol_CGB.sdf
+-rw-r--r--   0        0        0     2604 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/conftest/mol_PM2.sdf
+-rw-r--r--   0        0        0     2163 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/conftest/mol_RQ3_x00.sdf
+-rw-r--r--   0        0        0     2163 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/conftest/mol_RQ3_x01.sdf
+-rw-r--r--   0        0        0     2163 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/conftest/mol_RQ3_x10.sdf
+-rw-r--r--   0        0        0      160 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/conftest/mol_calcium.sdf
+-rw-r--r--   0        0        0     6253 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/conftest/mol_cholesterol.sdf
+-rw-r--r--   0        0        0      556 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/conftest/sample_bust_docks_table.csv
+-rw-r--r--   0        0        0      178 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/conftest/sample_bust_mols_table.csv
+-rw-r--r--   0        0        0      161 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/conftest/single_hydrogen.sdf
+-rw-r--r--   0        0        0     1488 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/test_cli.py
+-rw-r--r--   0        0        0      812 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/test_modules/test_distance_geometry.py
+-rw-r--r--   0        0        0      597 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/test_modules/test_energy_ratio.py
+-rw-r--r--   0        0        0     1405 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/test_modules/test_flatness.py
+-rw-r--r--   0        0        0     2966 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/test_modules/test_identity.py
+-rw-r--r--   0        0        0      675 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/test_modules/test_intermolecular_distance.py
+-rw-r--r--   0        0        0     1924 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/test_modules/test_rmsd.py
+-rw-r--r--   0        0        0     1191 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/test_modules/test_sanity.py
+-rw-r--r--   0        0        0     2778 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/test_modules/test_volume_overlap.py
+-rw-r--r--   0        0        0     2698 2023-12-08 20:39:23.405460 posebusters-0.2.9/tests/test_posebusters.py
+-rw-r--r--   0        0        0     4159 1970-01-01 00:00:00.000000 posebusters-0.2.9/PKG-INFO
```

### Comparing `posebusters-0.2.8/.github/workflows/publishing.yml` & `posebusters-0.2.9/.github/workflows/publishing.yml`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/.github/workflows/security.yml` & `posebusters-0.2.9/.github/workflows/security.yml`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/.github/workflows/testing.yml` & `posebusters-0.2.9/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/.github/workflows/validation.yml` & `posebusters-0.2.9/.github/workflows/validation.yml`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/.gitignore` & `posebusters-0.2.9/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Project specific
 data
 temp
 ignore*
 notebooks*
+.test*
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `posebusters-0.2.8/.pre-commit-config.yaml` & `posebusters-0.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/.vscode/launch.json` & `posebusters-0.2.9/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/.vscode/settings.json` & `posebusters-0.2.9/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/LICENSE` & `posebusters-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/README.md` & `posebusters-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/Makefile` & `posebusters-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/make.bat` & `posebusters-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/_static/logo_banner.png` & `posebusters-0.2.9/docs/source/_static/logo_banner.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/_static/logo_square.png` & `posebusters-0.2.9/docs/source/_static/logo_square.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/api.rst` & `posebusters-0.2.9/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/api_notebook.ipynb` & `posebusters-0.2.9/docs/source/api_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/checks.rst` & `posebusters-0.2.9/docs/source/checks.rst`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/cli.rst` & `posebusters-0.2.9/docs/source/cli.rst`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/conf.py` & `posebusters-0.2.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/images/crystal_astex_1hww.png` & `posebusters-0.2.9/docs/source/images/crystal_astex_1hww.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/images/crystal_astex_1k3u.png` & `posebusters-0.2.9/docs/source/images/crystal_astex_1k3u.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/images/crystal_astex_1s19.png` & `posebusters-0.2.9/docs/source/images/crystal_astex_1s19.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/images/crystal_astex_1s3v.png` & `posebusters-0.2.9/docs/source/images/crystal_astex_1s3v.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/images/crystal_astex_1t9b.png` & `posebusters-0.2.9/docs/source/images/crystal_astex_1t9b.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/images/crystal_astex_1tt1.png` & `posebusters-0.2.9/docs/source/images/crystal_astex_1tt1.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/images/crystal_astex_1tz8.png` & `posebusters-0.2.9/docs/source/images/crystal_astex_1tz8.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/images/crystal_fragalysis_NSP14-x1316.png` & `posebusters-0.2.9/docs/source/images/crystal_fragalysis_NSP14-x1316.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/images/deepdock_astex_1t9b.png` & `posebusters-0.2.9/docs/source/images/deepdock_astex_1t9b.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/images/diffdock_astex_1s19.png` & `posebusters-0.2.9/docs/source/images/diffdock_astex_1s19.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/images/diffdock_astex_1tt1.png` & `posebusters-0.2.9/docs/source/images/diffdock_astex_1tt1.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/images/equibind_astex_1tz8.png` & `posebusters-0.2.9/docs/source/images/equibind_astex_1tz8.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/images/tankbind_astex_1hww.png` & `posebusters-0.2.9/docs/source/images/tankbind_astex_1hww.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/images/tankbind_astex_1s3v.png` & `posebusters-0.2.9/docs/source/images/tankbind_astex_1s3v.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/images/unimol_astex_1k3u.png` & `posebusters-0.2.9/docs/source/images/unimol_astex_1k3u.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/images/unimol_fragalysis_NSP14-x1316.png` & `posebusters-0.2.9/docs/source/images/unimol_fragalysis_NSP14-x1316.png`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/index.rst` & `posebusters-0.2.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/1ia1/1ia1_ligand.sdf` & `posebusters-0.2.9/docs/source/inputs/1ia1/1ia1_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/1ia1/1ia1_ligands.sdf` & `posebusters-0.2.9/docs/source/inputs/1ia1/1ia1_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/1ia1/1ia1_protein_one_lig_removed.pdb` & `posebusters-0.2.9/docs/source/inputs/1ia1/1ia1_protein_one_lig_removed.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/1of6/1of6_ligand.sdf` & `posebusters-0.2.9/docs/source/inputs/1of6/1of6_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/1of6/1of6_ligands.sdf` & `posebusters-0.2.9/docs/source/inputs/1of6/1of6_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/1of6/1of6_protein_one_lig_removed.pdb` & `posebusters-0.2.9/docs/source/inputs/1of6/1of6_protein_one_lig_removed.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/1s3v/1s3v_ligand.sdf` & `posebusters-0.2.9/docs/source/inputs/1s3v/1s3v_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/1s3v/1s3v_ligands.sdf` & `posebusters-0.2.9/docs/source/inputs/1s3v/1s3v_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/1s3v/1s3v_protein_one_lig_removed.pdb` & `posebusters-0.2.9/docs/source/inputs/1s3v/1s3v_protein_one_lig_removed.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/1uou/1uou_ligand.sdf` & `posebusters-0.2.9/docs/source/inputs/1uou/1uou_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/1uou/1uou_ligands.sdf` & `posebusters-0.2.9/docs/source/inputs/1uou/1uou_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/1uou/1uou_protein_one_lig_removed.pdb` & `posebusters-0.2.9/docs/source/inputs/1uou/1uou_protein_one_lig_removed.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/crystal_ligand.sdf` & `posebusters-0.2.9/docs/source/inputs/crystal_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/generated_ligands.sdf` & `posebusters-0.2.9/docs/source/inputs/generated_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/generated_molecules.sdf` & `posebusters-0.2.9/docs/source/inputs/generated_molecules.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/protein.pdb` & `posebusters-0.2.9/docs/source/inputs/protein.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/docs/source/inputs/redocked_ligand.sdf` & `posebusters-0.2.9/docs/source/inputs/redocked_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/__init__.py` & `posebusters-0.2.9/posebusters/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     "check_identity",
     "check_intermolecular_distance",
     "check_loading",
     "check_rmsd",
     "check_volume_overlap",
 ]
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
```

### Comparing `posebusters-0.2.8/posebusters/cli.py` & `posebusters-0.2.9/posebusters/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Command line interface for PoseBusters."""
 from __future__ import annotations
 
 import argparse
 import logging
 import sys
 from pathlib import Path
-from typing import Any, Iterable
+from typing import Any, Iterable, TextIO
 
 import pandas as pd
 from rdkit.Chem.rdchem import Mol
 from yaml import safe_load
 
 from . import __version__
 from .posebusters import PoseBusters, _dataframe_from_output
@@ -29,15 +29,15 @@
 
 def bust(
     mol_pred: list[Path | Mol] = [],
     mol_true: Path | Mol | None = None,
     mol_cond: Path | Mol | None = None,
     table: Path | None = None,
     outfmt: str = "short",
-    output=sys.stdout,
+    output: Path | TextIO = sys.stdout,
     config: Path | None = None,
     no_header: bool = False,
     full_report: bool = False,
     top_n: int | None = None,
 ):
     """PoseBusters: Plausibility checks for generated molecule poses."""
     if table is None and len(mol_pred) == 0:
@@ -55,14 +55,17 @@
         d = {k for k, v in dict(mol_pred=mol_pred, mol_true=mol_true, mol_cond=mol_cond).items() if v}
         mode = _select_mode(config, d)
         posebusters = PoseBusters(mode, top_n=top_n)
         cols = ["mol_pred", "mol_true", "mol_cond"]
         posebusters.file_paths = pd.DataFrame([[mol_pred, mol_true, mol_cond] for mol_pred in mol_pred], columns=cols)
         posebusters_results = posebusters._run()
 
+    if isinstance(output, Path):
+        output = open(Path(output), "w", encoding="utf-8")
+
     for i, results_dict in enumerate(posebusters_results):
         results = _dataframe_from_output(results_dict, posebusters.config, full_report)
         output.write(_format_results(results, outfmt, no_header, i))
 
 
 def _parse_args(args):
     desc = "PoseBusters: Plausibility checks for generated molecule poses."
```

### Comparing `posebusters-0.2.8/posebusters/config/dock.yml` & `posebusters-0.2.9/posebusters/config/dock.yml`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/config/mol.yml` & `posebusters-0.2.9/posebusters/config/mol.yml`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/config/redock.yml` & `posebusters-0.2.9/posebusters/config/redock.yml`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/datasets/load_datasets.py` & `posebusters-0.2.9/posebusters/datasets/load_datasets.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/datasets/pdb/1ia1/1ia1_ligand.sdf` & `posebusters-0.2.9/posebusters/datasets/pdb/1ia1/1ia1_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/datasets/pdb/1ia1/1ia1_ligands.sdf` & `posebusters-0.2.9/posebusters/datasets/pdb/1ia1/1ia1_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/datasets/pdb/1ia1/1ia1_protein_one_lig_removed.pdb` & `posebusters-0.2.9/posebusters/datasets/pdb/1ia1/1ia1_protein_one_lig_removed.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/datasets/pdb/1of6/1of6_ligand.sdf` & `posebusters-0.2.9/posebusters/datasets/pdb/1of6/1of6_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/datasets/pdb/1of6/1of6_ligands.sdf` & `posebusters-0.2.9/posebusters/datasets/pdb/1of6/1of6_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/datasets/pdb/1of6/1of6_protein_one_lig_removed.pdb` & `posebusters-0.2.9/posebusters/datasets/pdb/1of6/1of6_protein_one_lig_removed.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/datasets/pdb/1s3v/1s3v_ligand.sdf` & `posebusters-0.2.9/posebusters/datasets/pdb/1s3v/1s3v_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/datasets/pdb/1s3v/1s3v_ligands.sdf` & `posebusters-0.2.9/posebusters/datasets/pdb/1s3v/1s3v_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/datasets/pdb/1s3v/1s3v_protein_one_lig_removed.pdb` & `posebusters-0.2.9/posebusters/datasets/pdb/1s3v/1s3v_protein_one_lig_removed.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/datasets/pdb/1uou/1uou_ligand.sdf` & `posebusters-0.2.9/posebusters/datasets/pdb/1uou/1uou_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/datasets/pdb/1uou/1uou_ligands.sdf` & `posebusters-0.2.9/posebusters/datasets/pdb/1uou/1uou_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/datasets/pdb/1uou/1uou_protein_one_lig_removed.pdb` & `posebusters-0.2.9/posebusters/datasets/pdb/1uou/1uou_protein_one_lig_removed.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/modules/distance_geometry.py` & `posebusters-0.2.9/posebusters/modules/distance_geometry.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/modules/energy_ratio.py` & `posebusters-0.2.9/posebusters/modules/energy_ratio.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/modules/flatness.py` & `posebusters-0.2.9/posebusters/modules/flatness.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/modules/identity.py` & `posebusters-0.2.9/posebusters/modules/identity.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/modules/intermolecular_distance.py` & `posebusters-0.2.9/posebusters/modules/intermolecular_distance.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/modules/loading.py` & `posebusters-0.2.9/posebusters/modules/loading.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/modules/rmsd.py` & `posebusters-0.2.9/posebusters/modules/rmsd.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/modules/sanity.py` & `posebusters-0.2.9/posebusters/modules/sanity.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/modules/volume_overlap.py` & `posebusters-0.2.9/posebusters/modules/volume_overlap.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/posebusters.py` & `posebusters-0.2.9/posebusters/posebusters.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/tools/formatting.py` & `posebusters-0.2.9/posebusters/tools/formatting.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/tools/loading.py` & `posebusters-0.2.9/posebusters/tools/loading.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/tools/logging.py` & `posebusters-0.2.9/posebusters/tools/logging.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/tools/molecules.py` & `posebusters-0.2.9/posebusters/tools/molecules.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/tools/parallel.py` & `posebusters-0.2.9/posebusters/tools/parallel.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/tools/protein.py` & `posebusters-0.2.9/posebusters/tools/protein.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/posebusters/tools/stats.py` & `posebusters-0.2.9/posebusters/tools/stats.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/pyproject.toml` & `posebusters-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest.py` & `posebusters-0.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1G9V_RQ3/1G9V_RQ3_gold_redock.sdf` & `posebusters-0.2.9/tests/conftest/1G9V_RQ3/1G9V_RQ3_gold_redock.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1G9V_RQ3/1G9V_RQ3_ligand.sdf` & `posebusters-0.2.9/tests/conftest/1G9V_RQ3/1G9V_RQ3_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1G9V_RQ3/1G9V_RQ3_ligand_start_conf.sdf` & `posebusters-0.2.9/tests/conftest/1G9V_RQ3/1G9V_RQ3_ligand_start_conf.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1G9V_RQ3/1G9V_RQ3_ligands.sdf` & `posebusters-0.2.9/tests/conftest/1G9V_RQ3/1G9V_RQ3_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1G9V_RQ3/1G9V_RQ3_protein.pdb` & `posebusters-0.2.9/tests/conftest/1G9V_RQ3/1G9V_RQ3_protein.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1IA1_TQ3/1IA1_TQ3_ligand.sdf` & `posebusters-0.2.9/tests/conftest/1IA1_TQ3/1IA1_TQ3_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1IA1_TQ3/1IA1_TQ3_ligand_start_conf.sdf` & `posebusters-0.2.9/tests/conftest/1IA1_TQ3/1IA1_TQ3_ligand_start_conf.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1IA1_TQ3/1IA1_TQ3_ligands.sdf` & `posebusters-0.2.9/tests/conftest/1IA1_TQ3/1IA1_TQ3_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1IA1_TQ3/1IA1_TQ3_no_ligand_no_solvent.pdb` & `posebusters-0.2.9/tests/conftest/1IA1_TQ3/1IA1_TQ3_no_ligand_no_solvent.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1IA1_TQ3/1IA1_TQ3_no_ligand_no_solvent_no_inorganic.pdb` & `posebusters-0.2.9/tests/conftest/1IA1_TQ3/1IA1_TQ3_no_ligand_no_solvent_no_inorganic.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1IA1_TQ3/1IA1_TQ3_no_ligand_no_solvent_no_inorganic_no_cofactors.pdb` & `posebusters-0.2.9/tests/conftest/1IA1_TQ3/1IA1_TQ3_no_ligand_no_solvent_no_inorganic_no_cofactors.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1MMV_3AR/1MMV_3AR_crystal.sdf` & `posebusters-0.2.9/tests/conftest/1MMV_3AR/1MMV_3AR_crystal.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1MMV_3AR/1MMV_3AR_tankbind.sdf` & `posebusters-0.2.9/tests/conftest/1MMV_3AR/1MMV_3AR_tankbind.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1OF6_DTY/1OF6_DTY_crystal.sdf` & `posebusters-0.2.9/tests/conftest/1OF6_DTY/1OF6_DTY_crystal.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1OF6_DTY/1OF6_DTY_vina.sdf` & `posebusters-0.2.9/tests/conftest/1OF6_DTY/1OF6_DTY_vina.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1Q1G_MTI/1Q1G_MTI_crystal.sdf` & `posebusters-0.2.9/tests/conftest/1Q1G_MTI/1Q1G_MTI_crystal.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1Q1G_MTI/1Q1G_MTI_tankbind.sdf` & `posebusters-0.2.9/tests/conftest/1Q1G_MTI/1Q1G_MTI_tankbind.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1W1P_GIO/1W1P_GIO_ligand.sdf` & `posebusters-0.2.9/tests/conftest/1W1P_GIO/1W1P_GIO_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1W1P_GIO/1W1P_GIO_ligand_start_conf.sdf` & `posebusters-0.2.9/tests/conftest/1W1P_GIO/1W1P_GIO_ligand_start_conf.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1W1P_GIO/1W1P_GIO_ligands.sdf` & `posebusters-0.2.9/tests/conftest/1W1P_GIO/1W1P_GIO_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1W1P_GIO/1W1P_GIO_protein.pdb` & `posebusters-0.2.9/tests/conftest/1W1P_GIO/1W1P_GIO_protein.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1ia1/1ia1_ligand.sdf` & `posebusters-0.2.9/tests/conftest/1ia1/1ia1_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1ia1/1ia1_ligands.sdf` & `posebusters-0.2.9/tests/conftest/1ia1/1ia1_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1ia1/1ia1_protein_one_lig_removed.pdb` & `posebusters-0.2.9/tests/conftest/1ia1/1ia1_protein_one_lig_removed.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1of6/1of6_ligand.sdf` & `posebusters-0.2.9/tests/conftest/1of6/1of6_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1of6/1of6_ligands.sdf` & `posebusters-0.2.9/tests/conftest/1of6/1of6_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1of6/1of6_protein_one_lig_removed.pdb` & `posebusters-0.2.9/tests/conftest/1of6/1of6_protein_one_lig_removed.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1s3v/1s3v_ligand.sdf` & `posebusters-0.2.9/tests/conftest/1s3v/1s3v_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1s3v/1s3v_ligands.sdf` & `posebusters-0.2.9/tests/conftest/1s3v/1s3v_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1s3v/1s3v_protein_one_lig_removed.pdb` & `posebusters-0.2.9/tests/conftest/1s3v/1s3v_protein_one_lig_removed.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1uou/1uou_ligand.sdf` & `posebusters-0.2.9/tests/conftest/1uou/1uou_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1uou/1uou_ligands.sdf` & `posebusters-0.2.9/tests/conftest/1uou/1uou_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/1uou/1uou_protein_one_lig_removed.pdb` & `posebusters-0.2.9/tests/conftest/1uou/1uou_protein_one_lig_removed.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/6YR2_T1C/6YR2_T1C_crystal.sdf` & `posebusters-0.2.9/tests/conftest/6YR2_T1C/6YR2_T1C_crystal.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/6YR2_T1C/6YR2_T1C_tankbind.sdf` & `posebusters-0.2.9/tests/conftest/6YR2_T1C/6YR2_T1C_tankbind.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/7CNQ_G8X/7CNQ_G8X_ligand.sdf` & `posebusters-0.2.9/tests/conftest/7CNQ_G8X/7CNQ_G8X_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/7CNQ_G8X/7CNQ_G8X_protein.pdb` & `posebusters-0.2.9/tests/conftest/7CNQ_G8X/7CNQ_G8X_protein.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/7ECR_SIN/7ECR_SIN_ligand.sdf` & `posebusters-0.2.9/tests/conftest/7ECR_SIN/7ECR_SIN_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/7ECR_SIN/7ECR_SIN_protein.pdb` & `posebusters-0.2.9/tests/conftest/7ECR_SIN/7ECR_SIN_protein.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/7ZTL_BCN/7ZTL_BCN_ligand.sdf` & `posebusters-0.2.9/tests/conftest/7ZTL_BCN/7ZTL_BCN_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/7ZTL_BCN/7ZTL_BCN_ligands.sdf` & `posebusters-0.2.9/tests/conftest/7ZTL_BCN/7ZTL_BCN_ligands.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/7ZTL_BCN/7ZTL_BCN_protein.pdb` & `posebusters-0.2.9/tests/conftest/7ZTL_BCN/7ZTL_BCN_protein.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/mol_1a30_clash_2.sdf` & `posebusters-0.2.9/tests/conftest/mol_1a30_clash_2.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/mol_1a30_clash_3.sdf` & `posebusters-0.2.9/tests/conftest/mol_1a30_clash_3.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/mol_1a30_ligand.mol2` & `posebusters-0.2.9/tests/conftest/mol_1a30_ligand.mol2`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/mol_2bm2_ligand.sdf` & `posebusters-0.2.9/tests/conftest/mol_2bm2_ligand.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/mol_2bm2_protein_one_ligand_removed.pdb` & `posebusters-0.2.9/tests/conftest/mol_2bm2_protein_one_ligand_removed.pdb`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/mol_CGB.sdf` & `posebusters-0.2.9/tests/conftest/mol_CGB.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/mol_PM2.sdf` & `posebusters-0.2.9/tests/conftest/mol_PM2.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/mol_RQ3_x00.sdf` & `posebusters-0.2.9/tests/conftest/mol_RQ3_x00.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/mol_RQ3_x01.sdf` & `posebusters-0.2.9/tests/conftest/mol_RQ3_x01.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/mol_RQ3_x10.sdf` & `posebusters-0.2.9/tests/conftest/mol_RQ3_x10.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/mol_cholesterol.sdf` & `posebusters-0.2.9/tests/conftest/mol_cholesterol.sdf`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/conftest/sample_bust_docks_table.csv` & `posebusters-0.2.9/tests/conftest/sample_bust_docks_table.csv`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/test_cli.py` & `posebusters-0.2.9/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,24 @@
     bust([Path(mol_pred_1ia1)], Path(mol_true_1ia1), Path(mol_cond_1ia1))
 
 
 def test_bust_table() -> None:
     bust(table=Path(mols_table))
 
 
+def test_output() -> None:
+    output = Path(".test_output.csv")
+    bust(
+        table=Path(mols_table),
+        outfmt="csv",
+        output=output,
+    )
+    assert output.exists()
+
+
 def test_bust_none() -> None:
     # check that ValueError is raised when no molecules are provided
     try:
         bust()
     except ValueError:
         pass
     else:
```

### Comparing `posebusters-0.2.8/tests/test_modules/test_distance_geometry.py` & `posebusters-0.2.9/tests/test_modules/test_distance_geometry.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/test_modules/test_energy_ratio.py` & `posebusters-0.2.9/tests/test_modules/test_energy_ratio.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/test_modules/test_flatness.py` & `posebusters-0.2.9/tests/test_modules/test_flatness.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/test_modules/test_identity.py` & `posebusters-0.2.9/tests/test_modules/test_identity.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/test_modules/test_intermolecular_distance.py` & `posebusters-0.2.9/tests/test_modules/test_intermolecular_distance.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/test_modules/test_rmsd.py` & `posebusters-0.2.9/tests/test_modules/test_rmsd.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/test_modules/test_sanity.py` & `posebusters-0.2.9/tests/test_modules/test_sanity.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/test_modules/test_volume_overlap.py` & `posebusters-0.2.9/tests/test_modules/test_volume_overlap.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/tests/test_posebusters.py` & `posebusters-0.2.9/tests/test_posebusters.py`

 * *Files identical despite different names*

### Comparing `posebusters-0.2.8/PKG-INFO` & `posebusters-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posebusters
-Version: 0.2.8
+Version: 0.2.9
 Summary: PoseBusters: Plausibility checks for generated molecule poses.
 Keywords: posebusters,docking,tests,metric
 Author-email: Martin Buttenschoen <martin.buttenschoen@stats.ox.ac.uk>
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

