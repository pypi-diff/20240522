# Comparing `tmp/smol_k8s_lab-5.1.0.tar.gz` & `tmp/smol_k8s_lab-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smol_k8s_lab-5.1.0.tar", max compression
+gzip compressed data, was "smol_k8s_lab-5.2.0.tar", max compression
```

## Comparing `smol_k8s_lab-5.1.0.tar` & `smol_k8s_lab-5.2.0.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0    34260 2024-05-21 12:03:43.355464 smol_k8s_lab-5.1.0/LICENSE
--rw-r--r--   0        0        0    29423 2024-05-21 12:03:43.355464 smol_k8s_lab-5.1.0/README.md
--rw-r--r--   0        0        0     3300 2024-05-21 12:03:43.651462 smol_k8s_lab-5.1.0/pyproject.toml
--rwxr-xr-x   0        0        0    16188 2024-05-21 12:03:43.651462 smol_k8s_lab-5.1.0/smol_k8s_lab/__init__.py
--rw-r--r--   0        0        0  5853144 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/audio/audio-en.tar.gz
--rwxr-xr-x   0        0        0    12759 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/bw_cli.py
--rw-r--r--   0        0        0     1679 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden.css
--rw-r--r--   0        0        0     2093 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden_app.py
--rw-r--r--   0        0        0     4524 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py
--rw-r--r--   0        0        0     2395 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss
--rw-r--r--   0        0        0     6916 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py
--rw-r--r--   0        0        0    17031 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/config/audio/en.yml
--rw-r--r--   0        0        0     2364 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/config/audio/nl.yml
--rw-r--r--   0        0        0    78462 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/config/default_config.yaml
--rw-r--r--   0        0        0     5666 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/config/keycloak_config.json
--rw-r--r--   0        0        0      237 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/config/kind/kind-config-cilium.yaml
--rw-r--r--   0        0        0      385 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/config/kind/kind_cluster_config.yaml
--rw-r--r--   0        0        0      831 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/config/smol-k8s-lab.appdata.xml
--rwxr-xr-x   0        0        0     3008 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/constants.py
--rwxr-xr-x   0        0        0    12945 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/env_config.py
--rw-r--r--   0        0        0     9821 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/__init__.py
--rw-r--r--   0        0        0     7789 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/argocd.py
--rw-r--r--   0        0        0        0 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/__init__.py
--rw-r--r--   0        0        0     6581 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py
--rw-r--r--   0        0        0     9763 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/vouch.py
--rw-r--r--   0        0        0    19076 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py
--rw-r--r--   0        0        0    20511 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py
--rw-r--r--   0        0        0     3372 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/ingress/cert_manager.py
--rw-r--r--   0        0        0     1285 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py
--rw-r--r--   0        0        0     9134 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/initial_special.py
--rw-r--r--   0        0        0        0 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/networking/__init__.py
--rw-r--r--   0        0        0     1766 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/networking/cilium.py
--rw-r--r--   0        0        0     2318 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/networking/metallb.py
--rw-r--r--   0        0        0    10977 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/networking/netmaker.py
--rw-r--r--   0        0        0     2383 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/operators/__init__.py
--rw-r--r--   0        0        0     8381 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/operators/minio.py
--rw-r--r--   0        0        0     3617 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/operators/postgres_operators.py
--rw-r--r--   0        0        0     4286 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/operators/seaweedfs.py
--rw-r--r--   0        0        0        0 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/secrets_management/__init__.py
--rw-r--r--   0        0        0     2675 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py
--rw-r--r--   0        0        0     3759 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/secrets_management/infisical.py
--rw-r--r--   0        0        0     4805 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/secrets_management/vault.py
--rw-r--r--   0        0        0    11623 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/home_assistant.py
--rw-r--r--   0        0        0    21465 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/mastodon.py
--rwxr-xr-x   0        0        0     1706 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/mastodon_rake.py
--rw-r--r--   0        0        0    18842 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/matrix.py
--rw-r--r--   0        0        0    20726 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/nextcloud.py
--rwxr-xr-x   0        0        0     6182 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py
--rw-r--r--   0        0        0     8034 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_distros/__init__.py
--rw-r--r--   0        0        0     3755 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_distros/k3d.py
--rw-r--r--   0        0        0     8481 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_distros/k3s.py
--rw-r--r--   0        0        0     4821 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_distros/kind.py
--rw-r--r--   0        0        0        1 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/__init__.py
--rw-r--r--   0        0        0     8642 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/argocd_util.py
--rw-r--r--   0        0        0     8689 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/backup.py
--rwxr-xr-x   0        0        0     8607 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/helm.py
--rw-r--r--   0        0        0    14252 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/k8s_lib.py
--rw-r--r--   0        0        0    22222 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/restores.py
--rw-r--r--   0        0        0     1358 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/__init__.py
--rw-r--r--   0        0        0        0 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/__init__.py
--rw-r--r--   0        0        0    14333 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py
--rw-r--r--   0        0        0     9712 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/argocd_widgets.py
--rw-r--r--   0        0        0    18578 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/backup_and_restore.py
--rw-r--r--   0        0        0    14373 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/input_widgets.py
--rwxr-xr-x   0        0        0     4002 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/invalid_apps.py
--rw-r--r--   0        0        0     6970 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/modify_globals.py
--rw-r--r--   0        0        0     3697 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/new_app_modal.py
--rwxr-xr-x   0        0        0    17593 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/apps_screen.py
--rw-r--r--   0        0        0    12891 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/base.py
--rw-r--r--   0        0        0    33063 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/base_widgets/audio_widget.py
--rw-r--r--   0        0        0     7189 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/base_widgets/cluster_modal.py
--rw-r--r--   0        0        0     3384 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/base_widgets/new_cluster_input.py
--rwxr-xr-x   0        0        0     8926 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/confirm_screen.py
--rw-r--r--   0        0        0     1546 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/add_nodes_widget.tcss
--rw-r--r--   0        0        0     7174 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/apps_config.tcss
--rw-r--r--   0        0        0     1184 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/apps_init_config.tcss
--rw-r--r--   0        0        0     6681 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/base.tcss
--rw-r--r--   0        0        0      988 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/base_modal.tcss
--rw-r--r--   0        0        0     1371 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/cluster_modal.tcss
--rw-r--r--   0        0        0     1278 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/confirm.tcss
--rw-r--r--   0        0        0     1564 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/distro_config.tcss
--rw-r--r--   0        0        0      927 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/help.tcss
--rw-r--r--   0        0        0      984 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/invalid_apps.tcss
--rw-r--r--   0        0        0     2198 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/k3s.tcss
--rw-r--r--   0        0        0     1901 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/kind.tcss
--rw-r--r--   0        0        0     1259 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/modify_globals_modal.tcss
--rw-r--r--   0        0        0      770 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/new_app_modal.tcss
--rw-r--r--   0        0        0      112 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/new_option_modal.tcss
--rw-r--r--   0        0        0     1168 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/node_inputs_widget.tcss
--rw-r--r--   0        0        0     1101 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/node_modal.tcss
--rw-r--r--   0        0        0     3433 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss
--rw-r--r--   0        0        0     2554 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/tui_config.tcss
--rwxr-xr-x   0        0        0    10391 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_screen.py
--rw-r--r--   0        0        0        0 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/__init__.py
--rw-r--r--   0        0        0    17214 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/add_nodes.py
--rw-r--r--   0        0        0    14337 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/k3s_config.py
--rw-r--r--   0        0        0     6754 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/kind_config.py
--rw-r--r--   0        0        0     6060 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/kubelet_config.py
--rw-r--r--   0        0        0     4359 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py
--rw-r--r--   0        0        0     4669 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/node_adjustment.py
--rw-r--r--   0        0        0     4193 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/help_screen.py
--rwxr-xr-x   0        0        0     4020 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/make_screenshots.py
--rwxr-xr-x   0        0        0    11139 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/smol_k8s_config_screen.py
--rwxr-xr-x   0        0        0     8811 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/tui_config_screen.py
--rw-r--r--   0        0        0     9901 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/util.py
--rw-r--r--   0        0        0        0 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/validators/__init__.py
--rw-r--r--   0        0        0      579 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/validators/already_exists.py
--rw-r--r--   0        0        0        0 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/__init__.py
--rw-r--r--   0        0        0    16300 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/minio_lib.py
--rw-r--r--   0        0        0     1184 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/passwords.py
--rwxr-xr-x   0        0        0     2423 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/rich_cli/console_logging.py
--rwxr-xr-x   0        0        0     4720 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/rich_cli/help_text.py
--rw-r--r--   0        0        0     2610 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/run/final_cmd.py
--rwxr-xr-x   0        0        0     7483 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/run/subproc.py
--rw-r--r--   0        0        0     2837 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/value_from.py
--rw-r--r--   0        0        0      315 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/yaml_with_comments.py
--rw-r--r--   0        0        0    31109 1970-01-01 00:00:00.000000 smol_k8s_lab-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34260 2024-05-22 14:09:13.857805 smol_k8s_lab-5.2.0/LICENSE
+-rw-r--r--   0        0        0    29423 2024-05-22 14:09:13.857805 smol_k8s_lab-5.2.0/README.md
+-rw-r--r--   0        0        0     3323 2024-05-22 14:09:14.125805 smol_k8s_lab-5.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0    16188 2024-05-22 14:09:14.125805 smol_k8s_lab-5.2.0/smol_k8s_lab/__init__.py
+-rw-r--r--   0        0        0  5853144 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/audio/audio-en.tar.gz
+-rwxr-xr-x   0        0        0    12759 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/bitwarden/bw_cli.py
+-rw-r--r--   0        0        0     1679 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/bitwarden/tui/bitwarden.css
+-rw-r--r--   0        0        0     2093 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/bitwarden/tui/bitwarden_app.py
+-rw-r--r--   0        0        0     4524 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py
+-rw-r--r--   0        0        0     2395 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss
+-rw-r--r--   0        0        0     6916 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py
+-rw-r--r--   0        0        0    17031 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/config/audio/en.yml
+-rw-r--r--   0        0        0     2364 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/config/audio/nl.yml
+-rw-r--r--   0        0        0    79433 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/config/default_config.yaml
+-rw-r--r--   0        0        0     5666 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/config/keycloak_config.json
+-rw-r--r--   0        0        0      237 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/config/kind/kind-config-cilium.yaml
+-rw-r--r--   0        0        0      385 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/config/kind/kind_cluster_config.yaml
+-rw-r--r--   0        0        0      831 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/config/smol-k8s-lab.appdata.xml
+-rwxr-xr-x   0        0        0     3008 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/constants.py
+-rwxr-xr-x   0        0        0    12945 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/env_config.py
+-rw-r--r--   0        0        0     9821 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/__init__.py
+-rw-r--r--   0        0        0     7789 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/argocd.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/identity_provider/__init__.py
+-rw-r--r--   0        0        0     6581 2024-05-22 14:09:14.133805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py
+-rw-r--r--   0        0        0     9763 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/identity_provider/vouch.py
+-rw-r--r--   0        0        0    19076 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py
+-rw-r--r--   0        0        0    20511 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py
+-rw-r--r--   0        0        0     3372 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/ingress/cert_manager.py
+-rw-r--r--   0        0        0     1285 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py
+-rw-r--r--   0        0        0     9134 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/initial_special.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/networking/__init__.py
+-rw-r--r--   0        0        0     1766 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/networking/cilium.py
+-rw-r--r--   0        0        0     2318 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/networking/metallb.py
+-rw-r--r--   0        0        0    10977 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/networking/netmaker.py
+-rw-r--r--   0        0        0     2383 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/operators/__init__.py
+-rw-r--r--   0        0        0     8381 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/operators/minio.py
+-rw-r--r--   0        0        0     3617 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/operators/postgres_operators.py
+-rw-r--r--   0        0        0     4286 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/operators/seaweedfs.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/secrets_management/__init__.py
+-rw-r--r--   0        0        0     2675 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py
+-rw-r--r--   0        0        0     3759 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/secrets_management/infisical.py
+-rw-r--r--   0        0        0     4805 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/secrets_management/vault.py
+-rw-r--r--   0        0        0    11623 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/social/home_assistant.py
+-rw-r--r--   0        0        0    21465 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/social/mastodon.py
+-rwxr-xr-x   0        0        0     1706 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/social/mastodon_rake.py
+-rw-r--r--   0        0        0    22808 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/social/matrix.py
+-rw-r--r--   0        0        0    20726 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/social/nextcloud.py
+-rwxr-xr-x   0        0        0     6182 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py
+-rw-r--r--   0        0        0     8034 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_distros/__init__.py
+-rw-r--r--   0        0        0     3755 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_distros/k3d.py
+-rw-r--r--   0        0        0     8481 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_distros/k3s.py
+-rw-r--r--   0        0        0     4821 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_distros/kind.py
+-rw-r--r--   0        0        0        1 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_tools/__init__.py
+-rw-r--r--   0        0        0     8642 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_tools/argocd_util.py
+-rw-r--r--   0        0        0     8689 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_tools/backup.py
+-rwxr-xr-x   0        0        0     8607 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_tools/helm.py
+-rw-r--r--   0        0        0    14252 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_tools/k8s_lib.py
+-rw-r--r--   0        0        0    22222 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_tools/restores.py
+-rw-r--r--   0        0        0     1358 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/app_widgets/__init__.py
+-rw-r--r--   0        0        0    14333 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py
+-rw-r--r--   0        0        0     9712 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/app_widgets/argocd_widgets.py
+-rw-r--r--   0        0        0    18578 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/app_widgets/backup_and_restore.py
+-rw-r--r--   0        0        0    14373 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/app_widgets/input_widgets.py
+-rwxr-xr-x   0        0        0     4002 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/app_widgets/invalid_apps.py
+-rw-r--r--   0        0        0     6970 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/app_widgets/modify_globals.py
+-rw-r--r--   0        0        0     3697 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/app_widgets/new_app_modal.py
+-rwxr-xr-x   0        0        0    17593 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/apps_screen.py
+-rw-r--r--   0        0        0    12891 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/base.py
+-rw-r--r--   0        0        0    33063 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/base_widgets/audio_widget.py
+-rw-r--r--   0        0        0     7189 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/base_widgets/cluster_modal.py
+-rw-r--r--   0        0        0     3384 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/base_widgets/new_cluster_input.py
+-rwxr-xr-x   0        0        0     8926 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/confirm_screen.py
+-rw-r--r--   0        0        0     1546 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/add_nodes_widget.tcss
+-rw-r--r--   0        0        0     7174 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/apps_config.tcss
+-rw-r--r--   0        0        0     1184 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/apps_init_config.tcss
+-rw-r--r--   0        0        0     6681 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/base.tcss
+-rw-r--r--   0        0        0      988 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/base_modal.tcss
+-rw-r--r--   0        0        0     1371 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/cluster_modal.tcss
+-rw-r--r--   0        0        0     1278 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/confirm.tcss
+-rw-r--r--   0        0        0     1564 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/distro_config.tcss
+-rw-r--r--   0        0        0      927 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/help.tcss
+-rw-r--r--   0        0        0      984 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/invalid_apps.tcss
+-rw-r--r--   0        0        0     2198 2024-05-22 14:09:14.137805 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/k3s.tcss
+-rw-r--r--   0        0        0     1901 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/kind.tcss
+-rw-r--r--   0        0        0     1259 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/modify_globals_modal.tcss
+-rw-r--r--   0        0        0      770 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/new_app_modal.tcss
+-rw-r--r--   0        0        0      112 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/new_option_modal.tcss
+-rw-r--r--   0        0        0     1168 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/node_inputs_widget.tcss
+-rw-r--r--   0        0        0     1101 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/node_modal.tcss
+-rw-r--r--   0        0        0     3433 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss
+-rw-r--r--   0        0        0     2554 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/tui_config.tcss
+-rwxr-xr-x   0        0        0    10391 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/distro_screen.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/distro_widgets/__init__.py
+-rw-r--r--   0        0        0    17214 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/distro_widgets/add_nodes.py
+-rw-r--r--   0        0        0    14337 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/distro_widgets/k3s_config.py
+-rw-r--r--   0        0        0     6754 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/distro_widgets/kind_config.py
+-rw-r--r--   0        0        0     6060 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/distro_widgets/kubelet_config.py
+-rw-r--r--   0        0        0     4359 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py
+-rw-r--r--   0        0        0     4669 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/distro_widgets/node_adjustment.py
+-rw-r--r--   0        0        0     4193 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/help_screen.py
+-rwxr-xr-x   0        0        0     4020 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/make_screenshots.py
+-rwxr-xr-x   0        0        0    11139 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/smol_k8s_config_screen.py
+-rwxr-xr-x   0        0        0     8811 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/tui_config_screen.py
+-rw-r--r--   0        0        0     9901 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/util.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/validators/__init__.py
+-rw-r--r--   0        0        0      579 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/tui/validators/already_exists.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/utils/__init__.py
+-rw-r--r--   0        0        0    16300 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/utils/minio_lib.py
+-rw-r--r--   0        0        0     1184 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/utils/passwords.py
+-rwxr-xr-x   0        0        0     2423 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/utils/rich_cli/console_logging.py
+-rwxr-xr-x   0        0        0     4720 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/utils/rich_cli/help_text.py
+-rw-r--r--   0        0        0     2610 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/utils/run/final_cmd.py
+-rwxr-xr-x   0        0        0     7483 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/utils/run/subproc.py
+-rw-r--r--   0        0        0     2837 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/utils/value_from.py
+-rw-r--r--   0        0        0      315 2024-05-22 14:09:14.141806 smol_k8s_lab-5.2.0/smol_k8s_lab/utils/yaml_with_comments.py
+-rw-r--r--   0        0        0    31153 1970-01-01 00:00:00.000000 smol_k8s_lab-5.2.0/PKG-INFO
```

### Comparing `smol_k8s_lab-5.1.0/LICENSE` & `smol_k8s_lab-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/README.md` & `smol_k8s_lab-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/pyproject.toml` & `smol_k8s_lab-5.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "smol_k8s_lab"
-version       = "5.1.0"
+version       = "5.2.0"
 description   = "CLI and TUI to quickly install slimmer Kubernetes distros and then manage apps declaratively using Argo CD"
 authors       = ["Jesse Hitch <jessebot@linux.com>",
                  "Max Roby <emax@cloudydev.net>"]
 readme        = "README.md"
 packages      = [{include = "smol_k8s_lab"}]
 license       = "AGPL-3.0-or-later"
 homepage      = "https://small-hack.github.io/smol-k8s-lab"
