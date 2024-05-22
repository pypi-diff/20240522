# Comparing `tmp/edgy-0.9.1.tar.gz` & `tmp/edgy-0.9.2.tar.gz`

## Comparing `edgy-0.9.1.tar` & `edgy-0.9.2.tar`

### file list

```diff
@@ -1,122 +1,122 @@
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/__main__.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/exceptions.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/py.typed
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/testclient.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/types.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/__init__.py
--rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/base.py
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/cli.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/constants.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/decorators.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/env.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/exceptions.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/__init__.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/branches.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/check.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/current.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/downgrade.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/edit.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/heads.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/history.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/init.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/inspectdb.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/list_templates.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/makemigrations.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/merge.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/migrate.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/revision.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/show.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/stamp.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/shell/__init__.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/shell/base.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/shell/enums.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/shell/ipython.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/shell/ptpython.py
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/operations/shell/utils.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/templates/default/README
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/templates/default/alembic.ini.mako
--rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/templates/default/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/cli/templates/default/script.py.mako
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/conf/__init__.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/conf/config.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/conf/enums.py
--rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/conf/functional.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/conf/global_settings.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/conf/module_import.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/contrib/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/contrib/multi_tenancy/__init__.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/contrib/multi_tenancy/base.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/contrib/multi_tenancy/exceptions.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/contrib/multi_tenancy/metaclasses.py
--rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/contrib/multi_tenancy/models.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/contrib/multi_tenancy/registry.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/contrib/multi_tenancy/settings.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/contrib/multi_tenancy/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/__init__.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/datastructures.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/events.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/sync.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/connection/__init__.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/connection/database.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/connection/registry.py
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/connection/schemas.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/constants.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/context_vars.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/datastructures.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/fields/__init__.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/fields/_base_fk.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/fields/_internal.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/fields/_validators.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/fields/base.py
--rw-r--r--   0        0        0    15633 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/fields/core.py
--rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/fields/foreign_keys.py
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/fields/many_to_many.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/fields/one_to_one_keys.py
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/fields/ref_foreign_key.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/models/__init__.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/models/_internal.py
--rw-r--r--   0        0        0    10911 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/models/base.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/models/managers.py
--rw-r--r--   0        0        0    22323 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/models/metaclasses.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/models/model.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/models/model_proxy.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/models/model_reference.py
--rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/models/row.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/models/utils.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/models/mixins/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/models/mixins/generics.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/querysets/__init__.py
--rw-r--r--   0        0        0    38457 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/querysets/base.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/querysets/clauses.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/querysets/mixins.py
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/querysets/prefetch.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/querysets/protocols.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/relationships/__init__.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/relationships/related_field.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/db/relationships/relation.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/extras/__init__.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/extras/base.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/extras/extra.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/signals/__init__.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/signals/handlers.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/signals/signal.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/terminal/__init__.py
--rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/terminal/base.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/terminal/print.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/terminal/terminal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/utils/__init__.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/utils/functional.py
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/utils/models.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/core/utils/sync.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/protocols/__init__.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/protocols/many_relationship.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/protocols/queryset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/utils/__init__.py
--rw-r--r--   0        0        0    11933 2020-02-02 00:00:00.000000 edgy-0.9.1/edgy/utils/inspect.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 edgy-0.9.1/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 edgy-0.9.1/LICENSE
--rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 edgy-0.9.1/README.md
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 edgy-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    14901 2020-02-02 00:00:00.000000 edgy-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/__main__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/exceptions.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/py.typed
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/testclient.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/types.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/__init__.py
+-rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/base.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/cli.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/constants.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/decorators.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/env.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/exceptions.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/__init__.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/branches.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/check.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/current.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/downgrade.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/edit.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/heads.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/history.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/init.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/inspectdb.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/list_templates.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/makemigrations.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/merge.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/migrate.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/revision.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/show.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/stamp.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/shell/__init__.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/shell/enums.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/operations/shell/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/templates/default/README
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/templates/default/alembic.ini.mako
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/templates/default/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/cli/templates/default/script.py.mako
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/conf/__init__.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/conf/config.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/conf/enums.py
+-rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/conf/functional.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/conf/global_settings.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/conf/module_import.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/contrib/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/contrib/multi_tenancy/__init__.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/contrib/multi_tenancy/base.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/contrib/multi_tenancy/exceptions.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/contrib/multi_tenancy/metaclasses.py
+-rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/contrib/multi_tenancy/models.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/contrib/multi_tenancy/registry.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/contrib/multi_tenancy/settings.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/contrib/multi_tenancy/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/__init__.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/datastructures.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/events.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/sync.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/connection/__init__.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/connection/database.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/connection/registry.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/connection/schemas.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/constants.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/context_vars.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/datastructures.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/fields/__init__.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/fields/_base_fk.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/fields/_internal.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/fields/_validators.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/fields/base.py
+-rw-r--r--   0        0        0    15633 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/fields/core.py
+-rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/fields/foreign_keys.py
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/fields/many_to_many.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/fields/one_to_one_keys.py
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/fields/ref_foreign_key.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/models/__init__.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/models/_internal.py
+-rw-r--r--   0        0        0    10911 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/models/base.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/models/managers.py
+-rw-r--r--   0        0        0    22323 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/models/metaclasses.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/models/model.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/models/model_proxy.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/models/model_reference.py
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/models/row.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/models/utils.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/models/mixins/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/models/mixins/generics.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/querysets/__init__.py
+-rw-r--r--   0        0        0    38457 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/querysets/base.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/querysets/clauses.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/querysets/mixins.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/querysets/prefetch.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/querysets/protocols.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/relationships/__init__.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/relationships/related_field.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/db/relationships/relation.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/extras/__init__.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/extras/base.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/extras/extra.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/signals/__init__.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/signals/handlers.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/signals/signal.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/terminal/base.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/terminal/print.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/terminal/terminal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/utils/__init__.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/utils/functional.py
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/utils/models.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/core/utils/sync.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/protocols/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/protocols/many_relationship.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/protocols/queryset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/utils/__init__.py
+-rw-r--r--   0        0        0    11933 2020-02-02 00:00:00.000000 edgy-0.9.2/edgy/utils/inspect.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 edgy-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 edgy-0.9.2/LICENSE
+-rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 edgy-0.9.2/README.md
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 edgy-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0    14901 2020-02-02 00:00:00.000000 edgy-0.9.2/PKG-INFO
```

