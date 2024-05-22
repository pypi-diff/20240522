# Comparing `tmp/bpp_iplweb-202405.1125-py3-none-any.whl.zip` & `tmp/bpp_iplweb-202405.1126-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6920473 bytes, number of entries: 2438
+Zip file size: 1812780 bytes, number of entries: 1406
 -rw-r--r--  2.0 unx      250 b- defN 80-Jan-01 00:00 AUTHORS.rst
 -rw-r--r--  2.0 unx     1645 b- defN 80-Jan-01 00:00 CONTRIBUTING.rst
--rw-r--r--  2.0 unx    70427 b- defN 80-Jan-01 00:00 HISTORY.rst
+-rw-r--r--  2.0 unx    70837 b- defN 80-Jan-01 00:00 HISTORY.rst
 -rw-r--r--  2.0 unx     7013 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx     1724 b- defN 80-Jan-01 00:00 README.rst
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 api_v1/__init__.py
 -rw-r--r--  2.0 unx       63 b- defN 80-Jan-01 00:00 api_v1/admin.py
 -rw-r--r--  2.0 unx       87 b- defN 80-Jan-01 00:00 api_v1/apps.py
 -rw-r--r--  2.0 unx      356 b- defN 80-Jan-01 00:00 api_v1/permissions.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 api_v1/serializers/__init__.py
@@ -60,15 +60,15 @@
 -rw-r--r--  2.0 unx      797 b- defN 80-Jan-01 00:00 bpp/admin/nagroda.py
 -rw-r--r--  2.0 unx     2538 b- defN 80-Jan-01 00:00 bpp/admin/patent.py
 -rw-r--r--  2.0 unx     4122 b- defN 80-Jan-01 00:00 bpp/admin/praca_doktorska.py
 -rw-r--r--  2.0 unx     3926 b- defN 80-Jan-01 00:00 bpp/admin/praca_habilitacyjna.py
 -rw-r--r--  2.0 unx      345 b- defN 80-Jan-01 00:00 bpp/admin/seria_wydawnicza.py
 -rw-r--r--  2.0 unx      929 b- defN 80-Jan-01 00:00 bpp/admin/szablondlaopisubibliograficznego.py
 -rw-r--r--  2.0 unx     5444 b- defN 80-Jan-01 00:00 bpp/admin/templates.py
--rw-r--r--  2.0 unx     5270 b- defN 80-Jan-01 00:00 bpp/admin/uczelnia.py
+-rw-r--r--  2.0 unx     6914 b- defN 80-Jan-01 00:00 bpp/admin/uczelnia.py
 -rw-r--r--  2.0 unx     3700 b- defN 80-Jan-01 00:00 bpp/admin/wydawca.py
 -rw-r--r--  2.0 unx     4708 b- defN 80-Jan-01 00:00 bpp/admin/wydawnictwo_autor_base.py
 -rw-r--r--  2.0 unx     9709 b- defN 80-Jan-01 00:00 bpp/admin/wydawnictwo_ciagle.py
 -rw-r--r--  2.0 unx      596 b- defN 80-Jan-01 00:00 bpp/admin/wydawnictwo_ciagle_autor.py
 -rw-r--r--  2.0 unx     9863 b- defN 80-Jan-01 00:00 bpp/admin/wydawnictwo_zwarte.py
 -rw-r--r--  2.0 unx      555 b- defN 80-Jan-01 00:00 bpp/admin/wydawnictwo_zwarte_autor.py
 -rw-r--r--  2.0 unx     1694 b- defN 80-Jan-01 00:00 bpp/admin/wydzial.py
@@ -575,14 +575,15 @@
 -rw-r--r--  2.0 unx      468 b- defN 80-Jan-01 00:00 bpp/migrations/0340_skasuj_anonimowe_zdarzenia.py
 -rw-r--r--  2.0 unx      705 b- defN 80-Jan-01 00:00 bpp/migrations/0341_dyscyplina_naukowa_pbn_uid.py
 -rw-r--r--  2.0 unx     3474 b- defN 80-Jan-01 00:00 bpp/migrations/0342_remove_dyscyplina_naukowa_pbn_uid.py
 -rw-r--r--  2.0 unx     7797 b- defN 80-Jan-01 00:00 bpp/migrations/0343_alter_typ_kbn_options_alter_patent_kc_punkty_kbn_and_more.py
 -rw-r--r--  2.0 unx      644 b- defN 80-Jan-01 00:00 bpp/migrations/0344_uczelnia_pbn_wysylaj_bez_oswiadczen.py
 -rw-r--r--  2.0 unx      427 b- defN 80-Jan-01 00:00 bpp/migrations/0345_alter_wydzial_opis.py
 -rw-r--r--  2.0 unx      710 b- defN 80-Jan-01 00:00 bpp/migrations/0346_rename_multiseek_searchform_data.py
+-rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 bpp/migrations/0347_uczelnia_deklaracja_dostepnosci_tekst_and_more.py
 -rw-r--r--  2.0 unx     6104 b- defN 80-Jan-01 00:00 bpp/migrations/107_bpp_autorzy.sql
 -rw-r--r--  2.0 unx    11808 b- defN 80-Jan-01 00:00 bpp/migrations/107_bpp_rekord.sql
 -rw-r--r--  2.0 unx     5475 b- defN 80-Jan-01 00:00 bpp/migrations/107_cache_functions.sql
 -rw-r--r--  2.0 unx      381 b- defN 80-Jan-01 00:00 bpp/migrations/108_bpp_nowe_sumy_view_bug.sql
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 bpp/migrations/__init__.py
 -rw-r--r--  2.0 unx     1820 b- defN 80-Jan-01 00:00 bpp/models/__init__.py
 -rw-r--r--  2.0 unx    39288 b- defN 80-Jan-01 00:00 bpp/models/abstract.py
@@ -610,15 +611,15 @@
 -rw-r--r--  2.0 unx       39 b- defN 80-Jan-01 00:00 bpp/models/sloty/exceptions.py
 -rw-r--r--  2.0 unx     2544 b- defN 80-Jan-01 00:00 bpp/models/sloty/wydawnictwo_ciagle.py
 -rw-r--r--  2.0 unx     1482 b- defN 80-Jan-01 00:00 bpp/models/sloty/wydawnictwo_zwarte.py
 -rw-r--r--  2.0 unx       72 b- defN 80-Jan-01 00:00 bpp/models/struktura.py
 -rw-r--r--  2.0 unx     1194 b- defN 80-Jan-01 00:00 bpp/models/sumy_views.py
 -rw-r--r--  2.0 unx    10786 b- defN 80-Jan-01 00:00 bpp/models/system.py
 -rw-r--r--  2.0 unx     3480 b- defN 80-Jan-01 00:00 bpp/models/szablondlaopisubibliograficznego.py
--rw-r--r--  2.0 unx    20355 b- defN 80-Jan-01 00:00 bpp/models/uczelnia.py
+-rw-r--r--  2.0 unx    21490 b- defN 80-Jan-01 00:00 bpp/models/uczelnia.py
 -rw-r--r--  2.0 unx     8579 b- defN 80-Jan-01 00:00 bpp/models/util.py
 -rw-r--r--  2.0 unx     3391 b- defN 80-Jan-01 00:00 bpp/models/wydawca.py
 -rw-r--r--  2.0 unx     9230 b- defN 80-Jan-01 00:00 bpp/models/wydawnictwo_ciagle.py
 -rw-r--r--  2.0 unx    11403 b- defN 80-Jan-01 00:00 bpp/models/wydawnictwo_zwarte.py
 -rw-r--r--  2.0 unx     5440 b- defN 80-Jan-01 00:00 bpp/models/wydzial.py
 -rw-r--r--  2.0 unx     5721 b- defN 80-Jan-01 00:00 bpp/models/zrodlo.py
 -rw-r--r--  2.0 unx      707 b- defN 80-Jan-01 00:00 bpp/monkey_patches.py
@@ -702,14 +703,15 @@
 -rw-r--r--  2.0 unx       82 b- defN 80-Jan-01 00:00 bpp/templates/autocompletes/jednostka.html
 -rw-r--r--  2.0 unx      193 b- defN 80-Jan-01 00:00 bpp/templates/autocompletes/non_admin.html
 -rw-r--r--  2.0 unx       79 b- defN 80-Jan-01 00:00 bpp/templates/autocompletes/zrodlo.html
 -rw-r--r--  2.0 unx      274 b- defN 80-Jan-01 00:00 bpp/templates/browse/article.html
 -rw-r--r--  2.0 unx     4556 b- defN 80-Jan-01 00:00 bpp/templates/browse/autor.html
 -rw-r--r--  2.0 unx     2243 b- defN 80-Jan-01 00:00 bpp/templates/browse/autorzy.html
 -rw-r--r--  2.0 unx      216 b- defN 80-Jan-01 00:00 bpp/templates/browse/brak_uczelni.html
+-rw-r--r--  2.0 unx      722 b- defN 80-Jan-01 00:00 bpp/templates/browse/deklaracja_dostepnosci.html
 -rw-r--r--  2.0 unx      204 b- defN 80-Jan-01 00:00 bpp/templates/browse/edit_if_logged_in.html
 -rw-r--r--  2.0 unx      285 b- defN 80-Jan-01 00:00 bpp/templates/browse/go_to_admin_change.html
 -rw-r--r--  2.0 unx      292 b- defN 80-Jan-01 00:00 bpp/templates/browse/go_to_admin_list.html
 -rw-r--r--  2.0 unx      869 b- defN 80-Jan-01 00:00 bpp/templates/browse/google_scholar.html
 -rw-r--r--  2.0 unx     5963 b- defN 80-Jan-01 00:00 bpp/templates/browse/jednostka.html
 -rw-r--r--  2.0 unx     1979 b- defN 80-Jan-01 00:00 bpp/templates/browse/jednostki.html
 -rw-r--r--  2.0 unx      697 b- defN 80-Jan-01 00:00 bpp/templates/browse/literki.html
@@ -753,30 +755,30 @@
 -rw-r--r--  2.0 unx      266 b- defN 80-Jan-01 00:00 bpp/templatetags/bpp_version.py
 -rw-r--r--  2.0 unx     2215 b- defN 80-Jan-01 00:00 bpp/templatetags/czy_pokazywac.py
 -rw-r--r--  2.0 unx      202 b- defN 80-Jan-01 00:00 bpp/templatetags/findfilter.py
 -rw-r--r--  2.0 unx      210 b- defN 80-Jan-01 00:00 bpp/templatetags/just_single_quotes.py
 -rw-r--r--  2.0 unx      172 b- defN 80-Jan-01 00:00 bpp/templatetags/model_to_class.py
 -rw-r--r--  2.0 unx     2915 b- defN 80-Jan-01 00:00 bpp/templatetags/prace.py
 -rw-r--r--  2.0 unx      279 b- defN 80-Jan-01 00:00 bpp/templatetags/user_in_group.py
--rw-r--r--  2.0 unx    14236 b- defN 80-Jan-01 00:00 bpp/urls.py
+-rw-r--r--  2.0 unx    14420 b- defN 80-Jan-01 00:00 bpp/urls.py
 -rw-r--r--  2.0 unx    18975 b- defN 80-Jan-01 00:00 bpp/util.py
 -rw-r--r--  2.0 unx     3484 b- defN 80-Jan-01 00:00 bpp/views/__init__.py
 -rw-r--r--  2.0 unx     1596 b- defN 80-Jan-01 00:00 bpp/views/admin.py
 -rw-r--r--  2.0 unx     4844 b- defN 80-Jan-01 00:00 bpp/views/api/__init__.py
 -rw-r--r--  2.0 unx     1286 b- defN 80-Jan-01 00:00 bpp/views/api/clarivate.py
 -rw-r--r--  2.0 unx      368 b- defN 80-Jan-01 00:00 bpp/views/api/const.py
 -rw-r--r--  2.0 unx     2158 b- defN 80-Jan-01 00:00 bpp/views/api/crossref.py
 -rw-r--r--  2.0 unx      875 b- defN 80-Jan-01 00:00 bpp/views/api/forms.py
 -rw-r--r--  2.0 unx     4353 b- defN 80-Jan-01 00:00 bpp/views/api/pbn_get_by_parameter.py
 -rw-r--r--  2.0 unx     1830 b- defN 80-Jan-01 00:00 bpp/views/api/pubmed.py
 -rw-r--r--  2.0 unx      700 b- defN 80-Jan-01 00:00 bpp/views/api/strona_tom_nr_zeszytu.py
 -rw-r--r--  2.0 unx     1976 b- defN 80-Jan-01 00:00 bpp/views/api/uzupelnij_rok.py
 -rw-r--r--  2.0 unx    23190 b- defN 80-Jan-01 00:00 bpp/views/autocomplete/__init__.py
 -rw-r--r--  2.0 unx     6064 b- defN 80-Jan-01 00:00 bpp/views/autocomplete/pbn_api.py
--rw-r--r--  2.0 unx    11444 b- defN 80-Jan-01 00:00 bpp/views/browse.py
+-rw-r--r--  2.0 unx    11906 b- defN 80-Jan-01 00:00 bpp/views/browse.py
 -rw-r--r--  2.0 unx     2335 b- defN 80-Jan-01 00:00 bpp/views/global_nav.py
 -rw-r--r--  2.0 unx     1874 b- defN 80-Jan-01 00:00 bpp/views/mixins.py
 -rw-r--r--  2.0 unx     4168 b- defN 80-Jan-01 00:00 bpp/views/mymultiseek.py
 -rw-r--r--  2.0 unx     7700 b- defN 80-Jan-01 00:00 bpp/views/oai.py
 -rw-r--r--  2.0 unx     7479 b- defN 80-Jan-01 00:00 bpp/views/raporty/__init__.py
 -rw-r--r--  2.0 unx     7411 b- defN 80-Jan-01 00:00 bpp/views/raporty/forms.py
 -rw-r--r--  2.0 unx     6057 b- defN 80-Jan-01 00:00 bpp/views/raporty/ranking_autorow.py
@@ -823,1053 +825,19 @@
 -rw-r--r--  2.0 unx     3680 b- defN 80-Jan-01 00:00 django_bpp/dashboard.py
 -rw-r--r--  2.0 unx      841 b- defN 80-Jan-01 00:00 django_bpp/forms.py
 -rw-r--r--  2.0 unx      298 b- defN 80-Jan-01 00:00 django_bpp/manage_command.py
 -rw-r--r--  2.0 unx     6546 b- defN 80-Jan-01 00:00 django_bpp/menu.py
 -rw-r--r--  2.0 unx      403 b- defN 80-Jan-01 00:00 django_bpp/routing.py
 -rw-r--r--  2.0 unx     1614 b- defN 80-Jan-01 00:00 django_bpp/selenium_util.py
 -rw-r--r--  2.0 unx       20 b- defN 80-Jan-01 00:00 django_bpp/settings/__init__.py
--rw-r--r--  2.0 unx    32154 b- defN 80-Jan-01 00:00 django_bpp/settings/base.py
+-rw-r--r--  2.0 unx    32362 b- defN 80-Jan-01 00:00 django_bpp/settings/base.py
 -rw-r--r--  2.0 unx     1685 b- defN 80-Jan-01 00:00 django_bpp/settings/local.py
 -rw-r--r--  2.0 unx     1855 b- defN 80-Jan-01 00:00 django_bpp/settings/production.py
 -rw-r--r--  2.0 unx      791 b- defN 80-Jan-01 00:00 django_bpp/settings/test.py
 -rw-r--r--  2.0 unx     3394 b- defN 80-Jan-01 00:00 django_bpp/sitemaps.py
