# Comparing `tmp/LbNightlyTools-4.0.8.tar.gz` & `tmp/LbNightlyTools-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LbNightlyTools-4.0.8.tar", last modified: Wed May 22 08:37:05 2024, max compression
+gzip compressed data, was "LbNightlyTools-4.0.9.tar", last modified: Wed May 22 14:25:10 2024, max compression
```

## Comparing `LbNightlyTools-4.0.8.tar` & `LbNightlyTools-4.0.9.tar`

### file list

```diff
@@ -1,424 +1,424 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.989827 LbNightlyTools-4.0.8/
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      339 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     4969 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      487 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    15557 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    35147 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/COPYING
--rw-r--r--   0 root         (0) root         (0)     1090 2024-05-22 08:37:05.989827 LbNightlyTools-4.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.963827 LbNightlyTools-4.0.8/admin/
--rw-rw-rw-   0 root         (0) root         (0)     1669 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/admin/LHCb_LbScripts.spectemplate
--rwxrwxrwx   0 root         (0) root         (0)     1882 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/admin/RpmHelpers.py
--rwxrwxrwx   0 root         (0) root         (0)     3688 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/admin/createLbScriptsRpm
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.963827 LbNightlyTools-4.0.8/couchdb/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      982 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/Push CouchDB Nightly Builds.launch
--rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.963827 LbNightlyTools-4.0.8/couchdb/auth/
--rw-rw-rw-   0 root         (0) root         (0)     1085 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/auth/validate_doc_update.js
--rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/build_id_index.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.964826 LbNightlyTools-4.0.8/couchdb/deployment/
--rw-rw-rw-   0 root         (0) root         (0)       19 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/deployment/_id
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/deployment/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.956827 LbNightlyTools-4.0.8/couchdb/deployment/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.964826 LbNightlyTools-4.0.8/couchdb/deployment/views/ready/
--rw-rw-rw-   0 root         (0) root         (0)      920 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/deployment/views/ready/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.964826 LbNightlyTools-4.0.8/couchdb/frontend-stats/
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/frontend-stats/.couchappignore
--rw-rw-rw-   0 root         (0) root         (0)      116 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/frontend-stats/.couchapprc
--rw-rw-rw-   0 root         (0) root         (0)      672 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/frontend-stats/README.md
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/frontend-stats/_id
--rw-rw-rw-   0 root         (0) root         (0)       83 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/frontend-stats/couchapp.json
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/frontend-stats/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.956827 LbNightlyTools-4.0.8/couchdb/frontend-stats/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.964826 LbNightlyTools-4.0.8/couchdb/frontend-stats/views/byDate/
--rw-rw-rw-   0 root         (0) root         (0)     2483 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/frontend-stats/views/byDate/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.964826 LbNightlyTools-4.0.8/couchdb/merge_requests/
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/merge_requests/_id
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/merge_requests/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.956827 LbNightlyTools-4.0.8/couchdb/merge_requests/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.964826 LbNightlyTools-4.0.8/couchdb/merge_requests/views/mr_slots_by_ref_slot/
--rw-rw-rw-   0 root         (0) root         (0)      307 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/merge_requests/views/mr_slots_by_ref_slot/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.964826 LbNightlyTools-4.0.8/couchdb/merge_requests/views/mrs/
--rw-rw-rw-   0 root         (0) root         (0)      756 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/merge_requests/views/mrs/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.965827 LbNightlyTools-4.0.8/couchdb/names/
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/names/_id
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/names/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.956827 LbNightlyTools-4.0.8/couchdb/names/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.965827 LbNightlyTools-4.0.8/couchdb/names/views/platforms/
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/names/views/platforms/map.js
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/names/views/platforms/reduce.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.965827 LbNightlyTools-4.0.8/couchdb/names/views/projects/
--rw-rw-rw-   0 root         (0) root         (0)      142 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/names/views/projects/map.js
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/names/views/projects/reduce.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.965827 LbNightlyTools-4.0.8/couchdb/names/views/slots/
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/names/views/slots/map.js
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/names/views/slots/reduce.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.965827 LbNightlyTools-4.0.8/couchdb/nightlies_summaries/
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/nightlies_summaries/_id
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/nightlies_summaries/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.957826 LbNightlyTools-4.0.8/couchdb/nightlies_summaries/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.965827 LbNightlyTools-4.0.8/couchdb/nightlies_summaries/views/by_app_version/
--rw-rw-rw-   0 root         (0) root         (0)       98 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/nightlies_summaries/views/by_app_version/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.966827 LbNightlyTools-4.0.8/couchdb/old_dashboard/
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/old_dashboard/_id
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/old_dashboard/language
--rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/old_dashboard/rewrites.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.966827 LbNightlyTools-4.0.8/couchdb/periodic_summaries/
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/periodic_summaries/_id
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/periodic_summaries/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.957826 LbNightlyTools-4.0.8/couchdb/periodic_summaries/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.966827 LbNightlyTools-4.0.8/couchdb/periodic_summaries/views/byTime/
--rw-rw-rw-   0 root         (0) root         (0)       74 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/periodic_summaries/views/byTime/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.966827 LbNightlyTools-4.0.8/couchdb/releases/
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/releases/_id
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/releases/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.966827 LbNightlyTools-4.0.8/couchdb/releases/lists/
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/releases/lists/projectBuildIds.js
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/releases/rewrites.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.957826 LbNightlyTools-4.0.8/couchdb/releases/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.966827 LbNightlyTools-4.0.8/couchdb/releases/views/projectBuildIds/
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/releases/views/projectBuildIds/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.967826 LbNightlyTools-4.0.8/couchdb/summaries/
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/summaries/_id
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/summaries/language
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/summaries/rewrites.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.957826 LbNightlyTools-4.0.8/couchdb/summaries/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.967826 LbNightlyTools-4.0.8/couchdb/summaries/views/byDay/
--rw-rw-rw-   0 root         (0) root         (0)      347 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/summaries/views/byDay/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.967826 LbNightlyTools-4.0.8/couchdb/summaries/views/lastBuildId/
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/summaries/views/lastBuildId/map.js
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/summaries/views/lastBuildId/reduce.js
--rwxrwxrwx   0 root         (0) root         (0)     3600 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/couchdb/webapp_testbench.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.967826 LbNightlyTools-4.0.8/cron/
--rwxrwxrwx   0 root         (0) root         (0)     1858 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/cron/cleanup_artifacts.sh
--rw-rw-rw-   0 root         (0) root         (0)      433 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/cron/logrotate.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.968827 LbNightlyTools-4.0.8/docs/
--rw-rw-rw-   0 root         (0) root         (0)    25550 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/Interactive builds of LHCb projects.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1318 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/LHCbPR2.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.968827 LbNightlyTools-4.0.8/docs/configuration/
--rw-rw-rw-   0 root         (0) root         (0)     3017 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/configuration/Example.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.968827 LbNightlyTools-4.0.8/docs/examples/
--rwxrwxrwx   0 root         (0) root         (0)     1247 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/examples/lbpr-example
--rw-rw-rw-   0 root         (0) root         (0)     2628 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/jenkins-scripts.dot
--rw-rw-rw-   0 root         (0) root         (0)   142880 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/jenkins-scripts.dot.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.970826 LbNightlyTools-4.0.8/docs/note/
--rw-rw-rw-   0 root         (0) root         (0)   946715 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/LHCb-INT-2013-006.pdf
--rw-rw-rw-   0 root         (0) root         (0)    24731 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/LHCb.bst
--rw-rw-rw-   0 root         (0) root         (0)     1679 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/README.txt
--rw-rw-rw-   0 root         (0) root         (0)     3132 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/appendix.tex
--rw-rw-rw-   0 root         (0) root         (0)     5159 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/bibliography.bib
--rw-rw-rw-   0 root         (0) root         (0)    32522 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/cite.sty
--rw-rw-rw-   0 root         (0) root         (0)      567 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/conclusions.tex
--rw-rw-rw-   0 root         (0) root         (0)     5975 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/dashboard.tex
--rw-rw-rw-   0 root         (0) root         (0)     2326 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/design.tex
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.971827 LbNightlyTools-4.0.8/docs/note/figs/
--rw-rw-rw-   0 root         (0) root         (0)    60108 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/figs/cdash-1.png
--rw-rw-rw-   0 root         (0) root         (0)    97134 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/figs/cdash-2.png
--rw-rw-rw-   0 root         (0) root         (0)   101416 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/figs/cdash-3.png
--rw-rw-rw-   0 root         (0) root         (0)   162025 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/figs/cdash-4.png
--rw-rw-rw-   0 root         (0) root         (0)    91381 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/figs/jenkins-1.png
--rw-rw-rw-   0 root         (0) root         (0)    81047 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/figs/jenkins-2.png
--rw-rw-rw-   0 root         (0) root         (0)   173109 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/figs/jenkins-3.png
--rw-rw-rw-   0 root         (0) root         (0)   160146 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/figs/lhcb-logo.eps
--rw-rw-rw-   0 root         (0) root         (0)    14116 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/figs/lhcb-logo.pdf
--rw-rw-rw-   0 root         (0) root         (0)   134216 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/figs/old-summary.png
--rw-rw-rw-   0 root         (0) root         (0)    33058 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/implementation.tex
--rw-rw-rw-   0 root         (0) root         (0)     2299 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/introduction.tex
--rw-rw-rw-   0 root         (0) root         (0)     5596 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/lhcb-int-2013-006.kilepr
--rwxrwxrwx   0 root         (0) root         (0)     3645 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/listsymbols
--rw-rw-rw-   0 root         (0) root         (0)     1586 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/main.tex
--rw-rw-rw-   0 root         (0) root         (0)    61167 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/mciteplus.sty
--rw-rw-rw-   0 root         (0) root         (0)     2787 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/preamble.tex
--rw-rw-rw-   0 root         (0) root         (0)     1363 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/requirements.tex
--rw-rw-rw-   0 root         (0) root         (0)     2478 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/title-LHCb-ANA.tex
--rw-rw-rw-   0 root         (0) root         (0)    28723 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/note/unsrturl.bst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.972827 LbNightlyTools-4.0.8/docs/operation/
--rw-rw-rw-   0 root         (0) root         (0)      974 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/operation/Makefile
--rw-rw-rw-   0 root         (0) root         (0)    26499 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/operation/NightlyBuildsOperation.html
--rw-rw-rw-   0 root         (0) root         (0)    11288 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/operation/NightlyBuildsOperation.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.972827 LbNightlyTools-4.0.8/docs/operation/images/
--rw-rw-rw-   0 root         (0) root         (0)      788 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/operation/images/jenkins-jobs.dot
--rw-rw-rw-   0 root         (0) root         (0)    32492 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/operation/images/jenkins-jobs.dot.png
--rw-rw-rw-   0 root         (0) root         (0)     7965 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/docs/pylint.rc
--rw-rw-rw-   0 root         (0) root         (0)      181 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.958826 LbNightlyTools-4.0.8/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.972827 LbNightlyTools-4.0.8/python/LbMsg/
--rwxrwxrwx   0 root         (0) root         (0)     3452 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbMsg/BuildMsg.py
--rw-rw-rw-   0 root         (0) root         (0)     4609 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbMsg/Common.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbMsg/TestMsg.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbMsg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.974827 LbNightlyTools-4.0.8/python/LbNightlyTools/
--rw-rw-rw-   0 root         (0) root         (0)     4457 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/ArtifactsServer.py
--rw-rw-rw-   0 root         (0) root         (0)    12315 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/BuildLogScanner.py
--rw-rw-rw-   0 root         (0) root         (0)    33812 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/BuildMethods.py
--rw-rw-rw-   0 root         (0) root         (0)     3715 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/CheckSlotPreconditions.py
--rw-rw-rw-   0 root         (0) root         (0)    34819 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/CheckoutMethods.py
--rw-rw-rw-   0 root         (0) root         (0)    81329 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Configuration.py
--rwxrwxrwx   0 root         (0) root         (0)     5166 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/GetNightlyRefs.py
--rw-rw-rw-   0 root         (0) root         (0)     8060 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/GitlabUtils.py
--rw-rw-rw-   0 root         (0) root         (0)    18542 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/HTMLUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     4305 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/LbScriptsUtils.py
--rw-rw-rw-   0 root         (0) root         (0)    21375 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/MergeRequestBuilds.py
--rw-rw-rw-   0 root         (0) root         (0)     6152 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/ProcUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     6339 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.976827 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/
--rw-rw-rw-   0 root         (0) root         (0)    36766 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/Build.py
--rw-rw-rw-   0 root         (0) root         (0)    15261 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/Checkout.py
--rw-rw-rw-   0 root         (0) root         (0)    15846 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/CollectBuildLogs.py
--rwxrwxrwx   0 root         (0) root         (0)    28293 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/Common.py
--rw-rw-rw-   0 root         (0) root         (0)    14322 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/EnabledSlots.py
--rw-rw-rw-   0 root         (0) root         (0)    14433 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/GitlabMR.py
--rw-rw-rw-   0 root         (0) root         (0)     7665 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/Index.py
--rw-rw-rw-   0 root         (0) root         (0)    29122 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/Install.py
--rw-rw-rw-   0 root         (0) root         (0)     4861 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/Preconditions.py
--rw-rw-rw-   0 root         (0) root         (0)    17852 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/Release.py
--rw-rw-rw-   0 root         (0) root         (0)    14262 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/Test.py
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24776 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/_entry_points.py
--rw-rw-rw-   0 root         (0) root         (0)     3002 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/extract.php
--rw-rw-rw-   0 root         (0) root         (0)      999 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/listzip.php
--rw-rw-rw-   0 root         (0) root         (0)     2663 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/wrapcmd.py
--rw-rw-rw-   0 root         (0) root         (0)    46060 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/Utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1479 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.978827 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/
--rw-rw-rw-   0 root         (0) root         (0)      921 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_apptainer.py
--rw-rw-rw-   0 root         (0) root         (0)     8920 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_build.py
--rw-rw-rw-   0 root         (0) root         (0)    19337 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_build_script.py
--rw-rw-rw-   0 root         (0) root         (0)    12989 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_checkout.py
--rw-rw-rw-   0 root         (0) root         (0)     4202 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_checkout_script.py
--rw-rw-rw-   0 root         (0) root         (0)     9317 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_config_load.py
--rw-rw-rw-   0 root         (0) root         (0)     2140 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_config_pickle.py
--rw-rw-rw-   0 root         (0) root         (0)    15201 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     2967 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_configuration_check.py
--rw-rw-rw-   0 root         (0) root         (0)     3233 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_copytree.py
--rw-rw-rw-   0 root         (0) root         (0)     5953 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_coverity_support.py
--rw-rw-rw-   0 root         (0) root         (0)    14609 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_enabled_slots_script.py
--rw-rw-rw-   0 root         (0) root         (0)     7275 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_gitlab_mr_script.py
--rw-rw-rw-   0 root         (0) root         (0)     1872 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_indexer.py
--rw-rw-rw-   0 root         (0) root         (0)     2597 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_install.py
--rw-rw-rw-   0 root         (0) root         (0)     1759 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_jobconfig.py
--rw-rw-rw-   0 root         (0) root         (0)    11780 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_merge_request_builds.py
--rw-rw-rw-   0 root         (0) root         (0)     8088 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_pack.py
--rw-rw-rw-   0 root         (0) root         (0)     1308 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_precond.py
--rw-rw-rw-   0 root         (0) root         (0)    10940 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_rel_gen_script.py
--rw-rw-rw-   0 root         (0) root         (0)     8064 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_release_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_retry.py
--rw-rw-rw-   0 root         (0) root         (0)     2457 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4594 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_wrapcmd.py
--rw-rw-rw-   0 root         (0) root         (0)     3338 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.974827 LbNightlyTools-4.0.8/python/LbNightlyTools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1090 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11572 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     2752 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      155 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbNightlyTools.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.978827 LbNightlyTools-4.0.8/python/LbPR/
--rw-rw-rw-   0 root         (0) root         (0)     3093 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbPR/LbPRJobManager.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbPR/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17311 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbPR/_entry_points.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.979827 LbNightlyTools-4.0.8/python/LbPeriodicTools/
--rw-rw-rw-   0 root         (0) root         (0)     4171 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbPeriodicTools/LbPeriodicStarter.py
--rw-rw-rw-   0 root         (0) root         (0)    11731 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbPeriodicTools/LbPeriodicTest.py
--rw-rw-rw-   0 root         (0) root         (0)     2178 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbPeriodicTools/LbPeriodicTestSchedule.py
--rw-rw-rw-   0 root         (0) root         (0)     1600 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbPeriodicTools/TestSchedule.xsd
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbPeriodicTools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10067 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbPeriodicTools/_entry_points.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.979827 LbNightlyTools-4.0.8/python/LbPeriodicTools/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbPeriodicTools/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2619 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbPeriodicTools/tests/test_LHCbPR.py
--rw-rw-rw-   0 root         (0) root         (0)     3561 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbPeriodicTools/tests/test_Starter.py
--rw-rw-rw-   0 root         (0) root         (0)     4012 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbPeriodicTools/tests/test_XMLParsing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.980827 LbNightlyTools-4.0.8/python/LbRPMTools/
--rw-rw-rw-   0 root         (0) root         (0)    10184 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbRPMTools/LHCbCompatSpecBuilder.py
--rw-rw-rw-   0 root         (0) root         (0)    22912 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbRPMTools/LHCbExternalsSpecBuilder.py
--rw-rw-rw-   0 root         (0) root         (0)    10040 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbRPMTools/LHCbGenericSpecBuilder.py
--rw-rw-rw-   0 root         (0) root         (0)    16527 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbRPMTools/LHCbLbScriptsSpecBuilder.py
--rw-rw-rw-   0 root         (0) root         (0)     8700 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbRPMTools/LHCbMetaSpecBuilder.py
--rw-rw-rw-   0 root         (0) root         (0)    54217 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbRPMTools/LHCbRPMSpecBuilder.py
--rw-rw-rw-   0 root         (0) root         (0)    29932 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbRPMTools/PackageSlot.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbRPMTools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.980827 LbNightlyTools-4.0.8/python/LbRPMTools/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbRPMTools/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6060 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbRPMTools/tests/test_ExternalSpec.py
--rw-rw-rw-   0 root         (0) root         (0)    14756 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbRPMTools/tests/test_PackageSlot.py
--rw-rw-rw-   0 root         (0) root         (0)    18876 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbRPMTools/tests/test_Spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.980827 LbNightlyTools-4.0.8/python/LbTools/
--rw-rw-rw-   0 root         (0) root         (0)     5602 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbTools/Manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     1676 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbTools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.981827 LbNightlyTools-4.0.8/python/LbTools/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3811 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbTools/tests/test_XMLParsing.py
--rw-rw-rw-   0 root         (0) root         (0)     1653 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/python/LbTools/tests/test_toolchain_info.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-22 08:37:05.990827 LbNightlyTools-4.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    11055 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.981827 LbNightlyTools-4.0.8/testdata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.959827 LbNightlyTools-4.0.8/testdata/artifacts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.959827 LbNightlyTools-4.0.8/testdata/artifacts/packs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.981827 LbNightlyTools-4.0.8/testdata/artifacts/packs/src/
--rw-rw-rw-   0 root         (0) root         (0)     2387 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/artifacts/packs/src/TestProject.HEAD.testing-slot.src.zip
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.959827 LbNightlyTools-4.0.8/testdata/build_tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.959827 LbNightlyTools-4.0.8/testdata/build_tests/orig/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.981827 LbNightlyTools-4.0.8/testdata/build_tests/orig/dummy/
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/build_tests/orig/dummy/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.982827 LbNightlyTools-4.0.8/testdata/build_tests/test_project/
--rw-rw-rw-   0 root         (0) root         (0)      258 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/build_tests/test_project/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/build_tests/test_project/lhcbproject.yml
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/build_tests/test_project/main.cpp
--rw-rw-rw-   0 root         (0) root         (0)     6010 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/ci-test-hook-content.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.960826 LbNightlyTools-4.0.8/testdata/collect_deps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.982827 LbNightlyTools-4.0.8/testdata/collect_deps/broken/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.959827 LbNightlyTools-4.0.8/testdata/collect_deps/broken/BadCMT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.982827 LbNightlyTools-4.0.8/testdata/collect_deps/broken/BadCMT/cmt/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/broken/BadCMT/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.982827 LbNightlyTools-4.0.8/testdata/collect_deps/broken/BadCMake/
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/broken/BadCMake/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.982827 LbNightlyTools-4.0.8/testdata/collect_deps/broken/Gaudi/
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/broken/Gaudi/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/broken/Gaudi/toolchain.cmake
--rw-rw-rw-   0 root         (0) root         (0)      295 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/broken/conf.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.982827 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.982827 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/Brunel/
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/Brunel/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.983827 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/Gaudi/
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/Gaudi/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/Gaudi/toolchain.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.983827 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/LHCb/
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/LHCb/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.983827 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/Lbcom/
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/Lbcom/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.983827 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/NewLHCbProj/
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/NewLHCbProj/lhcbproject.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.983827 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/NewProj/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/NewProj/project.info
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.983827 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/Online/
--rw-rw-rw-   0 root         (0) root         (0)      117 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/Online/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.983827 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/Rec/
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/Rec/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmake/conf.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.983827 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.960826 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/Brunel/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.983827 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/Brunel/cmt/
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/Brunel/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.960826 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/Gaudi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.983827 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/Gaudi/cmt/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/Gaudi/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.960826 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/LHCb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.983827 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/LHCb/cmt/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/LHCb/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.960826 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/Lbcom/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.983827 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/Lbcom/cmt/
--rw-rw-rw-   0 root         (0) root         (0)       19 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/Lbcom/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.984827 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/NewLHCbProj/
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/NewLHCbProj/lhcbproject.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.984827 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/NewProj/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/NewProj/project.info
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.960826 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/Online/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.984827 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/Online/cmt/
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/Online/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.960826 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/Rec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.984827 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/Rec/cmt/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/Rec/cmt/project.cmt
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/collect_deps/cmt/conf.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.960826 LbNightlyTools-4.0.8/testdata/coverity/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.984827 LbNightlyTools-4.0.8/testdata/coverity/bin/
--rwxrwxrwx   0 root         (0) root         (0)     1722 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/coverity/bin/cov-analyze
--rwxrwxrwx   0 root         (0) root         (0)     1630 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/coverity/bin/cov-build
--rwxrwxrwx   0 root         (0) root         (0)     1787 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/coverity/bin/cov-commit-defects
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.960826 LbNightlyTools-4.0.8/testdata/coverity/build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.960826 LbNightlyTools-4.0.8/testdata/coverity/build/TEST/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.984827 LbNightlyTools-4.0.8/testdata/coverity/build/TEST/TEST_HEAD/
--rw-rw-rw-   0 root         (0) root         (0)      310 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/coverity/build/TEST/TEST_HEAD/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.984827 LbNightlyTools-4.0.8/testdata/coverity/build/TEST/TEST_HEAD/InstallArea/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/coverity/build/TEST/TEST_HEAD/InstallArea/.empty
--rw-rw-rw-   0 root         (0) root         (0)      256 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/coverity/build/TEST/TEST_HEAD/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.985827 LbNightlyTools-4.0.8/testdata/coverity/configs/
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/coverity/configs/coverity_config.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/data-packs.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.961826 LbNightlyTools-4.0.8/testdata/fix_glimpse/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.985827 LbNightlyTools-4.0.8/testdata/fix_glimpse/docs/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/fix_glimpse/docs/.glimpse_filenames
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.985827 LbNightlyTools-4.0.8/testdata/fix_glimpse/level1/
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/fix_glimpse/level1/.glimpse_filenames
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.985827 LbNightlyTools-4.0.8/testdata/fix_glimpse/level1/level2/
--rw-rw-rw-   0 root         (0) root         (0)       19 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/fix_glimpse/level1/level2/.glimpse_filenames
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.961826 LbNightlyTools-4.0.8/testdata/fix_glimpse/levelA/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.985827 LbNightlyTools-4.0.8/testdata/fix_glimpse/levelA/levelB/
--rw-rw-rw-   0 root         (0) root         (0)       10 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/fix_glimpse/levelA/levelB/.glimpse_filenames
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.985827 LbNightlyTools-4.0.8/testdata/fix_glimpse/untouched/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/fix_glimpse/untouched/.glimpse_filenames
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.961826 LbNightlyTools-4.0.8/testdata/indexer/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.961826 LbNightlyTools-4.0.8/testdata/indexer/AProject/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.961826 LbNightlyTools-4.0.8/testdata/indexer/AProject/InstallArea/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.985827 LbNightlyTools-4.0.8/testdata/indexer/AProject/InstallArea/cmake/
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/InstallArea/cmake/AProjectConfig.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.985827 LbNightlyTools-4.0.8/testdata/indexer/AProject/InstallArea/include/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/InstallArea/include/GeneratedHeader.h
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/InstallArea/include/MyHeader.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.985827 LbNightlyTools-4.0.8/testdata/indexer/AProject/InstallArea/python/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/InstallArea/python/AProject_merged_confDb.py
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/InstallArea/python/GeneratedPython.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.986827 LbNightlyTools-4.0.8/testdata/indexer/AProject/InstallArea/python/MyPackage/
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackageConf.py
--rw-rw-rw-   0 root         (0) root         (0)       19 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackage_confDb.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackage_user_confDb.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/InstallArea/python/MyPackage/SomeModule.py
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/InstallArea/python/MyPackage/SomethingConf.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/InstallArea/python/MyPackage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.961826 LbNightlyTools-4.0.8/testdata/indexer/AProject/MyPackage/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.986827 LbNightlyTools-4.0.8/testdata/indexer/AProject/MyPackage/Headers/
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/MyPackage/Headers/MyHeader.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.961826 LbNightlyTools-4.0.8/testdata/indexer/AProject/MyPackage/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.986827 LbNightlyTools-4.0.8/testdata/indexer/AProject/MyPackage/python/MyPackage/
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/MyPackage/python/MyPackage/SomeModule.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/MyPackage/python/MyPackage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.986827 LbNightlyTools-4.0.8/testdata/indexer/AProject/MyPackage/scripts/
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/MyPackage/scripts/MyScript
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.986827 LbNightlyTools-4.0.8/testdata/indexer/AProject/MyPackage/src/
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/MyPackage/src/MySource.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.986827 LbNightlyTools-4.0.8/testdata/indexer/AProject/build.dir/
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/indexer/AProject/build.dir/IgnoredSource.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.987827 LbNightlyTools-4.0.8/testdata/periodic_tests/
--rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/periodic_tests/lhcbpr_schedule.xml
--rw-rw-rw-   0 root         (0) root         (0)      743 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/periodic_tests/schedule.xml
--rw-rw-rw-   0 root         (0) root         (0)      402 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/periodic_tests/scheduleIncorrect.xml
--rw-rw-rw-   0 root         (0) root         (0)    15858 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/periodic_tests/slotbuilds.json
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/periodic_tests/starter_schedule.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.988827 LbNightlyTools-4.0.8/testdata/rpm/
--rw-rw-rw-   0 root         (0) root         (0)     1265 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/rpm/Brunel_v46r0.spec
--rw-rw-rw-   0 root         (0) root         (0)     1687 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/rpm/Brunel_v46r0_x86_64-slc6-gcc48-opt.spec
--rw-rw-rw-   0 root         (0) root         (0)     2533 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/rpm/Gaudi_v27r0_x86_64-slc6-gcc49-do0.spec
--rw-rw-rw-   0 root         (0) root         (0)     7196 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/rpm/LCG_68_externalsDict.json
--rw-rw-rw-   0 root         (0) root         (0)     3230 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/rpm/PARAM_TMVAWeights.spec
--rw-rw-rw-   0 root         (0) root         (0)     3230 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/rpm/PARAM_TMVAWeights_rel5.spec
--rw-rw-rw-   0 root         (0) root         (0)      938 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/rpm/datapkg-slot-config.json
--rw-rw-rw-   0 root         (0) root         (0)     1981 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/rpm/glimpse_Brunel_v46r0.spec
--rw-rw-rw-   0 root         (0) root         (0)      617 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/rpm/manifest.xml
--rw-rw-rw-   0 root         (0) root         (0)     1273 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/rpm/manifest_do0.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.988827 LbNightlyTools-4.0.8/testdata/rpm/rel/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/rpm/rel/PARAM_TMVAWeights_v1r2-1.0.0-1.noarch.rpm
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-1.noarch.rpm
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-4.noarch.rpm
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-toto.noarch.rpm
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/rpm/slot-config.json
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/rpm/slot-configdo0.json
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/testing-slot-2.json
--rw-rw-rw-   0 root         (0) root         (0)      381 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/testing-slot-2b.json
--rw-rw-rw-   0 root         (0) root         (0)      364 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/testing-slot-env.json
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/testing-slot-lbcore-192.json
--rw-rw-rw-   0 root         (0) root         (0)      398 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/testing-slot-lbcore-664.json
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/testing-slot-with-shared.json
--rw-rw-rw-   0 root         (0) root         (0)      219 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/testing-slot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.989827 LbNightlyTools-4.0.8/testdata/tools/
--rw-rw-rw-   0 root         (0) root         (0)      658 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/tools/manifest.xml
--rw-rw-rw-   0 root         (0) root         (0)     1273 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/tools/manifest_do0.xml
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/tools/manifest_with_pkgs.xml
--rw-rw-rw-   0 root         (0) root         (0)     1588 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/tools/manifest_with_pkgs_new.xml
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/testdata/tools/mini_manifest.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:37:05.989827 LbNightlyTools-4.0.8/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-22 08:37:05.000000 LbNightlyTools-4.0.8/utils/add_ci_webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.841811 LbNightlyTools-4.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      339 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     4969 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      487 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    15557 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/COPYING
+-rw-r--r--   0 root         (0) root         (0)     1090 2024-05-22 14:25:10.841811 LbNightlyTools-4.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.816810 LbNightlyTools-4.0.9/admin/
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/admin/LHCb_LbScripts.spectemplate
+-rwxrwxrwx   0 root         (0) root         (0)     1882 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/admin/RpmHelpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     3688 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/admin/createLbScriptsRpm
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.816810 LbNightlyTools-4.0.9/couchdb/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      982 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/Push CouchDB Nightly Builds.launch
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.816810 LbNightlyTools-4.0.9/couchdb/auth/
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/auth/validate_doc_update.js
+-rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/build_id_index.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.816810 LbNightlyTools-4.0.9/couchdb/deployment/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/deployment/_id
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/deployment/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.809810 LbNightlyTools-4.0.9/couchdb/deployment/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.817810 LbNightlyTools-4.0.9/couchdb/deployment/views/ready/
+-rw-rw-rw-   0 root         (0) root         (0)      920 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/deployment/views/ready/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.817810 LbNightlyTools-4.0.9/couchdb/frontend-stats/
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/frontend-stats/.couchappignore
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/frontend-stats/.couchapprc
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/frontend-stats/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/frontend-stats/_id
+-rw-rw-rw-   0 root         (0) root         (0)       83 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/frontend-stats/couchapp.json
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/frontend-stats/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.809810 LbNightlyTools-4.0.9/couchdb/frontend-stats/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.817810 LbNightlyTools-4.0.9/couchdb/frontend-stats/views/byDate/
+-rw-rw-rw-   0 root         (0) root         (0)     2483 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/frontend-stats/views/byDate/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.817810 LbNightlyTools-4.0.9/couchdb/merge_requests/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/merge_requests/_id
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/merge_requests/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.809810 LbNightlyTools-4.0.9/couchdb/merge_requests/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.817810 LbNightlyTools-4.0.9/couchdb/merge_requests/views/mr_slots_by_ref_slot/
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/merge_requests/views/mr_slots_by_ref_slot/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.817810 LbNightlyTools-4.0.9/couchdb/merge_requests/views/mrs/
+-rw-rw-rw-   0 root         (0) root         (0)      756 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/merge_requests/views/mrs/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.818810 LbNightlyTools-4.0.9/couchdb/names/
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/names/_id
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/names/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.810810 LbNightlyTools-4.0.9/couchdb/names/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.818810 LbNightlyTools-4.0.9/couchdb/names/views/platforms/
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/names/views/platforms/map.js
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/names/views/platforms/reduce.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.818810 LbNightlyTools-4.0.9/couchdb/names/views/projects/
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/names/views/projects/map.js
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/names/views/projects/reduce.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.818810 LbNightlyTools-4.0.9/couchdb/names/views/slots/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/names/views/slots/map.js
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/names/views/slots/reduce.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.818810 LbNightlyTools-4.0.9/couchdb/nightlies_summaries/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/nightlies_summaries/_id
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/nightlies_summaries/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.810810 LbNightlyTools-4.0.9/couchdb/nightlies_summaries/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.818810 LbNightlyTools-4.0.9/couchdb/nightlies_summaries/views/by_app_version/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/nightlies_summaries/views/by_app_version/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.819810 LbNightlyTools-4.0.9/couchdb/old_dashboard/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/old_dashboard/_id
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/old_dashboard/language
+-rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/old_dashboard/rewrites.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.819810 LbNightlyTools-4.0.9/couchdb/periodic_summaries/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/periodic_summaries/_id
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/periodic_summaries/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.810810 LbNightlyTools-4.0.9/couchdb/periodic_summaries/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.819810 LbNightlyTools-4.0.9/couchdb/periodic_summaries/views/byTime/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/periodic_summaries/views/byTime/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.819810 LbNightlyTools-4.0.9/couchdb/releases/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/releases/_id
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/releases/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.819810 LbNightlyTools-4.0.9/couchdb/releases/lists/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/releases/lists/projectBuildIds.js
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/releases/rewrites.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.810810 LbNightlyTools-4.0.9/couchdb/releases/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.819810 LbNightlyTools-4.0.9/couchdb/releases/views/projectBuildIds/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/releases/views/projectBuildIds/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.819810 LbNightlyTools-4.0.9/couchdb/summaries/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/summaries/_id
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/summaries/language
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/summaries/rewrites.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.810810 LbNightlyTools-4.0.9/couchdb/summaries/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.819810 LbNightlyTools-4.0.9/couchdb/summaries/views/byDay/
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/summaries/views/byDay/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.820810 LbNightlyTools-4.0.9/couchdb/summaries/views/lastBuildId/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/summaries/views/lastBuildId/map.js
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/summaries/views/lastBuildId/reduce.js
+-rwxrwxrwx   0 root         (0) root         (0)     3600 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/couchdb/webapp_testbench.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.820810 LbNightlyTools-4.0.9/cron/
+-rwxrwxrwx   0 root         (0) root         (0)     1858 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/cron/cleanup_artifacts.sh
+-rw-rw-rw-   0 root         (0) root         (0)      433 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/cron/logrotate.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.820810 LbNightlyTools-4.0.9/docs/
+-rw-rw-rw-   0 root         (0) root         (0)    25550 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/Interactive builds of LHCb projects.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/LHCbPR2.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.820810 LbNightlyTools-4.0.9/docs/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/configuration/Example.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.821810 LbNightlyTools-4.0.9/docs/examples/
+-rwxrwxrwx   0 root         (0) root         (0)     1247 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/examples/lbpr-example
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/jenkins-scripts.dot
+-rw-rw-rw-   0 root         (0) root         (0)   142880 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/jenkins-scripts.dot.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.823810 LbNightlyTools-4.0.9/docs/note/
+-rw-rw-rw-   0 root         (0) root         (0)   946715 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/LHCb-INT-2013-006.pdf
+-rw-rw-rw-   0 root         (0) root         (0)    24731 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/LHCb.bst
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/README.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3132 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/appendix.tex
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/bibliography.bib
+-rw-rw-rw-   0 root         (0) root         (0)    32522 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/cite.sty
+-rw-rw-rw-   0 root         (0) root         (0)      567 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/conclusions.tex
+-rw-rw-rw-   0 root         (0) root         (0)     5975 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/dashboard.tex
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/design.tex
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.824810 LbNightlyTools-4.0.9/docs/note/figs/
+-rw-rw-rw-   0 root         (0) root         (0)    60108 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/figs/cdash-1.png
+-rw-rw-rw-   0 root         (0) root         (0)    97134 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/figs/cdash-2.png
+-rw-rw-rw-   0 root         (0) root         (0)   101416 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/figs/cdash-3.png
+-rw-rw-rw-   0 root         (0) root         (0)   162025 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/figs/cdash-4.png
+-rw-rw-rw-   0 root         (0) root         (0)    91381 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/figs/jenkins-1.png
+-rw-rw-rw-   0 root         (0) root         (0)    81047 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/figs/jenkins-2.png
+-rw-rw-rw-   0 root         (0) root         (0)   173109 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/figs/jenkins-3.png
+-rw-rw-rw-   0 root         (0) root         (0)   160146 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/figs/lhcb-logo.eps
+-rw-rw-rw-   0 root         (0) root         (0)    14116 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/figs/lhcb-logo.pdf
+-rw-rw-rw-   0 root         (0) root         (0)   134216 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/figs/old-summary.png
+-rw-rw-rw-   0 root         (0) root         (0)    33058 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/implementation.tex
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/introduction.tex
+-rw-rw-rw-   0 root         (0) root         (0)     5596 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/lhcb-int-2013-006.kilepr
+-rwxrwxrwx   0 root         (0) root         (0)     3645 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/listsymbols
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/main.tex
+-rw-rw-rw-   0 root         (0) root         (0)    61167 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/mciteplus.sty
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/preamble.tex
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/requirements.tex
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/title-LHCb-ANA.tex
+-rw-rw-rw-   0 root         (0) root         (0)    28723 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/note/unsrturl.bst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.824810 LbNightlyTools-4.0.9/docs/operation/
+-rw-rw-rw-   0 root         (0) root         (0)      974 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/operation/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)    26499 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/operation/NightlyBuildsOperation.html
+-rw-rw-rw-   0 root         (0) root         (0)    11288 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/operation/NightlyBuildsOperation.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.824810 LbNightlyTools-4.0.9/docs/operation/images/
+-rw-rw-rw-   0 root         (0) root         (0)      788 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/operation/images/jenkins-jobs.dot
+-rw-rw-rw-   0 root         (0) root         (0)    32492 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/operation/images/jenkins-jobs.dot.png
+-rw-rw-rw-   0 root         (0) root         (0)     7965 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/docs/pylint.rc
+-rw-rw-rw-   0 root         (0) root         (0)      181 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.811810 LbNightlyTools-4.0.9/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.825811 LbNightlyTools-4.0.9/python/LbMsg/
+-rwxrwxrwx   0 root         (0) root         (0)     3452 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbMsg/BuildMsg.py
+-rw-rw-rw-   0 root         (0) root         (0)     4609 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbMsg/Common.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbMsg/TestMsg.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbMsg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.826810 LbNightlyTools-4.0.9/python/LbNightlyTools/
+-rw-rw-rw-   0 root         (0) root         (0)     4457 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/ArtifactsServer.py
+-rw-rw-rw-   0 root         (0) root         (0)    12315 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/BuildLogScanner.py
+-rw-rw-rw-   0 root         (0) root         (0)    33812 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/BuildMethods.py
+-rw-rw-rw-   0 root         (0) root         (0)     3715 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/CheckSlotPreconditions.py
+-rw-rw-rw-   0 root         (0) root         (0)    34819 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/CheckoutMethods.py
+-rw-rw-rw-   0 root         (0) root         (0)    81329 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Configuration.py
+-rwxrwxrwx   0 root         (0) root         (0)     5166 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/GetNightlyRefs.py
+-rw-rw-rw-   0 root         (0) root         (0)     8060 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/GitlabUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)    18542 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/HTMLUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4305 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/LbScriptsUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)    21375 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/MergeRequestBuilds.py
+-rw-rw-rw-   0 root         (0) root         (0)     6152 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/ProcUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6339 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.828811 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/
+-rw-rw-rw-   0 root         (0) root         (0)    36766 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/Build.py
+-rw-rw-rw-   0 root         (0) root         (0)    15261 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/Checkout.py
+-rw-rw-rw-   0 root         (0) root         (0)    15846 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/CollectBuildLogs.py
+-rwxrwxrwx   0 root         (0) root         (0)    28293 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/Common.py
+-rw-rw-rw-   0 root         (0) root         (0)    14322 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/EnabledSlots.py
+-rw-rw-rw-   0 root         (0) root         (0)    14433 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/GitlabMR.py
+-rw-rw-rw-   0 root         (0) root         (0)     7665 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/Index.py
+-rw-rw-rw-   0 root         (0) root         (0)    29122 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/Install.py
+-rw-rw-rw-   0 root         (0) root         (0)     4861 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/Preconditions.py
+-rw-rw-rw-   0 root         (0) root         (0)    17852 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/Release.py
+-rw-rw-rw-   0 root         (0) root         (0)    14262 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/Test.py
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24776 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/_entry_points.py
+-rw-rw-rw-   0 root         (0) root         (0)     3002 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/extract.php
+-rw-rw-rw-   0 root         (0) root         (0)      999 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/listzip.php
+-rw-rw-rw-   0 root         (0) root         (0)     2663 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/wrapcmd.py
+-rw-rw-rw-   0 root         (0) root         (0)    46060 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/Utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1479 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.830810 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      921 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_apptainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     8920 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_build.py
+-rw-rw-rw-   0 root         (0) root         (0)    19337 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_build_script.py
+-rw-rw-rw-   0 root         (0) root         (0)    12989 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_checkout.py
+-rw-rw-rw-   0 root         (0) root         (0)     4202 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_checkout_script.py
+-rw-rw-rw-   0 root         (0) root         (0)     9317 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_config_load.py
+-rw-rw-rw-   0 root         (0) root         (0)     2140 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_config_pickle.py
+-rw-rw-rw-   0 root         (0) root         (0)    15201 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2967 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_configuration_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     3233 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_copytree.py
+-rw-rw-rw-   0 root         (0) root         (0)     5953 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_coverity_support.py
+-rw-rw-rw-   0 root         (0) root         (0)    14609 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_enabled_slots_script.py
+-rw-rw-rw-   0 root         (0) root         (0)     7275 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_gitlab_mr_script.py
+-rw-rw-rw-   0 root         (0) root         (0)     1872 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_indexer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2597 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_install.py
+-rw-rw-rw-   0 root         (0) root         (0)     1759 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_jobconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)    11780 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_merge_request_builds.py
+-rw-rw-rw-   0 root         (0) root         (0)     8088 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_pack.py
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_precond.py
+-rw-rw-rw-   0 root         (0) root         (0)    10940 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_rel_gen_script.py
+-rw-rw-rw-   0 root         (0) root         (0)     8064 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_release_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_retry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2457 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4594 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_wrapcmd.py
+-rw-rw-rw-   0 root         (0) root         (0)     3338 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbNightlyTools/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.827810 LbNightlyTools-4.0.9/python/LbNightlyTools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1090 2024-05-22 14:25:10.000000 LbNightlyTools-4.0.9/python/LbNightlyTools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11572 2024-05-22 14:25:10.000000 LbNightlyTools-4.0.9/python/LbNightlyTools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 14:25:10.000000 LbNightlyTools-4.0.9/python/LbNightlyTools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     2752 2024-05-22 14:25:10.000000 LbNightlyTools-4.0.9/python/LbNightlyTools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 14:25:10.000000 LbNightlyTools-4.0.9/python/LbNightlyTools.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      155 2024-05-22 14:25:10.000000 LbNightlyTools-4.0.9/python/LbNightlyTools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-05-22 14:25:10.000000 LbNightlyTools-4.0.9/python/LbNightlyTools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.831811 LbNightlyTools-4.0.9/python/LbPR/
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbPR/LbPRJobManager.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbPR/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17311 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbPR/_entry_points.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.831811 LbNightlyTools-4.0.9/python/LbPeriodicTools/
+-rw-rw-rw-   0 root         (0) root         (0)     4171 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbPeriodicTools/LbPeriodicStarter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbPeriodicTools/LbPeriodicTest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2178 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbPeriodicTools/LbPeriodicTestSchedule.py
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbPeriodicTools/TestSchedule.xsd
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbPeriodicTools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10067 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbPeriodicTools/_entry_points.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.831811 LbNightlyTools-4.0.9/python/LbPeriodicTools/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbPeriodicTools/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2619 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbPeriodicTools/tests/test_LHCbPR.py
+-rw-rw-rw-   0 root         (0) root         (0)     3561 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbPeriodicTools/tests/test_Starter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4012 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbPeriodicTools/tests/test_XMLParsing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.832810 LbNightlyTools-4.0.9/python/LbRPMTools/
+-rw-rw-rw-   0 root         (0) root         (0)    10184 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbRPMTools/LHCbCompatSpecBuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)    22912 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbRPMTools/LHCbExternalsSpecBuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)    10040 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbRPMTools/LHCbGenericSpecBuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)    16527 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbRPMTools/LHCbLbScriptsSpecBuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8700 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbRPMTools/LHCbMetaSpecBuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)    54217 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbRPMTools/LHCbRPMSpecBuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)    29932 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbRPMTools/PackageSlot.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbRPMTools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.833810 LbNightlyTools-4.0.9/python/LbRPMTools/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbRPMTools/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6060 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbRPMTools/tests/test_ExternalSpec.py
+-rw-rw-rw-   0 root         (0) root         (0)    14756 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbRPMTools/tests/test_PackageSlot.py
+-rw-rw-rw-   0 root         (0) root         (0)    18876 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbRPMTools/tests/test_Spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.833810 LbNightlyTools-4.0.9/python/LbTools/
+-rw-rw-rw-   0 root         (0) root         (0)     5602 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbTools/Manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1676 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbTools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.833810 LbNightlyTools-4.0.9/python/LbTools/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3811 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbTools/tests/test_XMLParsing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1653 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/python/LbTools/tests/test_toolchain_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-22 14:25:10.842810 LbNightlyTools-4.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    11055 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.834810 LbNightlyTools-4.0.9/testdata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.811810 LbNightlyTools-4.0.9/testdata/artifacts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.811810 LbNightlyTools-4.0.9/testdata/artifacts/packs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.834810 LbNightlyTools-4.0.9/testdata/artifacts/packs/src/
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/artifacts/packs/src/TestProject.HEAD.testing-slot.src.zip
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.812810 LbNightlyTools-4.0.9/testdata/build_tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.811810 LbNightlyTools-4.0.9/testdata/build_tests/orig/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.834810 LbNightlyTools-4.0.9/testdata/build_tests/orig/dummy/
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/build_tests/orig/dummy/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.834810 LbNightlyTools-4.0.9/testdata/build_tests/test_project/
+-rw-rw-rw-   0 root         (0) root         (0)      258 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/build_tests/test_project/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/build_tests/test_project/lhcbproject.yml
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/build_tests/test_project/main.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     6010 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/ci-test-hook-content.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.812810 LbNightlyTools-4.0.9/testdata/collect_deps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.834810 LbNightlyTools-4.0.9/testdata/collect_deps/broken/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.812810 LbNightlyTools-4.0.9/testdata/collect_deps/broken/BadCMT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.834810 LbNightlyTools-4.0.9/testdata/collect_deps/broken/BadCMT/cmt/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/broken/BadCMT/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.834810 LbNightlyTools-4.0.9/testdata/collect_deps/broken/BadCMake/
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/broken/BadCMake/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.834810 LbNightlyTools-4.0.9/testdata/collect_deps/broken/Gaudi/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/broken/Gaudi/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/broken/Gaudi/toolchain.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      295 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/broken/conf.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.835811 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.835811 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/Brunel/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/Brunel/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.835811 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/Gaudi/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/Gaudi/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/Gaudi/toolchain.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.835811 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/LHCb/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/LHCb/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.835811 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/Lbcom/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/Lbcom/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.835811 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/NewLHCbProj/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/NewLHCbProj/lhcbproject.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.835811 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/NewProj/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/NewProj/project.info
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.835811 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/Online/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/Online/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.835811 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/Rec/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/Rec/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmake/conf.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.835811 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.812810 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/Brunel/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.835811 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/Brunel/cmt/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/Brunel/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.812810 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/Gaudi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.836810 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/Gaudi/cmt/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/Gaudi/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.812810 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/LHCb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.836810 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/LHCb/cmt/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/LHCb/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.813810 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/Lbcom/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.836810 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/Lbcom/cmt/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/Lbcom/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.836810 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/NewLHCbProj/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/NewLHCbProj/lhcbproject.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.836810 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/NewProj/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/NewProj/project.info
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.813810 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/Online/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.836810 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/Online/cmt/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/Online/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.813810 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/Rec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.836810 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/Rec/cmt/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/Rec/cmt/project.cmt
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/collect_deps/cmt/conf.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.813810 LbNightlyTools-4.0.9/testdata/coverity/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.836810 LbNightlyTools-4.0.9/testdata/coverity/bin/
+-rwxrwxrwx   0 root         (0) root         (0)     1722 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/coverity/bin/cov-analyze
+-rwxrwxrwx   0 root         (0) root         (0)     1630 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/coverity/bin/cov-build
+-rwxrwxrwx   0 root         (0) root         (0)     1787 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/coverity/bin/cov-commit-defects
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.813810 LbNightlyTools-4.0.9/testdata/coverity/build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.813810 LbNightlyTools-4.0.9/testdata/coverity/build/TEST/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.836810 LbNightlyTools-4.0.9/testdata/coverity/build/TEST/TEST_HEAD/
+-rw-rw-rw-   0 root         (0) root         (0)      310 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/coverity/build/TEST/TEST_HEAD/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.837810 LbNightlyTools-4.0.9/testdata/coverity/build/TEST/TEST_HEAD/InstallArea/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/coverity/build/TEST/TEST_HEAD/InstallArea/.empty
+-rw-rw-rw-   0 root         (0) root         (0)      256 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/coverity/build/TEST/TEST_HEAD/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.837810 LbNightlyTools-4.0.9/testdata/coverity/configs/
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/coverity/configs/coverity_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/data-packs.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.814810 LbNightlyTools-4.0.9/testdata/fix_glimpse/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.837810 LbNightlyTools-4.0.9/testdata/fix_glimpse/docs/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/fix_glimpse/docs/.glimpse_filenames
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.837810 LbNightlyTools-4.0.9/testdata/fix_glimpse/level1/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/fix_glimpse/level1/.glimpse_filenames
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.837810 LbNightlyTools-4.0.9/testdata/fix_glimpse/level1/level2/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/fix_glimpse/level1/level2/.glimpse_filenames
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.814810 LbNightlyTools-4.0.9/testdata/fix_glimpse/levelA/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.837810 LbNightlyTools-4.0.9/testdata/fix_glimpse/levelA/levelB/
+-rw-rw-rw-   0 root         (0) root         (0)       10 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/fix_glimpse/levelA/levelB/.glimpse_filenames
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.837810 LbNightlyTools-4.0.9/testdata/fix_glimpse/untouched/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/fix_glimpse/untouched/.glimpse_filenames
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.814810 LbNightlyTools-4.0.9/testdata/indexer/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.814810 LbNightlyTools-4.0.9/testdata/indexer/AProject/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.814810 LbNightlyTools-4.0.9/testdata/indexer/AProject/InstallArea/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.837810 LbNightlyTools-4.0.9/testdata/indexer/AProject/InstallArea/cmake/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/InstallArea/cmake/AProjectConfig.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.837810 LbNightlyTools-4.0.9/testdata/indexer/AProject/InstallArea/include/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/InstallArea/include/GeneratedHeader.h
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/InstallArea/include/MyHeader.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.837810 LbNightlyTools-4.0.9/testdata/indexer/AProject/InstallArea/python/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/InstallArea/python/AProject_merged_confDb.py
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/InstallArea/python/GeneratedPython.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.838811 LbNightlyTools-4.0.9/testdata/indexer/AProject/InstallArea/python/MyPackage/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackageConf.py
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackage_confDb.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackage_user_confDb.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/InstallArea/python/MyPackage/SomeModule.py
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/InstallArea/python/MyPackage/SomethingConf.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/InstallArea/python/MyPackage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.814810 LbNightlyTools-4.0.9/testdata/indexer/AProject/MyPackage/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.838811 LbNightlyTools-4.0.9/testdata/indexer/AProject/MyPackage/Headers/
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/MyPackage/Headers/MyHeader.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.814810 LbNightlyTools-4.0.9/testdata/indexer/AProject/MyPackage/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.838811 LbNightlyTools-4.0.9/testdata/indexer/AProject/MyPackage/python/MyPackage/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/MyPackage/python/MyPackage/SomeModule.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/MyPackage/python/MyPackage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.838811 LbNightlyTools-4.0.9/testdata/indexer/AProject/MyPackage/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/MyPackage/scripts/MyScript
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.838811 LbNightlyTools-4.0.9/testdata/indexer/AProject/MyPackage/src/
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/MyPackage/src/MySource.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.839810 LbNightlyTools-4.0.9/testdata/indexer/AProject/build.dir/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/indexer/AProject/build.dir/IgnoredSource.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.839810 LbNightlyTools-4.0.9/testdata/periodic_tests/
+-rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/periodic_tests/lhcbpr_schedule.xml
+-rw-rw-rw-   0 root         (0) root         (0)      743 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/periodic_tests/schedule.xml
+-rw-rw-rw-   0 root         (0) root         (0)      402 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/periodic_tests/scheduleIncorrect.xml
+-rw-rw-rw-   0 root         (0) root         (0)    15858 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/periodic_tests/slotbuilds.json
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/periodic_tests/starter_schedule.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.840810 LbNightlyTools-4.0.9/testdata/rpm/
+-rw-rw-rw-   0 root         (0) root         (0)     1265 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/rpm/Brunel_v46r0.spec
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/rpm/Brunel_v46r0_x86_64-slc6-gcc48-opt.spec
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/rpm/Gaudi_v27r0_x86_64-slc6-gcc49-do0.spec
+-rw-rw-rw-   0 root         (0) root         (0)     7196 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/rpm/LCG_68_externalsDict.json
+-rw-rw-rw-   0 root         (0) root         (0)     3230 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/rpm/PARAM_TMVAWeights.spec
+-rw-rw-rw-   0 root         (0) root         (0)     3230 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/rpm/PARAM_TMVAWeights_rel5.spec
+-rw-rw-rw-   0 root         (0) root         (0)      938 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/rpm/datapkg-slot-config.json
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/rpm/glimpse_Brunel_v46r0.spec
+-rw-rw-rw-   0 root         (0) root         (0)      617 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/rpm/manifest.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/rpm/manifest_do0.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.840810 LbNightlyTools-4.0.9/testdata/rpm/rel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/rpm/rel/PARAM_TMVAWeights_v1r2-1.0.0-1.noarch.rpm
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-1.noarch.rpm
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-4.noarch.rpm
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-toto.noarch.rpm
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/rpm/slot-config.json
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/rpm/slot-configdo0.json
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/testing-slot-2.json
+-rw-rw-rw-   0 root         (0) root         (0)      381 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/testing-slot-2b.json
+-rw-rw-rw-   0 root         (0) root         (0)      364 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/testing-slot-env.json
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/testing-slot-lbcore-192.json
+-rw-rw-rw-   0 root         (0) root         (0)      398 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/testing-slot-lbcore-664.json
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/testing-slot-with-shared.json
+-rw-rw-rw-   0 root         (0) root         (0)      219 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/testing-slot.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.841811 LbNightlyTools-4.0.9/testdata/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      658 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/tools/manifest.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/tools/manifest_do0.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/tools/manifest_with_pkgs.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1588 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/tools/manifest_with_pkgs_new.xml
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/testdata/tools/mini_manifest.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:25:10.841811 LbNightlyTools-4.0.9/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-22 14:25:09.000000 LbNightlyTools-4.0.9/utils/add_ci_webhook.py
```

### Comparing `LbNightlyTools-4.0.8/.gitlab-ci.yml` & `LbNightlyTools-4.0.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/CHANGELOG.md` & `LbNightlyTools-4.0.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/COPYING` & `LbNightlyTools-4.0.9/COPYING`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/PKG-INFO` & `LbNightlyTools-4.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbNightlyTools
-Version: 4.0.8
+Version: 4.0.9
 Summary: LHCb Nightly tools
 Home-page: https://gitlab.cern.ch/lhcb-core/LbNightlyTools
 Author: CERN - LHCb Core Software
 Author-email: lhcb-core-soft@cern.ch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `LbNightlyTools-4.0.8/admin/LHCb_LbScripts.spectemplate` & `LbNightlyTools-4.0.9/admin/LHCb_LbScripts.spectemplate`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/admin/RpmHelpers.py` & `LbNightlyTools-4.0.9/admin/RpmHelpers.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/admin/createLbScriptsRpm` & `LbNightlyTools-4.0.9/admin/createLbScriptsRpm`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/couchdb/Push CouchDB Nightly Builds.launch` & `LbNightlyTools-4.0.9/couchdb/Push CouchDB Nightly Builds.launch`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/couchdb/README.md` & `LbNightlyTools-4.0.9/couchdb/README.md`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/couchdb/auth/validate_doc_update.js` & `LbNightlyTools-4.0.9/couchdb/auth/validate_doc_update.js`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/couchdb/deployment/views/ready/map.js` & `LbNightlyTools-4.0.9/couchdb/deployment/views/ready/map.js`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/couchdb/frontend-stats/README.md` & `LbNightlyTools-4.0.9/couchdb/frontend-stats/README.md`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/couchdb/frontend-stats/views/byDate/map.js` & `LbNightlyTools-4.0.9/couchdb/frontend-stats/views/byDate/map.js`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/couchdb/merge_requests/views/mrs/map.js` & `LbNightlyTools-4.0.9/couchdb/merge_requests/views/mrs/map.js`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/couchdb/old_dashboard/rewrites.json` & `LbNightlyTools-4.0.9/couchdb/old_dashboard/rewrites.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/couchdb/webapp_testbench.py` & `LbNightlyTools-4.0.9/couchdb/webapp_testbench.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/cron/cleanup_artifacts.sh` & `LbNightlyTools-4.0.9/cron/cleanup_artifacts.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/Interactive builds of LHCb projects.ipynb` & `LbNightlyTools-4.0.9/docs/Interactive builds of LHCb projects.ipynb`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/LHCbPR2.md` & `LbNightlyTools-4.0.9/docs/LHCbPR2.md`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/configuration/Example.py` & `LbNightlyTools-4.0.9/docs/configuration/Example.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/examples/lbpr-example` & `LbNightlyTools-4.0.9/docs/examples/lbpr-example`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/jenkins-scripts.dot` & `LbNightlyTools-4.0.9/docs/jenkins-scripts.dot`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/jenkins-scripts.dot.png` & `LbNightlyTools-4.0.9/docs/jenkins-scripts.dot.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/LHCb-INT-2013-006.pdf` & `LbNightlyTools-4.0.9/docs/note/LHCb-INT-2013-006.pdf`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/LHCb.bst` & `LbNightlyTools-4.0.9/docs/note/LHCb.bst`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/Makefile` & `LbNightlyTools-4.0.9/docs/note/Makefile`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/appendix.tex` & `LbNightlyTools-4.0.9/docs/note/appendix.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/bibliography.bib` & `LbNightlyTools-4.0.9/docs/note/bibliography.bib`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/cite.sty` & `LbNightlyTools-4.0.9/docs/note/cite.sty`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/conclusions.tex` & `LbNightlyTools-4.0.9/docs/note/conclusions.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/dashboard.tex` & `LbNightlyTools-4.0.9/docs/note/dashboard.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/design.tex` & `LbNightlyTools-4.0.9/docs/note/design.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/figs/cdash-1.png` & `LbNightlyTools-4.0.9/docs/note/figs/cdash-1.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/figs/cdash-2.png` & `LbNightlyTools-4.0.9/docs/note/figs/cdash-2.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/figs/cdash-3.png` & `LbNightlyTools-4.0.9/docs/note/figs/cdash-3.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/figs/cdash-4.png` & `LbNightlyTools-4.0.9/docs/note/figs/cdash-4.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/figs/jenkins-1.png` & `LbNightlyTools-4.0.9/docs/note/figs/jenkins-1.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/figs/jenkins-2.png` & `LbNightlyTools-4.0.9/docs/note/figs/jenkins-2.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/figs/jenkins-3.png` & `LbNightlyTools-4.0.9/docs/note/figs/jenkins-3.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/figs/lhcb-logo.eps` & `LbNightlyTools-4.0.9/docs/note/figs/lhcb-logo.eps`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/figs/lhcb-logo.pdf` & `LbNightlyTools-4.0.9/docs/note/figs/lhcb-logo.pdf`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/figs/old-summary.png` & `LbNightlyTools-4.0.9/docs/note/figs/old-summary.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/implementation.tex` & `LbNightlyTools-4.0.9/docs/note/implementation.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/introduction.tex` & `LbNightlyTools-4.0.9/docs/note/introduction.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/lhcb-int-2013-006.kilepr` & `LbNightlyTools-4.0.9/docs/note/lhcb-int-2013-006.kilepr`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/listsymbols` & `LbNightlyTools-4.0.9/docs/note/listsymbols`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/main.tex` & `LbNightlyTools-4.0.9/docs/note/main.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/mciteplus.sty` & `LbNightlyTools-4.0.9/docs/note/mciteplus.sty`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/preamble.tex` & `LbNightlyTools-4.0.9/docs/note/preamble.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/requirements.tex` & `LbNightlyTools-4.0.9/docs/note/requirements.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/title-LHCb-ANA.tex` & `LbNightlyTools-4.0.9/docs/note/title-LHCb-ANA.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/note/unsrturl.bst` & `LbNightlyTools-4.0.9/docs/note/unsrturl.bst`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/operation/Makefile` & `LbNightlyTools-4.0.9/docs/operation/Makefile`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/operation/NightlyBuildsOperation.html` & `LbNightlyTools-4.0.9/docs/operation/NightlyBuildsOperation.html`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/operation/NightlyBuildsOperation.rst` & `LbNightlyTools-4.0.9/docs/operation/NightlyBuildsOperation.rst`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/operation/images/jenkins-jobs.dot` & `LbNightlyTools-4.0.9/docs/operation/images/jenkins-jobs.dot`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/operation/images/jenkins-jobs.dot.png` & `LbNightlyTools-4.0.9/docs/operation/images/jenkins-jobs.dot.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/docs/pylint.rc` & `LbNightlyTools-4.0.9/docs/pylint.rc`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbMsg/BuildMsg.py` & `LbNightlyTools-4.0.9/python/LbMsg/BuildMsg.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbMsg/Common.py` & `LbNightlyTools-4.0.9/python/LbMsg/Common.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbMsg/TestMsg.py` & `LbNightlyTools-4.0.9/python/LbMsg/TestMsg.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/ArtifactsServer.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/ArtifactsServer.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/BuildLogScanner.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/BuildLogScanner.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/BuildMethods.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/BuildMethods.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/CheckSlotPreconditions.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/CheckSlotPreconditions.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/CheckoutMethods.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/CheckoutMethods.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Configuration.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Configuration.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/GetNightlyRefs.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/GetNightlyRefs.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/GitlabUtils.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/GitlabUtils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/HTMLUtils.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/HTMLUtils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/LbScriptsUtils.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/LbScriptsUtils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/MergeRequestBuilds.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/MergeRequestBuilds.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/ProcUtils.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/ProcUtils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Repository.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Repository.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/Build.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/Build.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/Checkout.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/Checkout.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/CollectBuildLogs.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/CollectBuildLogs.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/Common.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/Common.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/EnabledSlots.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/EnabledSlots.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/GitlabMR.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/GitlabMR.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/Index.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/Index.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/Install.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/Install.py`

 * *Files 0% similar despite different names*