### Comparing `edgy-0.9.1/edgy/__init__.py` & `edgy-0.9.2/edgy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 from .cli.base import Migrate
 from .conf import settings
 from .conf.global_settings import EdgySettings
 from .core.connection.database import Database, DatabaseURL
 from .core.connection.registry import Registry
 from .core.db import fields
```

### Comparing `edgy-0.9.1/edgy/cli/base.py` & `edgy-0.9.2/edgy/cli/base.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/cli.py` & `edgy-0.9.2/edgy/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Client to interact with Edgy models and migrations.
 """
+
 import inspect
 import sys
 import typing
 from functools import wraps
 
 import click
```

### Comparing `edgy-0.9.1/edgy/cli/env.py` & `edgy-0.9.2/edgy/cli/env.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/operations/__init__.py` & `edgy-0.9.2/edgy/cli/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/operations/branches.py` & `edgy-0.9.2/edgy/cli/operations/branches.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Client to interact with Edgy models and migrations.
 """
 
-
 import click
 
 from edgy.cli.base import branches as _branches
 from edgy.cli.env import MigrationEnv
 
 
 @click.option(
```

### Comparing `edgy-0.9.1/edgy/cli/operations/downgrade.py` & `edgy-0.9.2/edgy/cli/operations/downgrade.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/operations/heads.py` & `edgy-0.9.2/edgy/cli/operations/heads.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/operations/history.py` & `edgy-0.9.2/edgy/cli/operations/history.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/operations/init.py` & `edgy-0.9.2/edgy/cli/operations/init.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/operations/inspectdb.py` & `edgy-0.9.2/edgy/cli/operations/inspectdb.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/operations/makemigrations.py` & `edgy-0.9.2/edgy/cli/operations/makemigrations.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/operations/merge.py` & `edgy-0.9.2/edgy/cli/operations/merge.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/operations/migrate.py` & `edgy-0.9.2/edgy/cli/operations/migrate.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/operations/revision.py` & `edgy-0.9.2/edgy/cli/operations/revision.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/operations/stamp.py` & `edgy-0.9.2/edgy/cli/operations/stamp.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/operations/shell/base.py` & `edgy-0.9.2/edgy/cli/operations/shell/base.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/operations/shell/ipython.py` & `edgy-0.9.2/edgy/cli/operations/shell/ipython.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/operations/shell/ptpython.py` & `edgy-0.9.2/edgy/cli/operations/shell/ptpython.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/operations/shell/utils.py` & `edgy-0.9.2/edgy/cli/operations/shell/utils.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/templates/default/alembic.ini.mako` & `edgy-0.9.2/edgy/cli/templates/default/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/cli/templates/default/env.py` & `edgy-0.9.2/edgy/cli/templates/default/env.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/conf/__init__.py` & `edgy-0.9.2/edgy/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/conf/config.py` & `edgy-0.9.2/edgy/conf/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Configuration for Pydantic models."""
+
 from __future__ import annotations as _annotations
 
 from typing_extensions import TypedDict
 
 
 class ModelConfig(TypedDict, total=False):
     """
```

### Comparing `edgy-0.9.1/edgy/conf/functional.py` & `edgy-0.9.2/edgy/conf/functional.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/conf/global_settings.py` & `edgy-0.9.2/edgy/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/conf/module_import.py` & `edgy-0.9.2/edgy/conf/module_import.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/contrib/multi_tenancy/base.py` & `edgy-0.9.2/edgy/contrib/multi_tenancy/base.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/contrib/multi_tenancy/metaclasses.py` & `edgy-0.9.2/edgy/contrib/multi_tenancy/metaclasses.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/contrib/multi_tenancy/models.py` & `edgy-0.9.2/edgy/contrib/multi_tenancy/models.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/contrib/multi_tenancy/settings.py` & `edgy-0.9.2/edgy/contrib/multi_tenancy/settings.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/contrib/multi_tenancy/utils.py` & `edgy-0.9.2/edgy/contrib/multi_tenancy/utils.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/datastructures.py` & `edgy-0.9.2/edgy/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/events.py` & `edgy-0.9.2/edgy/core/events.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/sync.py` & `edgy-0.9.2/edgy/core/sync.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/connection/database.py` & `edgy-0.9.2/edgy/core/connection/database.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/connection/registry.py` & `edgy-0.9.2/edgy/core/connection/registry.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/connection/schemas.py` & `edgy-0.9.2/edgy/core/connection/schemas.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/context_vars.py` & `edgy-0.9.2/edgy/core/db/context_vars.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/datastructures.py` & `edgy-0.9.2/edgy/core/db/datastructures.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/fields/__init__.py` & `edgy-0.9.2/edgy/core/db/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/fields/_base_fk.py` & `edgy-0.9.2/edgy/core/db/fields/_base_fk.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/fields/_internal.py` & `edgy-0.9.2/edgy/core/db/fields/_internal.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/fields/_validators.py` & `edgy-0.9.2/edgy/core/db/fields/_validators.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/fields/base.py` & `edgy-0.9.2/edgy/core/db/fields/base.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/fields/core.py` & `edgy-0.9.2/edgy/core/db/fields/core.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/fields/foreign_keys.py` & `edgy-0.9.2/edgy/core/db/fields/foreign_keys.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/fields/many_to_many.py` & `edgy-0.9.2/edgy/core/db/fields/many_to_many.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/fields/one_to_one_keys.py` & `edgy-0.9.2/edgy/core/db/fields/one_to_one_keys.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/fields/ref_foreign_key.py` & `edgy-0.9.2/edgy/core/db/fields/ref_foreign_key.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/models/base.py` & `edgy-0.9.2/edgy/core/db/models/base.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/models/managers.py` & `edgy-0.9.2/edgy/core/db/models/managers.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/models/metaclasses.py` & `edgy-0.9.2/edgy/core/db/models/metaclasses.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/models/model.py` & `edgy-0.9.2/edgy/core/db/models/model.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/models/model_proxy.py` & `edgy-0.9.2/edgy/core/db/models/model_proxy.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/models/row.py` & `edgy-0.9.2/edgy/core/db/models/row.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/models/utils.py` & `edgy-0.9.2/edgy/core/db/models/utils.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/models/mixins/generics.py` & `edgy-0.9.2/edgy/core/db/models/mixins/generics.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/querysets/base.py` & `edgy-0.9.2/edgy/core/db/querysets/base.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/querysets/clauses.py` & `edgy-0.9.2/edgy/core/db/querysets/clauses.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/querysets/mixins.py` & `edgy-0.9.2/edgy/core/db/querysets/mixins.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/querysets/prefetch.py` & `edgy-0.9.2/edgy/core/db/querysets/prefetch.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/relationships/related_field.py` & `edgy-0.9.2/edgy/core/db/relationships/related_field.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/db/relationships/relation.py` & `edgy-0.9.2/edgy/core/db/relationships/relation.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/extras/extra.py` & `edgy-0.9.2/edgy/core/extras/extra.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/signals/handlers.py` & `edgy-0.9.2/edgy/core/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/signals/signal.py` & `edgy-0.9.2/edgy/core/signals/signal.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/terminal/base.py` & `edgy-0.9.2/edgy/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/terminal/print.py` & `edgy-0.9.2/edgy/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/terminal/terminal.py` & `edgy-0.9.2/edgy/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/core/utils/functional.py` & `edgy-0.9.2/edgy/core/utils/functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 All functional common to Edgy
 """
+
 from typing import Any, Dict, Tuple, Union
 
 from edgy.core.db.fields.base import BaseField
 
 edgy_setattr = object.__setattr__
```

### Comparing `edgy-0.9.1/edgy/core/utils/models.py` & `edgy-0.9.2/edgy/core/utils/models.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/edgy/protocols/queryset.py` & `edgy-0.9.2/edgy/protocols/queryset.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,107 +23,79 @@
 EdgyModel = Union[_EdgyModel, ReflectEdgyModel]
 
 
 @runtime_checkable
 class QuerySetProtocol(Protocol):
     """Defines the what needs to be implemented when using the ManyRelationProtocol"""
 
-    def filter(self, **kwargs: Any) -> "QuerySet":
-        ...
+    def filter(self, **kwargs: Any) -> "QuerySet": ...
 
-    def exclude(self, **kwargs: "Model") -> "QuerySet":
-        ...
+    def exclude(self, **kwargs: "Model") -> "QuerySet": ...
 
-    def lookup(self, **kwargs: Any) -> "QuerySet":
-        ...
+    def lookup(self, **kwargs: Any) -> "QuerySet": ...
 
-    def order_by(self, columns: Union[List, str]) -> "QuerySet":
-        ...
+    def order_by(self, columns: Union[List, str]) -> "QuerySet": ...
 
-    def limit(self, limit_count: int) -> "QuerySet":
-        ...
+    def limit(self, limit_count: int) -> "QuerySet": ...
 
-    def offset(self, offset: int) -> "QuerySet":
-        ...
+    def offset(self, offset: int) -> "QuerySet": ...
 
-    def group_by(self, group_by: Union[List, str]) -> "QuerySet":
-        ...
+    def group_by(self, group_by: Union[List, str]) -> "QuerySet": ...
 
-    def distinct(self, distinct_on: Union[List, str]) -> "QuerySet":
-        ...
+    def distinct(self, distinct_on: Union[List, str]) -> "QuerySet": ...
 
-    def select_related(self, related: Union[List, str]) -> "QuerySet":
-        ...
+    def select_related(self, related: Union[List, str]) -> "QuerySet": ...
 
-    def only(self, *fields: Sequence[str]) -> "QuerySet":
-        ...
+    def only(self, *fields: Sequence[str]) -> "QuerySet": ...
 
-    def defer(self, *fields: Sequence[str]) -> "QuerySet":
-        ...
+    def defer(self, *fields: Sequence[str]) -> "QuerySet": ...
 
-    async def exists(self) -> bool:
-        ...
+    async def exists(self) -> bool: ...
 
-    async def count(self) -> int:
-        ...
+    async def count(self) -> int: ...
 
-    async def get_or_none(self, **kwargs: Any) -> Union[EdgyModel, None]:
-        ...
+    async def get_or_none(self, **kwargs: Any) -> Union[EdgyModel, None]: ...
 
-    async def all(self, **kwargs: Any) -> Sequence[Optional[EdgyModel]]:
-        ...
+    async def all(self, **kwargs: Any) -> Sequence[Optional[EdgyModel]]: ...
 
-    async def get(self, **kwargs: Any) -> EdgyModel:
-        ...
+    async def get(self, **kwargs: Any) -> EdgyModel: ...
 
-    async def first(self, **kwargs: Any) -> Union[EdgyModel, None]:
-        ...
+    async def first(self, **kwargs: Any) -> Union[EdgyModel, None]: ...
 
-    async def last(self, **kwargs: Any) -> Union[EdgyModel, None]:
-        ...
+    async def last(self, **kwargs: Any) -> Union[EdgyModel, None]: ...
 
-    async def create(self, **kwargs: Any) -> EdgyModel:
-        ...
+    async def create(self, **kwargs: Any) -> EdgyModel: ...
 
-    async def bulk_create(self, objs: Sequence[List[Dict[Any, Any]]]) -> None:
-        ...
+    async def bulk_create(self, objs: Sequence[List[Dict[Any, Any]]]) -> None: ...
 
-    async def bulk_update(self, objs: Sequence[List[EdgyModel]], fields: List[str]) -> None:
-        ...
+    async def bulk_update(self, objs: Sequence[List[EdgyModel]], fields: List[str]) -> None: ...
 
-    async def delete(self) -> None:
-        ...
+    async def delete(self) -> None: ...
 
-    async def update(self, **kwargs: Any) -> None:
-        ...
+    async def update(self, **kwargs: Any) -> None: ...
 
     async def values(
         self,
         fields: Union[Sequence[str], str, None],
         exclude: Union[Sequence[str], Set[str]],
         exclude_none: bool,
         flatten: bool,
         **kwargs: Any,
-    ) -> List[Any]:
-        ...
+    ) -> List[Any]: ...
 
     async def values_list(
         self,
         fields: Union[Sequence[str], str, None],
         exclude: Union[Sequence[str], Set[str]],
         exclude_none: bool,
         flat: bool,
-    ) -> List[Any]:
-        ...
+    ) -> List[Any]: ...
 
     async def get_or_create(
         self,
         _defaults: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
-    ) -> Tuple[EdgyModel, bool]:
-        ...
+    ) -> Tuple[EdgyModel, bool]: ...
 
-    async def update_or_create(self, defaults: Any, **kwargs: Any) -> Tuple[EdgyModel, bool]:
-        ...
+    async def update_or_create(self, defaults: Any, **kwargs: Any) -> Tuple[EdgyModel, bool]: ...
 
-    async def contains(self, instance: EdgyModel) -> bool:
-        ...
+    async def contains(self, instance: EdgyModel) -> bool: ...
```

### Comparing `edgy-0.9.1/edgy/utils/inspect.py` & `edgy-0.9.2/edgy/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/LICENSE` & `edgy-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/README.md` & `edgy-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `edgy-0.9.1/pyproject.toml` & `edgy-0.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "alembic>=1.11.3,<2.0.0",
-    "anyio>=3.7.1,<4",
+    "anyio>=4.0.0,<5",
     "click>=8.1.3,<9.0.0",
     "databasez>=0.7.2",
     "loguru>=0.7.0,<0.10.0",
     "orjson >=3.8.5,<4.0.0",
     "pydantic>=2.5.3,<3.0.0",
     "pydantic-settings>=2.0.0,<3.0.0",
     "rich>=13.3.1,<14.0.0",
@@ -72,21 +72,21 @@
 [project.scripts]
 edgy = "edgy.__main__:run_cli"
 
 [project.optional-dependencies]
 test = [
     "asyncpg>=0.27.0,<1",
     "asyncmy>=0.2.7,<0.3.0",
-    "pytest>=7.1.3,<8.0.0",
+    "pytest>=7.1.3,<9.0.0",
     "esmerald[testing]>=2.0.4",
     "pytest-cov>=2.12.0,<5.0.0",
     "pytest-asyncio >=0.19.0",
     "mypy==1.7.1",
     "flake8>=5.0.4",
-    "black==23.7.0",
+    "black==24.1.1",
     "isort>=5.0.6,<6.0.0",
     "freezegun>=1.2.2,<2.0.0",
     "mock==5.1.0",
     "pytest-benchmark>=4.0.0,<5.0.0",
     "pymysql>=1.0.2,<2.0.0",
     "types-orjson==3.6.2",
     "ruff>=0.0.256,<1.0.0",
```

### Comparing `edgy-0.9.1/PKG-INFO` & `edgy-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgy
-Version: 0.9.1
+Version: 0.9.2
 Summary: 🔥 The perfect ORM to work with complex databases 🔥
 Project-URL: Homepage, https://github.com/tarsil/edgy
 Project-URL: Documentation, https://edgyorm.tarsild.io
 Project-URL: Changelog, https://edgyorm.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/edgy
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -34,15 +34,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: alembic<2.0.0,>=1.11.3
-Requires-Dist: anyio<4,>=3.7.1
+Requires-Dist: anyio<5,>=4.0.0
 Requires-Dist: click<9.0.0,>=8.1.3
 Requires-Dist: databasez>=0.7.2
 Requires-Dist: loguru<0.10.0,>=0.7.0
 Requires-Dist: orjson<4.0.0,>=3.8.5
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0
 Requires-Dist: pydantic<3.0.0,>=2.5.3
 Requires-Dist: rich<14.0.0,>=13.3.1
@@ -75,26 +75,26 @@
 Provides-Extra: ptpython
 Requires-Dist: ptpython<4.0.0,>=3.0.23; extra == 'ptpython'
 Provides-Extra: sqlite
 Requires-Dist: databasez[sqlite]; extra == 'sqlite'
 Provides-Extra: test
 Requires-Dist: asyncmy<0.3.0,>=0.2.7; extra == 'test'
 Requires-Dist: asyncpg<1,>=0.27.0; extra == 'test'
-Requires-Dist: black==23.7.0; extra == 'test'
+Requires-Dist: black==24.1.1; extra == 'test'
 Requires-Dist: esmerald[testing]>=2.0.4; extra == 'test'
 Requires-Dist: flake8>=5.0.4; extra == 'test'
 Requires-Dist: freezegun<2.0.0,>=1.2.2; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'test'
 Requires-Dist: mock==5.1.0; extra == 'test'
 Requires-Dist: mypy==1.7.1; extra == 'test'
 Requires-Dist: pymysql<2.0.0,>=1.0.2; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.19.0; extra == 'test'
 Requires-Dist: pytest-benchmark<5.0.0,>=4.0.0; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=2.12.0; extra == 'test'
-Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test'
+Requires-Dist: pytest<9.0.0,>=7.1.3; extra == 'test'
 Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
 Requires-Dist: types-orjson==3.6.2; extra == 'test'
 Provides-Extra: testing
 Requires-Dist: sqlalchemy-utils>=0.41.1; extra == 'testing'
 Description-Content-Type: text/markdown
 
 # Edgy
```