--rw-r--r--  2.0 unx     3730 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.096f10c22368.css
--rw-r--r--  2.0 unx   184756 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.0a872877d6e5.css
--rw-r--r--  2.0 unx      248 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.190bf892d4f4.css
--rw-r--r--  2.0 unx     1839 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.1932d9721a27.css
--rw-r--r--  2.0 unx     2795 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.1f790078cf5c.css
--rw-r--r--  2.0 unx      288 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.29cc8c364a3e.css
--rw-r--r--  2.0 unx      312 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.356143e41027.css
--rw-r--r--  2.0 unx   147650 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.379c10a9e812.css
--rw-r--r--  2.0 unx    30472 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.5696a0d0f1f1.css
--rw-r--r--  2.0 unx    36360 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.6a3cdad0db8d.css
--rw-r--r--  2.0 unx   147759 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.7f5b59a472ba.css
--rw-r--r--  2.0 unx     6764 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.89fd28600aa6.css
--rw-r--r--  2.0 unx       34 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.8b11ced9338f.css
--rw-r--r--  2.0 unx    17616 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.a810a58e3985.css
--rw-r--r--  2.0 unx    31076 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.b27842844e9e.css
--rw-r--r--  2.0 unx     1511 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.c55ee1d1f071.css
--rw-r--r--  2.0 unx     2685 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.c8c84bffe354.css
--rw-r--r--  2.0 unx    14923 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.c910af7b7054.css
--rw-r--r--  2.0 unx   147617 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.cecc011ac0ed.css
--rw-r--r--  2.0 unx      321 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.f0f7cd65549e.css
--rw-r--r--  2.0 unx      156 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/css/output.f9aaec1db0e7.css
--rw-r--r--  2.0 unx     1577 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.007d0f8196ce.js
--rw-r--r--  2.0 unx     2604 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.023974546012.js
--rw-r--r--  2.0 unx     7847 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.05c3452b5333.js
--rw-r--r--  2.0 unx      661 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.1b90b4fd0996.js
--rw-r--r--  2.0 unx    15934 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.1c85775ddde0.js
--rw-r--r--  2.0 unx    27665 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.343f6adb2a24.js
--rw-r--r--  2.0 unx     2932 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.42e671c2a38d.js
--rw-r--r--  2.0 unx   254915 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.5d38125bd1ad.js
--rw-r--r--  2.0 unx     2430 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.5ec89beef9ad.js
--rw-r--r--  2.0 unx    79172 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.68e3dd089325.js
--rw-r--r--  2.0 unx   134127 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.8d16d119404e.js
--rw-r--r--  2.0 unx   238306 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.8dd042ba56b5.js
--rw-r--r--  2.0 unx     6065 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.8ee655cf393b.js
--rw-r--r--  2.0 unx      369 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.96a46be1e5ad.js
--rw-r--r--  2.0 unx     1963 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.ab5d51d1c156.js
--rw-r--r--  2.0 unx      885 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.ad88da53bae4.js
--rw-r--r--  2.0 unx    27531 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.b42d7758508b.js
--rw-r--r--  2.0 unx    89500 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.b4ba48ed4f66.js
--rw-r--r--  2.0 unx      946 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.b7aa83a7edd6.js
--rw-r--r--  2.0 unx   193896 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.c86114addc24.js
--rw-r--r--  2.0 unx      504 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.cd1656272d36.js
--rw-r--r--  2.0 unx    18043 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.e01ae35807c6.js
--rw-r--r--  2.0 unx     9401 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.e40a6a191db5.js
--rw-r--r--  2.0 unx      806 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.ec76e5be931e.js
--rw-r--r--  2.0 unx     3347 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.f44161ebe543.js
--rw-r--r--  2.0 unx      986 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.f6d7b57c1be4.js
--rw-r--r--  2.0 unx     7698 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/js/output.f8daedf655e8.js
--rw-r--r--  2.0 unx    11304 b- defN 80-Jan-01 00:00 django_bpp/staticroot/CACHE-202405.1125/manifest.json
--rw-r--r--  2.0 unx     9114 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/css/autocomplete.css
--rw-r--r--  2.0 unx    21310 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/css/base.css
--rw-r--r--  2.0 unx     6566 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/css/changelists.css
--rw-r--r--  2.0 unx     2929 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/css/dark_mode.css
--rw-r--r--  2.0 unx      441 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/css/dashboard.css
--rw-r--r--  2.0 unx     9090 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/css/forms.css
--rw-r--r--  2.0 unx      958 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/css/login.css
--rw-r--r--  2.0 unx     2694 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/css/nav_sidebar.css
--rw-r--r--  2.0 unx    18559 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/css/responsive.css
--rw-r--r--  2.0 unx     1864 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/css/responsive_rtl.css
--rw-r--r--  2.0 unx     4918 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/css/rtl.css
--rw-r--r--  2.0 unx    17358 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/css/vendor/select2/select2.css
--rw-r--r--  2.0 unx    14966 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/css/vendor/select2/select2.min.css
--rw-r--r--  2.0 unx    11921 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/css/widgets.css
--rw-r--r--  2.0 unx     1094 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/calendar-icons.svg
--rw-r--r--  2.0 unx     1129 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/gis/move_vertex_off.svg
--rw-r--r--  2.0 unx     1129 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/gis/move_vertex_on.svg
--rw-r--r--  2.0 unx      331 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/icon-addlink.svg
--rw-r--r--  2.0 unx      504 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/icon-alert.svg
--rw-r--r--  2.0 unx     1086 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/icon-calendar.svg
--rw-r--r--  2.0 unx      380 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/icon-changelink.svg
--rw-r--r--  2.0 unx      677 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/icon-clock.svg
--rw-r--r--  2.0 unx      392 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/icon-deletelink.svg
--rw-r--r--  2.0 unx      560 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/icon-no.svg
--rw-r--r--  2.0 unx      655 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/icon-unknown-alt.svg
--rw-r--r--  2.0 unx      655 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/icon-unknown.svg
--rw-r--r--  2.0 unx      581 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/icon-viewlink.svg
--rw-r--r--  2.0 unx      436 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/icon-yes.svg
--rw-r--r--  2.0 unx      560 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/inline-delete.svg
--rw-r--r--  2.0 unx      458 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/search.svg
--rw-r--r--  2.0 unx     3291 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/selector-icons.svg
--rw-r--r--  2.0 unx     1097 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/sorting-icons.svg
--rw-r--r--  2.0 unx      331 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/tooltag-add.svg
--rw-r--r--  2.0 unx      280 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/img/tooltag-arrowright.svg
--rw-r--r--  2.0 unx     4530 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/SelectBox.js
--rw-r--r--  2.0 unx    15292 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/SelectFilter2.js
--rw-r--r--  2.0 unx     8337 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/actions.js
--rw-r--r--  2.0 unx       68 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/admin/DateTimeShortcuts.js
--rw-r--r--  2.0 unx     7923 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/admin/RelatedObjectLookups.js
--rw-r--r--  2.0 unx     1060 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/autocomplete.js
--rw-r--r--  2.0 unx     8466 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/calendar.js
--rw-r--r--  2.0 unx      884 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/cancel.js
--rw-r--r--  2.0 unx      606 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/change_form.js
--rw-r--r--  2.0 unx     1803 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/collapse.js
--rw-r--r--  2.0 unx     5682 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/core.js
--rw-r--r--  2.0 unx      978 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/filters.js
--rw-r--r--  2.0 unx    15526 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/inlines.js
--rw-r--r--  2.0 unx       78 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/jquery.init.js
--rw-r--r--  2.0 unx     3063 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/nav_sidebar.js
--rw-r--r--  2.0 unx      551 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/popup_response.js
--rw-r--r--  2.0 unx     1531 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/prepopulate.js
--rw-r--r--  2.0 unx      586 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/prepopulate_init.js
--rw-r--r--  2.0 unx     1943 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/theme.js
--rw-r--r--  2.0 unx     7887 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/urlify.js
--rw-r--r--  2.0 unx       78 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/jquery/jquery.js
--rw-r--r--  2.0 unx       78 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/jquery/jquery.min.js
--rw-r--r--  2.0 unx      866 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/af.js
--rw-r--r--  2.0 unx      905 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/ar.js
--rw-r--r--  2.0 unx      721 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/az.js
--rw-r--r--  2.0 unx      968 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/bg.js
--rw-r--r--  2.0 unx     1291 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/bn.js
--rw-r--r--  2.0 unx      965 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/bs.js
--rw-r--r--  2.0 unx      900 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/ca.js
--rw-r--r--  2.0 unx     1292 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/cs.js
--rw-r--r--  2.0 unx      828 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/da.js
--rw-r--r--  2.0 unx      866 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/de.js
--rw-r--r--  2.0 unx     1017 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/dsb.js
--rw-r--r--  2.0 unx     1182 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/el.js
--rw-r--r--  2.0 unx      844 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/en.js
--rw-r--r--  2.0 unx      922 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/es.js
--rw-r--r--  2.0 unx      801 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/et.js
--rw-r--r--  2.0 unx      868 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/eu.js
--rw-r--r--  2.0 unx     1023 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/fa.js
--rw-r--r--  2.0 unx      803 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/fi.js
--rw-r--r--  2.0 unx      924 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/fr.js
--rw-r--r--  2.0 unx      924 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/gl.js
--rw-r--r--  2.0 unx      984 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/he.js
--rw-r--r--  2.0 unx     1175 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/hi.js
--rw-r--r--  2.0 unx      852 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/hr.js
--rw-r--r--  2.0 unx     1018 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/hsb.js
--rw-r--r--  2.0 unx      831 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/hu.js
--rw-r--r--  2.0 unx     1028 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/hy.js
--rw-r--r--  2.0 unx      768 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/id.js
--rw-r--r--  2.0 unx      807 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/is.js
--rw-r--r--  2.0 unx      897 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/it.js
--rw-r--r--  2.0 unx      862 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/ja.js
--rw-r--r--  2.0 unx     1195 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/ka.js
--rw-r--r--  2.0 unx     1088 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/km.js
--rw-r--r--  2.0 unx      855 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/ko.js
--rw-r--r--  2.0 unx      944 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/lt.js
--rw-r--r--  2.0 unx      900 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/lv.js
--rw-r--r--  2.0 unx     1038 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/mk.js
--rw-r--r--  2.0 unx      811 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/ms.js
--rw-r--r--  2.0 unx      778 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/nb.js
--rw-r--r--  2.0 unx     1357 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/ne.js
--rw-r--r--  2.0 unx      904 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/nl.js
--rw-r--r--  2.0 unx      947 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/pl.js
--rw-r--r--  2.0 unx     1049 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/ps.js
--rw-r--r--  2.0 unx      876 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/pt-BR.js
--rw-r--r--  2.0 unx      878 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/pt.js
--rw-r--r--  2.0 unx      938 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/ro.js
--rw-r--r--  2.0 unx     1171 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/ru.js
--rw-r--r--  2.0 unx     1306 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/sk.js
--rw-r--r--  2.0 unx      925 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/sl.js
--rw-r--r--  2.0 unx      903 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/sq.js
--rw-r--r--  2.0 unx     1109 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/sr-Cyrl.js
--rw-r--r--  2.0 unx      980 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/sr.js
--rw-r--r--  2.0 unx      786 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/sv.js
--rw-r--r--  2.0 unx     1074 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/th.js
--rw-r--r--  2.0 unx      771 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/tk.js
--rw-r--r--  2.0 unx      775 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/tr.js
--rw-r--r--  2.0 unx     1156 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/uk.js
--rw-r--r--  2.0 unx      796 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/vi.js
--rw-r--r--  2.0 unx      768 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/zh-CN.js
--rw-r--r--  2.0 unx      707 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/i18n/zh-TW.js
--rw-r--r--  2.0 unx   173566 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/select2.full.js
--rw-r--r--  2.0 unx    79212 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/select2/select2.full.min.js
--rw-r--r--  2.0 unx   232381 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/xregexp/xregexp.js
--rw-r--r--  2.0 unx   125266 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin/js/vendor/xregexp/xregexp.min.js
--rw-r--r--  2.0 unx      457 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/dashboard-ie.css
--rw-r--r--  2.0 unx     6388 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/dashboard.css
--rw-r--r--  2.0 unx     1738 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/jquery/images/animated-overlay.gif
--rw-r--r--  2.0 unx      212 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/jquery/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-r--r--  2.0 unx      208 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/jquery/images/ui-bg_flat_75_ffffff_40x100.png
--rw-r--r--  2.0 unx      335 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/jquery/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--  2.0 unx      207 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/jquery/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/jquery/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/jquery/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--  2.0 unx      332 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/jquery/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--  2.0 unx      280 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/jquery/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--  2.0 unx     6922 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/jquery/images/ui-icons_222222_256x240.png
--rw-r--r--  2.0 unx     4549 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/jquery/images/ui-icons_2e83ff_256x240.png
--rw-r--r--  2.0 unx     6992 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/jquery/images/ui-icons_454545_256x240.png
--rw-r--r--  2.0 unx     6999 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/jquery/images/ui-icons_888888_256x240.png
--rw-r--r--  2.0 unx     4549 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/jquery/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--  2.0 unx    31890 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/jquery/jquery-ui.css
--rw-r--r--  2.0 unx      299 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/menu-ie.css
--rw-r--r--  2.0 unx     5349 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/menu.css
--rw-r--r--  2.0 unx      868 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/css/theming.css
--rw-r--r--  2.0 unx     7013 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/images/admin-tools.png
--rw-r--r--  2.0 unx     2947 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/images/django.png
--rw-r--r--  2.0 unx      495 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/js/dashboard.js
--rw-r--r--  2.0 unx   253668 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/js/jquery/jquery-ui.min.js
--rw-r--r--  2.0 unx     1043 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/js/jquery/jquery.cookie.min.js
--rw-r--r--  2.0 unx    13231 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/js/jquery/jquery.dashboard.js
--rw-r--r--  2.0 unx    89501 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/js/jquery/jquery.min.js
--rw-r--r--  2.0 unx     3390 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/js/json.min.js
--rw-r--r--  2.0 unx     2154 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/js/menu.js
--rw-r--r--  2.0 unx     1203 b- defN 80-Jan-01 00:00 django_bpp/staticroot/admin_tools/js/utils.js
--rw-r--r--  2.0 unx     1297 b- defN 80-Jan-01 00:00 django_bpp/staticroot/adminsortable2/css/sortable.css
--rw-r--r--  2.0 unx     1653 b- defN 80-Jan-01 00:00 django_bpp/staticroot/adminsortable2/icons/drag.png
--rw-r--r--  2.0 unx   113617 b- defN 80-Jan-01 00:00 django_bpp/staticroot/adminsortable2/js/adminsortable2.js
--rw-r--r--  2.0 unx    49197 b- defN 80-Jan-01 00:00 django_bpp/staticroot/adminsortable2/js/adminsortable2.min.js
--rw-r--r--  2.0 unx     3950 b- defN 80-Jan-01 00:00 django_bpp/staticroot/adminsortable2/js/list-sortable.js
--rw-r--r--  2.0 unx    17701 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/autocomplete_light.js
--rw-r--r--  2.0 unx     5315 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/autocomplete_light.min.js
--rw-r--r--  2.0 unx      950 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/af.js
--rw-r--r--  2.0 unx      989 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/ar.js
--rw-r--r--  2.0 unx      805 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/az.js
--rw-r--r--  2.0 unx     1052 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/bg.js
--rw-r--r--  2.0 unx     1359 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/bn.js
--rw-r--r--  2.0 unx     1019 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/bs.js
--rw-r--r--  2.0 unx      968 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/ca.js
--rw-r--r--  2.0 unx     1364 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/cs.js
--rw-r--r--  2.0 unx      912 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/da.js
--rw-r--r--  2.0 unx      949 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/de.js
--rw-r--r--  2.0 unx     1093 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/dsb.js
--rw-r--r--  2.0 unx     1266 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/el.js
--rw-r--r--  2.0 unx     1005 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/en.js
--rw-r--r--  2.0 unx      943 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/eo.js
--rw-r--r--  2.0 unx      990 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/es.js
--rw-r--r--  2.0 unx      882 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/et.js
--rw-r--r--  2.0 unx      948 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/eu.js
--rw-r--r--  2.0 unx     1107 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/fa.js
--rw-r--r--  2.0 unx      887 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/fi.js
--rw-r--r--  2.0 unx     1053 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/fr.js
--rw-r--r--  2.0 unx      998 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/gl.js
--rw-r--r--  2.0 unx     1056 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/he.js
--rw-r--r--  2.0 unx     1246 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/hi.js
--rw-r--r--  2.0 unx      936 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/hr.js
--rw-r--r--  2.0 unx     1094 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/hsb.js
--rw-r--r--  2.0 unx     1003 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/hu.js
--rw-r--r--  2.0 unx     1112 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/hy.js
--rw-r--r--  2.0 unx      852 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/id.js
--rw-r--r--  2.0 unx      890 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/is.js
--rw-r--r--  2.0 unx      972 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/it.js
--rw-r--r--  2.0 unx      946 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/ja.js
--rw-r--r--  2.0 unx     1279 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/ka.js
--rw-r--r--  2.0 unx     1172 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/km.js
--rw-r--r--  2.0 unx      939 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/ko.js
--rw-r--r--  2.0 unx      998 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/lt.js
--rw-r--r--  2.0 unx      959 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/lv.js
--rw-r--r--  2.0 unx     1122 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/mk.js
--rw-r--r--  2.0 unx      895 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/ms.js
--rw-r--r--  2.0 unx      862 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/nb.js
--rw-r--r--  2.0 unx     1438 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/ne.js
--rw-r--r--  2.0 unx      985 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/nl.js
--rw-r--r--  2.0 unx     1450 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/pa.js
--rw-r--r--  2.0 unx      988 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/pl.js
--rw-r--r--  2.0 unx     1127 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/ps.js
--rw-r--r--  2.0 unx      963 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/pt-BR.js
--rw-r--r--  2.0 unx      946 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/pt.js
--rw-r--r--  2.0 unx     1021 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/ro.js
--rw-r--r--  2.0 unx     1233 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/ru.js
--rw-r--r--  2.0 unx     1382 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/sk.js
--rw-r--r--  2.0 unx     1009 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/sl.js
--rw-r--r--  2.0 unx      987 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/sq.js
--rw-r--r--  2.0 unx     1168 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/sr-Cyrl.js
--rw-r--r--  2.0 unx     1034 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/sr.js
--rw-r--r--  2.0 unx      870 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/sv.js
--rw-r--r--  2.0 unx     1433 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/te.js
--rw-r--r--  2.0 unx     1158 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/th.js
--rw-r--r--  2.0 unx      855 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/tk.js
--rw-r--r--  2.0 unx      859 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/tr.js
--rw-r--r--  2.0 unx     1240 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/uk.js
--rw-r--r--  2.0 unx      880 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/vi.js
--rw-r--r--  2.0 unx      855 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/zh-CN.js
--rw-r--r--  2.0 unx      794 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/i18n/zh-TW.js
--rw-r--r--  2.0 unx      267 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/select2.css
--rw-r--r--  2.0 unx     4607 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/select2.js
--rw-r--r--  2.0 unx     1894 b- defN 80-Jan-01 00:00 django_bpp/staticroot/autocomplete_light/select2.min.js
--rw-r--r--  2.0 unx     4551 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/css/admin-menu.css
--rw-r--r--  2.0 unx     3167 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/css/admin-style.css
--rw-r--r--  2.0 unx      316 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/css/fix-djangoql-css-for-grappelli.css
--rw-r--r--  2.0 unx     1738 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/images/animated-overlay.gif
--rw-r--r--  2.0 unx      251 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-r--r--  2.0 unx      259 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/images/ui-bg_flat_0_eeeeee_40x100.png
--rw-r--r--  2.0 unx      247 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/images/ui-bg_flat_55_ffffff_40x100.png
--rw-r--r--  2.0 unx      247 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/images/ui-bg_flat_75_ffffff_40x100.png
--rw-r--r--  2.0 unx      246 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--  2.0 unx      316 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/images/ui-bg_highlight-soft_100_f6f6f6_1x100.png
--rw-r--r--  2.0 unx      374 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/images/ui-bg_highlight-soft_25_0073ea_1x100.png
--rw-r--r--  2.0 unx      319 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/images/ui-bg_highlight-soft_50_dddddd_1x100.png
--rw-r--r--  2.0 unx     4599 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/images/ui-icons_0073ea_256x240.png
--rw-r--r--  2.0 unx     7071 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/images/ui-icons_454545_256x240.png
--rw-r--r--  2.0 unx     7092 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/images/ui-icons_666666_256x240.png
--rw-r--r--  2.0 unx     4599 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/images/ui-icons_ff0084_256x240.png
--rw-r--r--  2.0 unx     6468 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/images/ui-icons_ffffff_256x240.png
--rw-r--r--  2.0 unx    32807 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/jquery-ui.css
--rw-r--r--  2.0 unx    27714 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/jquery-ui.min.css
--rw-r--r--  2.0 unx    17237 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/flick/theme.css
--rw-r--r--  2.0 unx    17368 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/images/giphy.gif
--rw-r--r--  2.0 unx     7750 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/images/lite-blue-check.png
--rw-r--r--  2.0 unx     7578 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/images/lite-green-check.png
--rw-r--r--  2.0 unx     8687 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/images/lite-red-check.png
--rw-r--r--  2.0 unx     9275 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/images/logo.png
--rw-r--r--  2.0 unx   267648 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/images/logo_bpp.png
--rw-r--r--  2.0 unx     2883 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/images/no-check.png
--rw-r--r--  2.0 unx     6555 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/images/printer.png
--rw-r--r--  2.0 unx      632 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/images/star_white.png
--rw-r--r--  2.0 unx      753 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/images/star_yellow.png
--rw-r--r--  2.0 unx    79335 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/images/test_server_background.jpg
--rw-r--r--  2.0 unx      846 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/js/Polish.json
--rw-r--r--  2.0 unx     2059 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/js/autorform_dependant.js
--rw-r--r--  2.0 unx      458 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/js/bpp.js
--rw-r--r--  2.0 unx     2043 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/svg/autor.svg
--rw-r--r--  2.0 unx     1668 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/svg/cache.svg
--rw-r--r--  2.0 unx     3715 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/svg/database.svg
--rw-r--r--  2.0 unx     5202 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/svg/jednostka.svg
--rw-r--r--  2.0 unx     1388 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/svg/paper.svg
--rw-r--r--  2.0 unx     1380 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/svg/patent.svg
--rw-r--r--  2.0 unx     1191 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/svg/pencil.svg
--rw-r--r--  2.0 unx     2545 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/svg/praca_doktorska.svg
--rw-r--r--  2.0 unx     2548 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/svg/praca_habilitacyjna.svg
--rw-r--r--  2.0 unx     1944 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/svg/user.svg
--rw-r--r--  2.0 unx     1063 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/svg/wydawnictwo_ciagle.svg
--rw-r--r--  2.0 unx     1668 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/svg/wydawnictwo_zwarte.svg
--rw-r--r--  2.0 unx     2343 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/svg/zrodlo.svg
--rw-r--r--  2.0 unx   159964 b- defN 80-Jan-01 00:00 django_bpp/staticroot/bpp/wav/alert.wav
--rw-r--r--  2.0 unx      200 b- defN 80-Jan-01 00:00 django_bpp/staticroot/close-alerts.js
--rw-r--r--  2.0 unx      340 b- defN 80-Jan-01 00:00 django_bpp/staticroot/cookielaw/css/cookielaw.css
--rw-r--r--  2.0 unx      190 b- defN 80-Jan-01 00:00 django_bpp/staticroot/cookielaw/img/close.png
--rw-r--r--  2.0 unx     1038 b- defN 80-Jan-01 00:00 django_bpp/staticroot/cookielaw/js/cookielaw.js
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 django_bpp/staticroot/css/columns.css
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 django_bpp/staticroot/css/flexible_reports.css
--rw-r--r--  2.0 unx   450425 b- defN 80-Jan-01 00:00 django_bpp/staticroot/datatables.net/js/jquery.dataTables.js
--rw-r--r--  2.0 unx     3037 b- defN 80-Jan-01 00:00 django_bpp/staticroot/datatables.net-zf/css/dataTables.foundation.css
--rw-r--r--  2.0 unx     4377 b- defN 80-Jan-01 00:00 django_bpp/staticroot/datatables.net-zf/js/dataTables.foundation.js
--rw-r--r--  2.0 unx      674 b- defN 80-Jan-01 00:00 django_bpp/staticroot/dbtemplates/css/django.css
--rw-r--r--  2.0 unx      339 b- defN 80-Jan-01 00:00 django_bpp/staticroot/dbtemplates/css/editor.css
--rw-r--r--  2.0 unx    18795 b- defN 80-Jan-01 00:00 django_bpp/staticroot/dbtemplates/js/codemirror.js
--rw-r--r--  2.0 unx    56597 b- defN 80-Jan-01 00:00 django_bpp/staticroot/dbtemplates/js/editor.js
--rw-r--r--  2.0 unx     2091 b- defN 80-Jan-01 00:00 django_bpp/staticroot/dbtemplates/js/highlight.js
--rw-r--r--  2.0 unx     2270 b- defN 80-Jan-01 00:00 django_bpp/staticroot/dbtemplates/js/mirrorframe.js
--rw-r--r--  2.0 unx    10295 b- defN 80-Jan-01 00:00 django_bpp/staticroot/dbtemplates/js/parsedjango.js
--rw-r--r--  2.0 unx    22680 b- defN 80-Jan-01 00:00 django_bpp/staticroot/dbtemplates/js/select.js
--rw-r--r--  2.0 unx     4216 b- defN 80-Jan-01 00:00 django_bpp/staticroot/dbtemplates/js/stringstream.js
--rw-r--r--  2.0 unx     2006 b- defN 80-Jan-01 00:00 django_bpp/staticroot/dbtemplates/js/tokenize.js
--rw-r--r--  2.0 unx    14390 b- defN 80-Jan-01 00:00 django_bpp/staticroot/dbtemplates/js/undo.js
--rw-r--r--  2.0 unx     3491 b- defN 80-Jan-01 00:00 django_bpp/staticroot/dbtemplates/js/util.js
--rw-r--r--  2.0 unx      740 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_extensions/css/jquery.autocomplete.css
--rw-r--r--  2.0 unx     1553 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_extensions/img/indicator.gif
--rw-r--r--  2.0 unx     2911 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_extensions/js/jquery.ajaxQueue.js
--rw-r--r--  2.0 unx    36679 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_extensions/js/jquery.autocomplete.js
--rw-r--r--  2.0 unx     1820 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_extensions/js/jquery.bgiframe.js
--rw-r--r--  2.0 unx      167 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_tables2/bootstrap.css
--rw-r--r--  2.0 unx     2774 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_tables2/themes/paleblue/css/screen.css
--rw-r--r--  2.0 unx      216 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_tables2/themes/paleblue/img/arrow-active-down.png
--rw-r--r--  2.0 unx      202 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_tables2/themes/paleblue/img/arrow-active-up.png
--rw-r--r--  2.0 unx      246 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_tables2/themes/paleblue/img/arrow-inactive-down.png
--rw-r--r--  2.0 unx      210 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_tables2/themes/paleblue/img/arrow-inactive-up.png
--rw-r--r--  2.0 unx      176 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_tables2/themes/paleblue/img/false.gif
--rw-r--r--  2.0 unx      130 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_tables2/themes/paleblue/img/header-bg.png
--rw-r--r--  2.0 unx      509 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_tables2/themes/paleblue/img/missing.png
--rw-r--r--  2.0 unx      273 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_tables2/themes/paleblue/img/pagination-bg.gif
--rw-r--r--  2.0 unx      299 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_tables2/themes/paleblue/img/true.gif
--rw-r--r--  2.0 unx     2381 b- defN 80-Jan-01 00:00 django_bpp/staticroot/django_tinymce/init_tinymce.js
--rw-r--r--  2.0 unx     1559 b- defN 80-Jan-01 00:00 django_bpp/staticroot/djangoql/css/completion.css
--rw-r--r--  2.0 unx     2467 b- defN 80-Jan-01 00:00 django_bpp/staticroot/djangoql/css/completion.css.map
--rw-r--r--  2.0 unx      416 b- defN 80-Jan-01 00:00 django_bpp/staticroot/djangoql/css/completion_admin.css
--rw-r--r--  2.0 unx      196 b- defN 80-Jan-01 00:00 django_bpp/staticroot/djangoql/css/syntax_help.css
--rw-r--r--  2.0 unx    91020 b- defN 80-Jan-01 00:00 django_bpp/staticroot/djangoql/img/completion_example.png
--rw-r--r--  2.0 unx    66780 b- defN 80-Jan-01 00:00 django_bpp/staticroot/djangoql/img/completion_example_scaled.png
--rw-r--r--  2.0 unx    27567 b- defN 80-Jan-01 00:00 django_bpp/staticroot/djangoql/js/completion.js
--rw-r--r--  2.0 unx   100354 b- defN 80-Jan-01 00:00 django_bpp/staticroot/djangoql/js/completion.js.map
--rw-r--r--  2.0 unx     3298 b- defN 80-Jan-01 00:00 django_bpp/staticroot/djangoql/js/completion_admin.js
--rw-r--r--  2.0 unx      132 b- defN 80-Jan-01 00:00 django_bpp/staticroot/djangoql/js/completion_admin_toggle.js
--rw-r--r--  2.0 unx      100 b- defN 80-Jan-01 00:00 django_bpp/staticroot/djangoql/js/completion_admin_toggle_off.js
--rw-r--r--  2.0 unx    10161 b- defN 80-Jan-01 00:00 django_bpp/staticroot/ewaluacja2021/xlsx/default.xlsx
--rw-r--r--  2.0 unx     2685 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/css/foundation-datepicker.min.css
--rw-r--r--  2.0 unx    19508 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/foundation-icons.css
--rw-r--r--  2.0 unx   150535 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/foundation-icons.svg
--rw-r--r--  2.0 unx    56976 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/foundation-icons.ttf
--rw-r--r--  2.0 unx    32020 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/foundation-icons.woff
--rw-r--r--  2.0 unx     1352 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-address-book.svg
--rw-r--r--  2.0 unx     1425 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-alert.svg
--rw-r--r--  2.0 unx     1372 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-align-center.svg
--rw-r--r--  2.0 unx     1292 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-align-justify.svg
--rw-r--r--  2.0 unx     1369 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-align-left.svg
--rw-r--r--  2.0 unx     1390 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-align-right.svg
--rw-r--r--  2.0 unx     1796 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-anchor.svg
--rw-r--r--  2.0 unx     1194 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-annotate.svg
--rw-r--r--  2.0 unx     1558 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-archive.svg
--rw-r--r--  2.0 unx      921 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-arrow-down.svg
--rw-r--r--  2.0 unx      919 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-arrow-left.svg
--rw-r--r--  2.0 unx      922 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-arrow-right.svg
--rw-r--r--  2.0 unx      921 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-arrow-up.svg
--rw-r--r--  2.0 unx     1435 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-arrows-compress.svg
--rw-r--r--  2.0 unx     1431 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-arrows-expand.svg
--rw-r--r--  2.0 unx     2365 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-arrows-in.svg
--rw-r--r--  2.0 unx     2354 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-arrows-out.svg
--rw-r--r--  2.0 unx     5365 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-asl.svg
--rw-r--r--  2.0 unx     1865 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-asterisk.svg
--rw-r--r--  2.0 unx     1718 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-at-sign.svg
--rw-r--r--  2.0 unx      984 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-background-color.svg
--rw-r--r--  2.0 unx      876 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-battery-empty.svg
--rw-r--r--  2.0 unx      937 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-battery-full.svg
--rw-r--r--  2.0 unx      956 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-battery-half.svg
--rw-r--r--  2.0 unx     1775 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-bitcoin-circle.svg
--rw-r--r--  2.0 unx     2227 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-bitcoin.svg
--rw-r--r--  2.0 unx     1817 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-blind.svg
--rw-r--r--  2.0 unx     1564 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-bluetooth.svg
--rw-r--r--  2.0 unx      976 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-bold.svg
--rw-r--r--  2.0 unx     1510 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-book-bookmark.svg
--rw-r--r--  2.0 unx     1450 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-book.svg
--rw-r--r--  2.0 unx      896 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-bookmark.svg
--rw-r--r--  2.0 unx      760 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-braille.svg
--rw-r--r--  2.0 unx     2421 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-burst-new.svg
--rw-r--r--  2.0 unx     2798 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-burst-sale.svg
--rw-r--r--  2.0 unx     1928 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-burst.svg
--rw-r--r--  2.0 unx     2561 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-calendar.svg
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-camera.svg
--rw-r--r--  2.0 unx      941 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-check.svg
--rw-r--r--  2.0 unx     1332 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-checkbox.svg
--rw-r--r--  2.0 unx     3130 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-clipboard-notes.svg
--rw-r--r--  2.0 unx     2028 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-clipboard-pencil.svg
--rw-r--r--  2.0 unx     1411 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-clipboard.svg
--rw-r--r--  2.0 unx     1258 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-clock.svg
--rw-r--r--  2.0 unx     2006 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-closed-caption.svg
--rw-r--r--  2.0 unx      869 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-cloud.svg
--rw-r--r--  2.0 unx     1162 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-comment-minus.svg
--rw-r--r--  2.0 unx     2858 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-comment-quotes.svg
--rw-r--r--  2.0 unx     1041 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-comment-video.svg
--rw-r--r--  2.0 unx      822 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-comment.svg
--rw-r--r--  2.0 unx     1164 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-comments.svg
--rw-r--r--  2.0 unx     1195 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-compass.svg
--rw-r--r--  2.0 unx      756 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-contrast.svg
--rw-r--r--  2.0 unx      986 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-credit-card.svg
--rw-r--r--  2.0 unx     1207 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-crop.svg
--rw-r--r--  2.0 unx     1818 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-crown.svg
--rw-r--r--  2.0 unx      929 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-css3.svg
--rw-r--r--  2.0 unx     1951 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-database.svg
--rw-r--r--  2.0 unx     1533 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-die-five.svg
--rw-r--r--  2.0 unx     1385 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-die-four.svg
--rw-r--r--  2.0 unx      881 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-die-one.svg
--rw-r--r--  2.0 unx     1697 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-die-six.svg
--rw-r--r--  2.0 unx     1227 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-die-three.svg
--rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-die-two.svg
--rw-r--r--  2.0 unx     1515 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-dislike.svg
--rw-r--r--  2.0 unx     3133 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-dollar-bill.svg
--rw-r--r--  2.0 unx     1693 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-dollar.svg
--rw-r--r--  2.0 unx     1231 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-download.svg
--rw-r--r--  2.0 unx     1219 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-eject.svg
--rw-r--r--  2.0 unx     3487 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-elevator.svg
--rw-r--r--  2.0 unx     2171 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-euro.svg
--rw-r--r--  2.0 unx     1190 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-eye.svg
--rw-r--r--  2.0 unx      984 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-fast-forward.svg
--rw-r--r--  2.0 unx     1398 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-female-symbol.svg
--rw-r--r--  2.0 unx     1925 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-female.svg
--rw-r--r--  2.0 unx     1052 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-filter.svg
--rw-r--r--  2.0 unx     1749 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-first-aid.svg
--rw-r--r--  2.0 unx     1093 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-flag.svg
--rw-r--r--  2.0 unx     1357 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-folder-add.svg
--rw-r--r--  2.0 unx     1318 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-folder-lock.svg
--rw-r--r--  2.0 unx      826 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-folder.svg
--rw-r--r--  2.0 unx     1122 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-foot.svg
--rw-r--r--  2.0 unx     4229 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-foundation.svg
--rw-r--r--  2.0 unx     1348 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-graph-bar.svg
--rw-r--r--  2.0 unx     1158 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-graph-horizontal.svg
--rw-r--r--  2.0 unx     1239 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-graph-pie.svg
--rw-r--r--  2.0 unx     1384 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-graph-trend.svg
--rw-r--r--  2.0 unx     2226 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-guide-dog.svg
--rw-r--r--  2.0 unx     2850 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-hearing-aid.svg
--rw-r--r--  2.0 unx      921 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-heart.svg
--rw-r--r--  2.0 unx      827 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-home.svg
--rw-r--r--  2.0 unx      935 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-html5.svg
--rw-r--r--  2.0 unx     1644 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-indent-less.svg
--rw-r--r--  2.0 unx     1644 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-indent-more.svg
--rw-r--r--  2.0 unx      997 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-info.svg
--rw-r--r--  2.0 unx      883 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-italic.svg
--rw-r--r--  2.0 unx     1423 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-key.svg
--rw-r--r--  2.0 unx     1237 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-laptop.svg
--rw-r--r--  2.0 unx     1105 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-layout.svg
--rw-r--r--  2.0 unx     2950 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-lightbulb.svg
--rw-r--r--  2.0 unx     1557 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-like.svg
--rw-r--r--  2.0 unx     1611 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-link.svg
--rw-r--r--  2.0 unx     1228 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-list-bullet.svg
--rw-r--r--  2.0 unx     2020 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-list-number.svg
--rw-r--r--  2.0 unx     2290 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-list-thumbnails.svg
--rw-r--r--  2.0 unx     1378 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-list.svg
--rw-r--r--  2.0 unx      990 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-lock.svg
--rw-r--r--  2.0 unx     1798 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-loop.svg
--rw-r--r--  2.0 unx     1028 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-magnifying-glass.svg
--rw-r--r--  2.0 unx     1910 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-mail.svg
--rw-r--r--  2.0 unx     2879 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-male-female.svg
--rw-r--r--  2.0 unx     1224 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-male-symbol.svg
--rw-r--r--  2.0 unx     1409 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-male.svg
--rw-r--r--  2.0 unx     1712 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-map.svg
--rw-r--r--  2.0 unx     1051 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-marker.svg
--rw-r--r--  2.0 unx     1670 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-megaphone.svg
--rw-r--r--  2.0 unx     1396 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-microphone.svg
--rw-r--r--  2.0 unx     1052 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-minus-circle.svg
--rw-r--r--  2.0 unx      681 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-minus.svg
--rw-r--r--  2.0 unx     2325 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-mobile-signal.svg
--rw-r--r--  2.0 unx      904 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-mobile.svg
--rw-r--r--  2.0 unx      940 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-monitor.svg
--rw-r--r--  2.0 unx     1004 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-mountains.svg
--rw-r--r--  2.0 unx      926 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-music.svg
--rw-r--r--  2.0 unx     1325 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-next.svg
--rw-r--r--  2.0 unx     2200 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-no-dogs.svg
--rw-r--r--  2.0 unx     1975 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-no-smoking.svg
--rw-r--r--  2.0 unx     1430 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-add.svg
--rw-r--r--  2.0 unx     1061 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-copy.svg
--rw-r--r--  2.0 unx     1670 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-csv.svg
--rw-r--r--  2.0 unx     1516 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-delete.svg
--rw-r--r--  2.0 unx     1674 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-doc.svg
--rw-r--r--  2.0 unx     1467 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-edit.svg
--rw-r--r--  2.0 unx     2306 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-export-csv.svg
--rw-r--r--  2.0 unx     2334 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-export-doc.svg
--rw-r--r--  2.0 unx     2075 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-export-pdf.svg
--rw-r--r--  2.0 unx     1453 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-export.svg
--rw-r--r--  2.0 unx     1019 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-filled.svg
--rw-r--r--  2.0 unx     1132 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-multiple.svg
--rw-r--r--  2.0 unx     1450 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-pdf.svg
--rw-r--r--  2.0 unx     1273 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-remove.svg
--rw-r--r--  2.0 unx     1504 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-search.svg
--rw-r--r--  2.0 unx      827 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page.svg
--rw-r--r--  2.0 unx     1418 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-paint-bucket.svg
--rw-r--r--  2.0 unx     1494 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-paperclip.svg
--rw-r--r--  2.0 unx     1297 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-pause.svg
--rw-r--r--  2.0 unx     1325 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-paw.svg
--rw-r--r--  2.0 unx     1845 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-paypal.svg
--rw-r--r--  2.0 unx      881 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-pencil.svg
--rw-r--r--  2.0 unx     1212 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-photo.svg
--rw-r--r--  2.0 unx     1192 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-play-circle.svg
--rw-r--r--  2.0 unx      888 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-play-video.svg
--rw-r--r--  2.0 unx      835 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-play.svg
--rw-r--r--  2.0 unx     1055 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-plus.svg
--rw-r--r--  2.0 unx     2228 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-pound.svg
--rw-r--r--  2.0 unx     1795 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-power.svg
--rw-r--r--  2.0 unx     1296 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-previous.svg
--rw-r--r--  2.0 unx     1326 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-price-tag.svg
--rw-r--r--  2.0 unx     1801 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-pricetag-multiple.svg
--rw-r--r--  2.0 unx     1085 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-print.svg
--rw-r--r--  2.0 unx      950 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-prohibited.svg
--rw-r--r--  2.0 unx     1163 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-projection-screen.svg
--rw-r--r--  2.0 unx     2292 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-puzzle.svg
--rw-r--r--  2.0 unx     2614 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-quote.svg
--rw-r--r--  2.0 unx      849 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-record.svg
--rw-r--r--  2.0 unx     1218 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-refresh.svg
--rw-r--r--  2.0 unx     2414 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-results-demographics.svg
--rw-r--r--  2.0 unx     2867 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-results.svg
--rw-r--r--  2.0 unx     2080 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-rewind-ten.svg
--rw-r--r--  2.0 unx      983 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-rewind.svg
--rw-r--r--  2.0 unx     1553 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-rss.svg
--rw-r--r--  2.0 unx     1141 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-safety-cone.svg
--rw-r--r--  2.0 unx     1533 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-save.svg
--rw-r--r--  2.0 unx     1130 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-share.svg
--rw-r--r--  2.0 unx     1537 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-sheriff-badge.svg
--rw-r--r--  2.0 unx      816 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-shield.svg
--rw-r--r--  2.0 unx      902 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-shopping-bag.svg
--rw-r--r--  2.0 unx     1307 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-shopping-cart.svg
--rw-r--r--  2.0 unx     1797 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-shuffle.svg
--rw-r--r--  2.0 unx     2076 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-skull.svg
--rw-r--r--  2.0 unx     2859 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-500px.svg
--rw-r--r--  2.0 unx      747 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-adobe.svg
--rw-r--r--  2.0 unx     2643 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-amazon.svg
--rw-r--r--  2.0 unx     2323 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-android.svg
--rw-r--r--  2.0 unx     1246 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-apple.svg
--rw-r--r--  2.0 unx     2333 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-behance.svg
--rw-r--r--  2.0 unx     1135 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-bing.svg
--rw-r--r--  2.0 unx     1504 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-blogger.svg
--rw-r--r--  2.0 unx      598 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-delicious.svg
--rw-r--r--  2.0 unx     1961 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-designer-news.svg
--rw-r--r--  2.0 unx     1758 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-deviant-art.svg
--rw-r--r--  2.0 unx     3703 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-digg.svg
--rw-r--r--  2.0 unx     1814 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-dribbble.svg
--rw-r--r--  2.0 unx      770 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-drive.svg
--rw-r--r--  2.0 unx      953 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-dropbox.svg
--rw-r--r--  2.0 unx     2253 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-evernote.svg
--rw-r--r--  2.0 unx      882 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-facebook.svg
--rw-r--r--  2.0 unx      923 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-flickr.svg
--rw-r--r--  2.0 unx      835 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-forrst.svg
--rw-r--r--  2.0 unx     1526 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-foursquare.svg
--rw-r--r--  2.0 unx     1568 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-game-center.svg
--rw-r--r--  2.0 unx     1495 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-github.svg
--rw-r--r--  2.0 unx     2616 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-google-plus.svg
--rw-r--r--  2.0 unx      814 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-hacker-news.svg
--rw-r--r--  2.0 unx     1811 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-hi5.svg
--rw-r--r--  2.0 unx     1645 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-instagram.svg
--rw-r--r--  2.0 unx     2862 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-joomla.svg
--rw-r--r--  2.0 unx     1334 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-lastfm.svg
--rw-r--r--  2.0 unx     1094 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-linkedin.svg
--rw-r--r--  2.0 unx     1041 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-medium.svg
--rw-r--r--  2.0 unx     1525 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-myspace.svg
--rw-r--r--  2.0 unx     1055 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-orkut.svg
--rw-r--r--  2.0 unx      977 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-path.svg
--rw-r--r--  2.0 unx     1477 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-picasa.svg
--rw-r--r--  2.0 unx     1436 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-pinterest.svg
--rw-r--r--  2.0 unx     1107 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-rdio.svg
--rw-r--r--  2.0 unx     1821 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-reddit.svg
--rw-r--r--  2.0 unx     3053 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-skillshare.svg
--rw-r--r--  2.0 unx     2562 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-skype.svg
--rw-r--r--  2.0 unx     3461 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-smashing-mag.svg
--rw-r--r--  2.0 unx     1836 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-snapchat.svg
--rw-r--r--  2.0 unx     2134 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-spotify.svg
--rw-r--r--  2.0 unx     2827 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-squidoo.svg
--rw-r--r--  2.0 unx     1460 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-stack-overflow.svg
--rw-r--r--  2.0 unx     1822 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-steam.svg
--rw-r--r--  2.0 unx     1388 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-stumbleupon.svg
--rw-r--r--  2.0 unx     2487 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-treehouse.svg
--rw-r--r--  2.0 unx     1178 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-tumblr.svg
--rw-r--r--  2.0 unx     1285 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-twitter.svg
--rw-r--r--  2.0 unx     1915 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-vimeo.svg
--rw-r--r--  2.0 unx      805 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-windows.svg
--rw-r--r--  2.0 unx     1285 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-xbox.svg
--rw-r--r--  2.0 unx     1883 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-yahoo.svg
--rw-r--r--  2.0 unx     1897 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-yelp.svg
--rw-r--r--  2.0 unx     3657 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-youtube.svg
--rw-r--r--  2.0 unx     1458 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-zerply.svg
--rw-r--r--  2.0 unx     1101 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-zurb.svg
--rw-r--r--  2.0 unx     4724 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-sound.svg
--rw-r--r--  2.0 unx     1041 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-star.svg
--rw-r--r--  2.0 unx      911 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-stop.svg
--rw-r--r--  2.0 unx     2065 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-strikethrough.svg
--rw-r--r--  2.0 unx     1966 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-subscript.svg
--rw-r--r--  2.0 unx     1969 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-superscript.svg
--rw-r--r--  2.0 unx     1014 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-tablet-landscape.svg
--rw-r--r--  2.0 unx     1015 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-tablet-portrait.svg
--rw-r--r--  2.0 unx     1453 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-target-two.svg
--rw-r--r--  2.0 unx     1187 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-target.svg
--rw-r--r--  2.0 unx     4361 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-telephone-accessible.svg
--rw-r--r--  2.0 unx     1238 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-telephone.svg
--rw-r--r--  2.0 unx     1314 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-text-color.svg
--rw-r--r--  2.0 unx     2960 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-thumbnails.svg
--rw-r--r--  2.0 unx     1861 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-ticket.svg
--rw-r--r--  2.0 unx     1688 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-torso-business.svg
--rw-r--r--  2.0 unx     1345 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-torso-female.svg
--rw-r--r--  2.0 unx     1042 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-torso.svg
--rw-r--r--  2.0 unx     1840 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-torsos-all-female.svg
--rw-r--r--  2.0 unx     1856 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-torsos-all.svg
--rw-r--r--  2.0 unx     1707 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-torsos-female-male.svg
--rw-r--r--  2.0 unx     1714 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-torsos-male-female.svg
--rw-r--r--  2.0 unx     1448 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-torsos.svg
--rw-r--r--  2.0 unx     1019 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-trash.svg
--rw-r--r--  2.0 unx     2086 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-trees.svg
--rw-r--r--  2.0 unx     1394 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-trophy.svg
--rw-r--r--  2.0 unx     1140 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-underline.svg
--rw-r--r--  2.0 unx     2013 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-universal-access.svg
--rw-r--r--  2.0 unx     3511 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-unlink.svg
--rw-r--r--  2.0 unx      995 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-unlock.svg
--rw-r--r--  2.0 unx     1352 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-upload-cloud.svg
--rw-r--r--  2.0 unx     1227 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-upload.svg
--rw-r--r--  2.0 unx     1105 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-usb.svg
--rw-r--r--  2.0 unx      713 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-video.svg
--rw-r--r--  2.0 unx      959 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-volume-none.svg
--rw-r--r--  2.0 unx     2438 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-volume-strike.svg
--rw-r--r--  2.0 unx     2398 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-volume.svg
--rw-r--r--  2.0 unx     1356 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-web.svg
--rw-r--r--  2.0 unx     1762 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-wheelchair.svg
--rw-r--r--  2.0 unx     1976 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-widget.svg
--rw-r--r--  2.0 unx     1520 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-wrench.svg
--rw-r--r--  2.0 unx     1455 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-x-circle.svg
--rw-r--r--  2.0 unx     1100 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-x.svg
--rw-r--r--  2.0 unx     1799 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-yen.svg
--rw-r--r--  2.0 unx     1743 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-zoom-in.svg
--rw-r--r--  2.0 unx     1233 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-zoom-out.svg
--rw-r--r--  2.0 unx    27530 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/js/foundation-datepicker.min.js
--rw-r--r--  2.0 unx      777 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-datepicker/js/locales/foundation-datepicker.pl.js
--rw-r--r--  2.0 unx   134868 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-sites/dist/css/foundation.min.css
--rw-r--r--  2.0 unx   193939 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-sites/dist/js/foundation.min.js
--rw-r--r--  2.0 unx   517750 b- defN 80-Jan-01 00:00 django_bpp/staticroot/foundation-sites/dist/js/foundation.min.js.map
--rw-r--r--  2.0 unx      244 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/backgrounds/changelist-results.png
--rw-r--r--  2.0 unx     3027 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/backgrounds/loading-small.gif
--rw-r--r--  2.0 unx     1247 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/backgrounds/messagelist.png
--rw-r--r--  2.0 unx      116 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/backgrounds/nav-grabber.gif
--rw-r--r--  2.0 unx      259 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/backgrounds/ui-sortable-placeholder.png
--rw-r--r--  2.0 unx     1000 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/add-another.png
--rw-r--r--  2.0 unx     1000 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/add-another_hover.png
--rw-r--r--  2.0 unx      192 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/back-link-rtl.png
--rw-r--r--  2.0 unx      192 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/back-link-rtl_hover.png
--rw-r--r--  2.0 unx     1009 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/back-link.png
--rw-r--r--  2.0 unx     1009 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/back-link_hover.png
--rw-r--r--  2.0 unx     1103 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/breadcrumbs-rtl.png
--rw-r--r--  2.0 unx     1104 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/breadcrumbs-rtl_hover.png
--rw-r--r--  2.0 unx     1098 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/breadcrumbs.png
--rw-r--r--  2.0 unx     1094 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/breadcrumbs_hover.png
--rw-r--r--  2.0 unx     1092 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/date-hierarchy-back-rtl.png
--rw-r--r--  2.0 unx     1092 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/date-hierarchy-back-rtl_hover.png
--rw-r--r--  2.0 unx     1018 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/date-hierarchy-back.png
--rw-r--r--  2.0 unx     1018 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/date-hierarchy-back_hover.png
--rw-r--r--  2.0 unx      256 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/datepicker.png
--rw-r--r--  2.0 unx      265 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/datepicker_hover.png
--rw-r--r--  2.0 unx     1181 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/datetime-now.png
--rw-r--r--  2.0 unx     1136 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/datetime-now_hover.png
--rw-r--r--  2.0 unx      289 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/form-select.png
--rw-r--r--  2.0 unx      198 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/link-internal-rtl.png
--rw-r--r--  2.0 unx      198 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/link-internal-rtl_hover.png
--rw-r--r--  2.0 unx     1056 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/object-tools-add-link.png
--rw-r--r--  2.0 unx     1082 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/object-tools-viewsite-link.png
--rw-r--r--  2.0 unx      225 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/pulldown-handler.png
--rw-r--r--  2.0 unx      228 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/pulldown-handler_hover.png
--rw-r--r--  2.0 unx      228 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/pulldown-handler_selected.png
--rw-r--r--  2.0 unx      375 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/related-lookup-m2m.png
--rw-r--r--  2.0 unx      368 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/related-lookup-m2m_hover.png
--rw-r--r--  2.0 unx      374 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/related-lookup.png
--rw-r--r--  2.0 unx      377 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/related-lookup_hover.png
--rw-r--r--  2.0 unx     1107 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/related-remove.png
--rw-r--r--  2.0 unx     1106 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/related-remove_hover.png
--rw-r--r--  2.0 unx     3136 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/searchbox.png
--rw-r--r--  2.0 unx     2991 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/selector-add-m2m-horizontal.png
--rw-r--r--  2.0 unx     2995 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/selector-add-m2m-horizontal_hover.png
--rw-r--r--  2.0 unx     3023 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/selector-add-m2m-vertical.png
--rw-r--r--  2.0 unx     3023 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/selector-add-m2m-vertical_hover.png
--rw-r--r--  2.0 unx      247 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/selector-filter.png
--rw-r--r--  2.0 unx     2998 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/selector-remove-m2m-horizontal.png
--rw-r--r--  2.0 unx     3003 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/selector-remove-m2m-horizontal_hover.png
--rw-r--r--  2.0 unx     3009 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/selector-remove-m2m-vertical.png
--rw-r--r--  2.0 unx     3009 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/selector-remove-m2m-vertical_hover.png
--rw-r--r--  2.0 unx     1130 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/sort-remove.png
--rw-r--r--  2.0 unx     1130 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/sort-remove_hover.png
--rw-r--r--  2.0 unx     1150 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/sorted-ascending.png
--rw-r--r--  2.0 unx     1148 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/sorted-descending.png
--rw-r--r--  2.0 unx      323 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/status-no.png
--rw-r--r--  2.0 unx      406 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/status-unknown.png
--rw-r--r--  2.0 unx      396 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/status-yes.png
--rw-r--r--  2.0 unx      243 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/th-ascending.png
--rw-r--r--  2.0 unx      240 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/th-descending.png
--rw-r--r--  2.0 unx      466 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/timepicker.png
--rw-r--r--  2.0 unx      463 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/timepicker_hover.png
--rw-r--r--  2.0 unx      226 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-add-handler.png
--rw-r--r--  2.0 unx      196 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-add-handler_hover.png
--rw-r--r--  2.0 unx      228 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-arrow-down-handler.png
--rw-r--r--  2.0 unx      225 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-arrow-down-handler_hover.png
--rw-r--r--  2.0 unx      217 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-arrow-up-handler.png
--rw-r--r--  2.0 unx      217 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-arrow-up-handler_hover.png
--rw-r--r--  2.0 unx      256 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-close-handler.png
--rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-close-handler_hover.png
--rw-r--r--  2.0 unx     1297 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-delete-handler-predelete.png
--rw-r--r--  2.0 unx      210 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-delete-handler.png
--rw-r--r--  2.0 unx      237 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-delete-handler_hover.png
--rw-r--r--  2.0 unx      253 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-drag-handler.png
--rw-r--r--  2.0 unx      221 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-drag-handler_hover.png
--rw-r--r--  2.0 unx      260 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-edit-handler.png
--rw-r--r--  2.0 unx      253 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-edit-handler_hover.png
--rw-r--r--  2.0 unx      274 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-open-handler.png
--rw-r--r--  2.0 unx      274 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-open-handler_hover.png
--rw-r--r--  2.0 unx      180 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-remove-handler.png
--rw-r--r--  2.0 unx      161 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-remove-handler_hover.png
--rw-r--r--  2.0 unx      269 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-trash-handler.png
--rw-r--r--  2.0 unx      277 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-trash-handler_hover.png
--rw-r--r--  2.0 unx      263 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-trash-list-toggle-handler.png
--rw-r--r--  2.0 unx      219 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-trash-list-toggle-handler_hover.png
--rw-r--r--  2.0 unx      251 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-viewsite-link.png
--rw-r--r--  2.0 unx      208 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/tools-viewsite-link_hover.png
--rw-r--r--  2.0 unx     1007 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/ui-datepicker-next.png
--rw-r--r--  2.0 unx     1007 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/ui-datepicker-next_hover.png
--rw-r--r--  2.0 unx     1009 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/ui-datepicker-prev.png
--rw-r--r--  2.0 unx     1009 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons/ui-datepicker-prev_hover.png
--rw-r--r--  2.0 unx     9844 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-s79f97b581c.png
--rw-r--r--  2.0 unx      986 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/add-link.png
--rw-r--r--  2.0 unx      986 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/add-link_hover.png
--rw-r--r--  2.0 unx     1166 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/autocomplete-multiple.png
--rw-r--r--  2.0 unx     1186 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/autocomplete-single.png
--rw-r--r--  2.0 unx      963 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/change-link.png
--rw-r--r--  2.0 unx      963 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/change-link_hover.png
--rw-r--r--  2.0 unx      979 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/delete-link.png
--rw-r--r--  2.0 unx     1098 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/filter-choice-selected.png
--rw-r--r--  2.0 unx      204 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/link-external-rtl.png
--rw-r--r--  2.0 unx      204 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/link-external-rtl_hover.png
--rw-r--r--  2.0 unx     1030 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/link-external.png
--rw-r--r--  2.0 unx     1030 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/link-external_hover.png
--rw-r--r--  2.0 unx      198 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/link-internal-rtl.png
--rw-r--r--  2.0 unx      199 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/link-internal-rtl_hover.png
--rw-r--r--  2.0 unx      206 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/link-internal.png
--rw-r--r--  2.0 unx     1022 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/link-internal_hover.png
--rw-r--r--  2.0 unx      979 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/sort-remove.png
--rw-r--r--  2.0 unx     1108 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/tools-related-add-handler-disabled.png
--rw-r--r--  2.0 unx     1108 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/tools-related-add-handler.png
--rw-r--r--  2.0 unx     1108 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/tools-related-add-handler_hover.png
--rw-r--r--  2.0 unx     1158 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/tools-related-edit-handler-disabled.png
--rw-r--r--  2.0 unx     1158 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/tools-related-edit-handler.png
--rw-r--r--  2.0 unx     1158 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/tools-related-edit-handler_hover.png
--rw-r--r--  2.0 unx     1164 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/tools-related-remove-handler-disabled.png
--rw-r--r--  2.0 unx     1164 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/tools-related-remove-handler.png
--rw-r--r--  2.0 unx     1163 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small/tools-related-remove-handler_hover.png
--rw-r--r--  2.0 unx     2438 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/images/icons-small-sc29b5b842f.png
--rw-r--r--  2.0 unx       80 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/img/admin/arrow-down.gif
--rw-r--r--  2.0 unx      838 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/img/admin/arrow-up.gif
--rw-r--r--  2.0 unx     1186 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/i18n/ui.datepicker-pl.js
--rw-r--r--  2.0 unx    17813 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/jquery-migrate-3.0.1.js
--rw-r--r--  2.0 unx    11421 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/jquery-migrate-3.0.1.min.js
--rw-r--r--  2.0 unx   288580 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/jquery.js
--rw-r--r--  2.0 unx    89501 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/jquery.min.js
--rw-r--r--  2.0 unx   288580 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/ui/external/jquery/jquery.js
--rw-r--r--  2.0 unx     7090 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/ui/images/ui-icons_444444_256x240.png
--rw-r--r--  2.0 unx     7074 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/ui/images/ui-icons_555555_256x240.png
--rw-r--r--  2.0 unx     4618 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/ui/images/ui-icons_777620_256x240.png
--rw-r--r--  2.0 unx     7111 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/ui/images/ui-icons_777777_256x240.png
--rw-r--r--  2.0 unx     4618 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/ui/images/ui-icons_cc0000_256x240.png
--rw-r--r--  2.0 unx     6487 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/ui/images/ui-icons_ffffff_256x240.png
--rw-r--r--  2.0 unx    32532 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/ui/index.html
--rw-r--r--  2.0 unx    36123 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/ui/jquery-ui.css
--rw-r--r--  2.0 unx   528735 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/ui/jquery-ui.js
--rw-r--r--  2.0 unx    30801 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/ui/jquery-ui.min.css
--rw-r--r--  2.0 unx   254916 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/ui/jquery-ui.min.js
--rw-r--r--  2.0 unx    18718 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/ui/jquery-ui.structure.css
--rw-r--r--  2.0 unx    15560 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/ui/jquery-ui.structure.min.css
--rw-r--r--  2.0 unx    17455 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/ui/jquery-ui.theme.css
--rw-r--r--  2.0 unx    13889 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/jquery/ui/jquery-ui.theme.min.css
--rw-r--r--  2.0 unx     9464 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/js/grappelli.js
--rw-r--r--  2.0 unx    27664 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/js/grappelli.min.js
--rw-r--r--  2.0 unx     6379 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/js/jquery.grp_autocomplete_fk.js
--rw-r--r--  2.0 unx     7840 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/js/jquery.grp_autocomplete_generic.js
--rw-r--r--  2.0 unx     9214 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/js/jquery.grp_autocomplete_m2m.js
--rw-r--r--  2.0 unx     1118 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/js/jquery.grp_collapsible.js
--rw-r--r--  2.0 unx     1963 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/js/jquery.grp_collapsible_group.js
--rw-r--r--  2.0 unx    10876 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/js/jquery.grp_inline.js
--rw-r--r--  2.0 unx     2604 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/js/jquery.grp_related_fk.js
--rw-r--r--  2.0 unx     3446 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/js/jquery.grp_related_generic.js
--rw-r--r--  2.0 unx     2870 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/js/jquery.grp_related_m2m.js
--rw-r--r--  2.0 unx     7301 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/js/jquery.grp_timepicker.js
--rw-r--r--  2.0 unx    36580 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/stylesheets/mueller/grid/output-rtl.css
--rw-r--r--  2.0 unx    36537 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/stylesheets/mueller/grid/output.css
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/stylesheets/mueller/screen.css
--rw-r--r--  2.0 unx     8090 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/stylesheets/partials/custom/tinymce.css
--rw-r--r--  2.0 unx    42813 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/stylesheets/rtl.css
--rw-r--r--  2.0 unx   184243 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/stylesheets/screen.css
--rw-r--r--  2.0 unx     5858 b- defN 80-Jan-01 00:00 django_bpp/staticroot/grappelli/tinymce_setup/tinymce_setup.js
--rw-r--r--  2.0 unx    58778 b- defN 80-Jan-01 00:00 django_bpp/staticroot/import_dyscyplin/xlsx/default.xlsx
--rw-r--r--  2.0 unx      765 b- defN 80-Jan-01 00:00 django_bpp/staticroot/import_export/action_formats.js
--rw-r--r--  2.0 unx      711 b- defN 80-Jan-01 00:00 django_bpp/staticroot/import_export/guess_format.js
--rw-r--r--  2.0 unx     2051 b- defN 80-Jan-01 00:00 django_bpp/staticroot/import_export/import.css
--rw-r--r--  2.0 unx     9452 b- defN 80-Jan-01 00:00 django_bpp/staticroot/import_list_if/import_list_if_przyklad.xlsx
--rw-r--r--  2.0 unx     9735 b- defN 80-Jan-01 00:00 django_bpp/staticroot/import_pracownikow/import_pracownikow_przyklad.xlsx
--rw-r--r--  2.0 unx    20604 b- defN 80-Jan-01 00:00 django_bpp/staticroot/jinplace/js/jinplace.js
--rw-r--r--  2.0 unx    89501 b- defN 80-Jan-01 00:00 django_bpp/staticroot/jquery/dist/jquery.min.js
--rw-r--r--  2.0 unx     3121 b- defN 80-Jan-01 00:00 django_bpp/staticroot/jquery.cookie/jquery.cookie.js
--rw-r--r--  2.0 unx    35348 b- defN 80-Jan-01 00:00 django_bpp/staticroot/jqueryui/jquery-ui.css
--rw-r--r--  2.0 unx   238314 b- defN 80-Jan-01 00:00 django_bpp/staticroot/jqueryui/jquery-ui.min.js
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 django_bpp/staticroot/js/columns.js
--rw-r--r--  2.0 unx     3706 b- defN 80-Jan-01 00:00 django_bpp/staticroot/js/crispy_forms_foundation/plugins.js
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 django_bpp/staticroot/js/flexible_reports.js
--rw-r--r--  2.0 unx     1469 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/css/jquery.keypad.alt.css
--rw-r--r--  2.0 unx     1833 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/css/jquery.keypad.css
--rw-r--r--  2.0 unx      109 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/img/keypad.png
--rw-r--r--  2.0 unx     1203 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/index.html
--rw-r--r--  2.0 unx      949 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-ca.js
--rw-r--r--  2.0 unx      908 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-cs.js
--rw-r--r--  2.0 unx     1646 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-de.js
--rw-r--r--  2.0 unx      948 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-es.js
--rw-r--r--  2.0 unx     1687 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-fr.js
--rw-r--r--  2.0 unx     1738 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-hu.js
--rw-r--r--  2.0 unx      941 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-it.js
--rw-r--r--  2.0 unx      917 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-nl.js
--rw-r--r--  2.0 unx      963 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-no.js
--rw-r--r--  2.0 unx      932 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-pl.js
--rw-r--r--  2.0 unx      977 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-pt-BR.js
--rw-r--r--  2.0 unx      931 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-sk.js
--rw-r--r--  2.0 unx      947 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-tr.js
--rw-r--r--  2.0 unx    37992 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad.js
--rw-r--r--  2.0 unx    14128 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad.min.js
--rw-r--r--  2.0 unx    17898 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad.min.map
--rw-r--r--  2.0 unx    14416 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.plugin.js
--rw-r--r--  2.0 unx     3392 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.plugin.min.js
--rw-r--r--  2.0 unx     4265 b- defN 80-Jan-01 00:00 django_bpp/staticroot/kbw-keypad/dist/js/jquery.plugin.min.map
--rw-r--r--  2.0 unx      457 b- defN 80-Jan-01 00:00 django_bpp/staticroot/mptt/arrow-move-black.png
--rw-r--r--  2.0 unx      740 b- defN 80-Jan-01 00:00 django_bpp/staticroot/mptt/arrow-move-white.png
--rw-r--r--  2.0 unx      457 b- defN 80-Jan-01 00:00 django_bpp/staticroot/mptt/arrow-move.png
--rw-r--r--  2.0 unx      496 b- defN 80-Jan-01 00:00 django_bpp/staticroot/mptt/disclosure-down-black.png
--rw-r--r--  2.0 unx      753 b- defN 80-Jan-01 00:00 django_bpp/staticroot/mptt/disclosure-down-white.png
--rw-r--r--  2.0 unx      496 b- defN 80-Jan-01 00:00 django_bpp/staticroot/mptt/disclosure-down.png
--rw-r--r--  2.0 unx      464 b- defN 80-Jan-01 00:00 django_bpp/staticroot/mptt/disclosure-right-black.png
--rw-r--r--  2.0 unx      711 b- defN 80-Jan-01 00:00 django_bpp/staticroot/mptt/disclosure-right-white.png
--rw-r--r--  2.0 unx      464 b- defN 80-Jan-01 00:00 django_bpp/staticroot/mptt/disclosure-right.png
--rw-r--r--  2.0 unx     1415 b- defN 80-Jan-01 00:00 django_bpp/staticroot/mptt/draggable-admin.css
--rw-r--r--  2.0 unx    14682 b- defN 80-Jan-01 00:00 django_bpp/staticroot/mptt/draggable-admin.js
--rw-r--r--  2.0 unx      396 b- defN 80-Jan-01 00:00 django_bpp/staticroot/multiseek/css/style.css
--rw-r--r--  2.0 unx    26582 b- defN 80-Jan-01 00:00 django_bpp/staticroot/multiseek/js/multiseek.js
--rw-r--r--  2.0 unx    18643 b- defN 80-Jan-01 00:00 django_bpp/staticroot/notifications/js/mustache.js
--rw-r--r--  2.0 unx     2275 b- defN 80-Jan-01 00:00 django_bpp/staticroot/notifications/js/notifications.js
--rw-r--r--  2.0 unx     1862 b- defN 80-Jan-01 00:00 src/django_bpp/staticroot/notifications/js/tests/index.html
--rw-r--r--  2.0 unx     2788 b- defN 80-Jan-01 00:00 src/django_bpp/staticroot/notifications/js/tests/tests.js
--rw-r--r--  2.0 unx    23411 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/css/bootstrap-theme.min.css
--rw-r--r--  2.0 unx    75600 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/css/bootstrap-theme.min.css.map
--rw-r--r--  2.0 unx     3385 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/css/bootstrap-tweaks.css
--rw-r--r--  2.0 unx   121457 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/css/bootstrap.min.css
--rw-r--r--  2.0 unx   540434 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/css/bootstrap.min.css.map
--rw-r--r--  2.0 unx     1152 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/css/default.css
--rw-r--r--  2.0 unx    21658 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/css/font-awesome-4.0.3.css
--rw-r--r--  2.0 unx      817 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/css/prettify.css
--rw-r--r--  2.0 unx   202148 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/fonts/fontawesome-webfont.svg
--rw-r--r--  2.0 unx    80652 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/fonts/fontawesome-webfont.ttf
--rw-r--r--  2.0 unx    44432 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/fonts/fontawesome-webfont.woff
--rw-r--r--  2.0 unx   108738 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/fonts/glyphicons-halflings-regular.svg
--rw-r--r--  2.0 unx    45404 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--  2.0 unx    23424 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/fonts/glyphicons-halflings-regular.woff
--rw-r--r--  2.0 unx    18028 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--  2.0 unx     8777 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/img/glyphicons-halflings-white.png
--rw-r--r--  2.0 unx    12762 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/img/glyphicons-halflings.png
--rw-r--r--  2.0 unx     1458 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/img/grid.png
--rw-r--r--  2.0 unx     3597 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/js/ajax-form.js
--rw-r--r--  2.0 unx    39680 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/js/bootstrap.min.js
--rw-r--r--  2.0 unx   157600 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/js/coreapi-0.1.1.js
--rw-r--r--  2.0 unx     1719 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/js/csrf.js
--rw-r--r--  2.0 unx     1268 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/js/default.js
--rw-r--r--  2.0 unx    89476 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/js/jquery-3.5.1.min.js
--rw-r--r--  2.0 unx    13632 b- defN 80-Jan-01 00:00 django_bpp/staticroot/rest_framework/js/prettify-min.js
--rw-r--r--  2.0 unx   147826 b- defN 80-Jan-01 00:00 django_bpp/staticroot/scss/app-blue.css
--rw-r--r--  2.0 unx   147862 b- defN 80-Jan-01 00:00 django_bpp/staticroot/scss/app-green.css
--rw-r--r--  2.0 unx   147971 b- defN 80-Jan-01 00:00 django_bpp/staticroot/scss/app-orange.css
--rw-r--r--  2.0 unx    14966 b- defN 80-Jan-01 00:00 django_bpp/staticroot/select2/dist/css/select2.min.css
--rw-r--r--  2.0 unx      947 b- defN 80-Jan-01 00:00 django_bpp/staticroot/select2/dist/js/i18n/pl.js
--rw-r--r--  2.0 unx    79172 b- defN 80-Jan-01 00:00 django_bpp/staticroot/select2/dist/js/select2.full.min.js
--rw-r--r--  2.0 unx     9461 b- defN 80-Jan-01 00:00 django_bpp/staticroot/select2-foundation_theme/dist/select2-foundation-theme.css
--rw-r--r--  2.0 unx     5899 b- defN 80-Jan-01 00:00 django_bpp/staticroot/session_security/script.js
--rw-r--r--  2.0 unx      512 b- defN 80-Jan-01 00:00 django_bpp/staticroot/session_security/style.css
--rw-r--r--  2.0 unx     2404 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tabular_permissions/tabular_permissions.js
--rw-r--r--  2.0 unx    63894 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/icons/default/icons.min.js
--rw-r--r--  2.0 unx     6596 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/jquery.tinymce.min.js
--rw-r--r--  2.0 unx    36455 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/ar.js
--rw-r--r--  2.0 unx    42728 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/bg_BG.js
--rw-r--r--  2.0 unx    15791 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/ca.js
--rw-r--r--  2.0 unx    20192 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/cs.js
--rw-r--r--  2.0 unx    20104 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/cs_CZ.js
--rw-r--r--  2.0 unx    16650 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/cy.js
--rw-r--r--  2.0 unx    17105 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/da.js
--rw-r--r--  2.0 unx    18133 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/de.js
--rw-r--r--  2.0 unx    14639 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/es.js
--rw-r--r--  2.0 unx    16426 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/es_419.js
--rw-r--r--  2.0 unx    14259 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/es_ES.js
--rw-r--r--  2.0 unx    14809 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/es_MX.js
--rw-r--r--  2.0 unx    14332 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/eu.js
--rw-r--r--  2.0 unx    39850 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/fa.js
--rw-r--r--  2.0 unx    33533 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/fa_IR.js
--rw-r--r--  2.0 unx    15129 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/fi.js
--rw-r--r--  2.0 unx    18729 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/fr_FR.js
--rw-r--r--  2.0 unx    14764 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/gl.js
--rw-r--r--  2.0 unx    31934 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/he_IL.js
--rw-r--r--  2.0 unx    15199 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/hr.js
--rw-r--r--  2.0 unx    21472 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/hu_HU.js
--rw-r--r--  2.0 unx    14248 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/id.js
--rw-r--r--  2.0 unx    14336 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/it.js
--rw-r--r--  2.0 unx    14026 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/it_IT.js
--rw-r--r--  2.0 unx    28067 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/ja.js
--rw-r--r--  2.0 unx    15351 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/kab.js
--rw-r--r--  2.0 unx    39334 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/kk.js
--rw-r--r--  2.0 unx    19170 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/ko_KR.js
--rw-r--r--  2.0 unx    16479 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/lt.js
--rw-r--r--  2.0 unx    16926 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/nb_NO.js
--rw-r--r--  2.0 unx    16972 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/nl.js
--rw-r--r--  2.0 unx    16530 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/nl_BE.js
--rw-r--r--  2.0 unx    18687 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/pl.js
--rw-r--r--  2.0 unx    18461 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/pt_BR.js
--rw-r--r--  2.0 unx    18707 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/pt_PT.js
--rw-r--r--  2.0 unx    19155 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/ro.js
--rw-r--r--  2.0 unx    14801 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/ro_RO.js
--rw-r--r--  2.0 unx    50976 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/ru.js
--rw-r--r--  2.0 unx    48932 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/ru_RU.js
--rw-r--r--  2.0 unx    17392 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/sk.js
--rw-r--r--  2.0 unx    17182 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/sl.js
--rw-r--r--  2.0 unx    14335 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/sl_SI.js
--rw-r--r--  2.0 unx     7209 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/sq.js
--rw-r--r--  2.0 unx    15138 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/sv_SE.js
--rw-r--r--  2.0 unx    50913 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/ta.js
--rw-r--r--  2.0 unx    50917 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/ta_IN.js
--rw-r--r--  2.0 unx    46546 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/th_TH.js
--rw-r--r--  2.0 unx    17090 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/tr.js
--rw-r--r--  2.0 unx    20116 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/tr_TR.js
--rw-r--r--  2.0 unx    48481 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/ug.js
--rw-r--r--  2.0 unx    41007 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/uk.js
--rw-r--r--  2.0 unx    21254 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/zh_CN.js
--rw-r--r--  2.0 unx    18814 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/langs/zh_TW.js
--rw-r--r--  2.0 unx     3466 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/advlist/plugin.min.js
--rw-r--r--  2.0 unx     2712 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/anchor/plugin.min.js
--rw-r--r--  2.0 unx     2741 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/autolink/plugin.min.js
--rw-r--r--  2.0 unx     2296 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/autoresize/plugin.min.js
--rw-r--r--  2.0 unx     2959 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/autosave/plugin.min.js
--rw-r--r--  2.0 unx     3084 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/bbcode/plugin.min.js
--rw-r--r--  2.0 unx    11666 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/charmap/plugin.min.js
--rw-r--r--  2.0 unx     1132 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/code/plugin.min.js
--rw-r--r--  2.0 unx    48363 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/codesample/plugin.min.js
--rw-r--r--  2.0 unx      397 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/colorpicker/plugin.min.js
--rw-r--r--  2.0 unx      397 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/contextmenu/plugin.min.js
--rw-r--r--  2.0 unx     5336 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/directionality/plugin.min.js
--rw-r--r--  2.0 unx   482540 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/emoticons/js/emojiimages.js
--rw-r--r--  2.0 unx   421324 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/emoticons/js/emojiimages.min.js
--rw-r--r--  2.0 unx   259301 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/emoticons/js/emojis.js
--rw-r--r--  2.0 unx   198085 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/emoticons/js/emojis.min.js
--rw-r--r--  2.0 unx     6884 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/emoticons/plugin.min.js
--rw-r--r--  2.0 unx     7820 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/fullpage/plugin.min.js
--rw-r--r--  2.0 unx    16499 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/fullscreen/plugin.min.js
--rw-r--r--  2.0 unx    13389 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/help/plugin.min.js
--rw-r--r--  2.0 unx      740 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/hr/plugin.min.js
--rw-r--r--  2.0 unx    20152 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/image/plugin.min.js
--rw-r--r--  2.0 unx    19461 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/imagetools/plugin.min.js
--rw-r--r--  2.0 unx     3988 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/importcss/plugin.min.js
--rw-r--r--  2.0 unx     3008 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/insertdatetime/plugin.min.js
--rw-r--r--  2.0 unx     3004 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/legacyoutput/plugin.min.js
--rw-r--r--  2.0 unx    15729 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/link/plugin.min.js
--rw-r--r--  2.0 unx    27941 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/lists/plugin.min.js
--rw-r--r--  2.0 unx    17548 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/media/plugin.min.js
--rw-r--r--  2.0 unx     1389 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/nonbreaking/plugin.min.js
--rw-r--r--  2.0 unx     1754 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/noneditable/plugin.min.js
--rw-r--r--  2.0 unx     1630 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/pagebreak/plugin.min.js
--rw-r--r--  2.0 unx    22574 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/paste/plugin.min.js
--rw-r--r--  2.0 unx     2096 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/preview/plugin.min.js
--rw-r--r--  2.0 unx      808 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/print/plugin.min.js
--rw-r--r--  2.0 unx     6058 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/quickbars/plugin.min.js
--rw-r--r--  2.0 unx     1716 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/save/plugin.min.js
--rw-r--r--  2.0 unx    14605 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/searchreplace/plugin.min.js
--rw-r--r--  2.0 unx     9786 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/spellchecker/plugin.min.js
--rw-r--r--  2.0 unx     1858 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/tabfocus/plugin.min.js
--rw-r--r--  2.0 unx   143478 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/table/plugin.min.js
--rw-r--r--  2.0 unx     8249 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/template/plugin.min.js
--rw-r--r--  2.0 unx      395 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/textcolor/plugin.min.js
--rw-r--r--  2.0 unx    17613 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/textpattern/plugin.min.js
--rw-r--r--  2.0 unx     3282 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/toc/plugin.min.js
--rw-r--r--  2.0 unx     1380 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/visualblocks/plugin.min.js
--rw-r--r--  2.0 unx     5776 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/visualchars/plugin.min.js
--rw-r--r--  2.0 unx    12105 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/plugins/wordcount/plugin.min.js
--rw-r--r--  2.0 unx     1469 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/content/dark/content.min.css
--rw-r--r--  2.0 unx     1399 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/content/default/content.min.css
--rw-r--r--  2.0 unx     1498 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/content/document/content.min.css
--rw-r--r--  2.0 unx     1420 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/content/writer/content.min.css
--rw-r--r--  2.0 unx    21775 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/ui/oxide/content.inline.min.css
--rw-r--r--  2.0 unx    21834 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/ui/oxide/content.min.css
--rw-r--r--  2.0 unx      544 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/ui/oxide/content.mobile.min.css
--rw-r--r--  2.0 unx     4624 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/ui/oxide/fonts/tinymce-mobile.woff
--rw-r--r--  2.0 unx    61537 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/ui/oxide/skin.min.css
--rw-r--r--  2.0 unx    21004 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/ui/oxide/skin.mobile.min.css
--rw-r--r--  2.0 unx      783 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/ui/oxide/skin.shadowdom.min.css
--rw-r--r--  2.0 unx    21775 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/ui/oxide-dark/content.inline.min.css
--rw-r--r--  2.0 unx    21451 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/ui/oxide-dark/content.min.css
--rw-r--r--  2.0 unx      544 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/ui/oxide-dark/content.mobile.min.css
--rw-r--r--  2.0 unx     4624 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/ui/oxide-dark/fonts/tinymce-mobile.woff
--rw-r--r--  2.0 unx    61424 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/ui/oxide-dark/skin.min.css
--rw-r--r--  2.0 unx    21004 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/ui/oxide-dark/skin.mobile.min.css
--rw-r--r--  2.0 unx      783 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/skins/ui/oxide-dark/skin.shadowdom.min.css
--rw-r--r--  2.0 unx   159748 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/themes/mobile/theme.min.js
--rw-r--r--  2.0 unx   423637 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/themes/silver/theme.min.js
--rw-r--r--  2.0 unx   392236 b- defN 80-Jan-01 00:00 django_bpp/staticroot/tinymce/tinymce.min.js
--rw-r--r--  2.0 unx    18931 b- defN 80-Jan-01 00:00 django_bpp/staticroot/vendor/select2/dist/css/select2.css
--rw-r--r--  2.0 unx    16264 b- defN 80-Jan-01 00:00 django_bpp/staticroot/vendor/select2/dist/css/select2.min.css
--rw-r--r--  2.0 unx    14811 b- defN 80-Jan-01 00:00 django_bpp/staticroot/what-input/dist/what-input.js
 -rw-r--r--  2.0 unx    11316 b- defN 80-Jan-01 00:00 django_bpp/templates/admin/base.html
 -rw-r--r--  2.0 unx     3246 b- defN 80-Jan-01 00:00 django_bpp/templates/admin/base_site.html
 -rw-r--r--  2.0 unx      245 b- defN 80-Jan-01 00:00 django_bpp/templates/admin/bpp/autor/change_form.html
 -rw-r--r--  2.0 unx      642 b- defN 80-Jan-01 00:00 django_bpp/templates/admin/bpp/bppuser/change_form.html
 -rw-r--r--  2.0 unx     2062 b- defN 80-Jan-01 00:00 django_bpp/templates/admin/bpp/patent/change_form.html
 -rw-r--r--  2.0 unx      283 b- defN 80-Jan-01 00:00 django_bpp/templates/admin/bpp/szablondlaopisubibliograficznego/change_form.html
 -rw-r--r--  2.0 unx      653 b- defN 80-Jan-01 00:00 django_bpp/templates/admin/bpp/wydawca/change_form.html