@@ -42,14 +42,15 @@
 requests           = "^2.32"
 rich               = "^13.0"
 ruamel-yaml        = "^0.18"
 ruamel-yaml-string = "^0.1"
 textual            = "^0.62"
 xdg-base-dirs      = "^6.0"
 pygame             = "^2.5.2"
+python-ulid = "^2.5.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.5"
 mkdocs-video    = "^1.5"
```

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/__init__.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/audio/audio-en.tar.gz` & `smol_k8s_lab-5.2.0/smol_k8s_lab/audio/audio-en.tar.gz`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/bw_cli.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/bitwarden/bw_cli.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden.css` & `smol_k8s_lab-5.2.0/smol_k8s_lab/bitwarden/tui/bitwarden.css`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden_app.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/bitwarden/tui/bitwarden_app.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/config/audio/en.yml` & `smol_k8s_lab-5.2.0/smol_k8s_lab/config/audio/en.yml`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/config/audio/nl.yml` & `smol_k8s_lab-5.2.0/smol_k8s_lab/config/audio/nl.yml`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/config/default_config.yaml` & `smol_k8s_lab-5.2.0/smol_k8s_lab/config/default_config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -874,27 +874,28 @@
         destination:
           # automatically includes the app's namespace and argocd's namespace
           namespaces: []
 
   matrix:
     description: |
       [link=https://matrix.org/]Matrix[/link] is an open protocol for decentralised, secure communications.
-      This deploys a matrix synapse server, element (web frontend), and turn server (voice)
+      This deploys synapse (as your matrix home server), element (as a web frontend), coturn (as a turn server for voice), and optionally matrix authentication service/matrix sliding sync if you enable the beta. (see below for more info)
 
       smol-k8s-lab supports initialization by creating initial secrets for your:
-        - matrix, element, and federation hostnames,
-        - credentials for: postgresql, admin user, S3 storage, and SMTP
+        - matrix, element, and federation hostnames (and optionally a sliding sync hostname)
+        - credentials for: postgresql, admin user, S3 storage, SMTP, and optionally matrix authentication service
 
-      smol-k8s-lab also sets up an OIDC application via Zitadel.
+      smol-k8s-lab also sets up an OIDC application via Zitadel. By default, we use the stable matrix Argo CD application directory, but if you'd like to start trying to the new [link=https://element.io/labs/element-x]element-x[/link] (the element beta apps), change the argo path to [gold3]app_of_apps_beta/[/gold3] and we will also deploy the [link=https://matrix-org.github.io/matrix-authentication-service/setup/homeserver.html]matrix authentication service[/link] as well as [link=https://github.com/matrix-org/sliding-sync]matrix sliding sync[/link].
 
       To provide sensitive values via environment variables to smol-k8s-lab use:
         - MATRIX_SMTP_PASSWORD
         - MATRIX_S3_BACKUP_ACCESS_ID
         - MATRIX_S3_BACKUP_SECRET_KEY
         - MATRIX_RESTIC_REPO_PASSWORD
+
     enabled: false
     init:
       enabled: true
       restore:
         # set to true to run a restic restore via a k8up job for your
         # seaweedfs PVCs, matrix signing key PVC, synapse config PVC, media PVC
         # and restoring your postgresql database
@@ -948,14 +949,18 @@
       secret_keys:
         # hostname of the synapse matrix server
         hostname: ""
         # the hostname of the element web interface
         element_hostname: ""
         # hostname for federation, that others can see you on the fediverse
         federation_hostname: ""
+        # sliding sync hostname to use for beta features
+        sliding_sync_hostname: "sliding sync hostname to use for beta features"
+        # auth hostname to use for beta features
+        auth_hostname: "auth hostname to use for beta features"
         # email for of the admin user
         admin_email: ""
         # enable persistent volume claim for matrix media storage
         media_pvc_enabled: "true"
         # size of media pvc storage
         media_storage: "20Gi"
         media_access_mode: "ReadWriteOnce"
```

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/config/keycloak_config.json` & `smol_k8s_lab-5.2.0/smol_k8s_lab/config/keycloak_config.json`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/config/smol-k8s-lab.appdata.xml` & `smol_k8s_lab-5.2.0/smol_k8s_lab/config/smol-k8s-lab.appdata.xml`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/constants.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/constants.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/env_config.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/env_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/__init__.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/argocd.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/argocd.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/vouch.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/identity_provider/vouch.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/ingress/cert_manager.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/ingress/cert_manager.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/initial_special.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/initial_special.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/networking/cilium.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/networking/cilium.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/networking/metallb.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/networking/metallb.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/networking/netmaker.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/networking/netmaker.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/operators/__init__.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/operators/minio.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/operators/minio.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/operators/postgres_operators.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/operators/postgres_operators.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/operators/seaweedfs.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/operators/seaweedfs.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/secrets_management/infisical.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/secrets_management/infisical.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/secrets_management/vault.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/secrets_management/vault.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/home_assistant.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/social/home_assistant.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/mastodon.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/social/mastodon.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/mastodon_rake.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/social/mastodon_rake.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/matrix.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/social/matrix.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+# internal libraries
 from smol_k8s_lab.bitwarden.bw_cli import BwCLI, create_custom_field
 from smol_k8s_lab.k8s_apps.operators.minio import create_minio_alias
 from smol_k8s_lab.k8s_apps.identity_provider.zitadel_api import Zitadel
 from smol_k8s_lab.k8s_tools.argocd_util import ArgoCD
 from smol_k8s_lab.k8s_tools.restores import (restore_seaweedfs,
                                              k8up_restore_pvc,
                                              recreate_pvc,
                                              restore_cnpg_cluster)
 from smol_k8s_lab.utils.value_from import process_backup_vals, extract_secret
 from smol_k8s_lab.utils.rich_cli.console_logging import sub_header, header
 from smol_k8s_lab.utils.passwords import create_password
 
