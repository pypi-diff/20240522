# Comparing `tmp/synrbl-0.0.8.tar.gz` & `tmp/synrbl-0.0.9.tar.gz`

## Comparing `synrbl-0.0.8.tar` & `synrbl-0.0.9.tar`

### file list

```diff
@@ -1,154 +1,155 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 synrbl-0.0.8/.coveragerc
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 synrbl-0.0.8/.gitattributes
--rwxr-xr-x   0        0        0      216 2020-02-02 00:00:00.000000 synrbl-0.0.8/lint.sh
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 synrbl-0.0.8/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 synrbl-0.0.8/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 synrbl-0.0.8/.github/workflows/test-and-lint.yml
--rw-r--r--   0        0        0   815176 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Raw_data/Golden/Golden.csv
--rw-r--r--   0        0        0    44593 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Raw_data/Jaworski/complex.csv
--rw-r--r--   0        0        0   128945 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Raw_data/Jaworski/patent.csv
--rw-r--r--   0        0        0    91588 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Raw_data/Jaworski/typical.csv
--rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Raw_data/USPTO/USPTO_50K.csv
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Rules/automated_rules.json.gz
--rw-r--r--   0        0        0    63599 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Validation_set/Jaworski.csv
--rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Validation_set/USPTO_50K.csv
--rw-r--r--   0        0        0   188656 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Validation_set/USPTO_diff.csv
--rw-r--r--   0        0        0    89839 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Validation_set/USPTO_random_class.csv
--rw-r--r--   0        0        0    64959 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Validation_set/USPTO_unbalance_class.csv
--rw-r--r--   0        0        0   677196 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Validation_set/golden_dataset.csv
--rw-r--r--   0        0        0  1955873 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Validation_set/validation_set.csv
--rw-r--r--   0        0        0  2769281 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Validation_set/validation_set.json
--rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 synrbl-0.0.8/Docs/Examples/notebook.ipynb
--rw-r--r--   0        0        0    86666 2020-02-02 00:00:00.000000 synrbl-0.0.8/Docs/Images/Flowchart.png
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 synrbl-0.0.8/Docs/Paper_fig/figures.py
--rw-r--r--   0        0        0    55850 2020-02-02 00:00:00.000000 synrbl-0.0.8/Pipeline/Validation/Analysis/Analysis_vis.ipynb
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv
--rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv
--rw-r--r--   0        0        0    13301 2020-02-02 00:00:00.000000 synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 synrbl-0.0.8/Scripts/result_evaluation.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 synrbl-0.0.8/Scripts/synrbl_pilot.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 synrbl-0.0.8/Scripts/validation_set_interface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/__init__.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/test_mcs_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynChemImputer/__init__.py
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynChemImputer/test_appeal_reaction.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynChemImputer/test_curate_oxidation.py
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynChemImputer/test_curate_reduction.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynChemImputer/test_molecule_standardizer.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynChemImputer/test_peroxide_imputer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/__init__.py
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/test_merge.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/test_model.py
--rw-r--r--   0        0        0    11025 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/test_rules.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/test_structure.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/__init__.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/test_molcurator.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/SubStructure/__init__.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py
--rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/SubStructure/test_mcs_process.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynProcessor/__init__.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynProcessor/test_check_carbon_balance.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynProcessor/test_rmsi_comparator.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynProcessor/test_rmsi_decomposer.py
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynProcessor/test_rmsi_processing.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynProcessor/test_rsmi_both_side_process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynRuleImputer/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynRuleImputer/test_auto_extract_rules.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynRuleImputer/test_auto_extract_smiles.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynRuleImputer/test_rule_constraint.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynRuleImputer/test_rule_data_manager.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynRuleImputer/test_synthetic_rule_imputer.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynRuleImputer/test_synthetic_rule_matcher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynUtils/__init__.py
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynUtils/test_chem_utils.py
--rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynUtils/test_functional_group_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynVis/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynVis/test_reaction_visualizer.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/__main__.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/balancing.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/confidence_prediction.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/mcs_search.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/postprocess.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/preprocess.py
--rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/rsmi_utils.py
--rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/rule_based.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynAnalysis/__init__.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynAnalysis/analysis_process.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynAnalysis/analysis_utils.py
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynAnalysis/eda_analysis.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynAnalysis/feature_analysis.py
--rw-r--r--   0        0        0   278926 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynAnalysis/scoring_function.dump
--rw-r--r--   0        0        0    16405 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynAnalysis/visualizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/__init__.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/appel_reaction.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/compounds_template.json
--rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/curate_oxidation.py
--rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/curate_reduction.py
--rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/molecule_standardizer.py
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/peroxide_imputer.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/post_process.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/reaction_template.json
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynCmd/__init__.py
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynCmd/cmd_benchmark.py
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynCmd/cmd_run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynCmd/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/__init__.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/compound_rules.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/expand_rules.json
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/merge.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/merge_rules.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/merge_rules_example.json
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/model.py
--rw-r--r--   0        0        0    29044 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/rules.py
--rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/structure.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/__init__.py
--rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/find_graph_dict.py
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/find_missing_graphs.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/molcurator.py
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/refinement_uncertainty.py
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/uncertainty_graph.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/__init__.py
--rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/extract_common_mcs.py
--rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/mcs_graph_detector.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/mcs_process.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/substructure_analyzer.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynProcessor/__init__.py
--rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynProcessor/check_carbon_balance.py
--rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynProcessor/rsmi_both_side_process.py
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynProcessor/rsmi_comparator.py
--rw-r--r--   0        0        0     7321 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynProcessor/rsmi_decomposer.py
--rw-r--r--   0        0        0     7210 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynProcessor/rsmi_processing.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynRuleImputer/__init__.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynRuleImputer/auto_extract_rules.py
--rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynRuleImputer/auto_extract_smiles.py
--rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynRuleImputer/rule_data_manager.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynRuleImputer/rules_manager.json.gz
--rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynRuleImputer/synthetic_rule_constraint.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynRuleImputer/synthetic_rule_imputer.py
--rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynRuleImputer/synthetic_rule_matcher.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynUtils/__init__.py
--rw-r--r--   0        0        0    11136 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynUtils/chem_utils.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynUtils/common.py
--rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynUtils/data_utils.py
--rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynUtils/functional_group_utils.py
--rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynUtils/rsmi_utils.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynVis/__init__.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynVis/mcs_visualizer.py
--rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynVis/reaction_visualizer.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynVis/rxnpdf.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynVis/rxnvis.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 synrbl-0.0.8/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 synrbl-0.0.8/LICENSE
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 synrbl-0.0.8/README.md
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 synrbl-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 synrbl-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 synrbl-0.0.9/.coveragerc
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 synrbl-0.0.9/.gitattributes
+-rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 synrbl-0.0.9/lint.sh
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 synrbl-0.0.9/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 synrbl-0.0.9/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 synrbl-0.0.9/.github/workflows/test-and-lint.yml
+-rw-r--r--   0        0        0   815176 2020-02-02 00:00:00.000000 synrbl-0.0.9/Data/Raw_data/Golden/Golden.csv
+-rw-r--r--   0        0        0    44593 2020-02-02 00:00:00.000000 synrbl-0.0.9/Data/Raw_data/Jaworski/complex.csv
+-rw-r--r--   0        0        0   128945 2020-02-02 00:00:00.000000 synrbl-0.0.9/Data/Raw_data/Jaworski/patent.csv
+-rw-r--r--   0        0        0    91588 2020-02-02 00:00:00.000000 synrbl-0.0.9/Data/Raw_data/Jaworski/typical.csv
+-rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.9/Data/Raw_data/USPTO/USPTO_50K.csv
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 synrbl-0.0.9/Data/Rules/automated_rules.json.gz
+-rw-r--r--   0        0        0    63599 2020-02-02 00:00:00.000000 synrbl-0.0.9/Data/Validation_set/Jaworski.csv
+-rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.9/Data/Validation_set/USPTO_50K.csv
+-rw-r--r--   0        0        0   188656 2020-02-02 00:00:00.000000 synrbl-0.0.9/Data/Validation_set/USPTO_diff.csv
+-rw-r--r--   0        0        0    89839 2020-02-02 00:00:00.000000 synrbl-0.0.9/Data/Validation_set/USPTO_random_class.csv
+-rw-r--r--   0        0        0    64959 2020-02-02 00:00:00.000000 synrbl-0.0.9/Data/Validation_set/USPTO_unbalance_class.csv
+-rw-r--r--   0        0        0   677196 2020-02-02 00:00:00.000000 synrbl-0.0.9/Data/Validation_set/golden_dataset.csv
+-rw-r--r--   0        0        0  1955873 2020-02-02 00:00:00.000000 synrbl-0.0.9/Data/Validation_set/validation_set.csv
+-rw-r--r--   0        0        0  2769281 2020-02-02 00:00:00.000000 synrbl-0.0.9/Data/Validation_set/validation_set.json
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 synrbl-0.0.9/Docs/Examples/notebook.ipynb
+-rw-r--r--   0        0        0    86666 2020-02-02 00:00:00.000000 synrbl-0.0.9/Docs/Images/Flowchart.png
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 synrbl-0.0.9/Docs/Paper_fig/figures.py
+-rw-r--r--   0        0        0    55850 2020-02-02 00:00:00.000000 synrbl-0.0.9/Pipeline/Validation/Analysis/Analysis_vis.ipynb
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 synrbl-0.0.9/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 synrbl-0.0.9/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv
+-rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 synrbl-0.0.9/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 synrbl-0.0.9/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv
+-rw-r--r--   0        0        0    13301 2020-02-02 00:00:00.000000 synrbl-0.0.9/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv
+-rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 synrbl-0.0.9/Scripts/result_evaluation.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 synrbl-0.0.9/Scripts/synrbl_pilot.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 synrbl-0.0.9/Scripts/validation_set_interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/__init__.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/test_mcs_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynChemImputer/__init__.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynChemImputer/test_appeal_reaction.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynChemImputer/test_curate_oxidation.py
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynChemImputer/test_curate_reduction.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynChemImputer/test_molecule_standardizer.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynChemImputer/test_peroxide_imputer.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynChemImputer/test_post_process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynMCSImputer/__init__.py
+-rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynMCSImputer/test_merge.py
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynMCSImputer/test_model.py
+-rw-r--r--   0        0        0    11025 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynMCSImputer/test_rules.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynMCSImputer/test_structure.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynMCSImputer/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynMCSImputer/MissingGraph/__init__.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynMCSImputer/MissingGraph/test_molcurator.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynMCSImputer/SubStructure/__init__.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynMCSImputer/SubStructure/test_mcs_process.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynProcessor/__init__.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynProcessor/test_check_carbon_balance.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynProcessor/test_rmsi_comparator.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynProcessor/test_rmsi_decomposer.py
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynProcessor/test_rmsi_processing.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynProcessor/test_rsmi_both_side_process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynRuleImputer/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynRuleImputer/test_auto_extract_rules.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynRuleImputer/test_auto_extract_smiles.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynRuleImputer/test_rule_constraint.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynRuleImputer/test_rule_data_manager.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynRuleImputer/test_synthetic_rule_imputer.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynRuleImputer/test_synthetic_rule_matcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynUtils/__init__.py
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynUtils/test_chem_utils.py
+-rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynUtils/test_functional_group_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynVis/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 synrbl-0.0.9/Test/SynVis/test_reaction_visualizer.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/__main__.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/balancing.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/confidence_prediction.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/mcs_search.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/postprocess.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/preprocess.py
+-rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/rsmi_utils.py
+-rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/rule_based.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynAnalysis/__init__.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynAnalysis/analysis_process.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynAnalysis/analysis_utils.py
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynAnalysis/eda_analysis.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynAnalysis/feature_analysis.py
+-rw-r--r--   0        0        0   278926 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynAnalysis/scoring_function.dump
+-rw-r--r--   0        0        0    16405 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynAnalysis/visualizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynChemImputer/__init__.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynChemImputer/appel_reaction.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynChemImputer/compounds_template.json
+-rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynChemImputer/curate_oxidation.py
+-rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynChemImputer/curate_reduction.py
+-rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynChemImputer/molecule_standardizer.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynChemImputer/peroxide_imputer.py
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynChemImputer/post_process.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynChemImputer/reaction_template.json
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynCmd/__init__.py
+-rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynCmd/cmd_benchmark.py
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynCmd/cmd_run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynCmd/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/compound_rules.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/expand_rules.json
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/merge.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/merge_rules.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/merge_rules_example.json
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/model.py
+-rw-r--r--   0        0        0    29044 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/rules.py
+-rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/structure.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/MissingGraph/__init__.py
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/MissingGraph/find_graph_dict.py
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/MissingGraph/find_missing_graphs.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/MissingGraph/molcurator.py
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/MissingGraph/refinement_uncertainty.py
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/MissingGraph/uncertainty_graph.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/SubStructure/__init__.py
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/SubStructure/extract_common_mcs.py
+-rw-r--r--   0        0        0    10265 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/SubStructure/mcs_graph_detector.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/SubStructure/mcs_process.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynMCSImputer/SubStructure/substructure_analyzer.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynProcessor/__init__.py
+-rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynProcessor/check_carbon_balance.py
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynProcessor/rsmi_both_side_process.py
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynProcessor/rsmi_comparator.py
+-rw-r--r--   0        0        0     7321 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynProcessor/rsmi_decomposer.py
+-rw-r--r--   0        0        0     7210 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynProcessor/rsmi_processing.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynRuleImputer/__init__.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynRuleImputer/auto_extract_rules.py
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynRuleImputer/auto_extract_smiles.py
+-rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynRuleImputer/rule_data_manager.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynRuleImputer/rules_manager.json.gz
+-rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynRuleImputer/synthetic_rule_constraint.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynRuleImputer/synthetic_rule_imputer.py
+-rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynRuleImputer/synthetic_rule_matcher.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynUtils/__init__.py
+-rw-r--r--   0        0        0    11136 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynUtils/chem_utils.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynUtils/common.py
+-rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynUtils/data_utils.py
+-rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynUtils/functional_group_utils.py
+-rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynUtils/rsmi_utils.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynVis/__init__.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynVis/mcs_visualizer.py
+-rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynVis/reaction_visualizer.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynVis/rxnpdf.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 synrbl-0.0.9/synrbl/SynVis/rxnvis.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 synrbl-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 synrbl-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 synrbl-0.0.9/README.md
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 synrbl-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 synrbl-0.0.9/PKG-INFO
```