@@ -1893,17 +861,17 @@
 -rw-r--r--  2.0 unx     2501 b- defN 80-Jan-01 00:00 django_bpp/templates/admin/liczba_cytowan_button_handler.html
 -rw-r--r--  2.0 unx     2930 b- defN 80-Jan-01 00:00 django_bpp/templates/admin/pubmed_id_button_handler.html
 -rw-r--r--  2.0 unx     2219 b- defN 80-Jan-01 00:00 django_bpp/templates/admin/strona_tom_nr_zeszytu_button_handler.html
 -rw-r--r--  2.0 unx     1398 b- defN 80-Jan-01 00:00 django_bpp/templates/admin/submit_line.html
 -rw-r--r--  2.0 unx     1679 b- defN 80-Jan-01 00:00 django_bpp/templates/admin/uzupelnij_rok_wydawnictwo_ciagle_button_handler.html
 -rw-r--r--  2.0 unx     1803 b- defN 80-Jan-01 00:00 django_bpp/templates/admin/uzupelnij_rok_wydawnictwo_zwarte_button_handler.html
 -rw-r--r--  2.0 unx      429 b- defN 80-Jan-01 00:00 django_bpp/templates/adminsortable2/change_list.html
--rw-r--r--  2.0 unx     5384 b- defN 80-Jan-01 00:00 django_bpp/templates/bare.html
+-rw-r--r--  2.0 unx     5750 b- defN 80-Jan-01 00:00 django_bpp/templates/bare.html
 -rw-r--r--  2.0 unx     6425 b- defN 80-Jan-01 00:00 django_bpp/templates/base.html
