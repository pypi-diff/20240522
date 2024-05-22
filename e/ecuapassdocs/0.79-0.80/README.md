# Comparing `tmp/ecuapassdocs-0.79.tar.gz` & `tmp/ecuapassdocs-0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecuapassdocs-0.79.tar", last modified: Thu May 16 12:56:41 2024, max compression
+gzip compressed data, was "ecuapassdocs-0.80.tar", last modified: Wed May 22 18:02:16 2024, max compression
```

## Comparing `ecuapassdocs-0.79.tar` & `ecuapassdocs-0.80.tar`

### file list

```diff
@@ -1,126 +1,122 @@
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.647493 ecuapassdocs-0.79/
--rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-05-16 12:56:41.647493 ecuapassdocs-0.79/PKG-INFO
--rw-rw-r--   0 lg        (1000) lg        (1000)       40 2024-04-22 18:48:50.000000 ecuapassdocs-0.79/README.md
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.543491 ecuapassdocs-0.79/ecuapassdocs/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.547491 ecuapassdocs-0.79/ecuapassdocs/info/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-17 23:52:12.000000 ecuapassdocs-0.79/ecuapassdocs/info/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     3416 2024-05-16 12:39:30.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_data.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    18226 2024-05-15 04:30:48.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_extractor.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     4490 2024-04-29 15:28:31.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_feedback.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     9457 2024-05-14 17:41:34.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    19585 2024-05-14 16:48:19.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     9140 2024-03-17 23:52:12.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1521 2024-05-12 16:16:09.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2732 2024-05-04 03:37:00.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1729 2024-03-17 23:52:12.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     4601 2024-03-17 23:52:12.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_declaracion.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    24020 2024-05-13 19:40:43.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1330 2024-03-17 23:52:12.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2187 2024-05-10 22:50:32.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2065 2024-05-13 22:36:59.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1654 2024-03-17 23:52:12.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    11223 2024-05-12 11:42:43.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_utils.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1463 2024-03-17 23:52:12.000000 ecuapassdocs-0.79/ecuapassdocs/info/resourceloader.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.547491 ecuapassdocs-0.79/ecuapassdocs/resources/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.567492 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-02-19 04:05:45.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-09-26 04:28:29.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-09-26 04:05:06.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-09-26 04:05:06.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-09-26 04:05:06.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      976 2023-09-26 04:05:06.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      195 2023-09-26 04:05:06.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/condiciones_transporte.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      108 2023-10-19 03:53:25.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/depositos_cebaf.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      369 2023-10-19 03:53:25.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/depositos_huaquillas.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      109 2023-10-19 03:53:25.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/depositos_loja.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      293 2023-10-19 03:53:25.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/depositos_quito.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      623 2024-05-14 16:35:53.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-09-26 04:05:06.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/derivado.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-09-26 04:28:51.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/distritos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      100 2023-09-26 04:29:01.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/documentos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       76 2023-10-16 19:53:52.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/empresa.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/meses.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-09-26 04:28:56.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/monedas.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 19:28:46.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/out.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-09-26 04:29:13.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/paises.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1971 2023-10-16 19:53:44.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/paises_todos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      124 2023-09-26 04:05:06.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/procedimientos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      924 2023-09-26 04:28:24.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/sustancias.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.567492 ecuapassdocs-0.79/ecuapassdocs/resources/data_declaracion/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_declaracion/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.595492 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1818 2023-10-16 13:31:38.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      554 2023-10-16 13:31:38.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      280 2023-10-16 13:31:38.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/aduanas_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      721 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       44 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/condiciones_unidadcarga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/derivado.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/distritos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       79 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/empresas_transporte.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/meses.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/paises.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      127 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/procedimientos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       70 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/sectores.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      105 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_carga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      103 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_documento.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_moneda.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       42 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1422 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.627493 ecuapassdocs-0.79/ecuapassdocs/resources/docs/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    18165 2024-03-26 00:09:58.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:08:52.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   185152 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    15815 2024-05-16 12:18:23.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte_input_parameters-CBIN_IDS.json
--rw-rw-r--   0 lg        (1000) lg        (1000)    15818 2024-05-16 12:20:48.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)   102275 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   184038 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    10893 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/declaracion_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)   281667 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   339751 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   361834 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:01:53.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/join.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)    74532 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   130529 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    18780 2024-05-16 12:23:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/manifiesto_input_parameters-CBIN_IDS.json
--rw-rw-r--   0 lg        (1000) lg        (1000)    18780 2024-05-12 00:44:17.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/manifiesto_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)   346795 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    95521 2024-03-26 00:59:47.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.647493 ecuapassdocs-0.79/ecuapassdocs/resources/images/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2379 2023-11-16 17:04:17.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/icon-colombia.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     2164 2023-11-16 17:08:35.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/icon-ecuador.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1449 2023-09-13 02:19:14.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/icon-white-bot.ico
--rw-rw-r--   0 lg        (1000) lg        (1000)   128273 2023-09-04 20:18:38.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    29117 2023-09-12 15:32:21.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-cartaporte-vacia.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    43614 2023-10-22 22:14:16.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-declaracion-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   134943 2023-10-06 23:29:34.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)      297 2023-10-21 21:41:16.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-scroll-up.png
--rw-rw-rw-   0 lg        (1000) lg        (1000)     1906 2023-08-13 18:09:07.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1727 2023-10-22 22:15:41.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1346 2023-10-21 20:53:42.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    10993 2023-11-23 18:07:54.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1270 2023-11-23 18:09:48.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png
--rw-rw-rw-   0 lg        (1000) lg        (1000)      418 2023-08-13 18:52:28.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-windows-WindowButtons.png
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.543491 ecuapassdocs-0.79/ecuapassdocs.egg-info/
--rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-05-16 12:56:41.000000 ecuapassdocs-0.79/ecuapassdocs.egg-info/PKG-INFO
--rw-rw-r--   0 lg        (1000) lg        (1000)     6139 2024-05-16 12:56:41.000000 ecuapassdocs-0.79/ecuapassdocs.egg-info/SOURCES.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)        1 2024-05-16 12:56:41.000000 ecuapassdocs-0.79/ecuapassdocs.egg-info/dependency_links.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       46 2024-05-16 12:56:41.000000 ecuapassdocs-0.79/ecuapassdocs.egg-info/requires.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       13 2024-05-16 12:56:41.000000 ecuapassdocs-0.79/ecuapassdocs.egg-info/top_level.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       38 2024-05-16 12:56:41.647493 ecuapassdocs-0.79/setup.cfg
--rw-rw-r--   0 lg        (1000) lg        (1000)     1661 2024-05-16 12:56:39.000000 ecuapassdocs-0.79/setup.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.749927 ecuapassdocs-0.80/
+-rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-05-22 18:02:16.749927 ecuapassdocs-0.80/PKG-INFO
+-rw-rw-r--   0 lg        (1000) lg        (1000)      144 2024-05-18 12:09:20.000000 ecuapassdocs-0.80/README.md
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.717928 ecuapassdocs-0.80/ecuapassdocs/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.725928 ecuapassdocs-0.80/ecuapassdocs/info/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-17 23:52:12.000000 ecuapassdocs-0.80/ecuapassdocs/info/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3416 2024-05-16 12:39:30.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_data.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18205 2024-05-20 18:19:53.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_extractor.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     4638 2024-05-18 12:32:53.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_feedback.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     9720 2024-05-20 18:17:08.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    19650 2024-05-19 22:14:26.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     9140 2024-03-17 23:52:12.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1521 2024-05-12 16:16:09.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2732 2024-05-04 03:37:00.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1729 2024-03-17 23:52:12.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     4601 2024-03-17 23:52:12.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_declaracion.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    24020 2024-05-13 19:40:43.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1330 2024-03-17 23:52:12.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2187 2024-05-10 22:50:32.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2065 2024-05-13 22:36:59.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1654 2024-03-17 23:52:12.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    13890 2024-05-20 12:55:05.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_utils.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1463 2024-03-17 23:52:12.000000 ecuapassdocs-0.80/ecuapassdocs/info/resourceloader.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.725928 ecuapassdocs-0.80/ecuapassdocs/resources/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.729928 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-02-19 04:05:45.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-09-26 04:28:29.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-09-26 04:05:06.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-09-26 04:05:06.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-09-26 04:05:06.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      976 2023-09-26 04:05:06.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      195 2023-09-26 04:05:06.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/condiciones_transporte.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      108 2023-10-19 03:53:25.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/depositos_cebaf.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      369 2023-10-19 03:53:25.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/depositos_huaquillas.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      109 2023-10-19 03:53:25.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/depositos_loja.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      293 2023-10-19 03:53:25.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/depositos_quito.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      623 2024-05-14 16:35:53.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-09-26 04:05:06.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/derivado.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-09-26 04:28:51.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/distritos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      100 2023-09-26 04:29:01.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/documentos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       76 2023-10-16 19:53:52.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/empresa.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/meses.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-09-26 04:28:56.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/monedas.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 19:28:46.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/out.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-09-26 04:29:13.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/paises.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1971 2023-10-16 19:53:44.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/paises_todos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      124 2023-09-26 04:05:06.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/procedimientos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      924 2023-09-26 04:28:24.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/sustancias.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.729928 ecuapassdocs-0.80/ecuapassdocs/resources/data_declaracion/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_declaracion/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.737928 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1818 2023-10-16 13:31:38.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      554 2023-10-16 13:31:38.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      280 2023-10-16 13:31:38.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/aduanas_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      721 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       44 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/condiciones_unidadcarga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/derivado.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/distritos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       79 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/empresas_transporte.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/meses.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/paises.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      127 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/procedimientos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       70 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/sectores.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      105 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_carga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      103 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_documento.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_moneda.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       42 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1422 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.741928 ecuapassdocs-0.80/ecuapassdocs/resources/docs/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18165 2024-03-26 00:09:58.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:08:52.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   185152 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    15818 2024-05-16 12:20:48.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/cartaporte_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)   281667 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   339751 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   361834 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    74532 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   130529 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18780 2024-05-12 00:44:17.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/manifiesto_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)    95521 2024-03-26 00:59:47.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.749927 ecuapassdocs-0.80/ecuapassdocs/resources/images/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)   218079 2024-05-22 13:19:12.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/cartaporte-DUMMY.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2379 2023-11-16 17:04:17.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/icon-colombia.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2164 2023-11-16 17:08:35.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/icon-ecuador.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1449 2023-09-13 02:19:14.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/icon-white-bot.ico
+-rw-rw-r--   0 lg        (1000) lg        (1000)   128273 2023-09-04 20:18:38.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    29117 2023-09-12 15:32:21.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-cartaporte-vacia.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    43614 2023-10-22 22:14:16.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-declaracion-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   134943 2023-10-06 23:29:34.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)      297 2023-10-21 21:41:16.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-scroll-up.png
+-rw-rw-rw-   0 lg        (1000) lg        (1000)     1906 2023-08-13 18:09:07.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1727 2023-10-22 22:15:41.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1346 2023-10-21 20:53:42.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    10993 2023-11-23 18:07:54.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1270 2023-11-23 18:09:48.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png
+-rw-rw-rw-   0 lg        (1000) lg        (1000)      418 2023-08-13 18:52:28.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-windows-WindowButtons.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    23824 2024-05-22 13:29:05.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image_DUMMY.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   267971 2024-05-22 13:19:51.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/manifiesto_DUMMY.png
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.721928 ecuapassdocs-0.80/ecuapassdocs.egg-info/
+-rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-05-22 18:02:16.000000 ecuapassdocs-0.80/ecuapassdocs.egg-info/PKG-INFO
+-rw-rw-r--   0 lg        (1000) lg        (1000)     5870 2024-05-22 18:02:16.000000 ecuapassdocs-0.80/ecuapassdocs.egg-info/SOURCES.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)        1 2024-05-22 18:02:16.000000 ecuapassdocs-0.80/ecuapassdocs.egg-info/dependency_links.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       46 2024-05-22 18:02:16.000000 ecuapassdocs-0.80/ecuapassdocs.egg-info/requires.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       13 2024-05-22 18:02:16.000000 ecuapassdocs-0.80/ecuapassdocs.egg-info/top_level.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       38 2024-05-22 18:02:16.749927 ecuapassdocs-0.80/setup.cfg
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1700 2024-05-22 18:02:14.000000 ecuapassdocs-0.80/setup.py
```

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_data.py` & `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_data.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_extractor.py` & `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 			subject ["pais"] = pais
 				
 			cities = Extractor.getSubjectCitiesString (pais, resourcesPath)
 
 			reLocation = f"(?P<ciudad>{cities})[\s\-,\s]+(?P<pais>{pais})[.\s]*"
 			result = re.search (reLocation, text, flags=re.I)
 			if (result == None):
-				printx (f"No se pudo localizar o no existe ciudad en: '{text}' de '{type}'")
+				printx (f"Ciudad desconocida en texto: '{text}' de '{type}'")
 			else:
 			#if (type in ["06_Recepcion", "07_Embarque", "08_Entrega", "19_Emision"]):
 				subject ["ciudad"] = result.group ("ciudad") if result else None
 				text	= text.replace (result.group (0), "")
 
 		except:
 			Utils.printException (f"Obteniendo ciudad-pais de '{type}'", text)
@@ -338,24 +338,24 @@
 	def getTipoEmbalaje (text, resourcesPath):
 		Utils.printx (f">>> Extrayendo embalaje desde el texto: '{text}'")
 		try:
 			reNumber   = r'\d+(?:[.,]*\d*)+' # RE for extracting a float number 
 			reEmbalaje = rf"{reNumber}\s+(\b(\w+)\b)"    # String after number
 			embalaje   = Extractor.getValueRE (reEmbalaje, text) 
 
-			if "PALLETS" in embalaje:
+			if "PALLET" in embalaje or "ESTIBA":
 				return "152" # "[152] PALETAS"
-			elif "SACOS" in embalaje.upper ():
+			elif "SACO" in embalaje.upper ():
 				return "104" # "[104] SACO"
-			elif "CAJAS" in embalaje.upper ():
+			elif "CAJA" in embalaje.upper ():
 				return "035" # "[035] CAJA"
 			else:
 				return embalaje.strip () + "||LOW"
 		except:
-			Utils.printx (f">>> EXCEPCION: Problemas extrayendo embalaje desde texto: '{text}'")
+			Utils.printx (f"Problemas extrayendo embalaje desde texto: '{text}'")
 			return None
 
 	#------------------------------------------------------------------
 	#-- Extract numerical or text date from text ----------------------
 	#------------------------------------------------------------------
 	def getDate (text, resourcesPath):
 		numericalDate = "||LOW"
```

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_feedback.py` & `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_feedback.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,26 +16,36 @@
 	#----------------------------------------------------------------
 	def getBlobClient (text_blob_name):
 		# Azure Blob Storage container name
 		container_name = "blobfeedback"
 
 		# Azure Storage account connection string
 		#connection_string = os.environ.get ("AZR_BLOB_CONN_STR")