### Comparing `synrbl-0.0.8/.github/workflows/publish-package.yml` & `synrbl-0.0.9/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/.github/workflows/test-and-lint.yml` & `synrbl-0.0.9/.github/workflows/test-and-lint.yml`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Data/Raw_data/Golden/Golden.csv` & `synrbl-0.0.9/Data/Raw_data/Golden/Golden.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Data/Raw_data/Jaworski/complex.csv` & `synrbl-0.0.9/Data/Raw_data/Jaworski/complex.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Data/Raw_data/Jaworski/patent.csv` & `synrbl-0.0.9/Data/Raw_data/Jaworski/patent.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Data/Raw_data/Jaworski/typical.csv` & `synrbl-0.0.9/Data/Raw_data/Jaworski/typical.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Data/Raw_data/USPTO/USPTO_50K.csv` & `synrbl-0.0.9/Data/Raw_data/USPTO/USPTO_50K.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Data/Rules/automated_rules.json.gz` & `synrbl-0.0.9/Data/Rules/automated_rules.json.gz`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Data/Validation_set/Jaworski.csv` & `synrbl-0.0.9/Data/Validation_set/Jaworski.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Data/Validation_set/USPTO_50K.csv` & `synrbl-0.0.9/Data/Validation_set/USPTO_50K.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Data/Validation_set/USPTO_diff.csv` & `synrbl-0.0.9/Data/Validation_set/USPTO_diff.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Data/Validation_set/USPTO_random_class.csv` & `synrbl-0.0.9/Data/Validation_set/USPTO_random_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Data/Validation_set/USPTO_unbalance_class.csv` & `synrbl-0.0.9/Data/Validation_set/USPTO_unbalance_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Data/Validation_set/golden_dataset.csv` & `synrbl-0.0.9/Data/Validation_set/golden_dataset.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Data/Validation_set/validation_set.csv` & `synrbl-0.0.9/Data/Validation_set/validation_set.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Data/Validation_set/validation_set.json` & `synrbl-0.0.9/Data/Validation_set/validation_set.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Docs/Images/Flowchart.png` & `synrbl-0.0.9/Docs/Images/Flowchart.png`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Docs/Paper_fig/figures.py` & `synrbl-0.0.9/Docs/Paper_fig/figures.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Pipeline/Validation/Analysis/Analysis_vis.ipynb` & `synrbl-0.0.9/Pipeline/Validation/Analysis/Analysis_vis.ipynb`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv` & `synrbl-0.0.9/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv` & `synrbl-0.0.9/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv` & `synrbl-0.0.9/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv` & `synrbl-0.0.9/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv` & `synrbl-0.0.9/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Scripts/result_evaluation.py` & `synrbl-0.0.9/Scripts/result_evaluation.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Scripts/synrbl_pilot.py` & `synrbl-0.0.9/Scripts/synrbl_pilot.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Scripts/validation_set_interface.py` & `synrbl-0.0.9/Scripts/validation_set_interface.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/test_mcs_search.py` & `synrbl-0.0.9/Test/test_mcs_search.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynChemImputer/test_appeal_reaction.py` & `synrbl-0.0.9/Test/SynChemImputer/test_appeal_reaction.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynChemImputer/test_curate_oxidation.py` & `synrbl-0.0.9/Test/SynChemImputer/test_curate_oxidation.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynChemImputer/test_curate_reduction.py` & `synrbl-0.0.9/Test/SynChemImputer/test_curate_reduction.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynChemImputer/test_molecule_standardizer.py` & `synrbl-0.0.9/Test/SynChemImputer/test_molecule_standardizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,18 +21,18 @@
         standardizer = MoleculeStandardizer(smiles)
         result = standardizer.standardize_hemiketal(smiles, atom_indices)
         expected = "C=O.O"  # Expected hemiketal cyclic structure
         self.assertEqual(
             result, expected, "Hemiketal transformation failed or incorrect"
         )
 