--rw-r--r--  2.0 unx     1559 b- defN 80-Jan-01 00:00 django_bpp/templates/base_footer.html
+-rw-r--r--  2.0 unx     1943 b- defN 80-Jan-01 00:00 django_bpp/templates/base_footer.html
 -rw-r--r--  2.0 unx      519 b- defN 80-Jan-01 00:00 django_bpp/templates/cookielaw/rejectable.html
 -rw-r--r--  2.0 unx      282 b- defN 80-Jan-01 00:00 django_bpp/templates/error.html
 -rw-r--r--  2.0 unx      293 b- defN 80-Jan-01 00:00 django_bpp/templates/google_analytics.html
 -rw-r--r--  2.0 unx      315 b- defN 80-Jan-01 00:00 django_bpp/templates/info.html
 -rw-r--r--  2.0 unx      217 b- defN 80-Jan-01 00:00 django_bpp/templates/make-jquery-ui.html
 -rw-r--r--  2.0 unx      296 b- defN 80-Jan-01 00:00 django_bpp/templates/microsoft/admin_login.html
 -rw-r--r--  2.0 unx    10609 b- defN 80-Jan-01 00:00 django_bpp/templates/multiseek/common-results.html
@@ -2184,15 +1152,15 @@
 -rw-r--r--  2.0 unx      608 b- defN 80-Jan-01 00:00 pbn_api/admin/tlumacz_dyscyplin.py
 -rw-r--r--  2.0 unx      724 b- defN 80-Jan-01 00:00 pbn_api/admin/widgets.py
 -rw-r--r--  2.0 unx      117 b- defN 80-Jan-01 00:00 pbn_api/apps.py
 -rw-r--r--  2.0 unx    31322 b- defN 80-Jan-01 00:00 pbn_api/client.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 pbn_api/conf/__init__.py
 -rw-r--r--  2.0 unx      572 b- defN 80-Jan-01 00:00 pbn_api/conf/settings.py
 -rw-r--r--  2.0 unx      836 b- defN 80-Jan-01 00:00 pbn_api/const.py