-		connection_string = "DefaultEndpointsProtocol=https;AccountName=lgformsstorage;AccountKey=BHsWkVaWQYStRq8FOpoIl0jI39W+WFvrSJmxesr0euIEJe+qkSi0LoTM0HZfyOn2XbYfnHir7CD8+ASt6ZJnwg==;EndpointSuffix=core.windows.net"
+		connection_string = EcuFeedback.getConnectionString ();
+		print ("ConnStr:", connection_string)
 
 		# Initialize the BlobServiceClient
 		blob_service_client = BlobServiceClient.from_connection_string (connection_string)
 
 		# Create a container (if it doesn't exist)
 		container_client = blob_service_client.get_container_client (container_name)
 		blob_client = container_client.get_blob_client (text_blob_name)
 
 		return (blob_client)
 
 	#----------------------------------------------------------------
+	#----------------------------------------------------------------
+	def getConnectionString ():
+
+		connStr = ""
+		connStr = ";".join ([f"k=i" for k,i in zip (azrKeys, azrInfo)])
+
+		return connStr
+
+	#----------------------------------------------------------------
 	# Send a text to blob
 	#----------------------------------------------------------------
 	def sendLog (empresa, filename):
 		logMessage = f"LOG_{empresa}_{filename.split ('.')[0]}"
 		print ("Sending log: ", logMessage)
 		try:
 			blob_client    = EcuFeedback.getBlobClient (f"{logMessage}")