-    # def test_MoleculeStandardizer(self):
-    #     smiles = "C(O)(O)C=CO"
-    #     standardizer = MoleculeStandardizer(smiles)
-    #     result = standardizer.fit()
-    #     expected = "O.O=CCC=O"
-    #     self.assertEqual(result, expected, "MoleculeStandardizer failed or incorrect")
+    def test_MoleculeStandardizer(self):
+        smiles = "C(O)(O)C=CO"
+        standardizer = MoleculeStandardizer(smiles)
+        result = standardizer.fit()
+        expected = "O.O=CCC=O"
+        self.assertEqual(result, expected, "MoleculeStandardizer failed or incorrect")
 
 
 # If the script is executed directly, run the tests
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `synrbl-0.0.8/Test/SynChemImputer/test_peroxide_imputer.py` & `synrbl-0.0.9/Test/SynChemImputer/test_peroxide_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynMCSImputer/test_merge.py` & `synrbl-0.0.9/Test/SynMCSImputer/test_merge.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynMCSImputer/test_model.py` & `synrbl-0.0.9/Test/SynMCSImputer/test_model.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynMCSImputer/test_rules.py` & `synrbl-0.0.9/Test/SynMCSImputer/test_rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynMCSImputer/test_structure.py` & `synrbl-0.0.9/Test/SynMCSImputer/test_structure.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynMCSImputer/test_utils.py` & `synrbl-0.0.9/Test/SynMCSImputer/test_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py` & `synrbl-0.0.9/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py` & `synrbl-0.0.9/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/test_molcurator.py` & `synrbl-0.0.9/Test/SynMCSImputer/MissingGraph/test_molcurator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py` & `synrbl-0.0.9/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py` & `synrbl-0.0.9/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py` & `synrbl-0.0.9/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynMCSImputer/SubStructure/test_mcs_process.py` & `synrbl-0.0.9/Test/SynMCSImputer/SubStructure/test_mcs_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py` & `synrbl-0.0.9/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynProcessor/test_check_carbon_balance.py` & `synrbl-0.0.9/Test/SynProcessor/test_check_carbon_balance.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynProcessor/test_rmsi_comparator.py` & `synrbl-0.0.9/Test/SynProcessor/test_rmsi_comparator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynProcessor/test_rmsi_decomposer.py` & `synrbl-0.0.9/Test/SynProcessor/test_rmsi_decomposer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynProcessor/test_rmsi_processing.py` & `synrbl-0.0.9/Test/SynProcessor/test_rmsi_processing.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynProcessor/test_rsmi_both_side_process.py` & `synrbl-0.0.9/Test/SynProcessor/test_rsmi_both_side_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynRuleImputer/test_auto_extract_rules.py` & `synrbl-0.0.9/Test/SynRuleImputer/test_auto_extract_rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynRuleImputer/test_auto_extract_smiles.py` & `synrbl-0.0.9/Test/SynRuleImputer/test_auto_extract_smiles.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynRuleImputer/test_rule_constraint.py` & `synrbl-0.0.9/Test/SynRuleImputer/test_rule_constraint.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynRuleImputer/test_rule_data_manager.py` & `synrbl-0.0.9/Test/SynRuleImputer/test_rule_data_manager.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynRuleImputer/test_synthetic_rule_imputer.py` & `synrbl-0.0.9/Test/SynRuleImputer/test_synthetic_rule_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynRuleImputer/test_synthetic_rule_matcher.py` & `synrbl-0.0.9/Test/SynRuleImputer/test_synthetic_rule_matcher.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynUtils/test_chem_utils.py` & `synrbl-0.0.9/Test/SynUtils/test_chem_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynUtils/test_functional_group_utils.py` & `synrbl-0.0.9/Test/SynUtils/test_functional_group_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/Test/SynVis/test_reaction_visualizer.py` & `synrbl-0.0.9/Test/SynVis/test_reaction_visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/balancing.py` & `synrbl-0.0.9/synrbl/balancing.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/confidence_prediction.py` & `synrbl-0.0.9/synrbl/confidence_prediction.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/mcs_search.py` & `synrbl-0.0.9/synrbl/mcs_search.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/postprocess.py` & `synrbl-0.0.9/synrbl/postprocess.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/preprocess.py` & `synrbl-0.0.9/synrbl/preprocess.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/rsmi_utils.py` & `synrbl-0.0.9/synrbl/rsmi_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/rule_based.py` & `synrbl-0.0.9/synrbl/rule_based.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynAnalysis/analysis_process.py` & `synrbl-0.0.9/synrbl/SynAnalysis/analysis_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynAnalysis/analysis_utils.py` & `synrbl-0.0.9/synrbl/SynAnalysis/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynAnalysis/eda_analysis.py` & `synrbl-0.0.9/synrbl/SynAnalysis/eda_analysis.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynAnalysis/feature_analysis.py` & `synrbl-0.0.9/synrbl/SynAnalysis/feature_analysis.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynAnalysis/scoring_function.dump` & `synrbl-0.0.9/synrbl/SynAnalysis/scoring_function.dump`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynAnalysis/visualizer.py` & `synrbl-0.0.9/synrbl/SynAnalysis/visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynChemImputer/appel_reaction.py` & `synrbl-0.0.9/synrbl/SynChemImputer/appel_reaction.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynChemImputer/compounds_template.json` & `synrbl-0.0.9/synrbl/SynChemImputer/compounds_template.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynChemImputer/curate_oxidation.py` & `synrbl-0.0.9/synrbl/SynChemImputer/curate_oxidation.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynChemImputer/curate_reduction.py` & `synrbl-0.0.9/synrbl/SynChemImputer/curate_reduction.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynChemImputer/molecule_standardizer.py` & `synrbl-0.0.9/synrbl/SynChemImputer/molecule_standardizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynChemImputer/peroxide_imputer.py` & `synrbl-0.0.9/synrbl/SynChemImputer/peroxide_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynChemImputer/post_process.py` & `synrbl-0.0.9/synrbl/SynChemImputer/post_process.py`

 * *Files 26% similar despite different names*

```diff
@@ -55,28 +55,42 @@
             "label": label,
             "reactants": reactants_smiles,
             "products": products_smiles,
         }
 
         return new_dict
 
