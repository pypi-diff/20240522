# Comparing `tmp/dbt_platform_helper-8.3.0.tar.gz` & `tmp/dbt_platform_helper-8.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_platform_helper-8.3.0.tar", max compression
+gzip compressed data, was "dbt_platform_helper-8.4.0.tar", max compression
```

## Comparing `dbt_platform_helper-8.3.0.tar` & `dbt_platform_helper-8.4.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0     1090 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/LICENSE
--rw-r--r--   0        0        0    17907 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/COMMANDS.md
--rw-r--r--   0        0        0     1762 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/README.md
--rw-r--r--   0        0        0        0 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/__init__.py
--rw-r--r--   0        0        0     4522 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/addon-plans.yml
--rw-r--r--   0        0        0     1315 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/addons-template-map.yml
--rw-r--r--   0        0        0        0 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/__init__.py
--rw-r--r--   0        0        0     9957 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/application.py
--rwxr-xr-x   0        0        0     3226 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/check_cloudformation.py
--rw-r--r--   0        0        0    11192 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/codebase.py
--rw-r--r--   0        0        0    14847 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/conduit.py
--rw-r--r--   0        0        0    11480 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/config.py
--rwxr-xr-x   0        0        0    16114 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/copilot.py
--rwxr-xr-x   0        0        0    35037 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/dns.py
--rw-r--r--   0        0        0    11417 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/environment.py
--rw-r--r--   0        0        0      853 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/generate.py
--rw-r--r--   0        0        0     6198 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/pipeline.py
--rwxr-xr-x   0        0        0     3860 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/secrets.py
--rw-r--r--   0        0        0        0 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/custom_resources/__init__.py
--rw-r--r--   0        0        0     2396 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/custom_resources/s3_object.py
--rw-r--r--   0        0        0      342 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/default-extensions.yml
--rw-r--r--   0        0        0      499 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/exceptions.py
--rw-r--r--   0        0        0      369 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/jinja2_tags.py
--rw-r--r--   0        0        0      158 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/.copilot/config.yml
--rwxr-xr-x   0        0        0      164 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/.copilot/image_build_run.sh
--rwxr-xr-x   0        0        0      121 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/.copilot/phases/build.sh
--rwxr-xr-x   0        0        0      123 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/.copilot/phases/install.sh
--rwxr-xr-x   0        0        0      126 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/.copilot/phases/post_build.sh
--rwxr-xr-x   0        0        0      125 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/.copilot/phases/pre_build.sh
--rw-r--r--   0        0        0     1081 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/COMMANDS.md.jinja
--rw-r--r--   0        0        0      618 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addon-instructions.txt
--rw-r--r--   0        0        0      412 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/README.md
--rw-r--r--   0        0        0      734 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml
--rw-r--r--   0        0        0    26381 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml
--rw-r--r--   0        0        0     6064 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/monitoring.yml
--rw-r--r--   0        0        0    10853 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/opensearch.yml
--rw-r--r--   0        0        0    25624 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml
--rw-r--r--   0        0        0     7613 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml
--rw-r--r--   0        0        0     7626 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/s3.yml
--rw-r--r--   0        0        0     3658 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/vpc.yml
--rw-r--r--   0        0        0      956 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml
--rw-r--r--   0        0        0     2403 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml
--rw-r--r--   0        0        0      893 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml
--rw-r--r--   0        0        0     1836 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json
--rw-r--r--   0        0        0      197 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/create-codebuild-role.json
--rw-r--r--   0        0        0     1180 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json
--rw-r--r--   0        0        0      781 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/manifest.yml
--rw-r--r--   0        0        0      169 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/.gitignore
--rw-r--r--   0        0        0      443 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/README.md
--rw-r--r--   0        0        0      284 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/bin/override.ts
--rw-r--r--   0        0        0      339 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/cdk.json
--rw-r--r--   0        0        0     1760 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json
--rw-r--r--   0        0        0   155387 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/package-lock.json
--rw-r--r--   0        0        0      536 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/package.json
--rw-r--r--   0        0        0     1910 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/stack.ts
--rw-r--r--   0        0        0      710 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/tsconfig.json
--rw-r--r--   0        0        0      208 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/terraform-overrides/cfn.patches.yml
--rw-r--r--   0        0        0     1959 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml
--rw-r--r--   0        0        0      169 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/.gitignore
--rw-r--r--   0        0        0      227 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/bin/override.ts
--rw-r--r--   0        0        0      287 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.deploy.yml
--rw-r--r--   0        0        0      781 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml
--rw-r--r--   0        0        0      339 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/cdk.json
--rw-r--r--   0        0        0   152518 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json
--rw-r--r--   0        0        0      536 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json
--rw-r--r--   0        0        0    20142 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts
--rw-r--r--   0        0        0      651 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json
--rw-r--r--   0        0        0     1205 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts
--rw-r--r--   0        0        0     3178 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml
--rw-r--r--   0        0        0     1778 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml
--rw-r--r--   0        0        0      617 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml
--rw-r--r--   0        0        0      741 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html
--rw-r--r--   0        0        0      783 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html
--rw-r--r--   0        0        0     2881 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/manifest-backend.yml
--rw-r--r--   0        0        0     3921 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/manifest-public.yml
--rw-r--r--   0        0        0      386 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/overrides/cfn.patches.yml
--rw-r--r--   0        0        0        0 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/__init__.py
--rw-r--r--   0        0        0     3555 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/application.py
--rw-r--r--   0        0        0    10297 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/aws.py
--rw-r--r--   0        0        0     2943 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/click.py
--rw-r--r--   0        0        0     1053 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/cloudformation.py
--rw-r--r--   0        0        0      484 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/cloudfoundry.py
--rw-r--r--   0        0        0     1720 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/files.py
--rw-r--r--   0        0        0      384 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/git.py
--rw-r--r--   0        0        0      507 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/manifests.py
--rw-r--r--   0        0        0      115 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/messages.py
--rw-r--r--   0        0        0      469 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/template.py
--rw-r--r--   0        0        0    14979 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/validation.py
--rw-r--r--   0        0        0     6695 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/versioning.py
--rwxr-xr-x   0        0        0     1930 2024-05-20 14:11:39.494018 dbt_platform_helper-8.3.0/platform_helper.py
--rw-r--r--   0        0        0     1392 2024-05-20 14:11:39.494018 dbt_platform_helper-8.3.0/pyproject.toml
--rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 dbt_platform_helper-8.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-05-22 14:16:42.571211 dbt_platform_helper-8.4.0/LICENSE
+-rw-r--r--   0        0        0    17907 2024-05-22 14:16:42.571211 dbt_platform_helper-8.4.0/dbt_platform_helper/COMMANDS.md
+-rw-r--r--   0        0        0     1762 2024-05-22 14:16:42.571211 dbt_platform_helper-8.4.0/dbt_platform_helper/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 14:16:42.571211 dbt_platform_helper-8.4.0/dbt_platform_helper/__init__.py
+-rw-r--r--   0        0        0     4522 2024-05-22 14:16:42.571211 dbt_platform_helper-8.4.0/dbt_platform_helper/addon-plans.yml
+-rw-r--r--   0        0        0     1315 2024-05-22 14:16:42.571211 dbt_platform_helper-8.4.0/dbt_platform_helper/addons-template-map.yml
+-rw-r--r--   0        0        0        0 2024-05-22 14:16:42.571211 dbt_platform_helper-8.4.0/dbt_platform_helper/commands/__init__.py
+-rw-r--r--   0        0        0     9957 2024-05-22 14:16:42.571211 dbt_platform_helper-8.4.0/dbt_platform_helper/commands/application.py
+-rwxr-xr-x   0        0        0     3226 2024-05-22 14:16:42.571211 dbt_platform_helper-8.4.0/dbt_platform_helper/commands/check_cloudformation.py
+-rw-r--r--   0        0        0    11192 2024-05-22 14:16:42.571211 dbt_platform_helper-8.4.0/dbt_platform_helper/commands/codebase.py
+-rw-r--r--   0        0        0    14847 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/commands/conduit.py
+-rw-r--r--   0        0        0    11480 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/commands/config.py
+-rwxr-xr-x   0        0        0    16217 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/commands/copilot.py
+-rwxr-xr-x   0        0        0    35037 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/commands/dns.py
+-rw-r--r--   0        0        0    11417 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/commands/environment.py
+-rw-r--r--   0        0        0      853 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/commands/generate.py
+-rw-r--r--   0        0        0     6674 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/commands/pipeline.py
+-rwxr-xr-x   0        0        0     3860 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/commands/secrets.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/custom_resources/__init__.py
+-rw-r--r--   0        0        0     2396 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/custom_resources/s3_object.py
+-rw-r--r--   0        0        0      342 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/default-extensions.yml
+-rw-r--r--   0        0        0      499 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/exceptions.py
+-rw-r--r--   0        0        0      369 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/jinja2_tags.py
+-rw-r--r--   0        0        0      158 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/.copilot/config.yml
+-rwxr-xr-x   0        0        0      164 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/.copilot/image_build_run.sh
+-rwxr-xr-x   0        0        0      121 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/.copilot/phases/build.sh
+-rwxr-xr-x   0        0        0      123 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/.copilot/phases/install.sh
+-rwxr-xr-x   0        0        0      126 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/.copilot/phases/post_build.sh
+-rwxr-xr-x   0        0        0      125 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/.copilot/phases/pre_build.sh
+-rw-r--r--   0        0        0     1081 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/COMMANDS.md.jinja
+-rw-r--r--   0        0        0      618 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addon-instructions.txt
+-rw-r--r--   0        0        0      412 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/README.md
+-rw-r--r--   0        0        0      734 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml
+-rw-r--r--   0        0        0    26381 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml
+-rw-r--r--   0        0        0     6064 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/env/monitoring.yml
+-rw-r--r--   0        0        0    10853 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/env/opensearch.yml
+-rw-r--r--   0        0        0    25624 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml
+-rw-r--r--   0        0        0     7613 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml
+-rw-r--r--   0        0        0     7626 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/env/s3.yml
+-rw-r--r--   0        0        0     3658 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/env/vpc.yml
+-rw-r--r--   0        0        0      956 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml
+-rw-r--r--   0        0        0     2403 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml
+-rw-r--r--   0        0        0      893 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml
+-rw-r--r--   0        0        0     1836 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json
+-rw-r--r--   0        0        0      197 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/create-codebuild-role.json
+-rw-r--r--   0        0        0     1180 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json
+-rw-r--r--   0        0        0      781 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/manifest.yml
+-rw-r--r--   0        0        0      169 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/overrides/.gitignore
+-rw-r--r--   0        0        0      443 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/overrides/README.md
+-rw-r--r--   0        0        0      284 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/overrides/bin/override.ts
+-rw-r--r--   0        0        0      339 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/overrides/cdk.json
+-rw-r--r--   0        0        0     1760 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json
+-rw-r--r--   0        0        0   155387 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/overrides/package-lock.json
+-rw-r--r--   0        0        0      536 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/overrides/package.json
+-rw-r--r--   0        0        0     1910 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/overrides/stack.ts
+-rw-r--r--   0        0        0      710 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/overrides/tsconfig.json
+-rw-r--r--   0        0        0      259 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/terraform-overrides/cfn.patches.yml
+-rw-r--r--   0        0        0     1959 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml
+-rw-r--r--   0        0        0      169 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/overrides/.gitignore
+-rw-r--r--   0        0        0      227 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/overrides/bin/override.ts
+-rw-r--r--   0        0        0      287 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.deploy.yml
+-rw-r--r--   0        0        0      781 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml
+-rw-r--r--   0        0        0      339 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/overrides/cdk.json
+-rw-r--r--   0        0        0   152518 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json
+-rw-r--r--   0        0        0      536 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json
+-rw-r--r--   0        0        0    20142 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts
+-rw-r--r--   0        0        0      651 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json
+-rw-r--r--   0        0        0     1205 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts
+-rw-r--r--   0        0        0     3178 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml
+-rw-r--r--   0        0        0     1778 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml
+-rw-r--r--   0        0        0      617 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml
+-rw-r--r--   0        0        0      741 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html
+-rw-r--r--   0        0        0      783 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html
+-rw-r--r--   0        0        0     2881 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/svc/manifest-backend.yml
+-rw-r--r--   0        0        0     3921 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/svc/manifest-public.yml
+-rw-r--r--   0        0        0      386 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/templates/svc/overrides/cfn.patches.yml
+-rw-r--r--   0        0        0        0 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/utils/__init__.py
+-rw-r--r--   0        0        0     3555 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/utils/application.py
+-rw-r--r--   0        0        0    10297 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/utils/aws.py
+-rw-r--r--   0        0        0     2943 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/utils/click.py
+-rw-r--r--   0        0        0     1053 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/utils/cloudformation.py
+-rw-r--r--   0        0        0      484 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/utils/cloudfoundry.py
+-rw-r--r--   0        0        0     1720 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/utils/files.py
+-rw-r--r--   0        0        0      384 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/utils/git.py
+-rw-r--r--   0        0        0      507 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/utils/manifests.py
+-rw-r--r--   0        0        0      115 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/utils/messages.py
+-rw-r--r--   0        0        0      469 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/utils/template.py
+-rw-r--r--   0        0        0    14979 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/utils/validation.py
+-rw-r--r--   0        0        0     6695 2024-05-22 14:16:42.581211 dbt_platform_helper-8.4.0/dbt_platform_helper/utils/versioning.py
+-rwxr-xr-x   0        0        0     1930 2024-05-22 14:16:42.591211 dbt_platform_helper-8.4.0/platform_helper.py
+-rw-r--r--   0        0        0     1392 2024-05-22 14:16:42.591211 dbt_platform_helper-8.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 dbt_platform_helper-8.4.0/PKG-INFO
```

### Comparing `dbt_platform_helper-8.3.0/LICENSE` & `dbt_platform_helper-8.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/COMMANDS.md` & `dbt_platform_helper-8.4.0/dbt_platform_helper/COMMANDS.md`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/README.md` & `dbt_platform_helper-8.4.0/dbt_platform_helper/README.md`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/addon-plans.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/addon-plans.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/addons-template-map.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/addons-template-map.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/application.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/commands/application.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/check_cloudformation.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/commands/check_cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/codebase.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/commands/codebase.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/conduit.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/commands/conduit.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/config.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/commands/config.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/copilot.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/commands/copilot.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,22 +207,23 @@
     overrides_file.write_text(templates.get_template("svc/overrides/cfn.patches.yml").render())
 
 
 def is_terraform_project() -> bool:
     return Path("./terraform").is_dir()
 
 