```

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info.py` & `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,49 +26,53 @@
 		self.ecudoc         = {}
 
 	#-- Implemented in subclasses
 	def getEmpresaInfo (self):
 		return None
 
 	#-- Updated Ecuapass document fields with values ready to transmit
-	#-- Change names to codes for additional presition
+	#-- Change names to codes for additional presition. Remove '||LOW'
 	def updateEcuapassFile (self, ecuJsonFile):
+		ecuapassFields    = json.load (open (ecuJsonFile))
+		ecuapassFieldsUpd = self.updateEcuapassFields (ecuapassFields)
+		ecuJsonFileUpd    = Utils.saveFields (ecuapassFieldsUpd, ecuJsonFile, "UPDATE")
+		return ecuapassFieldsUpd
+
+	def updateEcuapassFields (self, ecuapassFields):
 		print ("-- Updating Ecuapass fields...")
-		ecudoc = json.load (open (ecuJsonFile))
-		for key in ecudoc:
-			if ecudoc [key] is None:
+		for key in ecuapassFields:
+			if ecuapassFields [key] is None:
 				continue
 
 			# Vehiculo
 			if "Tipo_Vehiculo" in key:
 				vehiculos    = {"SEMIRREMOLQUE":"SR", "TRACTOCAMION":"TC", "CAMION":"CA"}
-				ecudoc [key] = vehiculos [ecudoc[key]]
+				ecuapassFields [key] = vehiculos [ecuapassFields[key]]
 
 			# Embalaje
 			if "Embalaje" in key: 
-				embalaje = ecudoc [key].upper()
-				if "PALLETS" in embalaje:
+				embalaje = ecuapassFields [key].upper()
+				if "PALLET" in embalaje:
 					embalaje = "152" # "[152] PALETAS"
 				elif "SACO" in embalaje:
 					embalaje = "104" # "[104] SACO"
 				elif "CAJA" in embalaje:
 					embalaje = "035" # "[035] CAJA"
-				ecudoc [key] = embalaje
+				ecuapassFields [key] = embalaje
 
 			# Moneda
 			if "Moneda" in key:
-				ecudoc [key] = "USD"
+				ecuapassFields [key] = "USD"
 
 			# Remove confidence string ("||LOW")
-			value        = ecudoc [key] 
+			value        = ecuapassFields [key] 
 			value        = value.split ("||")[0] if value else None
-			ecudoc [key] = value if value != "" else None
+			ecuapassFields [key] = value if value != "" else None
 
-		ecuJsonFileUpd = Utils.saveFields (ecudoc, ecuJsonFile, "UPDATE")
-		return ecudoc
+		return ecuapassFields
 
 
 	#-- For all types of documents (fixed fro NTA and BYZA, check the others)
 	def getNumeroDocumento (self):
 		text   = Utils.getValue (self.fields, "00b_Numero")
 		numero = Extractor.getNumeroDocumento (text)
```

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte.py` & `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,17 +243,18 @@
 		return (location)
 
 	#-----------------------------------------------------------
 	# Get "Entrega" location and suggest a date if it is None
 	#-----------------------------------------------------------
 	def getEntregaLocation (self, key):
 		location = self.getLocationInfo (key)
+		print ("++ location:", location)
 		try:
 			# Add a week to 'entrega' from 'embarque' date
-			if location ["fecha"] == "||LOW":
+			if location ["fecha"] == "||LOW" or location ["fecha"] is None:
 				fechaEmbarque      = self.ecudoc ["34_FechaEmbarque"]
 				date_obj           = datetime.strptime (fechaEmbarque, "%d-%m-%Y")
 				new_date_obj       = date_obj  # Fecha actual
 
 				if "BYZA" in self.getNombreEmpresa().upper():
 					new_date_obj       = date_obj + timedelta(weeks=2)   # 15 días
```

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py` & `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py` & `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py` & `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py` & `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_declaracion.py` & `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_declaracion.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto.py` & `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py` & `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py` & `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py` & `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py` & `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_utils.py` & `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, json, re, sys
+import os, json, re, sys, tempfile
 
 from traceback import format_exc as traceback_format_exc
 import traceback
 
 from ecuapassdocs.info.resourceloader import ResourceLoader 
 
 #--------------------------------------------------------------------
@@ -302,20 +302,80 @@
 			pais, codigo = "ecuador", "EC"
 		else:
 			raise Exception (f"No se encontró país en texto: '{text}'")
 
 		return pais, codigo
 
 	#----------------------------------------------------------------
+	#----------------------------------------------------------------
+	def getCodigoPaisFromProcedimiento (empresa, procedimiento):
+		procedimientosBYZA = {"importacion":"CO", "exportacion":"EC"}
+		procedimiento = procedimiento.lower()
+		if empresa == "BYZA" and "importacion" in procedimiento :
+			return procedimientosBYZA ["importacion"]
+		elif empresa == "BYZA" and "exportacion" in procedimiento :
+			return procedimientosBYZA ["exportacion"]
+		else:
+			raise Exception (f"No se identificó código pais desde procedimiento '{procedimiento}'")
+
+	#-------------------------------------------------------------------
+	# Return 'EXPORTACION' or 'IMPORTACION' according to 'pais' and 'empresa'
+	#-------------------------------------------------------------------
+	def getProcedimientoFromPais (empresa, pais):
+		procedimientosBYZA = {"CO":"IMPORTACION", "EC":"EXPORTACION"}
+		pais = pais.upper ()
+		if empresa == "BYZA" and pais.startswith ("CO"):
+			return "IMPORTACION"
+		elif empresa == "BYZA" and pais.startswith ("EC"):
+			return "EXPORTACION"
+		else:
+			raise Exception (f"No se pudo identificar procedimiento desde '{empresa}':'{pais}'")
+
+	#----------------------------------------------------------------
 	#-- Return input parameters file
 	#----------------------------------------------------------------
 	def getInputsParametersFile (docType):
 		if docType == "CARTAPORTE":
 			inputsParametersFile = "cartaporte_input_parameters.json"
 		elif docType == "MANIFIESTO":
 			inputsParametersFile = "manifiesto_input_parameters.json"
 		elif docType == "DECLARACION":
 			inputsParametersFile = "declaracion_input_parameters.json"
 		else:
 			raise Exception (f"Tipo de documento desconocido:", docType)
 		return inputsParametersFile
 
+
+	#-----------------------------------------------------------
+	# Load user settings (empresa, codebinUrl, codebinUser...)
+	#-----------------------------------------------------------
+	def loadSettings (runningDir):
+		settingsPath  = os.path.join (runningDir, "settings.txt")
+		if os.path.exists (settingsPath) == False:
+			Utils.printx (f"ALERTA: El archivo de configuración '{settingsPath}' no existe")
+			sys.exit (-1)
+
+		settings  = json.load (open (settingsPath, encoding="utf-8")) 
+
+		empresa   = settings ["empresa"]
+		Utils.printx ("Empresa actual: ", empresa)
+		return settings
+
+	#-----------------------------------------------------------
+	# Extract field info from azure fields using info clases (e.g.
+	# CartaporteBiza
+	#-----------------------------------------------------------
+	def getEcuapassFieldInfo (INFOCLASS, fieldName, docFields):
+		jsonFieldsPath, runningDir = Utils.createTemporalJson (docFields)
+		docInfo           = INFOCLASS (jsonFieldsPath, runningDir)
+		ecuapassFields    = docInfo.getMainFields ()
+		ecuapassFieldsUpd = docInfo.updateEcuapassFields (ecuapassFields)
+		fieldInfo         = ecuapassFieldsUpd [fieldName]
+		return fieldInfo
+
+	def createTemporalJson (docFields):
+		numero   = docFields ["00b_Numero"]
+		tmpPath        = tempfile.gettempdir ()
+		jsonFieldsPath = os.path.join (tmpPath, f"ECUDOC-{numero}.json")
+		json.dump (docFields, open (jsonFieldsPath, "w"))
+		return (jsonFieldsPath, tmpPath)
+
```