-    def fit(self, n_jobs=4, verbose=1):
+    def fit(self, n_jobs: int = 4, verbose: int = 1) -> List[Dict]:
+        """
+        Label reactions and curate data by reaction type.
+
+        Parameters:
+        - n_jobs (int): Number of CPUs to use for parallel processing.
+        - verbose (int): Level of verbosity.
+
+        Returns:
+        - List[Dict]: List of dictionaries, each representing a reaction and with
+          keys 'R-id', 'new_reaction', 'label', 'reactants', and 'products'.
+        """
         label_data = Parallel(n_jobs=n_jobs, verbose=verbose)(
             delayed(PostProcess.label_reactions)(d) for d in self.data
         )
 
         reduction_data = [
             value for value in label_data if value["label"] == "Reduction"
         ]
         oxidation_data = [
             value for value in label_data if value["label"] == "Oxidation"
         ]
+        other_data = [value for value in label_data if value["label"] == "unspecified"]
 
         curate_reduction = CurationReduction()
         curate_oxidation = CurationOxidation()
         result_reduction = curate_reduction.parallel_curate(
-            reduction_data, n_jobs=n_jobs, verbose=verbose
+            reduction_data, n_jobs=n_jobs, verbose=verbose, return_all=False
         )
         result_oxidation = curate_oxidation.parallel_curate(
-            oxidation_data, n_jobs=n_jobs, verbose=verbose
+            oxidation_data, n_jobs=n_jobs, verbose=verbose, return_all=False
         )
