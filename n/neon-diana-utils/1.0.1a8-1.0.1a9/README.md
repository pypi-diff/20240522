# Comparing `tmp/neon-diana-utils-1.0.1a8.tar.gz` & `tmp/neon-diana-utils-1.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-diana-utils-1.0.1a8.tar", last modified: Tue Nov 14 01:11:41 2023, max compression
+gzip compressed data, was "neon-diana-utils-1.0.1a9.tar", last modified: Tue Nov 21 22:27:28 2023, max compression
```

## Comparing `neon-diana-utils-1.0.1a8.tar` & `neon-diana-utils-1.0.1a9.tar`

### file list

```diff
@@ -1,293 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.789316 neon-diana-utils-1.0.1a8/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    15983 2023-11-14 01:11:41.789316 neon-diana-utils-1.0.1a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15574 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.761316 neon-diana-utils-1.0.1a8/neon_diana_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    31276 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.757316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.753316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.761316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/diana-backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/diana-backend/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.761316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/diana-backend/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/diana-backend/templates/_config-secret.tpl
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/diana-backend/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/diana-backend/templates/_rabbitmq-secret.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/diana-backend/templates/letsencrypt-issuer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/diana-backend/templates/secret_gh_token.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.761316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/diana-backend/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/diana-backend/templates/tests/test-connection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/diana-backend/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.765316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/http-services/
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/http-services/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.765316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/http-services/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/http-services/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/http-services/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.765316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/mq-services/
--rw-r--r--   0 runner    (1001) docker     (127)      897 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/mq-services/Chart.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/backend/mq-services/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.753316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.765316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-http/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-http/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.765316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-http/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-http/templates/_deployment.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-http/templates/_domain.tpl
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-http/templates/_ingress.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-http/templates/_service.tpl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.765316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-mq/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-mq/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.765316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-mq/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-mq/templates/_deployment.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-mq/templates/_service.tpl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.765316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-neon/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-neon/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.765316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-neon/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-neon/templates/_deployment.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/base-neon/templates/_service.tpl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.765316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/ingress-common/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/ingress-common/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.765316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/ingress-common/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/ingress-common/templates/namespace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/ingress-common/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.765316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/neon-rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/neon-rabbitmq/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.765316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/neon-rabbitmq/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/neon-rabbitmq/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      786 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/neon-rabbitmq/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/base/neon-rabbitmq/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.757316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.765316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/libretranslate/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/libretranslate/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.769316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/libretranslate/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/libretranslate/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/libretranslate/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/libretranslate/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/libretranslate/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/libretranslate/templates/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.769316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/libretranslate/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/libretranslate/templates/tests/test-connection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      767 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/libretranslate/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.769316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/stt-nemo/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/stt-nemo/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.769316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/stt-nemo/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/stt-nemo/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/stt-nemo/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/stt-nemo/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/stt-nemo/templates/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.769316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/stt-nemo/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/stt-nemo/templates/tests/test-connection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      722 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/stt-nemo/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.769316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-coqui/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-coqui/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.769316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-coqui/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-coqui/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-coqui/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-coqui/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-coqui/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-coqui/templates/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.769316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-coqui/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-coqui/templates/tests/test-connection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-coqui/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.769316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-glados/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-glados/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.769316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-glados/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-glados/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-glados/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-glados/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-glados/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-glados/templates/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.773316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-glados/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-glados/templates/tests/test-connection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-glados/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.773316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-larynx/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-larynx/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.773316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-larynx/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-larynx/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-larynx/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-larynx/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-larynx/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-larynx/templates/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.773316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-larynx/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-larynx/templates/tests/test-connection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-larynx/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.773316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-ljspeech/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-ljspeech/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.773316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-ljspeech/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-ljspeech/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-ljspeech/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-ljspeech/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-ljspeech/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-ljspeech/templates/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.773316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-ljspeech/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-ljspeech/templates/tests/test-connection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      722 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-ljspeech/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.773316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-mozilla/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-mozilla/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.773316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-mozilla/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-mozilla/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-mozilla/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-mozilla/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-mozilla/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-mozilla/templates/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.773316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-mozilla/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-mozilla/templates/tests/test-connection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      713 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-mozilla/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.773316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-nancy/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-nancy/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.777316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-nancy/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-nancy/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-nancy/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-nancy/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-nancy/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-nancy/templates/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.777316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-nancy/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-nancy/templates/tests/test-connection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/tts-nancy/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.777316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/ww-snowboy/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/ww-snowboy/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.777316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/ww-snowboy/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/ww-snowboy/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/ww-snowboy/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/ww-snowboy/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/ww-snowboy/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/ww-snowboy/templates/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.777316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/ww-snowboy/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/ww-snowboy/templates/tests/test-connection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      713 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/http/ww-snowboy/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.757316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/klat/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.777316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/klat/klat-chat/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/klat/klat-chat/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.777316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/klat/klat-chat/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/klat/klat-chat/templates/_config-map.tpl
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/klat/klat-chat/templates/deployment-client.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/klat/klat-chat/templates/deployment-observer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/klat/klat-chat/templates/deployment-server.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/klat/klat-chat/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/klat/klat-chat/templates/service-client.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/klat/klat-chat/templates/service-observer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/klat/klat-chat/templates/service-server.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/klat/klat-chat/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.757316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.777316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-api-proxy/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-api-proxy/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.781316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-api-proxy/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-api-proxy/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-api-proxy/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-api-proxy/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-api-proxy/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.781316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-brands-service/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-brands-service/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.781316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-brands-service/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-brands-service/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-brands-service/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-brands-service/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-brands-service/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.781316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-email-proxy/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-email-proxy/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.781316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-email-proxy/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-email-proxy/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-email-proxy/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-email-proxy/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-email-proxy/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.781316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-llm-chatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-llm-chatgpt/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.781316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-llm-chatgpt/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-llm-chatgpt/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-llm-chatgpt/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-llm-chatgpt/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-llm-chatgpt/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.781316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-llm-fastchat/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-llm-fastchat/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.781316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-llm-fastchat/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-llm-fastchat/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-llm-fastchat/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-llm-fastchat/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-llm-fastchat/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.781316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-metrics-service/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-metrics-service/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.785316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-metrics-service/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-metrics-service/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-metrics-service/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-metrics-service/templates/persistent-volume-claim.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-metrics-service/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-metrics-service/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.785316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-script-parser/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-script-parser/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.785316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-script-parser/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-script-parser/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-script-parser/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-script-parser/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/mq/neon-script-parser/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.757316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.785316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/core/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/core/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.785316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/core/templates/_config-map.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/core/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.785316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-audio/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-audio/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.785316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-audio/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-audio/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-audio/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-audio/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-audio/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.785316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-enclosure/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-enclosure/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.785316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-enclosure/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-enclosure/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-enclosure/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-enclosure/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-enclosure/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.785316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-gui/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-gui/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.785316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-gui/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-gui/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-gui/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-gui/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-gui/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.785316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-iris/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-iris/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.789316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-iris/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-iris/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-iris/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-iris/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-iris/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-iris/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.789316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-messagebus/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-messagebus/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.789316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-messagebus/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-messagebus/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-messagebus/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-messagebus/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-messagebus/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.789316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-skills/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-skills/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.789316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-skills/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-skills/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-skills/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-skills/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-skills/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.789316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-speech/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-speech/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.789316 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-speech/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-speech/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-speech/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-speech/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/helm_charts/neon/neon-speech/values.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/kubernetes_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/rabbitmq_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.789316 neon-diana-utils-1.0.1a8/neon_diana_utils/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/templates/mq_user_mapping.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/templates/rmq_backend_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/neon_diana_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 01:11:41.761316 neon-diana-utils-1.0.1a8/neon_diana_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15983 2023-11-14 01:11:41.000000 neon-diana-utils-1.0.1a8/neon_diana_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13189 2023-11-14 01:11:41.000000 neon-diana-utils-1.0.1a8/neon_diana_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 01:11:41.000000 neon-diana-utils-1.0.1a8/neon_diana_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-11-14 01:11:41.000000 neon-diana-utils-1.0.1a8/neon_diana_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-11-14 01:11:41.000000 neon-diana-utils-1.0.1a8/neon_diana_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-14 01:11:41.000000 neon-diana-utils-1.0.1a8/neon_diana_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 01:11:41.000000 neon-diana-utils-1.0.1a8/neon_diana_utils.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 01:11:41.789316 neon-diana-utils-1.0.1a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2023-11-14 01:11:38.000000 neon-diana-utils-1.0.1a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.351573 neon-diana-utils-1.0.1a9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15983 2023-11-21 22:27:28.351573 neon-diana-utils-1.0.1a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15574 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.347573 neon-diana-utils-1.0.1a9/neon_diana_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31276 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.343573 neon-diana-utils-1.0.1a9/neon_diana_utils/docker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.347573 neon-diana-utils-1.0.1a9/neon_diana_utils/docker/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/docker/backend/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/docker/backend/rabbitmq.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.347573 neon-diana-utils-1.0.1a9/neon_diana_utils/docker/neon_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/docker/neon_core/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.343573 neon-diana-utils-1.0.1a9/neon_diana_utils/docker/neon_core/xdg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.343573 neon-diana-utils-1.0.1a9/neon_diana_utils/docker/neon_core/xdg/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.343573 neon-diana-utils-1.0.1a9/neon_diana_utils/docker/neon_core/xdg/config/neon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.343573 neon-diana-utils-1.0.1a9/neon_diana_utils/docker/neon_core/xdg/config/neon/skills/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.347573 neon-diana-utils-1.0.1a9/neon_diana_utils/docker/neon_core/xdg/config/neon/skills/skill-homescreen-lite.openvoiceos/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/docker/neon_core/xdg/config/neon/skills/skill-homescreen-lite.openvoiceos/settings.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.347573 neon-diana-utils-1.0.1a9/neon_diana_utils/docker/neon_core/xdg/config/neon/skills/skill-local_music.neongeckocom/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/docker/neon_core/xdg/config/neon/skills/skill-local_music.neongeckocom/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/kubernetes_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/rabbitmq_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.347573 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.347573 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/backend/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.347573 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/backend/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/backend/templates/config-secret.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/backend/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.347573 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/klat/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/klat/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.351573 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/klat/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/klat/templates/config-map.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/klat/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/mq_user_mapping.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.351573 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/neon/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/neon/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.351573 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/neon/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/neon/templates/config-map.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/neon/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/templates/rmq_backend_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/neon_diana_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 22:27:28.347573 neon-diana-utils-1.0.1a9/neon_diana_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15983 2023-11-21 22:27:28.000000 neon-diana-utils-1.0.1a9/neon_diana_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-11-21 22:27:28.000000 neon-diana-utils-1.0.1a9/neon_diana_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 22:27:28.000000 neon-diana-utils-1.0.1a9/neon_diana_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2023-11-21 22:27:28.000000 neon-diana-utils-1.0.1a9/neon_diana_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2023-11-21 22:27:28.000000 neon-diana-utils-1.0.1a9/neon_diana_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-21 22:27:28.000000 neon-diana-utils-1.0.1a9/neon_diana_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 22:27:28.000000 neon-diana-utils-1.0.1a9/neon_diana_utils.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-21 22:27:28.351573 neon-diana-utils-1.0.1a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2023-11-21 22:27:25.000000 neon-diana-utils-1.0.1a9/setup.py
```

### Comparing `neon-diana-utils-1.0.1a8/LICENSE.md` & `neon-diana-utils-1.0.1a9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-diana-utils-1.0.1a8/PKG-INFO` & `neon-diana-utils-1.0.1a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-diana-utils
-Version: 1.0.1a8
+Version: 1.0.1a9
 Summary: Utilities for administration of Neon DIANA
 Home-page: https://github.com/NeonGeckoCom/neon-diana-backend
 Author: NeonGecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neon-diana-utils-1.0.1a8/README.md` & `neon-diana-utils-1.0.1a9/README.md`

 * *Files identical despite different names*

### Comparing `neon-diana-utils-1.0.1a8/neon_diana_utils/__init__.py` & `neon-diana-utils-1.0.1a9/neon_diana_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-diana-utils-1.0.1a8/neon_diana_utils/cli.py` & `neon-diana-utils-1.0.1a9/neon_diana_utils/cli.py`

 * *Files identical despite different names*

### Comparing `neon-diana-utils-1.0.1a8/neon_diana_utils/configuration.py` & `neon-diana-utils-1.0.1a9/neon_diana_utils/configuration.py`

 * *Files identical despite different names*

### Comparing `neon-diana-utils-1.0.1a8/neon_diana_utils/kubernetes_utils.py` & `neon-diana-utils-1.0.1a9/neon_diana_utils/kubernetes_utils.py`

 * *Files identical despite different names*

### Comparing `neon-diana-utils-1.0.1a8/neon_diana_utils/rabbitmq_api.py` & `neon-diana-utils-1.0.1a9/neon_diana_utils/rabbitmq_api.py`

 * *Files identical despite different names*

### Comparing `neon-diana-utils-1.0.1a8/neon_diana_utils/templates/rmq_backend_config.yml` & `neon-diana-utils-1.0.1a9/neon_diana_utils/templates/rmq_backend_config.yml`

 * *Files identical despite different names*

### Comparing `neon-diana-utils-1.0.1a8/neon_diana_utils/version.py` & `neon-diana-utils-1.0.1a9/neon_diana_utils/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a8"
+__version__ = "1.0.1a9"
```

### Comparing `neon-diana-utils-1.0.1a8/neon_diana_utils.egg-info/PKG-INFO` & `neon-diana-utils-1.0.1a9/neon_diana_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-diana-utils
-Version: 1.0.1a8
+Version: 1.0.1a9
 Summary: Utilities for administration of Neon DIANA
 Home-page: https://github.com/NeonGeckoCom/neon-diana-backend
 Author: NeonGecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neon-diana-utils-1.0.1a8/setup.py` & `neon-diana-utils-1.0.1a9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from setuptools import setup, find_packages