--rw-r--r--  2.0 unx     1559 b- defN 80-Jan-01 00:00 pbn_api/exceptions.py
+-rw-r--r--  2.0 unx     1662 b- defN 80-Jan-01 00:00 pbn_api/exceptions.py
 -rw-r--r--  2.0 unx    50130 b- defN 80-Jan-01 00:00 pbn_api/integrator/__init__.py
 -rw-r--r--  2.0 unx      606 b- defN 80-Jan-01 00:00 pbn_api/integrator/istarmap.py
 -rw-r--r--  2.0 unx     1722 b- defN 80-Jan-01 00:00 pbn_api/integrator/odswiez_tabele_publikacji.py
 -rw-r--r--  2.0 unx     1413 b- defN 80-Jan-01 00:00 pbn_api/integrator/pobierz_skasowane_prace.py
 -rw-r--r--  2.0 unx     1984 b- defN 80-Jan-01 00:00 pbn_api/integrator/threaded_page_getter.py
 -rw-r--r--  2.0 unx       26 b- defN 80-Jan-01 00:00 pbn_api/management/__init__.py
 -rw-r--r--  2.0 unx       26 b- defN 80-Jan-01 00:00 pbn_api/management/commands/__init__.py
@@ -2428,13 +1396,13 @@
 -rw-r--r--  2.0 unx      427 b- defN 80-Jan-01 00:00 zglos_publikacje/templates/templated_email/nowe_zgloszenie.email
 -rw-r--r--  2.0 unx      518 b- defN 80-Jan-01 00:00 zglos_publikacje/templates/templated_email/zwroc_zgloszenie.email
 -rw-r--r--  2.0 unx      508 b- defN 80-Jan-01 00:00 zglos_publikacje/templates/zglos_publikacje/sukces.html
 -rw-r--r--  2.0 unx     4214 b- defN 80-Jan-01 00:00 zglos_publikacje/templates/zglos_publikacje/zgloszenie_publikacji_form.html
 -rw-r--r--  2.0 unx      399 b- defN 80-Jan-01 00:00 zglos_publikacje/urls.py
 -rw-r--r--  2.0 unx      390 b- defN 80-Jan-01 00:00 zglos_publikacje/validators.py
 -rw-r--r--  2.0 unx    10771 b- defN 80-Jan-01 00:00 zglos_publikacje/views.py