-        return result_reduction, result_oxidation
+        other_data.extend(result_reduction)
+        other_data.extend(result_oxidation)
+        return other_data
```

### Comparing `synrbl-0.0.8/synrbl/SynChemImputer/reaction_template.json` & `synrbl-0.0.9/synrbl/SynChemImputer/reaction_template.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynCmd/__init__.py` & `synrbl-0.0.9/synrbl/SynCmd/__init__.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynCmd/cmd_benchmark.py` & `synrbl-0.0.9/synrbl/SynCmd/cmd_benchmark.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import logging
 import pandas as pd
+import rdkit.Chem.rdChemReactions as rdChemReactions
 
 from synrbl import Balancer
 from synrbl.SynUtils import normalize_smiles, wc_similarity
 
 logger = logging.getLogger(__name__)
 
 
@@ -46,37 +47,63 @@
             _sr(rb_correct, rb_s),
             _sr(mcs_correct, mcs_cth),
             _sr(rb_correct + mcs_correct, rb_s + mcs_cth),
         )
     )
 
 
-def check_columns(reactions, reaction_col, result_col):
+def check_columns(reactions, reaction_col, result_col, passthrouh_columns):
     if len(reactions) == 0:
         raise ValueError("No reactions found in input.")
     cols = reactions[0].keys()
     if reaction_col not in cols:
         raise KeyError("No column '{}' found in input.".format(reaction_col))