### Comparing `ecuapassdocs-0.79/ecuapassdocs/info/resourceloader.py` & `ecuapassdocs-0.80/ecuapassdocs/info/resourceloader.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/out.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/out.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/paises_todos.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/paises_todos.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/sustancias.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/sustancias.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf` & `ecuapassdocs-0.80/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf` & `ecuapassdocs-0.80/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg` & `ecuapassdocs-0.80/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte_input_parameters-CBIN_IDS.json` & `ecuapassdocs-0.80/ecuapassdocs/resources/docs/cartaporte_input_parameters.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990842490842491%*

 * *Differences: {"'txt09'": "{'codebinField': 'condiciones'}", "'txt18'": "{'codebinField': 'documentosr'}"}*

```diff
@@ -179,15 +179,15 @@
         "width": 501,
         "x": 555,
         "y": 405
     },
     "txt09": {
         "align": "left",
         "class": "input_condiciones",
-        "codebinField": "notificar",
+        "codebinField": "condiciones",
         "ecudocsField": "09_Condiciones",
         "font": "normal",
         "fontSize": "14px",
         "height": 70,
         "maxChars": 50,
         "maxLines": 4,
         "value": "",
@@ -573,15 +573,15 @@
         "width": 94,
         "x": 447,
         "y": 1061
     },
     "txt18": {
         "align": "left",
         "class": "input_documento",
-        "codebinField": "docmentosr",
+        "codebinField": "documentosr",
         "ecudocsField": "18_Documentos",
         "font": "normal",
         "fontSize": "14px",
         "height": 36,
         "maxChars": 50,
         "maxLines": 2,
         "value": "",
```

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte_input_parameters.json` & `ecuapassdocs-0.80/ecuapassdocs/resources/docs/manifiesto_input_parameters.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.29407548972766373%*

 * *Differences: {"'id'": "{'x': 400}",*

 * * "'numero'": "{'x': 200}",*

 * * "'txt00'": "{'codebinField': 'no', 'maxChars': 12, 'width': 203, 'x': 847, 'y': 94}",*

 * * "'txt01'": "{'fontSize': '28px', 'height': 150, 'maxChars': 100, 'maxLines': 5, 'width': 503, "*

 * *            "'x': 52, 'y': 172}",*

 * * "'txt02'": "{'align': 'center', 'class': 'input_permiso', 'ecudocsField': "*

 * *            "'02_Permiso_Originario', 'codebinField': '', 'font': 'large', 'fontSize': '28px', "*

 * *            "'height': 58, 'maxChars': 28, 'maxLines': 2, 'width': 485 […]*

```diff
@@ -12,15 +12,15 @@
         "restrictions": [
             "hidden",
             "readonly",
             "color=red"
         ],
         "value": "",
         "width": 233,
-        "x": 300,
+        "x": 400,
         "y": 88
     },
     "numero": {
         "align": "left",
         "class": "input_numero",
         "codebinField": "",
         "ecudocsField": "",
@@ -32,172 +32,172 @@
         "restrictions": [
             "hidden",
             "readonly",
             "color=red"
         ],
         "value": "",
         "width": 233,
-        "x": 300,
+        "x": 200,
         "y": 88
     },
     "txt00": {
         "align": "left",
         "class": "input_numero",
-        "codebinField": "nocpic",
+        "codebinField": "no",
         "ecudocsField": "00b_Numero",
         "font": "large",
         "fontSize": "26px",
         "height": 28,
-        "maxChars": 10,
+        "maxChars": 12,
         "maxLines": 1,
         "restrictions": [
             "color=red"
         ],
         "value": "",
-        "width": 233,
-        "x": 797,
-        "y": 88
+        "width": 203,
+        "x": 847,
+        "y": 94
     },
     "txt01": {
         "align": "left",
         "class": "input_numero",
         "codebinField": "",
         "ecudocsField": "01_Transportista",
         "font": "hidden",
-        "fontSize": "26px",
-        "height": 103,
-        "maxChars": 10,
-        "maxLines": 1,
+        "fontSize": "28px",
+        "height": 150,
+        "maxChars": 100,
+        "maxLines": 5,
         "restrictions": [
             "hidden"
         ],
         "value": "",
-        "width": 501,
-        "x": 40,
-        "y": 162
+        "width": 503,
+        "x": 52,
+        "y": 172
     },
     "txt02": {
-        "align": "left",
-        "class": "input_empresa",
-        "codebinField": "nremitente",
-        "ecudocsField": "02_Remitente",
-        "font": "normal",
-        "fontSize": "14px",
-        "height": 70,
-        "maxChars": 50,
-        "maxLines": 4,
+        "align": "center",
+        "class": "input_permiso",
+        "codebinField": "",
+        "ecudocsField": "02_Permiso_Originario",
+        "font": "large",
+        "fontSize": "28px",
+        "height": 58,
+        "maxChars": 28,
+        "maxLines": 2,
         "value": "",
-        "width": 501,
-        "x": 40,
-        "y": 302
+        "width": 485,
+        "x": 572,
+        "y": 172
     },
     "txt03": {
-        "align": "left",
-        "class": "input_empresa",
-        "codebinField": "ndestinatario",
-        "ecudocsField": "03_Destinatario",
-        "font": "normal",
-        "fontSize": "14px",
-        "height": 70,
-        "maxChars": 50,
-        "maxLines": 4,
+        "align": "center",
+        "class": "input_permiso",
+        "codebinField": "",
+        "ecudocsField": "03_Permiso_Servicios",
+        "font": "large",
+        "fontSize": "28px",
+        "height": 58,
+        "maxChars": 28,
+        "maxLines": 2,
         "value": "",
-        "width": 501,
-        "x": 40,
-        "y": 397
+        "width": 485,
+        "x": 572,
+        "y": 264
     },
     "txt04": {
         "align": "left",
-        "class": "input_empresa",
-        "codebinField": "consignatario",
-        "ecudocsField": "04_Consignatario",
+        "class": "input_general",
+        "codebinField": "a4",
+        "ecudocsField": "04_Camion_Marca",
         "font": "normal",
         "fontSize": "14px",
-        "height": 70,
-        "maxChars": 50,
-        "maxLines": 4,
+        "height": 25,
+        "maxChars": 25,
+        "maxLines": 1,
         "value": "",
-        "width": 501,
-        "x": 40,
-        "y": 492
+        "width": 251,
+        "x": 52,
+        "y": 372
     },
     "txt05": {
         "align": "left",
-        "class": "input_empresa",
-        "codebinField": "notificar",
-        "ecudocsField": "05_Notificado",
+        "class": "input_fecha",
+        "codebinField": "a5",
+        "ecudocsField": "05_Camion_AnoFabricacion",
         "font": "normal",
         "fontSize": "14px",
-        "height": 70,
-        "maxChars": 50,
-        "maxLines": 4,
+        "height": 25,
+        "maxChars": 15,
+        "maxLines": 1,
         "value": "",
-        "width": 501,
-        "x": 555,
-        "y": 140
+        "width": 135,
+        "x": 316,
+        "y": 372
     },
     "txt06": {
         "align": "left",
-        "class": "input-lugar-fecha",
-        "codebinField": "lugar1",
-        "ecudocsField": "06_Recepcion",
+        "class": "input_placaPais",
+        "codebinField": "a6",
+        "ecudocsField": "06_Camion_PlacaPais",
         "font": "normal",
         "fontSize": "14px",
-        "height": 40,
-        "maxChars": 50,
-        "maxLines": 2,
+        "height": 25,
+        "maxChars": 30,
+        "maxLines": 1,
         "value": "",
-        "width": 501,
-        "x": 555,
-        "y": 235
+        "width": 279,
+        "x": 463,
+        "y": 372
     },
     "txt07": {
         "align": "left",
-        "class": "input-lugar-fecha",
-        "codebinField": "lugar2",
-        "ecudocsField": "07_Embarque",
+        "class": "input_general",
+        "codebinField": "a7",
+        "ecudocsField": "07_Camion_Chasis",
         "font": "normal",
         "fontSize": "14px",
-        "height": 40,
-        "maxChars": 50,
-        "maxLines": 2,
+        "height": 25,
+        "maxChars": 30,
+        "maxLines": 1,
         "value": "",
-        "width": 501,
-        "x": 555,
-        "y": 312
+        "width": 304,
+        "x": 753,
+        "y": 372
     },
     "txt08": {
         "align": "left",
-        "class": "input_lugar",
-        "codebinField": "lugar3",
-        "ecudocsField": "08_Entrega",
+        "class": "input_certificado",
+        "codebinField": "a8",
+        "ecudocsField": "08_Certificado_Habilitacion",
         "font": "normal",
         "fontSize": "14px",
-        "height": 40,
-        "maxChars": 50,
-        "maxLines": 2,
+        "height": 20,
+        "maxChars": 80,
+        "maxLines": 1,
         "value": "",
-        "width": 501,
-        "x": 555,
-        "y": 405
+        "width": 700,
+        "x": 277,
+        "y": 403
     },
     "txt09": {
         "align": "left",
-        "class": "input_condiciones",
-        "codebinField": "condiciones",
-        "ecudocsField": "09_Condiciones",
+        "class": "input_general",
+        "codebinField": "a9",
+        "ecudocsField": "09_Remolque_Marca",
         "font": "normal",
         "fontSize": "14px",
-        "height": 70,
-        "maxChars": 50,
-        "maxLines": 4,
+        "height": 25,
+        "maxChars": 25,
+        "maxLines": 1,
         "value": "",
-        "width": 501,
-        "x": 555,
-        "y": 492
+        "width": 251,
+        "x": 52,
+        "y": 464
     },
     "txt0a": {
         "align": "left",
         "class": "input_numero",
         "codebinField": "",
         "ecudocsField": "00_Pais",
         "font": "large",
@@ -207,446 +207,584 @@
         "maxLines": 1,
         "restrictions": [
             "readonly",
             "color=red"
         ],
         "value": "",
         "width": 40,
-        "x": 696,
-        "y": 88
+        "x": 760,
+        "y": 94
     },
     "txt10": {
         "align": "left",
-        "class": "input_bultos",
+        "class": "input_general",
         "codebinField": "a10",
-        "ecudocsField": "10_CantidadClase_Bultos",
-        "font": "small",
-        "fontSize": "12px",
-        "height": 302,
-        "maxChars": 13,
-        "maxLines": 22,
+        "ecudocsField": "10_Remolque_AnoFabricacion",
+        "font": "normal",
+        "fontSize": "14px",
+        "height": 25,
+        "maxChars": 15,
+        "maxLines": 1,
         "value": "",
-        "width": 130,
-        "x": 43,
-        "y": 643
+        "width": 135,
+        "x": 316,
+        "y": 464
     },
     "txt11": {
         "align": "left",
-        "class": "input_bultos",
+        "class": "input_placaPais",
         "codebinField": "a11",
-        "ecudocsField": "11_MarcasNumeros_Bultos",
-        "font": "small",
-        "fontSize": "12px",
-        "height": 302,
-        "maxChars": 13,
-        "maxLines": 22,
+        "ecudocsField": "11_Remolque_PlacaPais",
+        "font": "normal",
+        "fontSize": "14px",
+        "height": 25,
+        "maxChars": 30,
+        "maxLines": 1,
         "value": "",
-        "width": 122,
-        "x": 183,
-        "y": 643
+        "width": 277,
+        "x": 464,
+        "y": 464
     },
     "txt12": {
         "align": "left",
-        "class": "input_descripcion",
-        "codebinField": "detalle",
-        "ecudocsField": "12_Descripcion_Bultos",
-        "font": "small",
-        "fontSize": "12px",
-        "height": 302,
-        "maxChars": 50,
-        "maxLines": 22,
-        "value": "",
-        "width": 472,
-        "x": 315,
-        "y": 643
-    },
-    "txt13_1": {
-        "align": "right",
-        "class": "input_valor",
-        "codebinField": "neto1",
-        "ecudocsField": "13a_Peso_Neto",
+        "class": "input_general",
+        "codebinField": "a12",
+        "ecudocsField": "12_Remolque_Otro",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 10,
+        "height": 25,
+        "maxChars": 30,
         "maxLines": 1,
         "value": "",
-        "width": 121,
-        "x": 797,
-        "y": 677
+        "width": 303,
+        "x": 754,
+        "y": 464
     },
-    "txt13_2": {
-        "align": "right",
-        "class": "input_valor",
-        "codebinField": "bruto1",
-        "ecudocsField": "13b_Peso_Bruto",
+    "txt13": {
+        "align": "left",
+        "class": "input_conductor",
+        "codebinField": "a13",
+        "ecudocsField": "13_Conductor_Nombre",
         "font": "normal",
         "fontSize": "14px",
         "height": 22,
-        "maxChars": 10,
+        "maxChars": 50,
         "maxLines": 1,
         "value": "",
-        "width": 121,
-        "x": 935,
-        "y": 677
+        "width": 470,
+        "x": 52,
+        "y": 526
     },
     "txt14": {
-        "align": "right",
-        "class": "input_valor",
-        "codebinField": "volumen",
-        "ecudocsField": "14_Volumen",
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "a14",
+        "ecudocsField": "14_Conductor_Id",
         "font": "normal",
         "fontSize": "14px",
         "height": 22,
-        "maxChars": 10,
+        "maxChars": 20,
         "maxLines": 1,
         "value": "",
-        "width": 121,
-        "x": 797,
-        "y": 777
+        "width": 210,
+        "x": 52,
+        "y": 571
     },
     "txt15": {
-        "align": "right",
-        "class": "input_valor",
-        "codebinField": "omedidas",
-        "ecudocsField": "15_Otras_Unidades",
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "a15",
+        "ecudocsField": "15_Conductor_Nacionalidad",
         "font": "normal",
         "fontSize": "14px",
         "height": 22,
-        "maxChars": 10,
+        "maxChars": 20,
         "maxLines": 1,
         "value": "",
-        "width": 121,
-        "x": 935,
-        "y": 777
+        "width": 247,
+        "x": 276,
+        "y": 571
     },
     "txt16": {
         "align": "left",
-        "class": "input_incoterm",
-        "codebinField": "precio",
-        "ecudocsField": "16_Incoterms",
+        "class": "input_general",
+        "codebinField": "a16",
+        "ecudocsField": "16_Conductor_Licencia",
         "font": "normal",
         "fontSize": "14px",
-        "height": 67,
-        "maxChars": 28,
-        "maxLines": 3,
+        "height": 22,
+        "maxChars": 20,
+        "maxLines": 1,
         "value": "",
-        "width": 263,
-        "x": 795,
-        "y": 869
+        "width": 210,
+        "x": 52,
+        "y": 615
     },
-    "txt17_11": {
-        "align": "right",
-        "class": "input_valor",
-        "codebinField": "montor",
-        "ecudocsField": "17_Gastos:ValorFlete,MontoRemitente",
+    "txt17": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "a17",
+        "ecudocsField": "17_Conductor_Libreta",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 10,
+        "height": 22,
+        "maxChars": 20,
         "maxLines": 1,
         "value": "",
-        "width": 114,
-        "x": 112,
-        "y": 997
+        "width": 245,
+        "x": 277,
+        "y": 615
     },
-    "txt17_12": {
-        "align": "right",
-        "class": "input_valor",
-        "codebinField": "montor1",
-        "ecudocsField": "17_Gastos:Seguro,MontoRemitente",
+    "txt18": {
+        "align": "left",
+        "class": "input_conductor",
+        "codebinField": "a18",
+        "ecudocsField": "18_Auxiliar_Nombre",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 10,
+        "height": 22,
+        "maxChars": 50,
         "maxLines": 1,
         "value": "",
-        "width": 114,
-        "x": 112,
-        "y": 1018
+        "width": 522,
+        "x": 535,
+        "y": 526
     },
-    "txt17_13": {
-        "align": "right",
-        "class": "input_valor",
-        "codebinField": "montoor",
-        "ecudocsField": "17_Gastos:OtrosGastos,MontoRemitente",
+    "txt19": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "a19",
+        "ecudocsField": "19_Auxiliar_Id",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 10,
+        "height": 22,
+        "maxChars": 20,
         "maxLines": 1,
         "value": "",
-        "width": 114,
-        "x": 112,
-        "y": 1039
+        "width": 252,
+        "x": 535,
+        "y": 571
     },
-    "txt17_14": {
-        "align": "right",
-        "class": "input_valor",
-        "codebinField": "totalmr",
-        "ecudocsField": "17_Gastos:Total,MontoRemitente",
+    "txt20": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "a20",
+        "ecudocsField": "20_Auxiliar_Nacionalidad",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 10,
+        "height": 22,
+        "maxChars": 20,
         "maxLines": 1,
         "value": "",
-        "width": 114,
-        "x": 112,
-        "y": 1061
+        "width": 257,
+        "x": 800,
+        "y": 571
     },
-    "txt17_21": {
+    "txt21": {
         "align": "left",
         "class": "input_general",
-        "codebinField": "moneda1",
-        "ecudocsField": "17_Gastos:ValorFlete,MonedaRemitente",
+        "codebinField": "a21",
+        "ecudocsField": "21_Auxiliar_Licencia",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 8,
+        "height": 22,
+        "maxChars": 20,
         "maxLines": 1,
         "value": "",
-        "width": 80,
-        "x": 240,
-        "y": 997
+        "width": 252,
+        "x": 535,
+        "y": 615
     },
-    "txt17_22": {
+    "txt22": {
         "align": "left",
         "class": "input_general",
-        "codebinField": "moneda3",
-        "ecudocsField": "17_Gastos:Seguro,MonedaRemitente",
+        "codebinField": "a22",
+        "ecudocsField": "22_Auxiliar_Libreta",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 8,
+        "height": 22,
+        "maxChars": 20,
         "maxLines": 1,
         "value": "",
-        "width": 80,
-        "x": 240,
-        "y": 1018
+        "width": 257,
+        "x": 800,
+        "y": 615
     },
-    "txt17_23": {
+    "txt23": {
         "align": "left",
-        "class": "input_general",
-        "codebinField": "moneda5",
-        "ecudocsField": "17_Gastos:OtrosGastos,MonedaRemitente",
+        "class": "input_lugar",
+        "codebinField": "23",
+        "ecudocsField": "23_Carga_CiudadPais",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 8,
+        "height": 22,
+        "maxChars": 50,
+        "maxLines": 1,
+        "value": "",
+        "width": 470,
+        "x": 52,
+        "y": 676
+    },
+    "txt24": {
+        "align": "left",
+        "class": "input_lugar",
+        "codebinField": "24",
+        "ecudocsField": "24_Descarga_CiudadPais",
+        "font": "normal",
+        "fontSize": "14px",
+        "height": 22,
+        "maxChars": 55,
+        "maxLines": 1,
+        "value": "",
+        "width": 522,
+        "x": 535,
+        "y": 676
+    },
+    "txt25_1": {
+        "align": "left",
+        "class": "input_tipocarga",
+        "codebinField": "radio-1-set",
+        "ecudocsField": "25a_Carga_TipoPeligrosa",
+        "font": "normal",
+        "fontSize": "18px",
+        "height": 22,
+        "maxChars": 2,
+        "maxLines": 1,
+        "value": "",
+        "width": 18,
+        "x": 152,
+        "y": 724
+    },
+    "txt25_2": {
+        "align": "left",
+        "class": "input_tipocarga",
+        "codebinField": "radio-3-set",
+        "ecudocsField": "25b_Carga_TipoSustancias",
+        "font": "normal",
+        "fontSize": "18px",
+        "height": 22,
+        "maxChars": 2,
+        "maxLines": 1,
+        "value": "",
+        "width": 18,
+        "x": 432,
+        "y": 724
+    },
+    "txt25_3": {
+        "align": "left",
+        "class": "input_tipocarga",
+        "codebinField": "radio-2-set",
+        "ecudocsField": "25c_Carga_TipoPerecible",
+        "font": "normal",
+        "fontSize": "18px",
+        "height": 22,
+        "maxChars": 2,
+        "maxLines": 1,
+        "value": "",
+        "width": 18,
+        "x": 575,
+        "y": 724
+    },
+    "txt25_4": {
+        "align": "left",
+        "class": "input_tipocarga",
+        "codebinField": "radio-4-set",
+        "ecudocsField": "25d_Carga_TipoOtra",
+        "font": "normal",
+        "fontSize": "18px",
+        "height": 22,
+        "maxChars": 2,
         "maxLines": 1,
         "value": "",
-        "width": 80,
-        "x": 240,
-        "y": 1039
+        "width": 18,
+        "x": 700,
+        "y": 724
     },
-    "txt17_24": {
+    "txt25_5": {
         "align": "left",
         "class": "input_general",
-        "codebinField": "monedat",
-        "ecudocsField": "17_Gastos:Total,MonedaRemitente",
+        "codebinField": "25d",
+        "ecudocsField": "25e_Carga_TipoDescripcion",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 8,
+        "height": 48,
+        "maxChars": 20,
+        "maxLines": 2,
+        "value": "",
+        "width": 258,
+        "x": 799,
+        "y": 710
+    },
+    "txt26": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "26",
+        "ecudocsField": "26_Carga_Contenedores",
+        "font": "normal",
+        "fontSize": "14px",
+        "height": 22,
+        "maxChars": 50,
         "maxLines": 1,
         "value": "",
-        "width": 80,
-        "x": 240,
-        "y": 1061
+        "width": 470,
+        "x": 52,
+        "y": 798
     },
-    "txt17_31": {
-        "align": "right",
-        "class": "input_valor",
-        "codebinField": "montod",
-        "ecudocsField": "17_Gastos:ValorFlete,MontoDestinatario",
+    "txt27": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "27",
+        "ecudocsField": "27_Carga_Precintos",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 10,
+        "height": 22,
+        "maxChars": 55,
         "maxLines": 1,
         "value": "",
-        "width": 100,
-        "x": 334,
-        "y": 997
+        "width": 522,
+        "x": 535,
+        "y": 798
+    },
+    "txt28": {
+        "align": "left",
+        "class": "input_cartaporte",
+        "codebinField": "a28",
+        "ecudocsField": "28_Mercancia_Cartaporte",
+        "font": "small",
+        "fontSize": "12px",
+        "height": 341,
+        "maxChars": 13,
+        "maxLines": 20,
+        "value": "",
+        "width": 95,
+        "x": 52,
+        "y": 857
+    },
+    "txt29": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "a29",
+        "ecudocsField": "29_Mercancia_Descripcion",
+        "font": "small",
+        "fontSize": "12px",
+        "height": 341,
+        "maxChars": 52,
+        "maxLines": 20,
+        "value": "",
+        "width": 380,
+        "x": 155,
+        "y": 857
+    },
+    "txt30": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "a30",
+        "ecudocsField": "30_Mercancia_Bultos",
+        "font": "small",
+        "fontSize": "12px",
+        "height": 341,
+        "maxChars": 14,
+        "maxLines": 20,
+        "value": "",
+        "width": 105,
+        "x": 540,
+        "y": 857
+    },
+    "txt31": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "a31",
+        "ecudocsField": "31_Mercancia_Embalaje",
+        "font": "small",
+        "fontSize": "12px",
+        "height": 341,
+        "maxChars": 17,
+        "maxLines": 20,
+        "value": "",
+        "width": 130,
+        "x": 651,
+        "y": 857
     },
-    "txt17_32": {
+    "txt32_1": {
         "align": "right",
         "class": "input_valor",
-        "codebinField": "montod1",
-        "ecudocsField": "17_Gastos:Seguro,MontoDestinatario",
+        "codebinField": "a32a",
+        "ecudocsField": "32a_Peso_Bruto",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 10,
-        "maxLines": 1,
+        "height": 341,
+        "maxChars": 9,
+        "maxLines": 20,
         "value": "",
-        "width": 100,
-        "x": 334,
-        "y": 1018
+        "width": 82,
+        "x": 795,
+        "y": 857
     },
-    "txt17_33": {
+    "txt32_2": {
         "align": "right",
         "class": "input_valor",
-        "codebinField": "montod2",
-        "ecudocsField": "17_Gastos:OtrosGastos,MontoDestinatario",
+        "codebinField": "a34b",
+        "ecudocsField": "32a_Peso_BrutoTotal",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 10,
+        "height": 22,
+        "maxChars": 9,
         "maxLines": 1,
         "value": "",
-        "width": 100,
-        "x": 334,
-        "y": 1039
+        "width": 82,
+        "x": 795,
+        "y": 1223
     },
-    "txt17_34": {
+    "txt32_3": {
         "align": "right",
         "class": "input_valor",
-        "codebinField": "totalmd",
-        "ecudocsField": "17_Gastos:Total,MontoDestinatario",
+        "codebinField": "a32b",
+        "ecudocsField": "32b_Peso_Neto",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 10,
-        "maxLines": 1,
+        "height": 341,
+        "maxChars": 9,
+        "maxLines": 20,
         "value": "",
-        "width": 100,
-        "x": 334,
-        "y": 1061
+        "width": 82,
+        "x": 887,
+        "y": 857
     },
-    "txt17_41": {
-        "align": "left",
-        "class": "input_general",
-        "codebinField": "moneda2",
-        "ecudocsField": "17_Gastos:ValorFlete,MonedaDestinatario",
+    "txt32_4": {
+        "align": "right",
+        "class": "input_valor",
+        "codebinField": "a34c",
+        "ecudocsField": "32b_Peso_NetoTotal",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 8,
+        "height": 22,
+        "maxChars": 9,
         "maxLines": 1,
         "value": "",
-        "width": 94,
-        "x": 447,
-        "y": 997
+        "width": 82,
+        "x": 887,
+        "y": 1223
     },
-    "txt17_42": {
+    "txt33_1": {
         "align": "left",
-        "class": "input_general",
-        "codebinField": "moneda4",
-        "ecudocsField": "17_Gastos:Seguro,MonedaDestinatario",
+        "class": "input_valor",
+        "codebinField": "a33",
+        "ecudocsField": "33_Otra_Medida",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 8,
-        "maxLines": 1,
+        "height": 341,
+        "maxChars": 9,
+        "maxLines": 20,
         "value": "",
-        "width": 94,
-        "x": 447,
-        "y": 1018
+        "width": 82,
+        "x": 979,
+        "y": 857
     },
-    "txt17_43": {
+    "txt33_2": {
         "align": "left",
-        "class": "input_general",
-        "codebinField": "moneda6",
-        "ecudocsField": "17_Gastos:OtrosGastos,MonedaDestinatario",
+        "class": "input_valor",
+        "codebinField": "a34d",
+        "ecudocsField": "33_Otra_MedidaTotal",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 8,
+        "height": 22,
+        "maxChars": 9,
         "maxLines": 1,
         "value": "",
-        "width": 94,
-        "x": 447,
-        "y": 1039
+        "width": 82,
+        "x": 979,
+        "y": 1223
     },
-    "txt17_44": {
+    "txt34": {
         "align": "left",
-        "class": "input_general",
-        "codebinField": "monedat2",
-        "ecudocsField": "17_Gastos:Total,MonedaDestinatario",
+        "class": "input_incoterm",
+        "codebinField": "a34a",
+        "ecudocsField": "34_Precio_Incoterm_Moneda",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 8,
+        "height": 22,
+        "maxChars": 70,
         "maxLines": 1,
         "value": "",
-        "width": 94,
-        "x": 447,
-        "y": 1061
+        "width": 653,
+        "x": 52,
+        "y": 1223
     },
-    "txt18": {
+    "txt35": {
         "align": "left",
-        "class": "input_documento",
-        "codebinField": "documentosr",
-        "ecudocsField": "18_Documentos",
+        "class": "input_general",
+        "codebinField": "35",
+        "ecudocsField": "35_Observaciones",
         "font": "normal",
         "fontSize": "14px",
         "height": 36,
         "maxChars": 50,
         "maxLines": 2,
         "value": "",
-        "width": 503,
-        "x": 40,
-        "y": 1103
+        "width": 470,
+        "x": 52,
+        "y": 1262
     },
-    "txt19": {
+    "txt37": {
         "align": "left",
-        "class": "input-lugar-fecha",
-        "codebinField": "lugaremision",
-        "ecudocsField": "19_Emision",
+        "class": "input_general",
+        "codebinField": "37",
+        "ecudocsField": "37_Aduana_Cruce",
         "font": "normal",
         "fontSize": "14px",
-        "height": 40,
-        "maxChars": 50,
-        "maxLines": 2,
+        "height": 22,
+        "maxChars": 27,
+        "maxLines": 1,
         "value": "",
-        "width": 503,
-        "x": 40,
-        "y": 1171
+        "width": 253,
+        "x": 535,
+        "y": 1262
     },
-    "txt21": {
+    "txt38": {
         "align": "left",
         "class": "input_general",
-        "codebinField": "instrucciones",
-        "ecudocsField": "21_Instrucciones",
+        "codebinField": "38",
+        "ecudocsField": "38_Aduana_Destino",
         "font": "normal",
         "fontSize": "14px",
-        "height": 85,
-        "maxChars": 50,
-        "maxLines": 5,
+        "height": 22,
+        "maxChars": 27,
+        "maxLines": 1,
         "value": "",
-        "width": 503,
-        "x": 560,
-        "y": 963
+        "width": 257,
+        "x": 800,
+        "y": 1262
     },
-    "txt22": {
+    "txt40": {
         "align": "left",
-        "class": "input_general",
-        "codebinField": "observaciones",
-        "ecudocsField": "22_Observaciones",
-        "font": "normal",
-        "fontSize": "14px",
-        "height": 85,
-        "maxChars": 53,
-        "maxLines": 5,
+        "class": "input_fecha",
+        "codebinField": "a40",
+        "ecudocsField": "40_Fecha_Emision",
+        "font": "small",
+        "fontSize": "12px",
+        "height": 22,
+        "maxChars": 50,
+        "maxLines": 1,
         "value": "",
-        "width": 503,
-        "x": 560,
-        "y": 1070
+        "width": 350,
+        "x": 180,
+        "y": 1366
     },
-    "txt24": {
+    "txt41": {
         "align": "center",
         "class": "input_tipo",
         "codebinField": "",
-        "ecudocsField": "24_OriginalCopia",
+        "ecudocsField": "41_OriginalCopia",
         "font": "large",
-        "fontSize": "26px",
+        "fontSize": "18px",
         "height": 30,
-        "maxChars": 10,
-        "maxLines": 1,
+        "nChars": 10,
+        "nlines": 1,
+        "restrictions": [
+            "readonly"
+        ],
         "value": "",
         "width": 173,
         "x": 477,
-        "y": 1357
+        "y": 1394
     }
 }
```

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt` & `ecuapassdocs-0.80/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf` & `ecuapassdocs-0.80/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf`

 * *Files 17% similar despite different names*

#### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf` & `ecuapassdocs-0.80/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf`

 * *Document info*

```diff
@@ -1,3 +1,3 @@
-CreationDate: "D:20240225094117-05'00"
+CreationDate: "D:20240228134719-05'00"
 Creator: 'Inkscape 1.1.2 (https://inkscape.org)'
 Producer: 'cairo 1.16.0 (https://cairographics.org)'
```

#### pdftotext {} -

```diff
@@ -1,77 +1,78 @@
-Declaración de Tránsito Aduanero Internacional (DTAI)
-
+Carta de Porte Internacional por Carretera (CPIC)
 No.
 
-COMUNIDAD ANDINA
-8. País y aduana de destino
+PO-CO-0033-22
 
-1. D enom inación o razón social y dirección del transportista autorizado
+5. Notificar a
 
-9. País de origen de la mercancía
+1. Denominación o razón social y dirección del Transportista
 
-2. Nombre y dirección del declarante
+6. Lugar, país y fecha en la que el transportista recibe las mercancías
 
-10. Placa y país de matrícula de los vehículos habilitados
+2. Nombre y dirección del remitente
 
-3. N om bre y dirección del rem itente
+7. Lugar, país y fecha de embarque de las mercancías
 
-11. Placa y país de matrícula o registro de las unidades de carga
+3. Nombre y dirección del destinatario
 
-4. Nombre y dirección del destinatario
+8. Lugar, país y fecha convenida para la entrega de las mercancías
 
-12. Número(s) de (los) Maniﬁesto(s) de Carga Internacional
+4. Nombre y dirección del consignatario
 
-5. Nombre y dirección del consignatario
+9. Condiciones del transporte y condiciones de pago
 
-13. N úm eros de identificación de los contenedores y su capacidad
-(Indicar si son de 20, 40 pies u otra)
+10. Cantidad clase
+de los bultos
 
-6. Aduana de carga
-14. Número(s) de los precintos aduaneros
+11. Marca y número 12. Descripción corriente de la naturaleza de las mercancías (indicar si son 13. PESO EN KILOGRAMOS
+de los bultos
+peligrosas)
+Neto
 
-7. País y aduana de partida
+Bruto
 
-16. Descripción de las mercancías
+14. Volumen en
+metros cúbicos
 
-21. Precio de las mercancías (INCOTERMS acordado
-entre las Partes) y tipo de moneda
+15. Otras unidades
+de medida
 
-17. Cantidad de
-los bultos
+16. Precio de las mercancías
+(INCOTERMS 2020) y tipo de
 
-Fecha
+21. Instrucciones al transportista
 
-19. Peso en kilogramos
-Bruto
+17. GASTOS A PAGAR
+Concepto
 
-Neto
+Remitente
+
+Tipo moneda
+
+Destinatario
 
-20. Volumen en
-metros cubicos u
-otra unidad de
-medida
+Flete
+Seguro
+Otros
+Total
 
-22. País y aduana(s) de cruce de fronteras
+Tipo moneda
 
-El suscrito se obliga a cum plir en esta O peración de Transito Aduanero
-Internacional, con las disposiciones de las norm as que conform an el
-ordenam iento jurídico de la C om unidad Andina
-23. Firm a y Sello del declarante, fecha
+22. Observaciones del transportista
 
-18. Tipo de embalaje
-y marca de los bultos
+19. Lugar, país y fecha de emisión
 
-TOTAL
-24. O bservaciones de la aduana de partida
+El suscrito al hacerse cargo de las mercancías, se obliga a cumplir las disposiciones de las normas que
+conforman el ordenamiento jurídico de la Comunidad Andina, en particular con la Decisión 837 y su Reglamento.
+En el Reverso de esta CPIC con hoja separada el motransportista autorizado podra establecer cláusulas
+generales o particulares de contratación del servicio de transporte.
 
-25. D ocum entos Anexos
+20. Nombre y firma del remitente o su representante o agente
 
-26. Firm a y sello de la autoridad que interviene en la aduana de partida,
-fecha
+23. Nombre, firma y sello del transportista autorizado o su representante o
 
 www.ecuapassdocs.com
 
-15. Carta de
-Porte No
+18. Documentos recibidos del remitentes
```

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png` & `ecuapassdocs-0.80/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png` & `ecuapassdocs-0.80/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png` & `ecuapassdocs-0.80/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf` & `ecuapassdocs-0.80/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg` & `ecuapassdocs-0.80/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/images/icon-colombia.png` & `ecuapassdocs-0.80/ecuapassdocs/resources/images/icon-colombia.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/images/icon-ecuador.png` & `ecuapassdocs-0.80/ecuapassdocs/resources/images/icon-ecuador.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/images/icon-white-bot.ico` & `ecuapassdocs-0.80/ecuapassdocs/resources/images/icon-white-bot.ico`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png` & `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-cartaporte-vacia.png` & `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-cartaporte-vacia.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-declaracion-ecuapass.png` & `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-declaracion-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png` & `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png` & `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png` & `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png` & `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png` & `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png` & `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.79/ecuapassdocs.egg-info/SOURCES.txt` & `ecuapassdocs-0.80/ecuapassdocs.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -77,38 +77,34 @@
 ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
 ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
 ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
 ecuapassdocs/resources/docs/__init__.py
 ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf
 ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
 ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
-ecuapassdocs/resources/docs/cartaporte_input_parameters-CBIN_IDS.json
 ecuapassdocs/resources/docs/cartaporte_input_parameters.json
 ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
-ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf
-ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg
-ecuapassdocs/resources/docs/declaracion_input_parameters.json
 ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
 ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
 ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
-ecuapassdocs/resources/docs/join.pdf
 ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
 ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
-ecuapassdocs/resources/docs/manifiesto_input_parameters-CBIN_IDS.json
 ecuapassdocs/resources/docs/manifiesto_input_parameters.json
-ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png
 ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf
 ecuapassdocs/resources/images/__init__.py
+ecuapassdocs/resources/images/cartaporte-DUMMY.png
 ecuapassdocs/resources/images/icon-colombia.png
 ecuapassdocs/resources/images/icon-ecuador.png
 ecuapassdocs/resources/images/icon-white-bot.ico
 ecuapassdocs/resources/images/image-cartaporte-ecuapass.png
 ecuapassdocs/resources/images/image-cartaporte-vacia.png
 ecuapassdocs/resources/images/image-declaracion-ecuapass.png
 ecuapassdocs/resources/images/image-manifiesto-ecuapass.png
 ecuapassdocs/resources/images/image-scroll-up.png
 ecuapassdocs/resources/images/image-text-CartaporteCarretera.png
 ecuapassdocs/resources/images/image-text-DeclaracionTransito.png
 ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png
 ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png
 ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png
-ecuapassdocs/resources/images/image-windows-WindowButtons.png
+ecuapassdocs/resources/images/image-windows-WindowButtons.png
+ecuapassdocs/resources/images/image_DUMMY.png
+ecuapassdocs/resources/images/manifiesto_DUMMY.png
```

### Comparing `ecuapassdocs-0.79/setup.py` & `ecuapassdocs-0.80/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ecuapassdocs',  # Package name
-    version='0.79',  # Package version
+    version='0.80',  # Package version
     url="https://github.com/lgarreta/ecuapassdocs",
     author='Luis Garreta',
     author_email='lgarreta@gmail.com',
     description='Utils for creating PDFs, loading resources and extracting info from fields in ECUAPASS docs: cartaportes, manifiestos, declaraciones',
     packages=find_packages(),  # Automatically finds packages within the directory
 	include_package_data=True, 
 	package_data={"ecuapassdocs": ["resources/images/*", 
@@ -17,14 +17,15 @@
 	# List any dependencies here
     install_requires = [
 		"PyPDF2==3.0.1",
 		"reportlab==4.0.8",
 		"Pillow==10.1.0"
 	], 
 	logs = {
+		"0.80"   : "Improved info:embalaje",
 		"0.79"   : "Search codebin form by NAME. Added settings for NTA",
 		"0.78"   : "Improved infos:depositos, dates, vehiculo",
 		"0.77"   : "Improved update (posprocessing) ECUAPASS file",
 		"0.76"   : "Improved Utils, getCodebinValues",
 		"0.75"   : "Simplified info classes (e.g. removed Gastos table)",
 		"0.74"   : "Changed tipoProc (Byza === NTA)",
 		"0.73"   : "Improved Byza's clean watermarks",
```