--rw-r--r--  2.0 unx     7013 b- defN 80-Jan-01 00:00 bpp_iplweb-202405.1125.dist-info/LICENSE
--rw-r--r--  2.0 unx     4302 b- defN 80-Jan-01 00:00 bpp_iplweb-202405.1125.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 bpp_iplweb-202405.1125.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 80-Jan-01 00:00 bpp_iplweb-202405.1125.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx   261030 b- defN 16-Jan-01 00:00 bpp_iplweb-202405.1125.dist-info/RECORD
-2438 files, 20660275 bytes uncompressed, 6489197 bytes compressed:  68.6%
+-rw-r--r--  2.0 unx     7013 b- defN 80-Jan-01 00:00 bpp_iplweb-202405.1126.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4302 b- defN 80-Jan-01 00:00 bpp_iplweb-202405.1126.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 bpp_iplweb-202405.1126.dist-info/WHEEL
+-rw-r--r--  2.0 unx       71 b- defN 80-Jan-01 00:00 bpp_iplweb-202405.1126.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx   135228 b- defN 16-Jan-01 00:00 bpp_iplweb-202405.1126.dist-info/RECORD
+1406 files, 4235931 bytes uncompressed, 1594056 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -1734,14 +1734,17 @@
 
 Filename: bpp/migrations/0345_alter_wydzial_opis.py
 Comment: 
 
 Filename: bpp/migrations/0346_rename_multiseek_searchform_data.py
 Comment: 
 
+Filename: bpp/migrations/0347_uczelnia_deklaracja_dostepnosci_tekst_and_more.py
+Comment: 
+
 Filename: bpp/migrations/107_bpp_autorzy.sql
 Comment: 
 
 Filename: bpp/migrations/107_bpp_rekord.sql
 Comment: 
 
 Filename: bpp/migrations/107_cache_functions.sql
@@ -2115,14 +2118,17 @@
 
 Filename: bpp/templates/browse/autorzy.html
 Comment: 
 
 Filename: bpp/templates/browse/brak_uczelni.html
 Comment: 
 
+Filename: bpp/templates/browse/deklaracja_dostepnosci.html
+Comment: 
+
 Filename: bpp/templates/browse/edit_if_logged_in.html
 Comment: 
 
 Filename: bpp/templates/browse/go_to_admin_change.html
 Comment: 
 
 Filename: bpp/templates/browse/go_to_admin_list.html