+# external libraries
 import logging as log
+from ulid import ULID
 
 
 def configure_matrix(argocd: ArgoCD,
                      cfg: dict,
                      pvc_storage_class: str,
                      zitadel: Zitadel,
                      bitwarden: BwCLI = None) -> bool:
@@ -88,14 +91,18 @@
             logout_uris = [f"https://{matrix_hostname}"]
             oidc_creds = zitadel.create_application("matrix",
                                                     redirect_uris,
                                                     logout_uris)
             zitadel.create_role("matrix_users", "Matrix Users", "matrix_users")
             zitadel.update_user_grant(['matrix_users'])
             zitadel_hostname = zitadel.hostname
+            mas_issuer = f"https://{zitadel.hostname}"
+            mas_client_id = str(ULID)
+            mas_client_secret = create_password()
+            mas_admin_token = create_password()
         else:
             zitadel_hostname = ""
 
         # if the user has bitwarden enabled
         if bitwarden and not restore_enabled:
             setup_bitwarden_items(argocd,
                                   matrix_hostname,
@@ -106,43 +113,78 @@
                                   s3_bucket,
                                   backup_vals['s3_user'],
                                   backup_vals['s3_password'],
                                   backup_vals['restic_repo_pass'],
                                   mail_host,
                                   mail_user,
                                   mail_pass,
-                                  oidc_creds,
                                   zitadel_hostname,
+                                  oidc_creds,
+                                  mas_issuer,
+                                  mas_client_id,
+                                  mas_client_secret,
+                                  mas_admin_token,
                                   bitwarden)
 
         # else create these as Kubernetes secrets
         elif not bitwarden and not restore_enabled:
             # postgresql credentials
             argocd.k8s.create_secret(
                     'matrix-pgsql-credentials',
                     'matrix',
-                    {"password": "we-use-tls-instead-of-password-now"}
+                    {"password": "we-use-tls-instead-of-password-now",
+                     "database": "matrix-postgres",
+                     "hostname": f"matrix-postgres-rw.{matrix_namespace}.svc"}
+                    )
+
+            argocd.k8s.create_secret(
+                    'mas-pgsql-credentials',
+                    'matrix',
+                    {"password": "we-use-tls-instead-of-password-now",
+                     "database": "mas",
+                     "hostname": f"mas-rw.{matrix_namespace}.svc"}
+                    )
+
+            argocd.k8s.create_secret(
+                    'sliding-sync-pgsql-credentials',
+                    'matrix',
+                    {"password": "we-use-tls-instead-of-password-now",
+                     "database": "syncv3",
+                     "hostname": f"syncv3-rw.{matrix_namespace}.svc"}
                     )
 
             # registation key
             matrix_registration_key = create_password()
             argocd.k8s.create_secret(
                     'matrix-registration',
                     'matrix',
                     {"registrationSharedSecret": matrix_registration_key}
                     )
 