-from os import getenv, path
+from os import getenv, path, walk
 
 BASE_PATH = path.abspath(path.dirname(__file__))
 
 
 def get_requirements(requirements_filename: str):
     requirements_file = path.join(BASE_PATH, "requirements", requirements_filename)
     with open(requirements_file, 'r', encoding='utf-8') as r:
@@ -57,27 +57,41 @@
     for line in v.readlines():
         if line.startswith("__version__"):
             if '"' in line:
                 version = line.split('"')[1]
             else:
                 version = line.split("'")[1]
 
+
+def find_resource_files():
+    base_path = path.join(BASE_PATH, "neon_diana_utils")
+    resource_base_dirs = ("docker", "templates")
+    package_data = []
+    for res in resource_base_dirs:
+        if path.isdir(path.join(base_path, res)):
+            for (directory, _, files) in walk(path.join(base_path, res)):
+                if files:
+                    package_data.append(
+                        path.join(directory.replace(base_path, "").lstrip('/'),
+                                  '*'))
+    return package_data
+
+
 setup(
     name='neon-diana-utils',
     version=version,
     description='Utilities for administration of Neon DIANA',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/NeonGeckoCom/neon-diana-backend',
     author='NeonGecko',
     author_email='developers@neon.ai',
     license='BSD-3-Clause',
     packages=find_packages(),
-    package_data={'neon_diana_utils': ['templates/*', 'helm_charts/**']
-                  },
+    package_data={'neon_diana_utils': find_resource_files()},
     include_package_data=True,
     install_requires=get_requirements("requirements.txt"),
     zip_safe=True,
     classifiers=[
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3.6',
     ],
```