@@ -2493,3116 +2499,14 @@
 
 Filename: django_bpp/settings/test.py
 Comment: 
 
 Filename: django_bpp/sitemaps.py
 Comment: 
 
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.096f10c22368.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.0a872877d6e5.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.190bf892d4f4.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.1932d9721a27.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.1f790078cf5c.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.29cc8c364a3e.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.356143e41027.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.379c10a9e812.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.5696a0d0f1f1.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.6a3cdad0db8d.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.7f5b59a472ba.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.89fd28600aa6.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.8b11ced9338f.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.a810a58e3985.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.b27842844e9e.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.c55ee1d1f071.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.c8c84bffe354.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.c910af7b7054.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.cecc011ac0ed.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.f0f7cd65549e.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/css/output.f9aaec1db0e7.css
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.007d0f8196ce.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.023974546012.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.05c3452b5333.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.1b90b4fd0996.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.1c85775ddde0.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.343f6adb2a24.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.42e671c2a38d.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.5d38125bd1ad.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.5ec89beef9ad.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.68e3dd089325.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.8d16d119404e.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.8dd042ba56b5.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.8ee655cf393b.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.96a46be1e5ad.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.ab5d51d1c156.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.ad88da53bae4.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.b42d7758508b.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.b4ba48ed4f66.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.b7aa83a7edd6.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.c86114addc24.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.cd1656272d36.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.e01ae35807c6.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.e40a6a191db5.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.ec76e5be931e.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.f44161ebe543.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.f6d7b57c1be4.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/js/output.f8daedf655e8.js
-Comment: 
-
-Filename: django_bpp/staticroot/CACHE-202405.1125/manifest.json
-Comment: 
-
-Filename: django_bpp/staticroot/admin/css/autocomplete.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin/css/base.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin/css/changelists.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin/css/dark_mode.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin/css/dashboard.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin/css/forms.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin/css/login.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin/css/nav_sidebar.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin/css/responsive.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin/css/responsive_rtl.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin/css/rtl.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin/css/vendor/select2/select2.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin/css/vendor/select2/select2.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin/css/widgets.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/calendar-icons.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/gis/move_vertex_off.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/gis/move_vertex_on.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/icon-addlink.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/icon-alert.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/icon-calendar.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/icon-changelink.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/icon-clock.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/icon-deletelink.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/icon-no.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/icon-unknown-alt.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/icon-unknown.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/icon-viewlink.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/icon-yes.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/inline-delete.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/search.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/selector-icons.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/sorting-icons.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/tooltag-add.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/img/tooltag-arrowright.svg
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/SelectBox.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/SelectFilter2.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/actions.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/admin/DateTimeShortcuts.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/admin/RelatedObjectLookups.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/autocomplete.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/calendar.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/cancel.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/change_form.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/collapse.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/core.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/filters.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/inlines.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/jquery.init.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/nav_sidebar.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/popup_response.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/prepopulate.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/prepopulate_init.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/theme.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/urlify.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/jquery/jquery.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/jquery/jquery.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/af.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/ar.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/az.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/bg.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/bn.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/bs.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/ca.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/cs.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/da.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/de.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/dsb.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/el.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/en.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/es.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/et.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/eu.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/fa.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/fi.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/fr.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/gl.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/he.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/hi.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/hr.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/hsb.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/hu.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/hy.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/id.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/is.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/it.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/ja.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/ka.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/km.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/ko.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/lt.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/lv.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/mk.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/ms.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/nb.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/ne.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/nl.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/pl.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/ps.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/pt-BR.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/pt.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/ro.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/ru.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/sk.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/sl.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/sq.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/sr-Cyrl.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/sr.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/sv.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/th.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/tk.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/tr.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/uk.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/vi.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/zh-CN.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/i18n/zh-TW.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/select2.full.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/select2/select2.full.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/xregexp/xregexp.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin/js/vendor/xregexp/xregexp.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/dashboard-ie.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/dashboard.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/jquery/images/animated-overlay.gif
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/jquery/images/ui-bg_flat_0_aaaaaa_40x100.png
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/jquery/images/ui-bg_flat_75_ffffff_40x100.png
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/jquery/images/ui-bg_glass_55_fbf9ee_1x400.png
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/jquery/images/ui-bg_glass_65_ffffff_1x400.png
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/jquery/images/ui-bg_glass_75_dadada_1x400.png
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/jquery/images/ui-bg_glass_75_e6e6e6_1x400.png
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/jquery/images/ui-bg_glass_95_fef1ec_1x400.png
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/jquery/images/ui-bg_highlight-soft_75_cccccc_1x100.png
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/jquery/images/ui-icons_222222_256x240.png
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/jquery/images/ui-icons_2e83ff_256x240.png
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/jquery/images/ui-icons_454545_256x240.png
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/jquery/images/ui-icons_888888_256x240.png
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/jquery/images/ui-icons_cd0a0a_256x240.png
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/jquery/jquery-ui.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/menu-ie.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/menu.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/css/theming.css
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/images/admin-tools.png
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/images/django.png
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/js/dashboard.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/js/jquery/jquery-ui.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/js/jquery/jquery.cookie.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/js/jquery/jquery.dashboard.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/js/jquery/jquery.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/js/json.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/js/menu.js
-Comment: 
-
-Filename: django_bpp/staticroot/admin_tools/js/utils.js
-Comment: 
-
-Filename: django_bpp/staticroot/adminsortable2/css/sortable.css
-Comment: 
-
-Filename: django_bpp/staticroot/adminsortable2/icons/drag.png
-Comment: 
-
-Filename: django_bpp/staticroot/adminsortable2/js/adminsortable2.js
-Comment: 
-
-Filename: django_bpp/staticroot/adminsortable2/js/adminsortable2.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/adminsortable2/js/list-sortable.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/autocomplete_light.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/autocomplete_light.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/af.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/ar.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/az.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/bg.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/bn.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/bs.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/ca.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/cs.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/da.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/de.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/dsb.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/el.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/en.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/eo.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/es.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/et.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/eu.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/fa.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/fi.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/fr.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/gl.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/he.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/hi.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/hr.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/hsb.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/hu.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/hy.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/id.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/is.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/it.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/ja.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/ka.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/km.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/ko.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/lt.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/lv.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/mk.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/ms.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/nb.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/ne.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/nl.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/pa.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/pl.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/ps.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/pt-BR.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/pt.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/ro.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/ru.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/sk.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/sl.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/sq.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/sr-Cyrl.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/sr.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/sv.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/te.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/th.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/tk.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/tr.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/uk.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/vi.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/zh-CN.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/i18n/zh-TW.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/select2.css
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/select2.js
-Comment: 
-
-Filename: django_bpp/staticroot/autocomplete_light/select2.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/css/admin-menu.css
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/css/admin-style.css
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/css/fix-djangoql-css-for-grappelli.css
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/images/animated-overlay.gif
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/images/ui-bg_flat_0_aaaaaa_40x100.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/images/ui-bg_flat_0_eeeeee_40x100.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/images/ui-bg_flat_55_ffffff_40x100.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/images/ui-bg_flat_75_ffffff_40x100.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/images/ui-bg_glass_65_ffffff_1x400.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/images/ui-bg_highlight-soft_100_f6f6f6_1x100.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/images/ui-bg_highlight-soft_25_0073ea_1x100.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/images/ui-bg_highlight-soft_50_dddddd_1x100.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/images/ui-icons_0073ea_256x240.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/images/ui-icons_454545_256x240.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/images/ui-icons_666666_256x240.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/images/ui-icons_ff0084_256x240.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/images/ui-icons_ffffff_256x240.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/jquery-ui.css
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/jquery-ui.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/flick/theme.css
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/images/giphy.gif
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/images/lite-blue-check.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/images/lite-green-check.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/images/lite-red-check.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/images/logo.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/images/logo_bpp.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/images/no-check.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/images/printer.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/images/star_white.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/images/star_yellow.png
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/images/test_server_background.jpg
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/js/Polish.json
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/js/autorform_dependant.js
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/js/bpp.js
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/svg/autor.svg
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/svg/cache.svg
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/svg/database.svg
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/svg/jednostka.svg
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/svg/paper.svg
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/svg/patent.svg
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/svg/pencil.svg
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/svg/praca_doktorska.svg
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/svg/praca_habilitacyjna.svg
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/svg/user.svg
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/svg/wydawnictwo_ciagle.svg
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/svg/wydawnictwo_zwarte.svg
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/svg/zrodlo.svg
-Comment: 
-
-Filename: django_bpp/staticroot/bpp/wav/alert.wav
-Comment: 
-
-Filename: django_bpp/staticroot/close-alerts.js
-Comment: 
-
-Filename: django_bpp/staticroot/cookielaw/css/cookielaw.css
-Comment: 
-
-Filename: django_bpp/staticroot/cookielaw/img/close.png
-Comment: 
-
-Filename: django_bpp/staticroot/cookielaw/js/cookielaw.js
-Comment: 
-
-Filename: django_bpp/staticroot/css/columns.css
-Comment: 
-
-Filename: django_bpp/staticroot/css/flexible_reports.css
-Comment: 
-
-Filename: django_bpp/staticroot/datatables.net/js/jquery.dataTables.js
-Comment: 
-
-Filename: django_bpp/staticroot/datatables.net-zf/css/dataTables.foundation.css
-Comment: 
-
-Filename: django_bpp/staticroot/datatables.net-zf/js/dataTables.foundation.js
-Comment: 
-
-Filename: django_bpp/staticroot/dbtemplates/css/django.css
-Comment: 
-
-Filename: django_bpp/staticroot/dbtemplates/css/editor.css
-Comment: 
-
-Filename: django_bpp/staticroot/dbtemplates/js/codemirror.js
-Comment: 
-
-Filename: django_bpp/staticroot/dbtemplates/js/editor.js
-Comment: 
-
-Filename: django_bpp/staticroot/dbtemplates/js/highlight.js
-Comment: 
-
-Filename: django_bpp/staticroot/dbtemplates/js/mirrorframe.js
-Comment: 
-
-Filename: django_bpp/staticroot/dbtemplates/js/parsedjango.js
-Comment: 
-
-Filename: django_bpp/staticroot/dbtemplates/js/select.js
-Comment: 
-
-Filename: django_bpp/staticroot/dbtemplates/js/stringstream.js
-Comment: 
-
-Filename: django_bpp/staticroot/dbtemplates/js/tokenize.js
-Comment: 
-
-Filename: django_bpp/staticroot/dbtemplates/js/undo.js
-Comment: 
-
-Filename: django_bpp/staticroot/dbtemplates/js/util.js
-Comment: 
-
-Filename: django_bpp/staticroot/django_extensions/css/jquery.autocomplete.css
-Comment: 
-
-Filename: django_bpp/staticroot/django_extensions/img/indicator.gif
-Comment: 
-
-Filename: django_bpp/staticroot/django_extensions/js/jquery.ajaxQueue.js
-Comment: 
-
-Filename: django_bpp/staticroot/django_extensions/js/jquery.autocomplete.js
-Comment: 
-
-Filename: django_bpp/staticroot/django_extensions/js/jquery.bgiframe.js
-Comment: 
-
-Filename: django_bpp/staticroot/django_tables2/bootstrap.css
-Comment: 
-
-Filename: django_bpp/staticroot/django_tables2/themes/paleblue/css/screen.css
-Comment: 
-
-Filename: django_bpp/staticroot/django_tables2/themes/paleblue/img/arrow-active-down.png
-Comment: 
-
-Filename: django_bpp/staticroot/django_tables2/themes/paleblue/img/arrow-active-up.png
-Comment: 
-
-Filename: django_bpp/staticroot/django_tables2/themes/paleblue/img/arrow-inactive-down.png
-Comment: 
-
-Filename: django_bpp/staticroot/django_tables2/themes/paleblue/img/arrow-inactive-up.png
-Comment: 
-
-Filename: django_bpp/staticroot/django_tables2/themes/paleblue/img/false.gif
-Comment: 
-
-Filename: django_bpp/staticroot/django_tables2/themes/paleblue/img/header-bg.png
-Comment: 
-
-Filename: django_bpp/staticroot/django_tables2/themes/paleblue/img/missing.png
-Comment: 
-
-Filename: django_bpp/staticroot/django_tables2/themes/paleblue/img/pagination-bg.gif
-Comment: 
-
-Filename: django_bpp/staticroot/django_tables2/themes/paleblue/img/true.gif
-Comment: 
-
-Filename: django_bpp/staticroot/django_tinymce/init_tinymce.js
-Comment: 
-
-Filename: django_bpp/staticroot/djangoql/css/completion.css
-Comment: 
-
-Filename: django_bpp/staticroot/djangoql/css/completion.css.map
-Comment: 
-
-Filename: django_bpp/staticroot/djangoql/css/completion_admin.css
-Comment: 
-
-Filename: django_bpp/staticroot/djangoql/css/syntax_help.css
-Comment: 
-
-Filename: django_bpp/staticroot/djangoql/img/completion_example.png
-Comment: 
-
-Filename: django_bpp/staticroot/djangoql/img/completion_example_scaled.png
-Comment: 
-
-Filename: django_bpp/staticroot/djangoql/js/completion.js
-Comment: 
-
-Filename: django_bpp/staticroot/djangoql/js/completion.js.map
-Comment: 
-
-Filename: django_bpp/staticroot/djangoql/js/completion_admin.js
-Comment: 
-
-Filename: django_bpp/staticroot/djangoql/js/completion_admin_toggle.js
-Comment: 
-
-Filename: django_bpp/staticroot/djangoql/js/completion_admin_toggle_off.js
-Comment: 
-
-Filename: django_bpp/staticroot/ewaluacja2021/xlsx/default.xlsx
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/css/foundation-datepicker.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/foundation-icons.css
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/foundation-icons.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/foundation-icons.ttf
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/foundation-icons.woff
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-address-book.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-alert.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-align-center.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-align-justify.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-align-left.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-align-right.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-anchor.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-annotate.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-archive.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-arrow-down.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-arrow-left.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-arrow-right.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-arrow-up.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-arrows-compress.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-arrows-expand.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-arrows-in.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-arrows-out.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-asl.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-asterisk.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-at-sign.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-background-color.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-battery-empty.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-battery-full.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-battery-half.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-bitcoin-circle.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-bitcoin.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-blind.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-bluetooth.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-bold.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-book-bookmark.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-book.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-bookmark.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-braille.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-burst-new.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-burst-sale.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-burst.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-calendar.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-camera.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-check.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-checkbox.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-clipboard-notes.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-clipboard-pencil.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-clipboard.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-clock.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-closed-caption.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-cloud.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-comment-minus.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-comment-quotes.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-comment-video.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-comment.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-comments.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-compass.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-contrast.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-credit-card.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-crop.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-crown.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-css3.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-database.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-die-five.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-die-four.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-die-one.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-die-six.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-die-three.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-die-two.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-dislike.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-dollar-bill.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-dollar.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-download.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-eject.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-elevator.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-euro.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-eye.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-fast-forward.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-female-symbol.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-female.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-filter.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-first-aid.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-flag.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-folder-add.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-folder-lock.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-folder.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-foot.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-foundation.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-graph-bar.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-graph-horizontal.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-graph-pie.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-graph-trend.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-guide-dog.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-hearing-aid.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-heart.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-home.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-html5.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-indent-less.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-indent-more.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-info.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-italic.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-key.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-laptop.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-layout.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-lightbulb.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-like.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-link.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-list-bullet.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-list-number.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-list-thumbnails.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-list.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-lock.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-loop.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-magnifying-glass.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-mail.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-male-female.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-male-symbol.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-male.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-map.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-marker.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-megaphone.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-microphone.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-minus-circle.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-minus.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-mobile-signal.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-mobile.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-monitor.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-mountains.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-music.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-next.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-no-dogs.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-no-smoking.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-add.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-copy.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-csv.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-delete.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-doc.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-edit.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-export-csv.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-export-doc.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-export-pdf.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-export.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-filled.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-multiple.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-pdf.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-remove.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page-search.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-page.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-paint-bucket.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-paperclip.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-pause.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-paw.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-paypal.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-pencil.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-photo.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-play-circle.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-play-video.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-play.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-plus.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-pound.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-power.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-previous.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-price-tag.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-pricetag-multiple.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-print.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-prohibited.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-projection-screen.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-puzzle.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-quote.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-record.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-refresh.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-results-demographics.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-results.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-rewind-ten.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-rewind.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-rss.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-safety-cone.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-save.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-share.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-sheriff-badge.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-shield.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-shopping-bag.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-shopping-cart.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-shuffle.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-skull.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-500px.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-adobe.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-amazon.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-android.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-apple.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-behance.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-bing.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-blogger.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-delicious.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-designer-news.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-deviant-art.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-digg.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-dribbble.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-drive.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-dropbox.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-evernote.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-facebook.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-flickr.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-forrst.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-foursquare.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-game-center.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-github.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-google-plus.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-hacker-news.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-hi5.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-instagram.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-joomla.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-lastfm.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-linkedin.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-medium.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-myspace.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-orkut.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-path.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-picasa.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-pinterest.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-rdio.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-reddit.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-skillshare.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-skype.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-smashing-mag.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-snapchat.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-spotify.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-squidoo.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-stack-overflow.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-steam.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-stumbleupon.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-treehouse.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-tumblr.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-twitter.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-vimeo.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-windows.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-xbox.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-yahoo.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-yelp.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-youtube.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-zerply.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-social-zurb.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-sound.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-star.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-stop.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-strikethrough.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-subscript.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-superscript.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-tablet-landscape.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-tablet-portrait.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-target-two.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-target.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-telephone-accessible.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-telephone.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-text-color.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-thumbnails.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-ticket.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-torso-business.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-torso-female.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-torso.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-torsos-all-female.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-torsos-all.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-torsos-female-male.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-torsos-male-female.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-torsos.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-trash.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-trees.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-trophy.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-underline.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-universal-access.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-unlink.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-unlock.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-upload-cloud.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-upload.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-usb.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-video.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-volume-none.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-volume-strike.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-volume.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-web.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-wheelchair.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-widget.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-wrench.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-x-circle.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-x.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-yen.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-zoom-in.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/foundation/fonts/svgs/fi-zoom-out.svg
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/js/foundation-datepicker.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-datepicker/js/locales/foundation-datepicker.pl.js
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-sites/dist/css/foundation.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-sites/dist/js/foundation.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/foundation-sites/dist/js/foundation.min.js.map
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/backgrounds/changelist-results.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/backgrounds/loading-small.gif
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/backgrounds/messagelist.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/backgrounds/nav-grabber.gif
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/backgrounds/ui-sortable-placeholder.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/add-another.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/add-another_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/back-link-rtl.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/back-link-rtl_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/back-link.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/back-link_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/breadcrumbs-rtl.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/breadcrumbs-rtl_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/breadcrumbs.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/breadcrumbs_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/date-hierarchy-back-rtl.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/date-hierarchy-back-rtl_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/date-hierarchy-back.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/date-hierarchy-back_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/datepicker.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/datepicker_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/datetime-now.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/datetime-now_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/form-select.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/link-internal-rtl.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/link-internal-rtl_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/object-tools-add-link.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/object-tools-viewsite-link.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/pulldown-handler.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/pulldown-handler_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/pulldown-handler_selected.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/related-lookup-m2m.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/related-lookup-m2m_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/related-lookup.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/related-lookup_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/related-remove.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/related-remove_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/searchbox.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/selector-add-m2m-horizontal.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/selector-add-m2m-horizontal_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/selector-add-m2m-vertical.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/selector-add-m2m-vertical_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/selector-filter.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/selector-remove-m2m-horizontal.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/selector-remove-m2m-horizontal_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/selector-remove-m2m-vertical.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/selector-remove-m2m-vertical_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/sort-remove.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/sort-remove_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/sorted-ascending.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/sorted-descending.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/status-no.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/status-unknown.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/status-yes.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/th-ascending.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/th-descending.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/timepicker.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/timepicker_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-add-handler.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-add-handler_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-arrow-down-handler.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-arrow-down-handler_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-arrow-up-handler.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-arrow-up-handler_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-close-handler.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-close-handler_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-delete-handler-predelete.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-delete-handler.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-delete-handler_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-drag-handler.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-drag-handler_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-edit-handler.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-edit-handler_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-open-handler.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-open-handler_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-remove-handler.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-remove-handler_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-trash-handler.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-trash-handler_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-trash-list-toggle-handler.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-trash-list-toggle-handler_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-viewsite-link.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/tools-viewsite-link_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/ui-datepicker-next.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/ui-datepicker-next_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/ui-datepicker-prev.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons/ui-datepicker-prev_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-s79f97b581c.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/add-link.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/add-link_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/autocomplete-multiple.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/autocomplete-single.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/change-link.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/change-link_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/delete-link.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/filter-choice-selected.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/link-external-rtl.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/link-external-rtl_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/link-external.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/link-external_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/link-internal-rtl.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/link-internal-rtl_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/link-internal.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/link-internal_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/sort-remove.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/tools-related-add-handler-disabled.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/tools-related-add-handler.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/tools-related-add-handler_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/tools-related-edit-handler-disabled.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/tools-related-edit-handler.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/tools-related-edit-handler_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/tools-related-remove-handler-disabled.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/tools-related-remove-handler.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small/tools-related-remove-handler_hover.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/images/icons-small-sc29b5b842f.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/img/admin/arrow-down.gif
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/img/admin/arrow-up.gif
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/i18n/ui.datepicker-pl.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/jquery-migrate-3.0.1.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/jquery-migrate-3.0.1.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/jquery.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/jquery.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/ui/external/jquery/jquery.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/ui/images/ui-icons_444444_256x240.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/ui/images/ui-icons_555555_256x240.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/ui/images/ui-icons_777620_256x240.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/ui/images/ui-icons_777777_256x240.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/ui/images/ui-icons_cc0000_256x240.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/ui/images/ui-icons_ffffff_256x240.png
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/ui/index.html
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/ui/jquery-ui.css
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/ui/jquery-ui.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/ui/jquery-ui.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/ui/jquery-ui.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/ui/jquery-ui.structure.css
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/ui/jquery-ui.structure.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/ui/jquery-ui.theme.css
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/jquery/ui/jquery-ui.theme.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/js/grappelli.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/js/grappelli.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/js/jquery.grp_autocomplete_fk.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/js/jquery.grp_autocomplete_generic.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/js/jquery.grp_autocomplete_m2m.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/js/jquery.grp_collapsible.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/js/jquery.grp_collapsible_group.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/js/jquery.grp_inline.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/js/jquery.grp_related_fk.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/js/jquery.grp_related_generic.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/js/jquery.grp_related_m2m.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/js/jquery.grp_timepicker.js
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/stylesheets/mueller/grid/output-rtl.css
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/stylesheets/mueller/grid/output.css
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/stylesheets/mueller/screen.css
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/stylesheets/partials/custom/tinymce.css
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/stylesheets/rtl.css
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/stylesheets/screen.css
-Comment: 
-
-Filename: django_bpp/staticroot/grappelli/tinymce_setup/tinymce_setup.js
-Comment: 
-
-Filename: django_bpp/staticroot/import_dyscyplin/xlsx/default.xlsx
-Comment: 
-
-Filename: django_bpp/staticroot/import_export/action_formats.js
-Comment: 
-
-Filename: django_bpp/staticroot/import_export/guess_format.js
-Comment: 
-
-Filename: django_bpp/staticroot/import_export/import.css
-Comment: 
-
-Filename: django_bpp/staticroot/import_list_if/import_list_if_przyklad.xlsx
-Comment: 
-
-Filename: django_bpp/staticroot/import_pracownikow/import_pracownikow_przyklad.xlsx
-Comment: 
-
-Filename: django_bpp/staticroot/jinplace/js/jinplace.js
-Comment: 
-
-Filename: django_bpp/staticroot/jquery/dist/jquery.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/jquery.cookie/jquery.cookie.js
-Comment: 
-
-Filename: django_bpp/staticroot/jqueryui/jquery-ui.css
-Comment: 
-
-Filename: django_bpp/staticroot/jqueryui/jquery-ui.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/js/columns.js
-Comment: 
-
-Filename: django_bpp/staticroot/js/crispy_forms_foundation/plugins.js
-Comment: 
-
-Filename: django_bpp/staticroot/js/flexible_reports.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/css/jquery.keypad.alt.css
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/css/jquery.keypad.css
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/img/keypad.png
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/index.html
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-ca.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-cs.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-de.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-es.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-fr.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-hu.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-it.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-nl.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-no.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-pl.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-pt-BR.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-sk.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad-tr.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.keypad.min.map
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.plugin.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/kbw-keypad/dist/js/jquery.plugin.min.map
-Comment: 
-
-Filename: django_bpp/staticroot/mptt/arrow-move-black.png
-Comment: 
-
-Filename: django_bpp/staticroot/mptt/arrow-move-white.png
-Comment: 
-
-Filename: django_bpp/staticroot/mptt/arrow-move.png
-Comment: 
-
-Filename: django_bpp/staticroot/mptt/disclosure-down-black.png
-Comment: 
-
-Filename: django_bpp/staticroot/mptt/disclosure-down-white.png
-Comment: 
-
-Filename: django_bpp/staticroot/mptt/disclosure-down.png
-Comment: 
-
-Filename: django_bpp/staticroot/mptt/disclosure-right-black.png
-Comment: 
-
-Filename: django_bpp/staticroot/mptt/disclosure-right-white.png
-Comment: 
-
-Filename: django_bpp/staticroot/mptt/disclosure-right.png
-Comment: 
-
-Filename: django_bpp/staticroot/mptt/draggable-admin.css
-Comment: 
-
-Filename: django_bpp/staticroot/mptt/draggable-admin.js
-Comment: 
-
-Filename: django_bpp/staticroot/multiseek/css/style.css
-Comment: 
-
-Filename: django_bpp/staticroot/multiseek/js/multiseek.js
-Comment: 
-
-Filename: django_bpp/staticroot/notifications/js/mustache.js
-Comment: 
-
-Filename: django_bpp/staticroot/notifications/js/notifications.js
-Comment: 
-
-Filename: src/django_bpp/staticroot/notifications/js/tests/index.html
-Comment: 
-
-Filename: src/django_bpp/staticroot/notifications/js/tests/tests.js
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/css/bootstrap-theme.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/css/bootstrap-theme.min.css.map
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/css/bootstrap-tweaks.css
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/css/bootstrap.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/css/bootstrap.min.css.map
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/css/default.css
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/css/font-awesome-4.0.3.css
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/css/prettify.css
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/fonts/fontawesome-webfont.svg
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/fonts/fontawesome-webfont.ttf
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/fonts/fontawesome-webfont.woff
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/fonts/glyphicons-halflings-regular.svg
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/fonts/glyphicons-halflings-regular.ttf
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/fonts/glyphicons-halflings-regular.woff
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/fonts/glyphicons-halflings-regular.woff2
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/img/glyphicons-halflings-white.png
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/img/glyphicons-halflings.png
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/img/grid.png
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/js/ajax-form.js
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/js/bootstrap.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/js/coreapi-0.1.1.js
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/js/csrf.js
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/js/default.js
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/js/jquery-3.5.1.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/rest_framework/js/prettify-min.js
-Comment: 
-
-Filename: django_bpp/staticroot/scss/app-blue.css
-Comment: 
-
-Filename: django_bpp/staticroot/scss/app-green.css
-Comment: 
-
-Filename: django_bpp/staticroot/scss/app-orange.css
-Comment: 
-
-Filename: django_bpp/staticroot/select2/dist/css/select2.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/select2/dist/js/i18n/pl.js
-Comment: 
-
-Filename: django_bpp/staticroot/select2/dist/js/select2.full.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/select2-foundation_theme/dist/select2-foundation-theme.css
-Comment: 
-
-Filename: django_bpp/staticroot/session_security/script.js
-Comment: 
-
-Filename: django_bpp/staticroot/session_security/style.css
-Comment: 
-
-Filename: django_bpp/staticroot/tabular_permissions/tabular_permissions.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/icons/default/icons.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/jquery.tinymce.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/ar.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/bg_BG.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/ca.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/cs.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/cs_CZ.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/cy.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/da.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/de.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/es.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/es_419.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/es_ES.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/es_MX.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/eu.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/fa.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/fa_IR.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/fi.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/fr_FR.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/gl.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/he_IL.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/hr.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/hu_HU.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/id.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/it.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/it_IT.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/ja.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/kab.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/kk.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/ko_KR.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/lt.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/nb_NO.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/nl.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/nl_BE.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/pl.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/pt_BR.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/pt_PT.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/ro.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/ro_RO.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/ru.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/ru_RU.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/sk.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/sl.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/sl_SI.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/sq.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/sv_SE.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/ta.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/ta_IN.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/th_TH.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/tr.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/tr_TR.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/ug.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/uk.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/zh_CN.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/langs/zh_TW.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/advlist/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/anchor/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/autolink/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/autoresize/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/autosave/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/bbcode/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/charmap/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/code/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/codesample/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/colorpicker/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/contextmenu/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/directionality/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/emoticons/js/emojiimages.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/emoticons/js/emojiimages.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/emoticons/js/emojis.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/emoticons/js/emojis.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/emoticons/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/fullpage/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/fullscreen/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/help/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/hr/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/image/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/imagetools/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/importcss/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/insertdatetime/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/legacyoutput/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/link/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/lists/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/media/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/nonbreaking/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/noneditable/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/pagebreak/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/paste/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/preview/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/print/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/quickbars/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/save/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/searchreplace/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/spellchecker/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/tabfocus/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/table/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/template/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/textcolor/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/textpattern/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/toc/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/visualblocks/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/visualchars/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/plugins/wordcount/plugin.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/content/dark/content.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/content/default/content.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/content/document/content.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/content/writer/content.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/ui/oxide/content.inline.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/ui/oxide/content.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/ui/oxide/content.mobile.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/ui/oxide/fonts/tinymce-mobile.woff
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/ui/oxide/skin.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/ui/oxide/skin.mobile.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/ui/oxide/skin.shadowdom.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/ui/oxide-dark/content.inline.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/ui/oxide-dark/content.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/ui/oxide-dark/content.mobile.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/ui/oxide-dark/fonts/tinymce-mobile.woff
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/ui/oxide-dark/skin.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/ui/oxide-dark/skin.mobile.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/skins/ui/oxide-dark/skin.shadowdom.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/themes/mobile/theme.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/themes/silver/theme.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/tinymce/tinymce.min.js
-Comment: 
-
-Filename: django_bpp/staticroot/vendor/select2/dist/css/select2.css
-Comment: 
-
-Filename: django_bpp/staticroot/vendor/select2/dist/css/select2.min.css
-Comment: 
-
-Filename: django_bpp/staticroot/what-input/dist/what-input.js
-Comment: 
-
 Filename: django_bpp/templates/admin/base.html
 Comment: 
 
 Filename: django_bpp/templates/admin/base_site.html
 Comment: 
 
 Filename: django_bpp/templates/admin/bpp/autor/change_form.html
@@ -7293,23 +4197,23 @@
 
 Filename: zglos_publikacje/validators.py
 Comment: 
 
 Filename: zglos_publikacje/views.py
 Comment: 
 
-Filename: bpp_iplweb-202405.1125.dist-info/LICENSE
+Filename: bpp_iplweb-202405.1126.dist-info/LICENSE
 Comment: 
 
-Filename: bpp_iplweb-202405.1125.dist-info/METADATA
+Filename: bpp_iplweb-202405.1126.dist-info/METADATA
 Comment: 
 
-Filename: bpp_iplweb-202405.1125.dist-info/WHEEL
+Filename: bpp_iplweb-202405.1126.dist-info/WHEEL
 Comment: 
 
-Filename: bpp_iplweb-202405.1125.dist-info/entry_points.txt
+Filename: bpp_iplweb-202405.1126.dist-info/entry_points.txt
 Comment: 
 
-Filename: bpp_iplweb-202405.1125.dist-info/RECORD
+Filename: bpp_iplweb-202405.1126.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## HISTORY.rst

```diff
@@ -1,13 +1,31 @@
 ==============
 Historia zmian
 ==============
 
 .. towncrier release notes start
 
+Bpp 202405.1126 (2024-05-22)
+============================
+
+Naprawione
+----------
+
+- poprawne edytowanie autorów wydawnictwa zwartego przez "zakładkę"
+
+
+Usprawnienie
+------------
+
+- dodano deklarację dostępności z opcją skonfigurowania jej w ramach serwisu
+  lub na zewnątrz (#1398)
+- dodaj flagi HttpOnly oraz Secure do ciasteczek sessionId oraz csrftoken,
+  dodaj nagłówek X-Frame-Options (#1406)
+
+
 Bpp 202405.1125 (2024-05-13)
 ============================
 
 Usprawnienie
 ------------
 
 - dodano kolumnę "impact factor" do raportu uczelnia - ewaluacja (new-1)
```

## bpp/admin/uczelnia.py