-            # oidc secret
-            argocd.k8s.create_secret(
-                    'matrix-oidc-credentials',
-                    'matrix',
-                    {'user': oidc_creds['client_id'],
-                     'password': oidc_creds['client_secret'],
-                     'issuer': zitadel.hostname}
-                    )
+            if zitadel:
+                # oidc secret
+                argocd.k8s.create_secret(
+                        'matrix-oidc-credentials',
+                        'matrix',
+                        {'user': oidc_creds['client_id'],
+                         'password': oidc_creds['client_secret'],
+                         'issuer': zitadel.hostname}
+                        )
+
+                # matrix-athentication-service secret
+                argocd.k8s.create_secret(
+                        'matrix-authentication-service-secret',
+                        'matrix',
+                        {'issuer': mas_issuer,
+                         'client_id': mas_client_id,
+                         'client_auth_method': "client_secret_basic",
+                         'client_secret': mas_client_secret,
+                         'admin_token': mas_admin_token,
+                         'account_management_url': zitadel.hostname}
+                        )
 
     if not app_installed:
         # if the user is restoring, the process is a little different
         if init_enabled and restore_enabled:
             restore_matrix(argocd,
                            matrix_hostname,
                            matrix_namespace,
@@ -230,17 +272,21 @@
                           s3_bucket: str,
                           backups_s3_user: str,
                           backups_s3_password: str,
                           restic_repo_pass: str,
                           mail_host: str,
                           mail_user: str,
                           mail_pass: str,
-                          oidc_creds: str,
                           zitadel_hostname: str,
-                          bitwarden):
+                          oidc_creds: str,
+                          mas_issuer: str,
+                          mas_client_id: str,
+                          mas_client_secret: str,
+                          mas_admin_token: str,
+                          bitwarden: BwCLI):
     """
     setup all the required secrets as items in bitwarden
     """
     sub_header("Creating matrix secrets in Bitwarden")
 
     # S3 credentials
     if "http" not in s3_endpoint:
@@ -284,27 +330,50 @@
             item_url=matrix_hostname,
             user=backups_s3_user,
             password=backups_s3_password,
             fields=[restic_repo_pass_obj]
             )
 
     # postgresql credentials
-    # matrix_pgsql_password = bitwarden.generate()
     db_hostname_obj = create_custom_field("hostname",
                                           f"matrix-postgres-rw.{matrix_namespace}.svc")
     # the database name
     db_obj = create_custom_field("database", "matrix")
     db_id = bitwarden.create_login(
             name='matrix-pgsql-credentials',
             item_url=matrix_hostname,
             user='matrix',
             password="we-use-tls-instead-of-password-now",
             fields=[db_hostname_obj, db_obj]
             )
 
+    # postgres matrix authentication service credentials
+    db_hostname_obj = create_custom_field("hostname",
+                                          f"mas-rw.{matrix_namespace}.svc")
+    db_obj = create_custom_field("database", "mas")
+    db_id = bitwarden.create_login(
+            name='mas-pgsql-credentials',
+            item_url=matrix_hostname,
+            user='mas',
+            password="we-use-tls-instead-of-password-now",
+            fields=[db_hostname_obj, db_obj]
+            )
+
+    # postgres sliding sync credentials
+    db_hostname_obj = create_custom_field("hostname",
+                                          f"syncv3-rw.{matrix_namespace}.svc")
+    db_obj = create_custom_field("database", "syncv3")
+    db_id = bitwarden.create_login(
+            name='syncv3-pgsql-credentials',
+            item_url=matrix_hostname,
+            user='syncv3',
+            password="we-use-tls-instead-of-password-now",
+            fields=[db_hostname_obj, db_obj]
+            )
+
     # SMTP credentials
     matrix_smtp_host_obj = create_custom_field("smtpHostname", mail_host)
     smtp_id = bitwarden.create_login(
             name='matrix-smtp-credentials',
             item_url=matrix_hostname,
             user=mail_user,
             password=mail_pass,
@@ -321,41 +390,61 @@
             )
 
     # OIDC credentials
     log.info("Creating OIDC credentials for Matrix in Bitwarden")
     if zitadel_hostname:
         idp_id = "zitadel"
         idp_name = "Zitadel Auth"