+    if not isinstance(reactions[0][reaction_col], str):
+        raise TypeError(
+            "Reaction column '{}' must be of type string not '{}'.".format(
+                reaction_col, type(reactions[0][reaction_col])
+            )
+        )
+    mol = None
+    try:
+        mol = rdChemReactions.ReactionFromSmarts(
+            reactions[0][reaction_col], useSmiles=True
+        )
+    except Exception:
+        pass
+    if mol is None:
+        raise ValueError(
+            "Value '{}...' in reaction column '{}' is not a valid SMILES.".format(
+                reactions[0][reaction_col][0:30], reaction_col
+            )
+        )
     if result_col not in cols:
         raise KeyError("No column '{}' found in input.".format(result_col))
+    for c in passthrouh_columns:
+        if c not in reactions[0].keys():
+            raise KeyError("Column '{}' not found.".format(c))
 
 
 def run(args):
+    columns = args.columns if isinstance(args.columns, list) else [args.columns]
+    synrbl_cols = [c for c in columns if c in ["mcs"]]
+    passthrough_cols = [c for c in columns if c not in synrbl_cols]
     input_reactions = pd.read_csv(args.inputfile).to_dict("records")
     logger.info(
         "Run benchmark on {} containing {} reactions.".format(
             args.inputfile, len(input_reactions)
         )
     )
-    check_columns(input_reactions, args.col, args.result_col)
+    check_columns(input_reactions, args.col, args.result_col, passthrough_cols)
 
     stats = {}
     synrbl = Balancer(
         reaction_col=args.col, confidence_threshold=args.min_confidence, n_jobs=args.p
     )
+    synrbl.columns.extend(synrbl_cols)
     rbl_reactions = synrbl.rebalance(input_reactions, output_dict=True, stats=stats)
 
     rb_correct = 0
     mcs_correct = 0
     for i, (in_r, out_r) in enumerate(zip(input_reactions, rbl_reactions)):
         if not out_r["solved"]:
             continue
@@ -96,15 +123,17 @@
                 rb_correct += 1
             elif out_r["solved_by"] == "mcs-based":
                 mcs_correct += 1
     print_result(stats, rb_correct, mcs_correct)
 
     if args.o is not None:
         for in_r, out_r in zip(input_reactions, rbl_reactions):
-            out_r[args.result_col] = in_r[args.result_col]
+            for c in columns + [args.result_col]:
+                if c in in_r.keys():
+                    out_r[c] = in_r[c]
         df = pd.DataFrame(rbl_reactions)
         df.to_csv(args.o)
 
 
 class Range(object):
     def __init__(self, start, end):
         self.start = start
@@ -113,17 +142,21 @@
     def __eq__(self, other):
         return self.start <= other <= self.end
 
     def __str__(self):
         return "[{}, {}]".format(self.start, self.end)
 
 
+def list_of_strings(arg):
+    return arg.split(",")
+
+
 def configure_argparser(argparser: argparse._SubParsersAction):
     default_similarity_method = "pathway"