```diff
@@ -1,17 +1,18 @@
 from django import forms
 
 from ewaluacja2021.models import LiczbaNDlaUczelni
+from pbn_api.exceptions import PraceSerwisoweException
 from ..models import Uczelnia, Ukryj_Status_Korekty, Wydzial
 
 # Uczelnia
 from .core import BaseBppAdminMixin, RestrictDeletionToAdministracjaGroupMixin
 from .helpers import ADNOTACJE_FIELDSET, ZapiszZAdnotacjaMixin
 
-from django.contrib import admin
+from django.contrib import admin, messages
 
 
 class WydzialInlineForm(forms.ModelForm):
     class Meta:
         fields = ["nazwa", "skrot", "widoczny", "kolejnosc"]
         model = Wydzial
         widgets = {"kolejnosc": forms.HiddenInput}
@@ -158,17 +159,53 @@
         (
             "Clarivate Analytics API",
             {
                 "classes": ("grp-collapse grp-closed",),
                 "fields": ("clarivate_username", "clarivate_password"),
             },
         ),
+        (
+            "Deklaracja dostępności",
+            {
+                "classes": ("grp-collapse grp-closed"),
+                "fields": (
+                    "pokazuj_deklaracje_dostepnosci",
+                    "deklaracja_dostepnosci_url",
+                    "deklaracja_dostepnosci_tekst",
+                ),
+            },
+        ),
     )
 
     inlines = [
         WydzialInline,
         Ukryj_Status_KorektyInline,
         LiczbaNDlaUczelniInline,
     ]
 
+    def save_model(self, request, obj, form, change):
+        ret = super().save_model(request, obj, form, change)
+
+        if obj.pbn_integracja:
+            # Wykonaj próbne pobranie rekordu z PBNu
+            client = obj.pbn_client()
+            try:
+                client.get_languages()
+            except PraceSerwisoweException:
+                messages.warning(
+                    request,
+                    "Nie można zweryfikować konfiguracji dla połączenia z PBN, gdyż po stronie PBN "
+                    "trwają prace serwisowe. Prosimy spróbować później.",
+                )
+            except Exception as e:
+                messages.warning(
+                    request,
+                    f"To nie błąd - to ostrzeżenie. Nie można pobrać przykładowych rekordów "
+                    f"przez PBN API celem weryfikacji konfiguracji połączenia z PBNem. "
+                    f"Kod błędu podczas próbnego pobrania danych z PBN: {e}. "
+                    f"Jeżeli bład nie dotyczy problemów z siecią lub z autoryzacją PBN, skontaktuj się "
+                    f"proszę z administratorem, gdyż konfiguracja PBN może być niekompletna. ",
+                )
+            return ret
+
 
 admin.site.register(Uczelnia, UczelniaAdmin)
```

## bpp/models/uczelnia.py

```diff
@@ -3,17 +3,18 @@
 """
 from typing import TYPE_CHECKING, List, Union
 
 from autoslug import AutoSlugField
 from django.core.exceptions import ImproperlyConfigured, ValidationError
 from django.core.validators import MaxValueValidator, MinValueValidator
 from django.db import ProgrammingError, models
-from django.db.models import SET_NULL, Max
+from django.db.models import SET_NULL, Max, URLField
 from django.urls.base import reverse
 from model_utils import Choices
+from tinymce.models import HTMLField
 
 from pbn_api.exceptions import WillNotExportError
 from .. import const
 from ..const import GR_RAPORTY_WYSWIETLANIE
 from ..util import year_last_month
 from .fields import OpcjaWyswietlaniaField
 
@@ -329,14 +330,30 @@
         "przeprowadzane w tle przez procesy działające na serwerze i pobierające dane z PBN np w nocy. Jeżeli ten "
         "użytkownik dokona autoryzacji w PBN za pomocą przeglądarki, to możliwe będzie również aktualizowanie "
         "(wgrywanie) rekordów przez niego na serwer PBN. ",
         blank=True,
         null=True,
     )
 
+    class DeklaracjaDostepnosciChoices(models.IntegerChoices):
+        NIE_POKAZUJ = 0, "nie pokazuj"
+        ZEWNETRZNY_URL = 1, "zewnętrzny adres URL"
+        TEKST = 2, "tekst na podstronie serwisu BPP"
+
+    pokazuj_deklaracje_dostepnosci = models.PositiveSmallIntegerField(
+        choices=DeklaracjaDostepnosciChoices.choices,
+        default=DeklaracjaDostepnosciChoices.NIE_POKAZUJ,
+    )
+    deklaracja_dostepnosci_tekst = HTMLField(
+        verbose_name="Tekst na stronę BPP dla deklaracji dostępności",
+        blank=True,
+        null=True,
+    )
+    deklaracja_dostepnosci_url = URLField(blank=True, null=True)
+
     objects = UczelniaManager()
 
     class Meta:
         verbose_name = "uczelnia"
         verbose_name_plural = "uczelnie"
         app_label = "bpp"
 
@@ -362,28 +379,38 @@
         if self.pbn_aktualizuj_na_biezaco and not self.pbn_integracja:
             raise ValidationError(
                 {
                     "pbn_aktualizuj_na_biezaco": "Jeżeli nie używasz integracji z PBN, odznacz również i to pole. "
                 }
             )
 
-        if self.pbn_integracja:
-            # Wykonaj próbne pobranie rekordu z PBNu
-            client = self.pbn_client()
-            try:
-                client.get_languages()
-            except Exception as e:
-                raise ValidationError(
-                    {
-                        "pbn_integracja": f"Nie można pobrać przykładowych rekordów przez API celem weryfikacji. "
-                        f"Kod błędu: {e}. "
-                        f"Jeżeli bład nie dotyczy problemów z siecią lub z autoryzacją, skontaktuj się"
-                        f"z administratorem. "
-                    }
-                )
+        if (
+            self.pokazuj_deklaracje_dostepnosci
+            == Uczelnia.DeklaracjaDostepnosciChoices.ZEWNETRZNY_URL
+            and not self.deklaracja_dostepnosci_url
+        ):
+            raise ValidationError(
+                {
+                    "pokazuj_deklaracje_dostepnosci": "Wybrano pokazywanie deklaracji dostępności "
+                    "z zewnętrznego adresu URL... ",
+                    "deklaracja_dostepnosci_url": "... ale nie został on wpisany poprawnie. Proszę skorygować.",
+                }
+            )
+        if (
+            self.pokazuj_deklaracje_dostepnosci
+            == Uczelnia.DeklaracjaDostepnosciChoices.TEKST
+            and not self.deklaracja_dostepnosci_tekst
+        ):
+            raise ValidationError(
+                {
+                    "pokazuj_deklaracje_dostepnosci": "Wybrano pokazywanie deklaracji dostępności za "
+                    "pomocą tekstu w serwisie BPP... ",
+                    "deklaracja_dostepnosci_tekst": "... ale nie został on wpisany poprawnie. Proszę skorygować.",
+                }
+            )
 
     def save(self, *args, **kw):
         self.clean()
         return super().save(*args, **kw)
 
     def wosclient(self):
         """
```

## bpp/urls.py

```diff
@@ -75,14 +75,15 @@
     JednostkiView,
     OldPracaView,
     PracaView,
     PracaViewBySlug,
     RekordToPracaView,
     UczelniaView,
     WydzialView,
+    WyswietlDeklaracjeDostepnosci,
     ZrodlaView,
     ZrodloView,
 )
 from bpp.views.oai import OAIView
 from bpp.views.raporty import (
     KasowanieRaportu,
     PobranieRaportu,
@@ -180,14 +181,19 @@
     ),
     url(r"^oai/", OAIView.as_view(), name="oai"),
     url(
         r"^jednostka/(?P<slug>[\w-]+)/$",
         JednostkaView.as_view(),
         name="browse_jednostka",
     ),
+    url(
+        r"^deklaracja-dostepnosci/$",
+        WyswietlDeklaracjeDostepnosci.as_view(),
+        name="browse_deklaracja_dostepnosci",
+    ),
     url(r"^jednostki/$", JednostkiView.as_view(), name="browse_jednostki"),
     url(
         r"^jednostki/(?P<literka>.)/$",
         JednostkiView.as_view(),
         name="browse_jednostki_literka",
     ),
     url(r"^wydzial/(?P<slug>[\w-]+)/$", WydzialView.as_view(), name="browse_wydzial"),
```

## bpp/views/browse.py

```diff
@@ -7,15 +7,15 @@
     from django.core.urlresolvers import reverse
 except ImportError:
     from django.urls import reverse
 
 from django.db.models.query_utils import Q
 from django.http import Http404, HttpResponseForbidden, HttpResponseRedirect
 from django.shortcuts import get_object_or_404
-from django.views.generic import DetailView, ListView, RedirectView
+from django.views.generic import DetailView, ListView, RedirectView, TemplateView
 from multiseek.logic import AND, OR
 from multiseek.util import make_field
 from multiseek.views import MULTISEEK_SESSION_KEY, MULTISEEK_SESSION_KEY_REMOVED
 
 from miniblog.models import Article
 
 from bpp.models import Autor, Jednostka, Rekord, Uczelnia, Wydzial, Zrodlo
@@ -397,7 +397,21 @@
     model = Rekord
 
     def get_redirect_url(self, *args, **kw):
         return reverse(
             "bpp:browse_praca",
             args=(self.kwargs["content_type_id"], self.kwargs["object_id"]),
         )
+
+
+class WyswietlDeklaracjeDostepnosci(TemplateView):
+    template_name = "browse/deklaracja_dostepnosci.html"
+
+    def get_context_data(self, **kwargs):
+        uczelnia = Uczelnia.objects.get_for_request(self.request)
+        if uczelnia is None:
+            raise Http404
+
+        tekst = uczelnia.deklaracja_dostepnosci_tekst
+        url = uczelnia.deklaracja_dostepnosci_tekst
+
+        return {"tekst": tekst, "url": url, "uczelnia": uczelnia}
```

## django_bpp/settings/base.py

```diff
@@ -234,15 +234,15 @@
     "django.middleware.locale.LocaleMiddleware",
     "django.middleware.security.SecurityMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
-    # "django.middleware.clickjacking.XFrameOptionsMiddleware",
+    "django.middleware.clickjacking.XFrameOptionsMiddleware",
     "password_policies.middleware.PasswordChangeMiddleware",
     "dj_pagination.middleware.PaginationMiddleware",
     "session_security.middleware.SessionSecurityMiddleware",
     "notifications.middleware.NotificationsMiddleware",
 ]
 
 INTERNAL_IPS = ("127.0.0.1",)
@@ -1079,7 +1079,21 @@
 }
 
 #
 # django-static-sitemaps
 #
 
 STATICSITEMAPS_PING_GOOGLE = False
+
+#
+# "Audyt" bezpieczeństwa
+#
+
+CSRF_COOKIE_HTTPONLY = True
+CSRF_COOKIE_SECURE = True
+
+SESSION_COOKIE_HTTPONLY = True
+SESSION_COOKIE_SECURE = True
+
+LANGUAGE_COOKIE_SECURE = True
+
+X_FRAME_OPTIONS = "SAMEORIGIN"
```

## django_bpp/templates/admin/bpp/wydawnictwo_zwarte/change_form.html

```diff
@@ -13,15 +13,15 @@
         <li><a target="_blank" href="../../?q-l=on&q=wydawnictwo_nadrzedne.id%3D+{{ original.pk }}">Powiązane</a></li>
     {% endif %}
     {% if original.pk %}
         <li><a
                 {% if original.autorzy.count > 25 %}
                     style="background: red !important; color: yellow;"
                 {% endif %}
-                    href="/admin/bpp/wydawnictwo_ciagle_autor/?rekord__id__exact={{ original.pk }}">
+                    href="/admin/bpp/wydawnictwo_zwarte_autor/?rekord__id__exact={{ original.pk }}">
             {% if original.autorzy.count > 25 %}
                 ⚠️
             {% endif %}
             Autorzy
             {% if original.autorzy.count > 25 %}
                 ⚠️
             {% endif %}
```

## django_bpp/templates/bare.html

```diff
@@ -2,20 +2,29 @@
 {#PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN"#}
 {#        "http://www.w3.org/TR/html4/loose.dtd">#}
 <html class="no-js" lang="pl" dir="ltr">
 <head>
     <meta http-equiv="X-UA-Compatible" content="IE=10">
     {% load static %}
     {% load compress %}
-    <title>{% if "test" in request.get_host %}** SERWER TESTOWY ** {% endif %}{% block title %}{% block extratitle %}{% endblock %}
+    <title>{% if "test" in request.get_host %}** SERWER TESTOWY ** {% endif %}{% block title %}{% block extratitle %}
+    {% endblock %}
         - Bibliografia Publikacji {{ uczelnia.skrot }}
     {% endblock %}</title>
     <meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width"/>
 
+    {% if uczelnia.pokazuj_deklaracje_dostepnosci == 1 %}
+        <meta name="deklaracja-dostępności" content="{{ uczelnia.deklaracja_dostepnosci_url }}"/>
+    {% endif %}
+
+    {% if uczelnia.pokazuj_deklaracje_dostepnosci == 2 %}
+        <meta name="deklaracja-dostępności" content="{% url "bpp:browse_deklaracja_dostepnosci" %}}"/>
+    {% endif %}
+
     {% load i18n %}
     <script type="text/javascript" src="/bpp/jsi18n/?language={{ LANGUAGE_CODE }}"></script>
 
     {#        bare.html #}
     {% compress css %}
         {#        base.html #}
         <link rel="stylesheet" type="text/css" href="{% static THEME_NAME %}"/>
@@ -28,16 +37,16 @@
               href="{% static "foundation-datepicker/css/foundation-datepicker.min.css" %}">
         <link rel="stylesheet" type="text/css" href="{% static "select2/dist/css/select2.min.css" %}">
         <link rel="stylesheet" type="text/css" href="{% static "autocomplete_light/select2.css" %}">
         <link rel="stylesheet" type="text/css"
               href="{% static "select2-foundation_theme/dist/select2-foundation-theme.css" %}">
 
         <link rel="stylesheet" href="{% static "multiseek/css/style.css" %}"/>
-        <link rel="stylesheet" href="{% static "cookielaw/css/cookielaw.css" %}" />
-{#        <link rel="stylesheet" href="{% static "datatables.net-dt/css/jquery.dataTables.css" %}"/>#}
+        <link rel="stylesheet" href="{% static "cookielaw/css/cookielaw.css" %}"/>
+        {#        <link rel="stylesheet" href="{% static "datatables.net-dt/css/jquery.dataTables.css" %}"/>#}
         <link rel="stylesheet" href="{% static "datatables.net-zf/css/dataTables.foundation.css" %}"/>
 
 
     {% endcompress %}
 
     {% compress js %}
         {#        bare.html #}
@@ -95,27 +104,27 @@
 {% endblock %}
 <script type="text/javascript">
     $(document).foundation();
     $.fn.select2.defaults.set('language', 'pl');
     $.fn.select2.defaults.set('theme', 'foundation');
 
     $(document).on('select2:open', () => {
-        function _(){
+        function _() {
             document.querySelector('.select2-search__field').focus()
         }
 
         setTimeout(_, 10);
     });
 
     $.extend(true, $.fn.dataTable.defaults, {
         // Przetłumacz wszystkie tabelki DataTables
         "language": {
             "url": "{% static "bpp/js/Polish.json" %}"
         },
-        "lengthMenu": [ [10, 25, 50, 100, -1], [10, 25, 50, 100, "wszystkie"] ]
+        "lengthMenu": [[10, 25, 50, 100, -1], [10, 25, 50, 100, "wszystkie"]]
     });
 
 
 </script>
 </body>
 <footer>
     {% load bpp_version %}
```

### html2text {}

```diff
@@ -1,22 +1,24 @@
 {% load compress %}
  {#PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN"#} {# "http://www.w3.org/TR/
 html4/loose.dtd">#}
 {% load static %} {% load compress %}
-{% load i18n %}
+{% if uczelnia.pokazuj_deklaracje_dostepnosci == 1 %}
+{% endif %} {% if uczelnia.pokazuj_deklaracje_dostepnosci == 2 %}
+}}"/> {% endif %} {% load i18n %}
 {# bare.html #} {% compress css %} {# base.html #}
 }">
 }">
 }">
 }">
 }">
 }">
 }">
 }"/>
-}" /> {#
+}"/> {#
 }"/>#}
 }"/> {% endcompress %} {% compress js %} {# bare.html #}
 }">
 }">
 {# base.html #}
 }" type="text/javascript">
 }">
```

## django_bpp/templates/base_footer.html

```diff
@@ -1,11 +1,19 @@
 <div class="cell">
     <div class="hide-for-print cell">
         <hr size="1"/>
         <div style="text-align: right; font-size: 70%;">
+            {% if uczelnia.pokazuj_deklaracje_dostepnosci == 1 %}
+                <a href="{{ uczelnia.deklaracja_dostepnosci_url }}">deklaracja dostępności</a> |
+            {% endif %}
+
+            {% if uczelnia.pokazuj_deklaracje_dostepnosci == 2 %}
+                <a href="{% url "bpp:browse_deklaracja_dostepnosci" %}">deklaracja dostępności</a> |
+            {% endif %}
+
             {% if not request.user.is_anonymous %}
                 zalogowany/a jako {{ request.user.username }} -
             {% endif %}
             Oprogramowanie <a href="http://bpp.iplweb.pl/">Bibliografia Publikacji Pracowników</a> &copy;
             2004-2022 <a href="http://iplweb.pl">IPLweb</a>; wersja {% load bpp_version %}{% bpp_version %}
             <div id="test-image-copyright" style="display: none;">
                 Obrazek tła dla serwera testowego: <a href=http://www.freepik.com>Designed by pch.vector /
```

### html2text {}

```diff
@@ -1,9 +1,12 @@
 ===============================================================================
-{% if not request.user.is_anonymous %} zalogowany/a jako {
+{% if uczelnia.pokazuj_deklaracje_dostepnosci == 1 %} _d_e_k_l_a_r_a_c_j_a_ _d_o_s_t_Ä__p_n_o_Å__c_i
+| {% endif %} {% if uczelnia.pokazuj_deklaracje_dostepnosci == 2 %}
+}">deklaracja dostÄpnoÅci
+ | {% endif %} {% if not request.user.is_anonymous %} zalogowany/a jako {
 { request.user.username }} - {% endif %} Oprogramowanie _B_i_b_l_i_o_g_r_a_f_i_a_ _P_u_b_l_i_k_a_c_j_i
 _P_r_a_c_o_w_n_i_k_Ã_³_w © 2004-2022 _I_P_L_w_e_b; wersja {% load bpp_version %}{% bpp_version %}
 Obrazek tÅa dla serwera testowego: _D_e_s_i_g_n_e_d_ _b_y_ _p_c_h_._v_e_c_t_o_r_ _/_ _F_r_e_e_p_i_k.
 Dokument wygenerowano przy pomocy systemu Bibliografia Publikacji PracownikÃ³w
 w wersji {{%% bbpppp__vveerrssiioonn %%}} dnia {{%% nnooww ""SSHHOORRTT__DDAATTEE__FFOORRMMAATT"" %%}} oo ggooddzziinniiee {{%% nnooww
 ""HH::ii"" %%}} {% if not request.user.is_anonymous %} przez uÅ¼ytkownika {{
 {{ rreeqquueesstt..uusseerr..uusseerrnnaammee }}}} {% endif %}
```

## django_bpp/version.py

```diff
@@ -1,8 +1,8 @@
-VERSION = "202405.1125"
+VERSION = "202405.1126"
 
 if __name__ == "__main__":
     import sys
 
     OUTPUT = VERSION
 
     if "--json" in sys.argv:
```

## pbn_api/exceptions.py

```diff
@@ -2,15 +2,16 @@
 
 
 class TlumaczDyscyplinException(ValueError):
     pass
 
 
 class PraceSerwisoweException(Exception):
-    pass
+    def __str__(self):
+        return "Po stronie PBN trwają prace serwisowe. Prosimy spróbować później. "
 
 
 class HttpException(Exception):
     def __init__(self, status_code, url, content):
         self.status_code = status_code
         self.url = url
         self.content = content
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `bpp_iplweb-202405.1125.dist-info/LICENSE` & `bpp_iplweb-202405.1126.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bpp_iplweb-202405.1125.dist-info/METADATA` & `bpp_iplweb-202405.1126.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpp_iplweb
-Version: 202405.1125
+Version: 202405.1126
 Summary: 
 License: MIT
 Author: Michał Pasternak
 Author-email: michal.dtz@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