+        issuer_url = "https://" + zitadel_hostname
+
         if oidc_creds:
-            issuer_obj = create_custom_field("issuer", "https://" + zitadel_hostname)
+            issuer_obj = create_custom_field("issuer", issuer_url)
             idp_id_obj = create_custom_field("idp_id", idp_id)
             idp_name_obj = create_custom_field("idp_name", idp_name)
+
+            # for the credentials to zitadel
             oidc_id = bitwarden.create_login(
                     name='matrix-oidc-credentials',
                     item_url=matrix_hostname,
                     user=oidc_creds['client_id'],
                     password=oidc_creds['client_secret'],
                     fields=[issuer_obj, idp_id_obj, idp_name_obj]
                     )
+
+            # for credentials b/w matrix authentication service and synapse (matrix homeserver)
+            mas_token_obj = create_custom_field("admin_token", mas_admin_token)
+            acct_url_obj = create_custom_field("account_management_url", issuer_url)
+            issuer_obj = create_custom_field("issuer", mas_issuer)
+            mas_id = bitwarden.create_login(
+                    name='matrix-authentication-service-credentials',
+                    item_url=matrix_hostname,
+                    user=mas_client_id,
+                    password=mas_client_secret,
+                    fields=[issuer_obj, mas_token_obj, acct_url_obj]
+                    )
         else:
             # we assume the credentials already exist if they fail to create
             oidc_id = bitwarden.get_item(
                     f"matrix-oidc-credentials-{matrix_hostname}"
                     )[0]['id']