-def _get_s3_kms_alias_arns(session, application_name, extension_name):
+def _get_s3_kms_alias_arns(session, application_name, config):
     application = load_application(application_name, session)
 
     arns = {}
     for environment_name, environment in application.environments.items():
-        client = environment.session.client("kms")
-
-        alias_name = f"alias/{application_name}-{environment_name}-{extension_name}-key"
+        if environment_name in config:
+            bucket_name = config[environment_name]["bucket_name"]
+            client = environment.session.client("kms")
+            alias_name = f"alias/{application_name}-{environment_name}-{bucket_name}-key"
 
         try:
             response = client.describe_key(KeyId=alias_name)
         except client.exceptions.NotFoundException:
             pass
         else:
             arns[environment_name] = response["KeyMetadata"]["Arn"]
@@ -304,15 +305,15 @@
             **addon_config,
         }
 
         log_destination_arns = get_log_destination_arn()
 
         if addon_type in ["s3", "s3-policy"]:
             if is_terraform:
-                s3_kms_arns = _get_s3_kms_alias_arns(session, application_name, addon_name)
+                s3_kms_arns = _get_s3_kms_alias_arns(session, application_name, environments)
                 for environment_name in environments:
                     environments[environment_name]["kms_key_arn"] = s3_kms_arns.get(
                         environment_name, "kms-key-not-found"
                     )
             else:
                 service_addon_config["kms_key_reference"] = service_addon_config["prefix"].rsplit(
                     "BucketAccess", 1
```

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/dns.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/commands/dns.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/environment.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/commands/environment.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/generate.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/commands/generate.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/pipeline.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/commands/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 from os import makedirs
 from pathlib import Path
+from shutil import rmtree
 
 import click
 from yaml.parser import ParserError
 
 from dbt_platform_helper.commands.copilot import is_terraform_project
 from dbt_platform_helper.utils.application import get_application_name
 from dbt_platform_helper.utils.aws import get_account_details
@@ -45,28 +46,52 @@
     if not git_repo:
         abort_with_error("The current directory is not a git repository")
 
     codestar_connection_arn = get_codestar_connection_arn(app_name)
     if codestar_connection_arn is None:
         abort_with_error(f'There is no CodeStar Connection named "{app_name}" to use')
 
+    base_path = Path(".")
+    pipelines_dir = base_path / f"copilot/pipelines"
+
+    _clean_pipeline_config(pipelines_dir)
+
     if not is_terraform_project() and "environments" in pipeline_config:
         _generate_environments_pipeline(
-            app_name, codestar_connection_arn, git_repo, pipeline_config["environments"], templates
+            app_name,
+            codestar_connection_arn,
+            git_repo,
+            pipeline_config["environments"],
+            base_path,
+            pipelines_dir,
+            templates,
         )
 
     if "codebases" in pipeline_config:
         account_id, _ = get_account_details()
 
         for codebase in pipeline_config["codebases"]:
             _generate_codebase_pipeline(
-                account_id, app_name, codestar_connection_arn, git_repo, codebase, templates
+                account_id,
+                app_name,
+                codestar_connection_arn,
+                git_repo,
+                codebase,
+                base_path,
+                pipelines_dir,
+                templates,
             )
 
 
+def _clean_pipeline_config(pipelines_dir):
+    if pipelines_dir.exists():
+        click.echo("Deleting copilot/pipelines directory.")
+        rmtree(pipelines_dir)
+
+
 def _validate_pipelines_configuration(pipeline_config):
     if not ("codebases" in pipeline_config or "environments" in pipeline_config):
         abort_with_error("No environment or codebase pipelines defined in pipelines.yml")
 
     if "codebases" in pipeline_config:
         for codebase in pipeline_config["codebases"]:
             codebase_environments = []
@@ -80,18 +105,23 @@
                 abort_with_error(
                     "The pipelines.yml file is invalid, each environment can only be "
                     "listed in a single pipeline per codebase"
                 )
 
 
 def _generate_codebase_pipeline(
-    account_id, app_name, codestar_connection_arn, git_repo, codebase, templates
+    account_id,
+    app_name,
+    codestar_connection_arn,
+    git_repo,
+    codebase,
+    base_path,
+    pipelines_dir,
+    templates,
 ):
-    base_path = Path(".")
-    pipelines_dir = base_path / f"copilot/pipelines"
     makedirs(pipelines_dir / codebase["name"] / "overrides", exist_ok=True)
     environments = []
     for pipelines in codebase["pipelines"]:
         environments += pipelines["environments"]
 
     additional_ecr = codebase.get("additional_ecr_repository", None)
     add_public_perms = additional_ecr and additional_ecr.startswith("public.ecr.aws")
@@ -119,18 +149,16 @@
     overrides_path = Path(__file__).parent.parent.joinpath("templates/pipelines/codebase/overrides")
     generate_override_files(
         base_path, overrides_path, pipelines_dir / codebase["name"] / "overrides"
     )
 
 
 def _generate_environments_pipeline(
-    app_name, codestar_connection_arn, git_repo, configuration, templates
+    app_name, codestar_connection_arn, git_repo, configuration, base_path, pipelines_dir, templates
 ):
-    base_path = Path(".")
-    pipelines_dir = base_path / f"copilot/pipelines"
     makedirs(pipelines_dir / "environments/overrides", exist_ok=True)
 
     template_data = {
         "app_name": app_name,
         "git_repo": git_repo,
         "codestar_connection_arn": codestar_connection_arn,
         "pipeline_environments": configuration,
```

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/secrets.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/commands/secrets.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/custom_resources/s3_object.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/custom_resources/s3_object.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/COMMANDS.md.jinja` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/COMMANDS.md.jinja`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addon-instructions.txt` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addon-instructions.txt`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/monitoring.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/env/monitoring.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/opensearch.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/env/opensearch.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/s3.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/env/s3.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/vpc.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/env/vpc.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/manifest.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/package-lock.json` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/overrides/package-lock.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/package.json` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/overrides/package.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/stack.ts` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/overrides/stack.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/tsconfig.json` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/env/overrides/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/manifest-backend.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/svc/manifest-backend.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/manifest-public.yml` & `dbt_platform_helper-8.4.0/dbt_platform_helper/templates/svc/manifest-public.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/utils/application.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/utils/application.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/utils/aws.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/utils/aws.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/utils/click.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/utils/click.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/utils/cloudformation.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/utils/cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/utils/files.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/utils/files.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/utils/validation.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/utils/validation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/dbt_platform_helper/utils/versioning.py` & `dbt_platform_helper-8.4.0/dbt_platform_helper/utils/versioning.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/platform_helper.py` & `dbt_platform_helper-8.4.0/platform_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.3.0/pyproject.toml` & `dbt_platform_helper-8.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "dbt-platform-helper"
-version = "8.3.0"
+version = "8.4.0"
 description = "Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 license = "MIT"
 readme = "dbt_platform_helper/README.md"
 packages = [
     { include = "dbt_platform_helper" },
     { include = "platform_helper.py" }
```

### Comparing `dbt_platform_helper-8.3.0/PKG-INFO` & `dbt_platform_helper-8.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-platform-helper
-Version: 8.3.0
+Version: 8.4.0
 Summary: Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot.
 License: MIT
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