-    default_similarity_threshold = 0.85
+    default_similarity_threshold = 1
     default_p = -1
     default_col = "reaction"
     default_result_col = "expected_reaction"
     default_min_confidence = 0.5
 
     test_parser = argparser.add_parser(
         "benchmark", description="Benchmark SynRBL on your own dataset."
@@ -153,14 +186,21 @@
     test_parser.add_argument(
         "--result-col",
         default=default_result_col,
         help="The reactions column name for in the expected output. "
         + "(Default: {})".format(default_result_col),
     )
     test_parser.add_argument(
+        "--columns",
+        default=[],
+        type=list_of_strings,
+        help="A comma separated list of columns from the input that should "
+        + "be added to the output. (e.g.: col1,col2,col3)",
+    )
+    test_parser.add_argument(
         "--min-confidence",
         type=float,
         default=default_min_confidence,
         choices=[Range(0.0, 1.0)],
         help=(
             "Set a confidence threshold for the results "
             + "from the MCS-based method. (Default: {})".format(default_min_confidence)
```

### Comparing `synrbl-0.0.8/synrbl/SynCmd/cmd_run.py` & `synrbl-0.0.9/synrbl/SynCmd/cmd_run.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/compound_rules.json` & `synrbl-0.0.9/synrbl/SynMCSImputer/compound_rules.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/expand_rules.json` & `synrbl-0.0.9/synrbl/SynMCSImputer/expand_rules.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/merge.py` & `synrbl-0.0.9/synrbl/SynMCSImputer/merge.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/merge_rules.json` & `synrbl-0.0.9/synrbl/SynMCSImputer/merge_rules.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/model.py` & `synrbl-0.0.9/synrbl/SynMCSImputer/model.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/rules.py` & `synrbl-0.0.9/synrbl/SynMCSImputer/rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/structure.py` & `synrbl-0.0.9/synrbl/SynMCSImputer/structure.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/utils.py` & `synrbl-0.0.9/synrbl/SynMCSImputer/utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/find_graph_dict.py` & `synrbl-0.0.9/synrbl/SynMCSImputer/MissingGraph/find_graph_dict.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/find_missing_graphs.py` & `synrbl-0.0.9/synrbl/SynMCSImputer/MissingGraph/find_missing_graphs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/molcurator.py` & `synrbl-0.0.9/synrbl/SynMCSImputer/MissingGraph/molcurator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/refinement_uncertainty.py` & `synrbl-0.0.9/synrbl/SynMCSImputer/MissingGraph/refinement_uncertainty.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/uncertainty_graph.py` & `synrbl-0.0.9/synrbl/SynMCSImputer/MissingGraph/uncertainty_graph.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/extract_common_mcs.py` & `synrbl-0.0.9/synrbl/SynMCSImputer/SubStructure/extract_common_mcs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/mcs_graph_detector.py` & `synrbl-0.0.9/synrbl/SynMCSImputer/SubStructure/mcs_graph_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,27 +197,27 @@
             molecules.
         """
 
         # define parameters
 
         if method == "MCIS":
             params = rdFMCS.MCSParameters()
-            params.Timeout = Timeout
+            params.Timeout = 1  # Timeout
             params.BondCompareParameters.RingMatchesRingOnly = RingMatchesRingOnly
             params.BondCompareParameters.CompleteRingsOnly = CompleteRingsOnly
             if ignore_bond_order:
                 params.BondTyper = rdFMCS.BondCompare.CompareAny
             if ignore_atom_map:
                 params.AtomTyper = rdFMCS.AtomCompare.CompareAny
 
         elif method == "MCES":
             params = rdRascalMCES.RascalOptions()
             params.singleLargestFrag = False
             params.returnEmptyMCES = True
-            params.timeout = Timeout
+            params.timeout = 1  # Timeout
             params.similarityThreshold = similarityThreshold
 
         else:
             raise ValueError("Method '{}' is not implemented.".format(method))
 
         if reaction_dict["carbon_balance_check"] in ["products", "balanced"]:
             # Calculate the MCS for each reactant with the product
```

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/mcs_process.py` & `synrbl-0.0.9/synrbl/SynMCSImputer/SubStructure/mcs_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/substructure_analyzer.py` & `synrbl-0.0.9/synrbl/SynMCSImputer/SubStructure/substructure_analyzer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynProcessor/check_carbon_balance.py` & `synrbl-0.0.9/synrbl/SynProcessor/check_carbon_balance.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynProcessor/rsmi_both_side_process.py` & `synrbl-0.0.9/synrbl/SynProcessor/rsmi_both_side_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynProcessor/rsmi_comparator.py` & `synrbl-0.0.9/synrbl/SynProcessor/rsmi_comparator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynProcessor/rsmi_decomposer.py` & `synrbl-0.0.9/synrbl/SynProcessor/rsmi_decomposer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynProcessor/rsmi_processing.py` & `synrbl-0.0.9/synrbl/SynProcessor/rsmi_processing.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynRuleImputer/auto_extract_rules.py` & `synrbl-0.0.9/synrbl/SynRuleImputer/auto_extract_rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynRuleImputer/auto_extract_smiles.py` & `synrbl-0.0.9/synrbl/SynRuleImputer/auto_extract_smiles.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynRuleImputer/rule_data_manager.py` & `synrbl-0.0.9/synrbl/SynRuleImputer/rule_data_manager.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynRuleImputer/rules_manager.json.gz` & `synrbl-0.0.9/synrbl/SynRuleImputer/rules_manager.json.gz`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynRuleImputer/synthetic_rule_constraint.py` & `synrbl-0.0.9/synrbl/SynRuleImputer/synthetic_rule_constraint.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynRuleImputer/synthetic_rule_imputer.py` & `synrbl-0.0.9/synrbl/SynRuleImputer/synthetic_rule_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynRuleImputer/synthetic_rule_matcher.py` & `synrbl-0.0.9/synrbl/SynRuleImputer/synthetic_rule_matcher.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynUtils/chem_utils.py` & `synrbl-0.0.9/synrbl/SynUtils/chem_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynUtils/data_utils.py` & `synrbl-0.0.9/synrbl/SynUtils/data_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynUtils/functional_group_utils.py` & `synrbl-0.0.9/synrbl/SynUtils/functional_group_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynUtils/rsmi_utils.py` & `synrbl-0.0.9/synrbl/SynUtils/rsmi_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynVis/mcs_visualizer.py` & `synrbl-0.0.9/synrbl/SynVis/mcs_visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynVis/reaction_visualizer.py` & `synrbl-0.0.9/synrbl/SynVis/reaction_visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynVis/rxnpdf.py` & `synrbl-0.0.9/synrbl/SynVis/rxnpdf.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/synrbl/SynVis/rxnvis.py` & `synrbl-0.0.9/synrbl/SynVis/rxnvis.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/.gitignore` & `synrbl-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/LICENSE` & `synrbl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.8/pyproject.toml` & `synrbl-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "synrbl"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
 	{name="Tieu Long Phan", email="long.tieu_phan@uni-leipzig.de"}, 
 	{name="Klaus Weinbauer", email="klaus@bioinf.uni-leipzig.de"}
 	]
 description = "Synthesis Rebalancing Framework for Computational Chemistry"
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `synrbl-0.0.8/PKG-INFO` & `synrbl-0.0.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.3
-Name: synrbl
-Version: 0.0.8
-Summary: Synthesis Rebalancing Framework for Computational Chemistry
-Project-URL: homepage, https://github.com/TieuLongPhan/SynRBL
-Project-URL: source, https://github.com/TieuLongPhan/SynRBL
-Project-URL: issues, https://github.com/TieuLongPhan/SynRBL/issues
-Author-email: Tieu Long Phan <long.tieu_phan@uni-leipzig.de>, Klaus Weinbauer <klaus@bioinf.uni-leipzig.de>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
-Requires-Dist: imbalanced-learn>=0.12.0
-Requires-Dist: joblib>=1.3.2
-Requires-Dist: rdkit>=2023.9.4
-Requires-Dist: reportlab>=4.1.0
-Requires-Dist: scikit-learn>=1.4.1.post1
-Requires-Dist: seaborn>=0.13.2
-Requires-Dist: xgboost>=2.0.3
-Description-Content-Type: text/markdown
-
 # SynRBL: Synthesis Rebalancing Framework
 
 SynRBL is a toolkit tailored for computational chemistry, aimed at correcting imbalances in chemical reactions. It employs a dual strategy: a rule-based method for adjusting non-carbon elements and an mcs-based (maximum common substructure) technique for carbon element adjustments.
 
 ![screenshot](./Docs/Images/Flowchart.png)
 
 
@@ -45,15 +23,15 @@
 - RDKit == 2023.9.4
 - joblib==1.3.2
 - seaborn==0.13.2
 - xgoost==2.0.3
 - scikit_learn==1.4.1.post1
 - imbalanced_learn==0.12.0
 - reportlab==4.1.0
-
+- fgutils==0.0.13
 
 ### Step-by-Step Installation Guide
 
 1. **Python Installation:**
   Ensure that Python 3.11 or later is installed on your system. You can download it from [python.org](https://www.python.org/downloads/).
 
 2. **Creating a Virtual Environment (Optional but Recommended):**
@@ -74,24 +52,43 @@
   Clone the SynRBL repository from GitHub and install it:
 
   ```bash
   pip install synrbl
   ```
 
 4. **Verify Installation:**
-  After installation, you can verify that SynRBL is correctly installed by running a simple test or checking the package version.
+  After installation, you can verify that SynRBL is correctly installed by running a simple test.
 
   ```python
-  python -c "import synrbl; print(synrbl.__version__)"
+  python -c "from synrbl import Balancer; bal = Balancer(reaction_col='reactions', id_col='id'); print(bal.rebalance(reactions='CCO>>CC=O', output_dict=True))"
   ```
 
 ## Usage
 1. **Jupyter Notebook:**
   ```python
   from synrbl import Balancer
+
+  test = (
+      "COC(=O)[C@H](CCCCNC(=O)OCc1ccccc1)NC(=O)Nc1cc(OC)cc(C(C)(C)C)c1O>>"
+      + "COC(=O)[C@H](CCCCN)NC(=O)Nc1cc(OC)cc(C(C)(C)C)c1O"
+  )
+  synrbl = Balancer(reaction_col="reactions", id_col="id")
+
+  results = synrbl.rebalance(reactions=test, output_dict=True)
+  >> [{
+          "reactions": "COC(=O)[C@H](CCCCNC(=O)OCc1ccccc1)NC(=O)Nc1cc(OC)cc(C(C)(C)C)c1O.O>>"
+          + "COC(=O)[C@H](CCCCN)NC(=O)Nc1cc(OC)cc(C(C)(C)C)c1O.O=C(O)OCc1ccccc1",
+          "solved": True,
+          "input_reaction": "COC(=O)[C@H](CCCCNC(=O)OCc1ccccc1)NC(=O)Nc1cc(OC)cc(C(C)(C)C)c1O>>"
+          + "COC(=O)[C@H](CCCCN)NC(=O)Nc1cc(OC)cc(C(C)(C)C)c1O",
+          "issue": "",
+          "rules": ["append O when next to O or N", "default single bond"],
+          "solved_by": "mcs-based",
+          "confidence": 0.999,
+      }]
   ```
 2. **Command line**
   ```bash
   python -m synrbl run --help
   ```
 
 3. **Reproduce the experiment**
```