+            mas_id = bitwarden.get_item(
+                    f"matrix-authentication-service-credentials-{matrix_hostname}"
+                    )[0]['id']
 
     # update the matrix values for the argocd appset
     argocd.update_appset_secret(
             {'matrix_registration_credentials_bitwarden_id': reg_id,
              'matrix_smtp_credentials_bitwarden_id': smtp_id,
              'matrix_s3_admin_credentials_bitwarden_id': s3_admin_id,
              'matrix_s3_postgres_credentials_bitwarden_id': s3_db_id,
              'matrix_s3_matrix_credentials_bitwarden_id': s3_id,
              'matrix_s3_backups_credentials_bitwarden_id': s3_backups_id,
              'matrix_postgres_credentials_bitwarden_id': db_id,
              'matrix_oidc_credentials_bitwarden_id': oidc_id,
+             'matrix_authentication_service_bitwarden_id': mas_id,
              'matrix_idp_name': idp_name,
              'matrix_idp_id': idp_id})
 
     # reload the bitwarden ESO provider
     try:
         argocd.k8s.reload_deployment('bitwarden-eso-provider',
                                      'external-secrets')
```

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/nextcloud.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/social/nextcloud.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_distros/__init__.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_distros/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_distros/k3d.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_distros/k3d.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_distros/k3s.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_distros/k3s.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_distros/kind.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_distros/kind.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/argocd_util.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_tools/argocd_util.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/backup.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_tools/backup.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/helm.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_tools/helm.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/k8s_lib.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_tools/k8s_lib.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/restores.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/k8s_tools/restores.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/__init__.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/argocd_widgets.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/app_widgets/argocd_widgets.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/backup_and_restore.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/app_widgets/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/input_widgets.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/app_widgets/input_widgets.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/invalid_apps.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/app_widgets/invalid_apps.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/modify_globals.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/app_widgets/modify_globals.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/new_app_modal.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/app_widgets/new_app_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/apps_screen.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/apps_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/base.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/base.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/base_widgets/audio_widget.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/base_widgets/audio_widget.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/base_widgets/cluster_modal.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/base_widgets/cluster_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/base_widgets/new_cluster_input.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/base_widgets/new_cluster_input.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/confirm_screen.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/confirm_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/add_nodes_widget.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/add_nodes_widget.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/apps_config.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/apps_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/apps_init_config.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/apps_init_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/base.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/base.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/base_modal.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/base_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/cluster_modal.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/cluster_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/confirm.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/confirm.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/distro_config.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/distro_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/help.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/help.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/invalid_apps.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/invalid_apps.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/k3s.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/k3s.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/kind.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/kind.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/modify_globals_modal.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/modify_globals_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/new_app_modal.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/new_app_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/node_inputs_widget.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/node_inputs_widget.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/node_modal.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/node_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/tui_config.tcss` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/css/tui_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_screen.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/distro_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/add_nodes.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/distro_widgets/add_nodes.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/k3s_config.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/distro_widgets/k3s_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/kind_config.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/distro_widgets/kind_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/kubelet_config.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/distro_widgets/kubelet_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/node_adjustment.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/distro_widgets/node_adjustment.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/help_screen.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/help_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/make_screenshots.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/make_screenshots.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/smol_k8s_config_screen.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/smol_k8s_config_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/tui_config_screen.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/tui_config_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/util.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/util.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/validators/already_exists.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/tui/validators/already_exists.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/utils/minio_lib.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/utils/minio_lib.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/utils/passwords.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/utils/passwords.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/utils/rich_cli/console_logging.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/utils/rich_cli/console_logging.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/utils/rich_cli/help_text.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/utils/rich_cli/help_text.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/utils/run/final_cmd.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/utils/run/final_cmd.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/utils/run/subproc.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/utils/run/subproc.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/smol_k8s_lab/utils/value_from.py` & `smol_k8s_lab-5.2.0/smol_k8s_lab/utils/value_from.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.1.0/PKG-INFO` & `smol_k8s_lab-5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smol_k8s_lab
-Version: 5.1.0
+Version: 5.2.0
 Summary: CLI and TUI to quickly install slimmer Kubernetes distros and then manage apps declaratively using Argo CD
 Home-page: https://small-hack.github.io/smol-k8s-lab
 License: AGPL-3.0-or-later
 Keywords: kubernetes,homelab,kind,k3s,k8s
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<3.13
@@ -21,14 +21,15 @@
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: cryptography (>=42.0,<43.0)
 Requires-Dist: kubernetes (>=29,<30)
 Requires-Dist: minio (>=7.2,<8.0)
 Requires-Dist: pyfiglet (>=1.0,<2.0)
 Requires-Dist: pygame (>=2.5.2,<3.0.0)
 Requires-Dist: pyjwt (>=2.8,<3.0)