```diff
@@ -670,15 +670,15 @@
             expected_files_patterns = [
                 re.compile(
                     ".*/{}\\..*\\.{}\\.".format(re.escape(project), re.escape(platform))
                 )
                 for project in (opts.projects or [])
                 for platform in (opts.platforms or [])
                 if platform != "shared"  # the shared pack is optional
-                and project.lower() not in ("DDDB", "PARAM")  # ignore data projects
+                and project.upper() not in ("DDDB", "PARAM")  # ignore data projects
             ]
             tarfiles = [
                 "packs/{0}/{1}".format(subdir, f)
                 for subdir in listdir(url + "/packs")
                 for f in listdir(url + "/packs/" + subdir)
                 if f.endswith(".tar.bz2") or f.endswith(".zip")
             ]
```

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/Preconditions.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/Preconditions.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/Release.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/Release.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/Test.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/Test.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/__init__.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/_entry_points.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/_entry_points.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/extract.php` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/extract.php`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/listzip.php` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/listzip.php`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Scripts/wrapcmd.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Scripts/wrapcmd.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/Utils.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/Utils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/__init__.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/__init__.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/__init__.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_apptainer.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_apptainer.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_build.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_build_script.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_build_script.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_checkout.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_checkout.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_checkout_script.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_checkout_script.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_config_load.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_config_load.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_config_pickle.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_config_pickle.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_configuration.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_configuration_check.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_configuration_check.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_copytree.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_copytree.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_coverity_support.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_coverity_support.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_enabled_slots_script.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_enabled_slots_script.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_gitlab_mr_script.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_gitlab_mr_script.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_indexer.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_indexer.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_install.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_jobconfig.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_jobconfig.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_merge_request_builds.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_merge_request_builds.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_pack.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_pack.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_precond.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_precond.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_rel_gen_script.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_rel_gen_script.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_release_poll.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_release_poll.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_repository.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_retry.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_utils.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/test_wrapcmd.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/test_wrapcmd.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools/tests/utils.py` & `LbNightlyTools-4.0.9/python/LbNightlyTools/tests/utils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools.egg-info/PKG-INFO` & `LbNightlyTools-4.0.9/python/LbNightlyTools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbNightlyTools
-Version: 4.0.8
+Version: 4.0.9
 Summary: LHCb Nightly tools
 Home-page: https://gitlab.cern.ch/lhcb-core/LbNightlyTools
 Author: CERN - LHCb Core Software
 Author-email: lhcb-core-soft@cern.ch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools.egg-info/SOURCES.txt` & `LbNightlyTools-4.0.9/python/LbNightlyTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbNightlyTools.egg-info/entry_points.txt` & `LbNightlyTools-4.0.9/python/LbNightlyTools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbPR/LbPRJobManager.py` & `LbNightlyTools-4.0.9/python/LbPR/LbPRJobManager.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbPR/_entry_points.py` & `LbNightlyTools-4.0.9/python/LbPR/_entry_points.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbPeriodicTools/LbPeriodicStarter.py` & `LbNightlyTools-4.0.9/python/LbPeriodicTools/LbPeriodicStarter.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbPeriodicTools/LbPeriodicTest.py` & `LbNightlyTools-4.0.9/python/LbPeriodicTools/LbPeriodicTest.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbPeriodicTools/LbPeriodicTestSchedule.py` & `LbNightlyTools-4.0.9/python/LbPeriodicTools/LbPeriodicTestSchedule.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbPeriodicTools/TestSchedule.xsd` & `LbNightlyTools-4.0.9/python/LbPeriodicTools/TestSchedule.xsd`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbPeriodicTools/_entry_points.py` & `LbNightlyTools-4.0.9/python/LbPeriodicTools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbPeriodicTools/tests/test_LHCbPR.py` & `LbNightlyTools-4.0.9/python/LbPeriodicTools/tests/test_LHCbPR.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbPeriodicTools/tests/test_Starter.py` & `LbNightlyTools-4.0.9/python/LbPeriodicTools/tests/test_Starter.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbPeriodicTools/tests/test_XMLParsing.py` & `LbNightlyTools-4.0.9/python/LbPeriodicTools/tests/test_XMLParsing.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbRPMTools/LHCbCompatSpecBuilder.py` & `LbNightlyTools-4.0.9/python/LbRPMTools/LHCbCompatSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbRPMTools/LHCbExternalsSpecBuilder.py` & `LbNightlyTools-4.0.9/python/LbRPMTools/LHCbExternalsSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbRPMTools/LHCbGenericSpecBuilder.py` & `LbNightlyTools-4.0.9/python/LbRPMTools/LHCbGenericSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbRPMTools/LHCbLbScriptsSpecBuilder.py` & `LbNightlyTools-4.0.9/python/LbRPMTools/LHCbLbScriptsSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbRPMTools/LHCbMetaSpecBuilder.py` & `LbNightlyTools-4.0.9/python/LbRPMTools/LHCbMetaSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbRPMTools/LHCbRPMSpecBuilder.py` & `LbNightlyTools-4.0.9/python/LbRPMTools/LHCbRPMSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbRPMTools/PackageSlot.py` & `LbNightlyTools-4.0.9/python/LbRPMTools/PackageSlot.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbRPMTools/tests/test_ExternalSpec.py` & `LbNightlyTools-4.0.9/python/LbRPMTools/tests/test_ExternalSpec.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbRPMTools/tests/test_PackageSlot.py` & `LbNightlyTools-4.0.9/python/LbRPMTools/tests/test_PackageSlot.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbRPMTools/tests/test_Spec.py` & `LbNightlyTools-4.0.9/python/LbRPMTools/tests/test_Spec.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbTools/Manifest.py` & `LbNightlyTools-4.0.9/python/LbTools/Manifest.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbTools/__init__.py` & `LbNightlyTools-4.0.9/python/LbTools/__init__.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbTools/tests/test_XMLParsing.py` & `LbNightlyTools-4.0.9/python/LbTools/tests/test_XMLParsing.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/python/LbTools/tests/test_toolchain_info.py` & `LbNightlyTools-4.0.9/python/LbTools/tests/test_toolchain_info.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/setup.py` & `LbNightlyTools-4.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/artifacts/packs/src/TestProject.HEAD.testing-slot.src.zip` & `LbNightlyTools-4.0.9/testdata/artifacts/packs/src/TestProject.HEAD.testing-slot.src.zip`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/ci-test-hook-content.json` & `LbNightlyTools-4.0.9/testdata/ci-test-hook-content.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/collect_deps/cmake/conf.json` & `LbNightlyTools-4.0.9/testdata/collect_deps/cmake/conf.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/collect_deps/cmt/conf.json` & `LbNightlyTools-4.0.9/testdata/collect_deps/cmt/conf.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/coverity/bin/cov-analyze` & `LbNightlyTools-4.0.9/testdata/coverity/bin/cov-analyze`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/coverity/bin/cov-build` & `LbNightlyTools-4.0.9/testdata/coverity/bin/cov-build`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/coverity/bin/cov-commit-defects` & `LbNightlyTools-4.0.9/testdata/coverity/bin/cov-commit-defects`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/periodic_tests/lhcbpr_schedule.xml` & `LbNightlyTools-4.0.9/testdata/periodic_tests/lhcbpr_schedule.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/periodic_tests/schedule.xml` & `LbNightlyTools-4.0.9/testdata/periodic_tests/schedule.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/periodic_tests/slotbuilds.json` & `LbNightlyTools-4.0.9/testdata/periodic_tests/slotbuilds.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/periodic_tests/starter_schedule.xml` & `LbNightlyTools-4.0.9/testdata/periodic_tests/starter_schedule.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/rpm/Brunel_v46r0.spec` & `LbNightlyTools-4.0.9/testdata/rpm/Brunel_v46r0.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/rpm/Brunel_v46r0_x86_64-slc6-gcc48-opt.spec` & `LbNightlyTools-4.0.9/testdata/rpm/Brunel_v46r0_x86_64-slc6-gcc48-opt.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/rpm/Gaudi_v27r0_x86_64-slc6-gcc49-do0.spec` & `LbNightlyTools-4.0.9/testdata/rpm/Gaudi_v27r0_x86_64-slc6-gcc49-do0.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/rpm/LCG_68_externalsDict.json` & `LbNightlyTools-4.0.9/testdata/rpm/LCG_68_externalsDict.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/rpm/PARAM_TMVAWeights.spec` & `LbNightlyTools-4.0.9/testdata/rpm/PARAM_TMVAWeights.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/rpm/PARAM_TMVAWeights_rel5.spec` & `LbNightlyTools-4.0.9/testdata/rpm/PARAM_TMVAWeights_rel5.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/rpm/datapkg-slot-config.json` & `LbNightlyTools-4.0.9/testdata/rpm/datapkg-slot-config.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/rpm/glimpse_Brunel_v46r0.spec` & `LbNightlyTools-4.0.9/testdata/rpm/glimpse_Brunel_v46r0.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/rpm/manifest.xml` & `LbNightlyTools-4.0.9/testdata/rpm/manifest.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/rpm/manifest_do0.xml` & `LbNightlyTools-4.0.9/testdata/rpm/manifest_do0.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/rpm/slot-config.json` & `LbNightlyTools-4.0.9/testdata/rpm/slot-config.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/rpm/slot-configdo0.json` & `LbNightlyTools-4.0.9/testdata/rpm/slot-configdo0.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/tools/manifest.xml` & `LbNightlyTools-4.0.9/testdata/tools/manifest.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/tools/manifest_do0.xml` & `LbNightlyTools-4.0.9/testdata/tools/manifest_do0.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/tools/manifest_with_pkgs.xml` & `LbNightlyTools-4.0.9/testdata/tools/manifest_with_pkgs.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/testdata/tools/manifest_with_pkgs_new.xml` & `LbNightlyTools-4.0.9/testdata/tools/manifest_with_pkgs_new.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.8/utils/add_ci_webhook.py` & `LbNightlyTools-4.0.9/utils/add_ci_webhook.py`

 * *Files identical despite different names*