+Requires-Dist: python-ulid (>=2.5.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.32,<3.0)
 Requires-Dist: rich (>=13.0,<14.0)
 Requires-Dist: ruamel-yaml (>=0.18,<0.19)
 Requires-Dist: ruamel-yaml-string (>=0.1,<0.2)
 Requires-Dist: textual (>=0.62,<0.63)
 Requires-Dist: xdg-base-dirs (>=6.0,<7.0)
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1 Name: smol_k8s_lab Version: 5.1.0 Summary: CLI and TUI to
+Metadata-Version: 2.1 Name: smol_k8s_lab Version: 5.2.0 Summary: CLI and TUI to
 quickly install slimmer Kubernetes distros and then manage apps declaratively
 using Argo CD Home-page: https://small-hack.github.io/smol-k8s-lab License:
 AGPL-3.0-or-later Keywords: kubernetes,homelab,kind,k3s,k8s Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<3.13 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
 License v3 or later (AGPLv3+) Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: System ::
 Installation/Setup Requires-Dist: bcrypt (>=4.1,<5.0) Requires-Dist: click
 (>=8.1,<9.0) Requires-Dist: cryptography (>=42.0,<43.0) Requires-Dist:
 kubernetes (>=29,<30) Requires-Dist: minio (>=7.2,<8.0) Requires-Dist: pyfiglet
 (>=1.0,<2.0) Requires-Dist: pygame (>=2.5.2,<3.0.0) Requires-Dist: pyjwt
-(>=2.8,<3.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: requests
-(>=2.32,<3.0) Requires-Dist: rich (>=13.0,<14.0) Requires-Dist: ruamel-yaml
-(>=0.18,<0.19) Requires-Dist: ruamel-yaml-string (>=0.1,<0.2) Requires-Dist:
-textual (>=0.62,<0.63) Requires-Dist: xdg-base-dirs (>=6.0,<7.0) Project-URL:
-Bug Tracker, http://github.com/small-hack/smol-k8s-lab/issues Project-URL:
-Documentation, https://small-hack.github.io/smol-k8s-lab Project-URL:
-Repository, http://github.com/small-hack/smol-k8s-lab Description-Content-Type:
-text/markdown
+(>=2.8,<3.0) Requires-Dist: python-ulid (>=2.5.0,<3.0.0) Requires-Dist: pyyaml
+(>=6.0,<7.0) Requires-Dist: requests (>=2.32,<3.0) Requires-Dist: rich
+(>=13.0,<14.0) Requires-Dist: ruamel-yaml (>=0.18,<0.19) Requires-Dist: ruamel-
+yaml-string (>=0.1,<0.2) Requires-Dist: textual (>=0.62,<0.63) Requires-Dist:
+xdg-base-dirs (>=6.0,<7.0) Project-URL: Bug Tracker, http://github.com/small-
+hack/smol-k8s-lab/issues Project-URL: Documentation, https://small-
+hack.github.io/smol-k8s-lab Project-URL: Repository, http://github.com/small-
+hack/smol-k8s-lab Description-Content-Type: text/markdown
   ********** [[hhttttppss::////rraaww..ggiitthhuubbuusseerrccoonntteenntt..ccoomm//ccaattppppuucccciinn//ccaattppppuucccciinn//mmaaiinn//aasssseettss//
 mmiisscc//ttrraannssppaarreenntt..ppnngg]]?ð??§?¸ ssmmooll--kk88ss--llaabb_[[_hh_tt_tt_pp_ss_::_//_//_ii_mm_gg_.._ss_hh_ii_ee_ll_dd_ss_.._ii_oo_//_gg_ii_tt_hh_uu_bb_//_vv_//_rr_ee_ll_ee_aa_ss_ee_//
                              _ss_mm_aa_ll_ll_--_hh_aa_cc_kk_//_ss_mm_oo_ll_--_kk_88_ss_--
  _ll_aa_bb_??_ss_tt_yy_ll_ee_==_pp_ll_aa_ss_tt_ii_cc_&&_ll_aa_bb_ee_ll_CC_oo_ll_oo_rr_==_44_88_44_88_44_88_&&_cc_oo_ll_oo_rr_==_33_CC_AA_33_22_44_&&_ll_oo_gg_oo_==_GG_ii_tt_HH_uu_bb_&&_ll_oo_gg_oo_CC_oo_ll_oo_rr_==_ww_hh_ii_tt_ee_]]
                                      **********
  A terminal based tool to install slimmer k8s distros on metal, with batteries
                                    included!
```

