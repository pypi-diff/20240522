# Comparing `tmp/django_herobiz_dental-2.0.0.tar.gz` & `tmp/django_herobiz_dental-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_herobiz_dental-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_herobiz_dental-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_herobiz_dental-2.0.0.tar` & `django_herobiz_dental-2.1.0.tar`

### file list

```diff
@@ -1,178 +1,178 @@
--rw-r--r--   0        0        0    10244 2024-05-10 07:12:48.789350 django_herobiz_dental-2.0.0/.DS_Store
--rw-r--r--   0        0        0       66 2024-04-05 05:27:06.902059 django_herobiz_dental-2.0.0/.gitattributes
--rw-r--r--   0        0        0       44 2024-05-07 00:58:27.030831 django_herobiz_dental-2.0.0/.gitignore
--rw-r--r--   0        0        0       52 2024-04-05 05:27:59.025754 django_herobiz_dental-2.0.0/.idea/.gitignore
--rw-r--r--   0        0        0      411 2024-04-05 05:27:58.943620 django_herobiz_dental-2.0.0/.idea/django-herobiz-dental.iml
--rw-r--r--   0        0        0      174 2024-04-05 05:27:58.956024 django_herobiz_dental-2.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      433 2024-04-05 06:12:30.213755 django_herobiz_dental-2.0.0/.idea/misc.xml
--rw-r--r--   0        0        0      294 2024-04-05 05:27:58.950052 django_herobiz_dental-2.0.0/.idea/modules.xml
--rw-r--r--   0        0        0      167 2024-04-05 05:27:58.958164 django_herobiz_dental-2.0.0/.idea/vcs.xml
--rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_herobiz_dental-2.0.0/LICENSE
--rw-r--r--   0        0        0     5026 2024-05-16 04:53:09.814235 django_herobiz_dental-2.0.0/README.md
--rw-r--r--   0        0        0        0 2024-04-05 06:12:24.810066 django_herobiz_dental-2.0.0/django_herobiz_dental/__init__.py
--rw-r--r--   0        0        0      612 2024-04-21 04:03:56.019184 django_herobiz_dental-2.0.0/django_herobiz_dental/admin.py
--rw-r--r--   0        0        0      172 2024-04-05 06:12:24.811671 django_herobiz_dental-2.0.0/django_herobiz_dental/apps.py
--rw-r--r--   0        0        0     1201 2024-04-21 04:03:56.010074 django_herobiz_dental-2.0.0/django_herobiz_dental/forms.py
--rw-r--r--   0        0        0     2088 2024-04-05 06:31:38.858042 django_herobiz_dental-2.0.0/django_herobiz_dental/migrations/0001_initial.py
--rw-r--r--   0        0        0      334 2024-04-11 05:20:55.981354 django_herobiz_dental-2.0.0/django_herobiz_dental/migrations/0002_remove_portfolio_client.py
--rw-r--r--   0        0        0     2553 2024-04-21 04:08:50.044472 django_herobiz_dental-2.0.0/django_herobiz_dental/migrations/0003_portfolio_client_post_profile.py
--rw-r--r--   0        0        0        0 2024-04-05 06:12:24.812107 django_herobiz_dental-2.0.0/django_herobiz_dental/migrations/__init__.py
--rw-r--r--   0        0        0     3149 2024-05-16 05:59:24.869835 django_herobiz_dental-2.0.0/django_herobiz_dental/models.py
--rw-r--r--   0        0        0      559 2024-04-21 04:03:56.001901 django_herobiz_dental-2.0.0/django_herobiz_dental/sitemaps.py
--rwxr-xr-x   0        0        0    60252 2024-03-29 01:14:08.439726 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/css/main.css
--rwxr-xr-x   0        0        0     7992 2024-04-03 08:26:33.002126 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/css/variables-blue.css
--rwxr-xr-x   0        0        0     7989 2024-04-03 08:32:44.614276 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/css/variables-green.css
--rwxr-xr-x   0        0        0     7992 2024-04-03 08:32:44.619981 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/css/variables-orange.css
--rwxr-xr-x   0        0        0     7994 2024-04-03 08:32:44.616432 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/css/variables-pink.css
--rwxr-xr-x   0        0        0     7992 2024-04-03 08:32:44.612088 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/css/variables-purple.css
--rwxr-xr-x   0        0        0     7986 2024-04-03 08:32:44.607824 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/css/variables-red.css
--rwxr-xr-x   0        0        0     7985 2024-04-03 08:32:44.618152 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/css/variables.css
--rwxr-xr-x   0        0        0      766 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/img/about-bg.png
--rwxr-xr-x   0        0        0    95604 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/img/faq.jpg
--rwxr-xr-x   0        0        0    13287 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/img/hero-bg.png
--rwxr-xr-x   0        0        0    13081 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/img/onfocus-content-bg.jpg
--rwxr-xr-x   0        0        0    61855 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/img/pricing-bg.jpg
--rwxr-xr-x   0        0        0     8186 2024-03-17 05:37:08.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/js/main.js
--rwxr-xr-x   0        0        0      281 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/_blog.scss
--rwxr-xr-x   0        0        0     3649 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/_footer.scss
--rwxr-xr-x   0        0        0     3770 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/_general.scss
--rwxr-xr-x   0        0        0     1118 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/_header.scss
--rwxr-xr-x   0        0        0      643 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/_index.scss
--rwxr-xr-x   0        0        0     5712 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/_nav.scss
--rwxr-xr-x   0        0        0     1320 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/_portfolio-details.scss
--rwxr-xr-x   0        0        0     2172 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_comments.scss
--rwxr-xr-x   0        0        0     3738 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_details.scss
--rwxr-xr-x   0        0        0      758 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_pagination.scss
--rwxr-xr-x   0        0        0     1813 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_posts-list.scss
--rwxr-xr-x   0        0        0     3480 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_sidebar.scss
--rwxr-xr-x   0        0        0     1676 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_about.scss
--rwxr-xr-x   0        0        0      377 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_clients.scss
--rwxr-xr-x   0        0        0     3086 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_contact.scss
--rwxr-xr-x   0        0        0     1882 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_cta.scss
--rwxr-xr-x   0        0        0     1674 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_faq.scss
--rwxr-xr-x   0        0        0      981 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_featured-services.scss
--rwxr-xr-x   0        0        0     1762 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_features.scss
--rwxr-xr-x   0        0        0     2205 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-animated.scss
--rwxr-xr-x   0        0        0     1990 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-fullscreen.scss
--rwxr-xr-x   0        0        0     1764 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-static.scss
--rwxr-xr-x   0        0        0     3481 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_hero.scss
--rwxr-xr-x   0        0        0     3798 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_onfocus.scss
--rwxr-xr-x   0        0        0     2264 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_portfolio.scss
--rwxr-xr-x   0        0        0     2551 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_pricing.scss
--rwxr-xr-x   0        0        0     1512 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_recent-blog-posts.scss
--rwxr-xr-x   0        0        0     1718 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_services.scss
--rwxr-xr-x   0        0        0     1922 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_team.scss
--rwxr-xr-x   0        0        0     2203 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_testimonials.scss
--rwxr-xr-x   0        0        0      253 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/main.scss
--rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/variables-blue.css
--rwxr-xr-x   0        0        0     7957 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/variables-green.css
--rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/variables-orange.css
--rwxr-xr-x   0        0        0     7962 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/variables-pink.css
--rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/variables-purple.css
--rwxr-xr-x   0        0        0     7954 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/variables-red.css
--rwxr-xr-x   0        0        0     7953 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/variables.css
--rw-r--r--   0        0        0    19941 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.cjs.js
--rw-r--r--   0        0        0    28765 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.css
--rw-r--r--   0        0        0    19768 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.esm.js
--rw-r--r--   0        0        0    13800 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.js
--rw-r--r--   0        0        0    56459 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.js.map
--rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.css
--rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.json
--rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.min.css
--rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.scss
--rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.css
--rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.css.map
--rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.js
--rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.js
--rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.js.map
--rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.min.js.map
--rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/glightbox.css
--rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/glightbox.min.css
--rw-r--r--   0        0        0    52561 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/plyr.css
--rw-r--r--   0        0        0    45081 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/plyr.min.css
--rw-r--r--   0        0        0   109391 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/js/glightbox.js
--rw-r--r--   0        0        0    55880 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/js/glightbox.min.js
--rw-r--r--   0        0        0    91398 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/isotope-layout/isotope.pkgd.js
--rw-r--r--   0        0        0    35445 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/isotope-layout/isotope.pkgd.min.js
--rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/php-email-form/php-email-form.php
--rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/php-email-form/validate.js
--rw-r--r--   0        0        0    18436 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.css
--rw-r--r--   0        0        0   149147 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.js
--rw-r--r--   0        0        0   201656 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.js.map
--rw-r--r--   0        0        0     2102 2024-04-09 00:04:07.573124 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_about.html
--rw-r--r--   0        0        0      434 2024-04-05 06:31:15.204362 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_clients.html
--rw-r--r--   0        0        0     2846 2024-04-12 02:19:51.757891 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_contact.html
--rw-r--r--   0        0        0     1175 2024-05-04 00:59:47.337426 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_cta.html
--rw-r--r--   0        0        0     1599 2024-04-05 06:31:15.205949 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_faq.html
--rw-r--r--   0        0        0      794 2024-03-29 06:50:25.784512 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_featured-services.html
--rw-r--r--   0        0        0     2039 2024-04-05 06:31:15.185290 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_features.html
--rw-r--r--   0        0        0      976 2024-04-05 08:05:20.508185 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_hero-animated.html
--rw-r--r--   0        0        0     1827 2024-04-09 00:03:36.818036 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_hero-carousel.html
--rw-r--r--   0        0        0      866 2024-04-05 07:58:17.230132 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_hero-fullscreen.html
--rw-r--r--   0        0        0      871 2024-04-05 06:31:15.195476 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_hero-static.html
--rw-r--r--   0        0        0     2039 2024-05-04 01:19:12.465694 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_onfocus.html
--rw-r--r--   0        0        0     1486 2024-04-05 06:31:15.182443 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_portfolio.html
--rw-r--r--   0        0        0     1462 2024-05-09 00:00:35.838293 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_pricing.html
--rw-r--r--   0        0        0     1105 2024-05-16 06:11:06.297596 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_recent-blog-posts.html
--rw-r--r--   0        0        0      990 2024-05-17 04:40:54.995837 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_services.html
--rw-r--r--   0        0        0     1699 2024-05-16 05:16:41.130030 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_sidebar.html
--rw-r--r--   0        0        0     1676 2024-04-11 00:36:54.545452 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_team.html
--rw-r--r--   0        0        0     1333 2024-04-05 06:31:15.202919 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_testimonials.html
--rwxr-xr-x   0        0        0    10531 2024-04-30 05:50:18.836953 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/blog-details.html
--rwxr-xr-x   0        0        0     2891 2024-04-21 04:11:21.315431 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/blog.html
--rw-r--r--   0        0        0      346 2024-04-05 06:31:15.198382 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/breadcrumb.html
--rw-r--r--   0        0        0     2215 2024-04-11 03:29:47.000571 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/footer.html
--rwxr-xr-x   0        0        0     1341 2024-03-12 00:49:58.000000 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/forms/contact.php
--rw-r--r--   0        0        0     1430 2024-05-16 04:59:12.184906 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/header.html
--rwxr-xr-x   0        0        0     5184 2024-05-02 04:54:51.026951 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/index.html
--rwxr-xr-x   0        0        0     4995 2024-04-11 05:42:55.439634 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/portfolio-details.html
--rwxr-xr-x   0        0        0    16277 2024-04-21 04:03:55.997732 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/privacy.html
--rw-r--r--   0        0        0     2028 2024-04-05 06:31:15.187765 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/seo.html
--rwxr-xr-x   0        0        0    16317 2024-04-21 04:03:56.020846 django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/terms.html
--rw-r--r--   0        0        0        0 2023-03-21 07:32:09.033136 django_herobiz_dental-2.0.0/django_herobiz_dental/templatetags/__init__.py
--rw-r--r--   0        0        0     4813 2024-05-03 01:08:11.844770 django_herobiz_dental-2.0.0/django_herobiz_dental/templatetags/herobizdental_tags.py
--rw-r--r--   0        0        0       60 2024-04-05 06:12:24.811958 django_herobiz_dental-2.0.0/django_herobiz_dental/tests.py
--rw-r--r--   0        0        0     1115 2024-04-21 04:03:56.022033 django_herobiz_dental-2.0.0/django_herobiz_dental/urls.py
--rw-r--r--   0        0        0     7429 2024-05-02 07:51:11.143076 django_herobiz_dental-2.0.0/django_herobiz_dental/views.py
--rw-r--r--   0        0        0      972 2024-05-17 04:41:48.321512 django_herobiz_dental-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     5766 1970-01-01 00:00:00.000000 django_herobiz_dental-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    10244 2024-05-17 05:37:55.112002 django_herobiz_dental-2.1.0/.DS_Store
+-rw-r--r--   0        0        0       66 2024-04-05 05:27:06.902059 django_herobiz_dental-2.1.0/.gitattributes
+-rw-r--r--   0        0        0       55 2024-05-18 01:48:26.698611 django_herobiz_dental-2.1.0/.gitignore
+-rw-r--r--   0        0        0       52 2024-04-05 05:27:59.025754 django_herobiz_dental-2.1.0/.idea/.gitignore
+-rw-r--r--   0        0        0      411 2024-04-05 05:27:58.943620 django_herobiz_dental-2.1.0/.idea/django-herobiz-dental.iml
+-rw-r--r--   0        0        0      174 2024-04-05 05:27:58.956024 django_herobiz_dental-2.1.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      433 2024-04-05 06:12:30.213755 django_herobiz_dental-2.1.0/.idea/misc.xml
+-rw-r--r--   0        0        0      294 2024-04-05 05:27:58.950052 django_herobiz_dental-2.1.0/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-04-05 05:27:58.958164 django_herobiz_dental-2.1.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_herobiz_dental-2.1.0/LICENSE
+-rw-r--r--   0        0        0     5042 2024-05-18 19:44:22.970154 django_herobiz_dental-2.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 06:12:24.810066 django_herobiz_dental-2.1.0/django_herobiz_dental/__init__.py
+-rw-r--r--   0        0        0      612 2024-04-21 04:03:56.019184 django_herobiz_dental-2.1.0/django_herobiz_dental/admin.py
+-rw-r--r--   0        0        0      172 2024-04-05 06:12:24.811671 django_herobiz_dental-2.1.0/django_herobiz_dental/apps.py
+-rw-r--r--   0        0        0     1201 2024-04-21 04:03:56.010074 django_herobiz_dental-2.1.0/django_herobiz_dental/forms.py
+-rw-r--r--   0        0        0     2088 2024-04-05 06:31:38.858042 django_herobiz_dental-2.1.0/django_herobiz_dental/migrations/0001_initial.py
+-rw-r--r--   0        0        0      334 2024-04-11 05:20:55.981354 django_herobiz_dental-2.1.0/django_herobiz_dental/migrations/0002_remove_portfolio_client.py
+-rw-r--r--   0        0        0     2553 2024-04-21 04:08:50.044472 django_herobiz_dental-2.1.0/django_herobiz_dental/migrations/0003_portfolio_client_post_profile.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:12:24.812107 django_herobiz_dental-2.1.0/django_herobiz_dental/migrations/__init__.py
+-rw-r--r--   0        0        0     3149 2024-05-16 05:59:24.869835 django_herobiz_dental-2.1.0/django_herobiz_dental/models.py
+-rw-r--r--   0        0        0      559 2024-04-21 04:03:56.001901 django_herobiz_dental-2.1.0/django_herobiz_dental/sitemaps.py
+-rwxr-xr-x   0        0        0    60252 2024-03-29 01:14:08.439726 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/css/main.css
+-rwxr-xr-x   0        0        0     7992 2024-04-03 08:26:33.002126 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/css/variables-blue.css
+-rwxr-xr-x   0        0        0     7989 2024-04-03 08:32:44.614276 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/css/variables-green.css
+-rwxr-xr-x   0        0        0     7992 2024-04-03 08:32:44.619981 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/css/variables-orange.css
+-rwxr-xr-x   0        0        0     7994 2024-04-03 08:32:44.616432 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/css/variables-pink.css
+-rwxr-xr-x   0        0        0     7992 2024-04-03 08:32:44.612088 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/css/variables-purple.css
+-rwxr-xr-x   0        0        0     7986 2024-04-03 08:32:44.607824 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/css/variables-red.css
+-rwxr-xr-x   0        0        0     7985 2024-04-03 08:32:44.618152 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/css/variables.css
+-rwxr-xr-x   0        0        0      766 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/img/about-bg.png
+-rwxr-xr-x   0        0        0    95604 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/img/faq.jpg
+-rwxr-xr-x   0        0        0    13287 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/img/hero-bg.png
+-rwxr-xr-x   0        0        0    13081 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/img/onfocus-content-bg.jpg
+-rwxr-xr-x   0        0        0    61855 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/img/pricing-bg.jpg
+-rwxr-xr-x   0        0        0     8186 2024-03-17 05:37:08.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/js/main.js
+-rwxr-xr-x   0        0        0      281 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/_blog.scss
+-rwxr-xr-x   0        0        0     3649 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/_footer.scss
+-rwxr-xr-x   0        0        0     3770 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/_general.scss
+-rwxr-xr-x   0        0        0     1118 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/_header.scss
+-rwxr-xr-x   0        0        0      643 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/_index.scss
+-rwxr-xr-x   0        0        0     5712 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/_nav.scss
+-rwxr-xr-x   0        0        0     1320 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/_portfolio-details.scss
+-rwxr-xr-x   0        0        0     2172 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/blog/_comments.scss
+-rwxr-xr-x   0        0        0     3738 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/blog/_details.scss
+-rwxr-xr-x   0        0        0      758 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/blog/_pagination.scss
+-rwxr-xr-x   0        0        0     1813 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/blog/_posts-list.scss
+-rwxr-xr-x   0        0        0     3480 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/blog/_sidebar.scss
+-rwxr-xr-x   0        0        0     1676 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_about.scss
+-rwxr-xr-x   0        0        0      377 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_clients.scss
+-rwxr-xr-x   0        0        0     3086 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_contact.scss
+-rwxr-xr-x   0        0        0     1882 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_cta.scss
+-rwxr-xr-x   0        0        0     1674 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_faq.scss
+-rwxr-xr-x   0        0        0      981 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_featured-services.scss
+-rwxr-xr-x   0        0        0     1762 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_features.scss
+-rwxr-xr-x   0        0        0     2205 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-animated.scss
+-rwxr-xr-x   0        0        0     1990 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-fullscreen.scss
+-rwxr-xr-x   0        0        0     1764 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-static.scss
+-rwxr-xr-x   0        0        0     3481 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_hero.scss
+-rwxr-xr-x   0        0        0     3798 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_onfocus.scss
+-rwxr-xr-x   0        0        0     2264 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_portfolio.scss
+-rwxr-xr-x   0        0        0     2551 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_pricing.scss
+-rwxr-xr-x   0        0        0     1512 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_recent-blog-posts.scss
+-rwxr-xr-x   0        0        0     1718 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_services.scss
+-rwxr-xr-x   0        0        0     1922 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_team.scss
+-rwxr-xr-x   0        0        0     2203 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_testimonials.scss
+-rwxr-xr-x   0        0        0      253 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/main.scss
+-rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/variables-blue.css
+-rwxr-xr-x   0        0        0     7957 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/variables-green.css
+-rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/variables-orange.css
+-rwxr-xr-x   0        0        0     7962 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/variables-pink.css
+-rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/variables-purple.css
+-rwxr-xr-x   0        0        0     7954 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/variables-red.css
+-rwxr-xr-x   0        0        0     7953 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/variables.css
+-rw-r--r--   0        0        0    19941 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.cjs.js
+-rw-r--r--   0        0        0    28765 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.css
+-rw-r--r--   0        0        0    19768 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.esm.js
+-rw-r--r--   0        0        0    13800 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.js
+-rw-r--r--   0        0        0    56459 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.js.map
+-rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.min.css
+-rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.scss
+-rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.css
+-rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.js
+-rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/glightbox.css
+-rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/glightbox.min.css
+-rw-r--r--   0        0        0    52561 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/plyr.css
+-rw-r--r--   0        0        0    45081 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/plyr.min.css
+-rw-r--r--   0        0        0   109391 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/js/glightbox.js
+-rw-r--r--   0        0        0    55880 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/js/glightbox.min.js
+-rw-r--r--   0        0        0    91398 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/isotope-layout/isotope.pkgd.js
+-rw-r--r--   0        0        0    35445 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/isotope-layout/isotope.pkgd.min.js
+-rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/php-email-form/php-email-form.php
+-rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/php-email-form/validate.js
+-rw-r--r--   0        0        0    18436 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.css
+-rw-r--r--   0        0        0   149147 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.js
+-rw-r--r--   0        0        0   201656 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.js.map
+-rw-r--r--   0        0        0     2102 2024-04-09 00:04:07.573124 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_about.html
+-rw-r--r--   0        0        0      434 2024-04-05 06:31:15.204362 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_clients.html
+-rw-r--r--   0        0        0     2846 2024-04-12 02:19:51.757891 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_contact.html
+-rw-r--r--   0        0        0     1175 2024-05-04 00:59:47.337426 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_cta.html
+-rw-r--r--   0        0        0     1599 2024-04-05 06:31:15.205949 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_faq.html
+-rw-r--r--   0        0        0      794 2024-03-29 06:50:25.784512 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_featured-services.html
+-rw-r--r--   0        0        0     2039 2024-04-05 06:31:15.185290 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_features.html
+-rw-r--r--   0        0        0      976 2024-04-05 08:05:20.508185 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_hero-animated.html
+-rw-r--r--   0        0        0     1827 2024-04-09 00:03:36.818036 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_hero-carousel.html
+-rw-r--r--   0        0        0      866 2024-04-05 07:58:17.230132 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_hero-fullscreen.html
+-rw-r--r--   0        0        0      871 2024-04-05 06:31:15.195476 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_hero-static.html
+-rw-r--r--   0        0        0     2039 2024-05-04 01:19:12.465694 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_onfocus.html
+-rw-r--r--   0        0        0     1486 2024-04-05 06:31:15.182443 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_portfolio.html
+-rw-r--r--   0        0        0     1462 2024-05-09 00:00:35.838293 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_pricing.html
+-rw-r--r--   0        0        0     1105 2024-05-16 06:11:06.297596 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_recent-blog-posts.html
+-rw-r--r--   0        0        0      990 2024-05-17 04:40:54.995837 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_services.html
+-rw-r--r--   0        0        0     1699 2024-05-16 05:16:41.130030 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_sidebar.html
+-rw-r--r--   0        0        0     1676 2024-04-11 00:36:54.545452 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_team.html
+-rw-r--r--   0        0        0     1333 2024-04-05 06:31:15.202919 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_testimonials.html
+-rwxr-xr-x   0        0        0    10531 2024-04-30 05:50:18.836953 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/blog-details.html
+-rwxr-xr-x   0        0        0     2907 2024-05-21 08:38:04.788593 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/blog.html
+-rw-r--r--   0        0        0      346 2024-04-05 06:31:15.198382 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/breadcrumb.html
+-rw-r--r--   0        0        0     2215 2024-04-11 03:29:47.000571 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/footer.html
+-rwxr-xr-x   0        0        0     1341 2024-03-12 00:49:58.000000 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/forms/contact.php
+-rw-r--r--   0        0        0     1430 2024-05-16 04:59:12.184906 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/header.html
+-rwxr-xr-x   0        0        0     5184 2024-05-02 04:54:51.026951 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/index.html
+-rwxr-xr-x   0        0        0     4995 2024-04-11 05:42:55.439634 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/portfolio-details.html
+-rwxr-xr-x   0        0        0    16277 2024-04-21 04:03:55.997732 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/privacy.html
+-rw-r--r--   0        0        0     2028 2024-04-05 06:31:15.187765 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/seo.html
+-rwxr-xr-x   0        0        0    16317 2024-04-21 04:03:56.020846 django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/terms.html
+-rw-r--r--   0        0        0        0 2023-03-21 07:32:09.033136 django_herobiz_dental-2.1.0/django_herobiz_dental/templatetags/__init__.py
+-rw-r--r--   0        0        0     4813 2024-05-03 01:08:11.844770 django_herobiz_dental-2.1.0/django_herobiz_dental/templatetags/herobizdental_tags.py
+-rw-r--r--   0        0        0       60 2024-04-05 06:12:24.811958 django_herobiz_dental-2.1.0/django_herobiz_dental/tests.py
+-rw-r--r--   0        0        0     1115 2024-04-21 04:03:56.022033 django_herobiz_dental-2.1.0/django_herobiz_dental/urls.py
+-rw-r--r--   0        0        0     7429 2024-05-02 07:51:11.143076 django_herobiz_dental-2.1.0/django_herobiz_dental/views.py
+-rw-r--r--   0        0        0      972 2024-05-21 08:40:01.258244 django_herobiz_dental-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 django_herobiz_dental-2.1.0/PKG-INFO
```

### Comparing `django_herobiz_dental-2.0.0/.DS_Store` & `django_herobiz_dental-2.1.0/.DS_Store`

 * *Files 7% similar despite different names*

```diff
@@ -342,54 +342,54 @@
 00001550: 4100 0000 0400 6400 6900 7300 746d 6f64  A.....d.i.s.tmod
 00001560: 4462 6c6f 6200 0000 08ef 517e 5ee2 f2c5  Dblob.....Q~^...
 00001570: 4100 0000 0400 6400 6900 7300 7470 6831  A.....d.i.s.tph1
 00001580: 5363 6f6d 7000 0000 0003 7e00 0000 0000  Scomp.....~.....
 00001590: 1500 6400 6a00 6100 6e00 6700 6f00 5f00  ..d.j.a.n.g.o._.
 000015a0: 6800 6500 7200 6f00 6200 6900 7a00 5f00  h.e.r.o.b.i.z._.
 000015b0: 6400 6500 6e00 7400 6100 6c62 7773 7062  d.e.n.t.a.lbwspb
-000015c0: 6c6f 6200 0000 b862 706c 6973 7430 30d6  lob....bplist00.
+000015c0: 6c6f 6200 0000 b962 706c 6973 7430 30d6  lob....bplist00.
 000015d0: 0102 0304 0506 0708 0708 0b08 5d53 686f  ............]Sho
 000015e0: 7753 7461 7475 7342 6172 5b53 686f 7754  wStatusBar[ShowT
 000015f0: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
 00001600: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
 00001610: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
 00001620: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
-00001630: 6172 0809 0809 5f10 187b 7b33 3133 2c20  ar...._..{{313, 
-00001640: 3530 7d2c 207b 3132 3332 2c20 3638 377d  50}, {1232, 687}
-00001650: 7d09 0815 232f 3b52 5f6b 6c6d 6e6f 8a00  }...#/;R_klmno..
-00001660: 0000 0000 0001 0100 0000 0000 0000 0d00  ................
-00001670: 0000 0000 0000 0000 0000 0000 0000 8b00  ................
-00001680: 0000 1500 6400 6a00 6100 6e00 6700 6f00  ....d.j.a.n.g.o.
-00001690: 5f00 6800 6500 7200 6f00 6200 6900 7a00  _.h.e.r.o.b.i.z.
-000016a0: 5f00 6400 6500 6e00 7400 6100 6c6c 6731  _.d.e.n.t.a.llg1
-000016b0: 5363 6f6d 7000 0000 0000 a885 9500 0000  Scomp...........
-000016c0: 1500 6400 6a00 6100 6e00 6700 6f00 5f00  ..d.j.a.n.g.o._.
-000016d0: 6800 6500 7200 6f00 6200 6900 7a00 5f00  h.e.r.o.b.i.z._.
-000016e0: 6400 6500 6e00 7400 6100 6c6d 6f44 4462  d.e.n.t.a.lmoDDb
-000016f0: 6c6f 6200 0000 08dd 3bc5 9e64 f2c5 4100  lob.....;..d..A.
-00001700: 0000 1500 6400 6a00 6100 6e00 6700 6f00  ....d.j.a.n.g.o.
-00001710: 5f00 6800 6500 7200 6f00 6200 6900 7a00  _.h.e.r.o.b.i.z.
-00001720: 5f00 6400 6500 6e00 7400 6100 6c6d 6f64  _.d.e.n.t.a.lmod
-00001730: 4462 6c6f 6200 0000 08dd 3bc5 9e64 f2c5  Dblob.....;..d..
-00001740: 4100 0000 1500 6400 6a00 6100 6e00 6700  A.....d.j.a.n.g.
-00001750: 6f00 5f00 6800 6500 7200 6f00 6200 6900  o._.h.e.r.o.b.i.
-00001760: 7a00 5f00 6400 6500 6e00 7400 6100 6c70  z._.d.e.n.t.a.lp
-00001770: 6831 5363 6f6d 7000 0000 0000 adf0 0000  h1Scomp.........
-00001780: 0000 1500 6400 6a00 6100 6e00 6700 6f00  ....d.j.a.n.g.o.
-00001790: 5f00 6800 6500 7200 6f00 6200 6900 7a00  _.h.e.r.o.b.i.z.
-000017a0: 5f00 6400 6500 6e00 7400 6100 6c76 5372  _.d.e.n.t.a.lvSr
-000017b0: 6e6c 6f6e 6700 0000 0100 0000 0500 6d00  nlong.........m.
-000017c0: 6500 6400 6900 616c 6731 5363 6f6d 7000  e.d.i.alg1Scomp.
-000017d0: 0000 0000 4795 c500 0000 0500 6d00 6500  ....G.......m.e.
-000017e0: 6400 6900 616d 6f44 4462 6c6f 6200 0000  d.i.amoDDblob...
-000017f0: 0805 ecb3 3888 eac5 4100 0000 0500 6d00  ....8...A.....m.
-00001800: 6500 6400 6900 616d 6f64 4462 6c6f 6200  e.d.i.amodDblob.
-00001810: 0000 0805 ecb3 3888 eac5 4100 0000 0500  ......8...A.....
-00001820: 6d00 6500 6400 6900 6170 6831 5363 6f6d  m.e.d.i.aph1Scom
-00001830: 7000 0000 0000 47e0 0000 0000 0000 0000  p.....G.........
+00001630: 6172 0809 0809 5f10 197b 7b31 3133 332c  ar...._..{{1133,
+00001640: 2031 3033 7d2c 207b 3932 302c 2034 3336   103}, {920, 436
+00001650: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8b  }}...#/;R_klmno.
+00001660: 0000 0000 0000 0101 0000 0000 0000 000d  ................
+00001670: 0000 0000 0000 0000 0000 0000 0000 008c  ................
+00001680: 0000 0015 0064 006a 0061 006e 0067 006f  .....d.j.a.n.g.o
+00001690: 005f 0068 0065 0072 006f 0062 0069 007a  ._.h.e.r.o.b.i.z
+000016a0: 005f 0064 0065 006e 0074 0061 006c 6c67  ._.d.e.n.t.a.llg
+000016b0: 3153 636f 6d70 0000 0000 00a8 8595 0000  1Scomp..........
+000016c0: 0015 0064 006a 0061 006e 0067 006f 005f  ...d.j.a.n.g.o._
+000016d0: 0068 0065 0072 006f 0062 0069 007a 005f  .h.e.r.o.b.i.z._
+000016e0: 0064 0065 006e 0074 0061 006c 6d6f 4444  .d.e.n.t.a.lmoDD
+000016f0: 626c 6f62 0000 0008 dd3b c59e 64f2 c541  blob.....;..d..A
+00001700: 0000 0015 0064 006a 0061 006e 0067 006f  .....d.j.a.n.g.o
+00001710: 005f 0068 0065 0072 006f 0062 0069 007a  ._.h.e.r.o.b.i.z
+00001720: 005f 0064 0065 006e 0074 0061 006c 6d6f  ._.d.e.n.t.a.lmo
+00001730: 6444 626c 6f62 0000 0008 dd3b c59e 64f2  dDblob.....;..d.
+00001740: c541 0000 0015 0064 006a 0061 006e 0067  .A.....d.j.a.n.g
+00001750: 006f 005f 0068 0065 0072 006f 0062 0069  .o._.h.e.r.o.b.i
+00001760: 007a 005f 0064 0065 006e 0074 0061 006c  .z._.d.e.n.t.a.l
+00001770: 7068 3153 636f 6d70 0000 0000 00ad f000  ph1Scomp........
+00001780: 0000 0015 0064 006a 0061 006e 0067 006f  .....d.j.a.n.g.o
+00001790: 005f 0068 0065 0072 006f 0062 0069 007a  ._.h.e.r.o.b.i.z
+000017a0: 005f 0064 0065 006e 0074 0061 006c 7653  ._.d.e.n.t.a.lvS
+000017b0: 726e 6c6f 6e67 0000 0001 0000 0005 006d  rnlong.........m
+000017c0: 0065 0064 0069 0061 6c67 3153 636f 6d70  .e.d.i.alg1Scomp
+000017d0: 0000 0000 0047 95c5 0000 0005 006d 0065  .....G.......m.e
+000017e0: 0064 0069 0061 6d6f 4444 626c 6f62 0000  .d.i.amoDDblob..
+000017f0: 0008 05ec b338 88ea c541 0000 0005 006d  .....8...A.....m
+00001800: 0065 0064 0069 0061 6d6f 6444 626c 6f62  .e.d.i.amodDblob
+00001810: 0000 0008 05ec b338 88ea c541 0000 0005  .......8...A....
+00001820: 006d 0065 0064 0069 0061 7068 3153 636f  .m.e.d.i.aph1Sco
+00001830: 6d70 0000 0000 0047 e000 0000 0000 0000  mp.....G........
 00001840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000018a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -598,44 +598,44 @@
 00002550: 4100 0000 0400 6400 6900 7300 746d 6f64  A.....d.i.s.tmod
 00002560: 4462 6c6f 6200 0000 08ef 517e 5ee2 f2c5  Dblob.....Q~^...
 00002570: 4100 0000 0400 6400 6900 7300 7470 6831  A.....d.i.s.tph1
 00002580: 5363 6f6d 7000 0000 0003 7e00 0000 0000  Scomp.....~.....
 00002590: 1500 6400 6a00 6100 6e00 6700 6f00 5f00  ..d.j.a.n.g.o._.
 000025a0: 6800 6500 7200 6f00 6200 6900 7a00 5f00  h.e.r.o.b.i.z._.
 000025b0: 6400 6500 6e00 7400 6100 6c62 7773 7062  d.e.n.t.a.lbwspb
-000025c0: 6c6f 6200 0000 b862 706c 6973 7430 30d6  lob....bplist00.
+000025c0: 6c6f 6200 0000 b962 706c 6973 7430 30d6  lob....bplist00.
 000025d0: 0102 0304 0506 0708 0708 0b08 5d53 686f  ............]Sho
 000025e0: 7753 7461 7475 7342 6172 5b53 686f 7754  wStatusBar[ShowT
 000025f0: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
 00002600: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
 00002610: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
 00002620: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
-00002630: 6172 0809 0809 5f10 187b 7b33 3133 2c20  ar...._..{{313, 
-00002640: 3530 7d2c 207b 3132 3332 2c20 3638 377d  50}, {1232, 687}
-00002650: 7d09 0815 232f 3b52 5f6b 6c6d 6e6f 8a00  }...#/;R_klmno..
-00002660: 0000 0000 0001 0100 0000 0000 0000 0d00  ................
-00002670: 0000 0000 0000 0000 0000 0000 0000 8b00  ................
-00002680: 0000 1500 6400 6a00 6100 6e00 6700 6f00  ....d.j.a.n.g.o.
-00002690: 5f00 6800 6500 7200 6f00 6200 6900 7a00  _.h.e.r.o.b.i.z.
-000026a0: 5f00 6400 6500 6e00 7400 6100 6c6c 6731  _.d.e.n.t.a.llg1
-000026b0: 5363 6f6d 7000 0000 0000 a885 9500 0000  Scomp...........
-000026c0: 1500 6400 6a00 6100 6e00 6700 6f00 5f00  ..d.j.a.n.g.o._.
-000026d0: 6800 6500 7200 6f00 6200 6900 7a00 5f00  h.e.r.o.b.i.z._.
-000026e0: 6400 6500 6e00 7400 6100 6c6d 6f44 4462  d.e.n.t.a.lmoDDb
-000026f0: 6c6f 6200 0000 08dd 3bc5 9e64 f2c5 4100  lob.....;..d..A.
-00002700: 0000 1500 6400 6a00 6100 6e00 6700 6f00  ....d.j.a.n.g.o.
-00002710: 5f00 6800 6500 7200 6f00 6200 6900 7a00  _.h.e.r.o.b.i.z.
-00002720: 5f00 6400 6500 6e00 7400 6100 6c6d 6f64  _.d.e.n.t.a.lmod
-00002730: 4462 6c6f 6200 0000 08dd 3bc5 9e64 f2c5  Dblob.....;..d..
-00002740: 4100 0000 1500 6400 6a00 6100 6e00 6700  A.....d.j.a.n.g.
-00002750: 6f00 5f00 6800 6500 7200 6f00 6200 6900  o._.h.e.r.o.b.i.
-00002760: 7a00 5f00 6400 6500 6e00 7400 6100 6c70  z._.d.e.n.t.a.lp
-00002770: 6831 5363 6f6d 7000 0000 0000 adf0 0000  h1Scomp.........
-00002780: 0000 1500 6400 6a00 6100 6e00 6700 6f00  ....d.j.a.n.g.o.
-00002790: 5f00 6800 6500 7200 6f00 6200 6900 7a00  _.h.e.r.o.b.i.z.
-000027a0: 5f00 6400 6500 6e00 7400 6100 6c76 5372  _.d.e.n.t.a.lvSr
-000027b0: 6e6c 6f6e 6700 0000 0100 0000 0500 6d00  nlong.........m.
-000027c0: 6500 6400 6900 616c 6731 5363 6f6d 7000  e.d.i.alg1Scomp.
-000027d0: 0000 0000 4795 c500 0000 0500 6d00 6500  ....G.......m.e.
-000027e0: 6400 6900 616d 6f44 4462 6c6f 6200 0000  d.i.amoDDblob...
-000027f0: 0805 ecb3 3888 eac5 4100 0000 0500 6d00  ....8...A.....m.
-00002800: 6500 6400                                e.d.
+00002630: 6172 0809 0809 5f10 197b 7b31 3133 332c  ar...._..{{1133,
+00002640: 2031 3033 7d2c 207b 3932 302c 2034 3336   103}, {920, 436
+00002650: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8b  }}...#/;R_klmno.
+00002660: 0000 0000 0000 0101 0000 0000 0000 000d  ................
+00002670: 0000 0000 0000 0000 0000 0000 0000 008c  ................
+00002680: 0000 0015 0064 006a 0061 006e 0067 006f  .....d.j.a.n.g.o
+00002690: 005f 0068 0065 0072 006f 0062 0069 007a  ._.h.e.r.o.b.i.z
+000026a0: 005f 0064 0065 006e 0074 0061 006c 6c67  ._.d.e.n.t.a.llg
+000026b0: 3153 636f 6d70 0000 0000 00a8 8595 0000  1Scomp..........
+000026c0: 0015 0064 006a 0061 006e 0067 006f 005f  ...d.j.a.n.g.o._
+000026d0: 0068 0065 0072 006f 0062 0069 007a 005f  .h.e.r.o.b.i.z._
+000026e0: 0064 0065 006e 0074 0061 006c 6d6f 4444  .d.e.n.t.a.lmoDD
+000026f0: 626c 6f62 0000 0008 dd3b c59e 64f2 c541  blob.....;..d..A
+00002700: 0000 0015 0064 006a 0061 006e 0067 006f  .....d.j.a.n.g.o
+00002710: 005f 0068 0065 0072 006f 0062 0069 007a  ._.h.e.r.o.b.i.z
+00002720: 005f 0064 0065 006e 0074 0061 006c 6d6f  ._.d.e.n.t.a.lmo
+00002730: 6444 626c 6f62 0000 0008 dd3b c59e 64f2  dDblob.....;..d.
+00002740: c541 0000 0015 0064 006a 0061 006e 0067  .A.....d.j.a.n.g
+00002750: 006f 005f 0068 0065 0072 006f 0062 0069  .o._.h.e.r.o.b.i
+00002760: 007a 005f 0064 0065 006e 0074 0061 006c  .z._.d.e.n.t.a.l
+00002770: 7068 3153 636f 6d70 0000 0000 00ad f000  ph1Scomp........
+00002780: 0000 0015 0064 006a 0061 006e 0067 006f  .....d.j.a.n.g.o
+00002790: 005f 0068 0065 0072 006f 0062 0069 007a  ._.h.e.r.o.b.i.z
+000027a0: 005f 0064 0065 006e 0074 0061 006c 7653  ._.d.e.n.t.a.lvS
+000027b0: 726e 6c6f 6e67 0000 0001 0000 0005 006d  rnlong.........m
+000027c0: 0065 0064 0069 0061 6c67 3153 636f 6d70  .e.d.i.alg1Scomp
+000027d0: 0000 0000 0047 95c5 0000 0005 006d 0065  .....G.......m.e
+000027e0: 0064 0069 0061 6d6f 4444 626c 6f62 0000  .d.i.amoDDblob..
+000027f0: 0008 05ec b338 88ea c541 0000 0005 006d  .....8...A.....m
+00002800: 0065 0064                                .e.d
```

### Comparing `django_herobiz_dental-2.0.0/LICENSE` & `django_herobiz_dental-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/README.md` & `django_herobiz_dental-2.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-### django-herobiz-ds
+### django-herobiz-dental
 
 #### Introduction 
 demiansoft homepage templates
 
 블로그 포스트를 위해 admin에서 markdown 형식으로 글작성이 가능하다. 단, 이미지 삽입시 responsive 를 위해 class=img-fluid 클래스명 설정이
 필요하며 마크다운 에디터에서 이미지 마크 다운에 {: .img-fluid}를 넣어줘야 적용이 된다.
 
@@ -125,15 +125,15 @@
         ],
     }
 } 
 ```
 
 in the shell
 ```
->> pip install django-herobiz-ds
+>> pip install django-herobiz-dental
 >> python manage.py makemigrations django_calendards django_modalds
 >> python manage.py migrate
 >> python manage.py createsuperuser
 ```
 
 
 urls.py
@@ -141,22 +141,22 @@
 from django.contrib import admin  
 from django.urls import path, include  
 from django.conf import settings  
 from django.conf.urls.static import static  
   
 urlpatterns = [  
     path('admin/', admin.site.urls),  
-    path('', include('django_herobiz_ds.urls')),  
+    path('', include('django_herobiz_dental.urls')),  
 ] + static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
 ```
 
 ---
 #### Composition
 
-프로젝트 내의 \_data 폴더 안에 herobizds.py 파일을 생성하고 다음과 같은 형식으로 작성한다.(예제 파일 참조)
+프로젝트 내의 \_data 폴더 안에 herobizdental.py 파일을 생성하고 다음과 같은 형식으로 작성한다.(예제 파일 참조)
 
 ```
 context = {
     "color": '-orange',  # ['', '-blue', '-green', '-orange', '-purple', '-red', '-pink']
     "hero_type": 'fullscreen',  # ['animated', 'carousel', 'fullscreen', 'static']
 }
```

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/admin.py` & `django_herobiz_dental-2.1.0/django_herobiz_dental/admin.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/forms.py` & `django_herobiz_dental-2.1.0/django_herobiz_dental/forms.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/migrations/0001_initial.py` & `django_herobiz_dental-2.1.0/django_herobiz_dental/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/migrations/0003_portfolio_client_post_profile.py` & `django_herobiz_dental-2.1.0/django_herobiz_dental/migrations/0003_portfolio_client_post_profile.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/models.py` & `django_herobiz_dental-2.1.0/django_herobiz_dental/models.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/sitemaps.py` & `django_herobiz_dental-2.1.0/django_herobiz_dental/sitemaps.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/css/main.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/css/main.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/css/variables-blue.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/css/variables-blue.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/css/variables-green.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/css/variables-green.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/css/variables-orange.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/css/variables-orange.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/css/variables-pink.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/css/variables-pink.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/css/variables-purple.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/css/variables-purple.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/css/variables-red.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/css/variables-red.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/css/variables.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/css/variables.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/img/about-bg.png` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/img/about-bg.png`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/img/faq.jpg` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/img/faq.jpg`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/img/hero-bg.png` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/img/hero-bg.png`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/img/onfocus-content-bg.jpg` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/img/onfocus-content-bg.jpg`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/img/pricing-bg.jpg` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/img/pricing-bg.jpg`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/js/main.js` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/js/main.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/_footer.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/_footer.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/_general.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/_general.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/_header.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/_index.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/_index.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/_nav.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/_portfolio-details.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/_portfolio-details.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_comments.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/blog/_comments.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_details.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/blog/_details.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_pagination.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/blog/_pagination.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_posts-list.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/blog/_posts-list.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_sidebar.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/blog/_sidebar.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_about.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_about.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_contact.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_contact.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_cta.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_cta.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_faq.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_faq.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_featured-services.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_featured-services.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_features.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_features.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-animated.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-animated.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-fullscreen.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-fullscreen.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-static.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-static.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_hero.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_hero.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_onfocus.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_onfocus.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_portfolio.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_portfolio.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_pricing.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_pricing.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_recent-blog-posts.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_recent-blog-posts.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_services.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_services.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_team.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_team.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/index/_testimonials.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/index/_testimonials.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/variables-blue.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/variables-blue.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/variables-green.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/variables-green.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/variables-orange.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/variables-orange.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/variables-pink.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/variables-pink.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/variables-purple.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/variables-purple.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/variables-red.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/variables-red.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/scss/variables.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/scss/variables.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.cjs.js` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.cjs.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.esm.js` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.esm.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.js` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.js.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.json` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.min.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.scss` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.css.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.min.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.css.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.css.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.min.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.css.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.min.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.min.css.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.css.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.min.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.js` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.js.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.js` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.js.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.min.js` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.js` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.js.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.min.js` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.min.js.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/glightbox.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/glightbox.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/glightbox.min.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/plyr.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/plyr.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/plyr.min.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/plyr.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/js/glightbox.js` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/js/glightbox.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/js/glightbox.min.js` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/js/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/isotope-layout/isotope.pkgd.js` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/isotope-layout/isotope.pkgd.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/isotope-layout/isotope.pkgd.min.js` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/isotope-layout/isotope.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/php-email-form/php-email-form.php` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/php-email-form/php-email-form.php`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/php-email-form/validate.js` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.css` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.js` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.js.map` & `django_herobiz_dental-2.1.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_about.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_about.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_contact.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_contact.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_cta.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_cta.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_faq.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_faq.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_featured-services.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_featured-services.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_features.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_features.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_hero-animated.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_hero-animated.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_hero-carousel.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_hero-carousel.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_hero-fullscreen.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_hero-fullscreen.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_hero-static.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_hero-static.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_onfocus.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_onfocus.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_portfolio.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_portfolio.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_pricing.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_pricing.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_recent-blog-posts.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_recent-blog-posts.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_services.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_services.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_sidebar.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_sidebar.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_team.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_team.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/_testimonials.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/_testimonials.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/blog-details.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/blog-details.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/blog.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/blog.html`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     <div class="container" data-aos="fade-up">
       <div class="row g-5">
         <div class="col-lg-8">
           <div class="row gy-4 posts-list">
             {% for item in page_obj %}
             <div class="col-lg-6">
               <article class="d-flex flex-column">
-                <div class="post-img">
+                <div class="post-img ratio ratio-4x3">
                   <img src="{{ item.thumbnail.url }}" alt="" class="img-fluid">
                 </div>
                 <h2 class="title">
                   <a href="{% url 'herobizdental:post_detail' item.slug %}">{{ item.title }}</a>
                 </h2>
                 <div class="meta-top">
                   <ul>
```

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/footer.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/footer.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/forms/contact.php` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/forms/contact.php`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/header.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/header.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/index.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/index.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/portfolio-details.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/portfolio-details.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/privacy.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/privacy.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/seo.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/seo.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templates/herobizdental/terms.html` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templates/herobizdental/terms.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/templatetags/herobizdental_tags.py` & `django_herobiz_dental-2.1.0/django_herobiz_dental/templatetags/herobizdental_tags.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/urls.py` & `django_herobiz_dental-2.1.0/django_herobiz_dental/urls.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/django_herobiz_dental/views.py` & `django_herobiz_dental-2.1.0/django_herobiz_dental/views.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.0.0/pyproject.toml` & `django_herobiz_dental-2.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django_herobiz_dental"
-version = "2.0.0"
+version = "2.1.0"
 description = "my demiansoft templates"
 authors = [{name = "Hyungjin Kim", email = "hj3415@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
     "Django >= 4.2.11",
```

### Comparing `django_herobiz_dental-2.0.0/PKG-INFO` & `django_herobiz_dental-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_herobiz_dental
-Version: 2.0.0
+Version: 2.1.0
 Summary: my demiansoft templates
 Author-email: Hyungjin Kim <hj3415@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django >= 4.2.11
 Requires-Dist: libsass>=0.23.0
 Requires-Dist: django-analyticsds >= 0.3.1
@@ -15,15 +15,15 @@
 Requires-Dist: django-hitcount >= 1.3.5
 Requires-Dist: django-taggit >= 5.0.1
 Requires-Dist: django-markdownify >= 0.9.3
 Requires-Dist: django-light >= 0.1.0
 Requires-Dist: pillow >= 10.3.0
 Project-URL: Home, https://www.demiansoft.com
 
-### django-herobiz-ds
+### django-herobiz-dental
 
 #### Introduction 
 demiansoft homepage templates
 
 블로그 포스트를 위해 admin에서 markdown 형식으로 글작성이 가능하다. 단, 이미지 삽입시 responsive 를 위해 class=img-fluid 클래스명 설정이
 필요하며 마크다운 에디터에서 이미지 마크 다운에 {: .img-fluid}를 넣어줘야 적용이 된다.
 
@@ -146,15 +146,15 @@
         ],
     }
 } 
 ```
 
 in the shell
 ```
->> pip install django-herobiz-ds
+>> pip install django-herobiz-dental
 >> python manage.py makemigrations django_calendards django_modalds
 >> python manage.py migrate
 >> python manage.py createsuperuser
 ```
 
 
 urls.py
@@ -162,22 +162,22 @@
 from django.contrib import admin  
 from django.urls import path, include  
 from django.conf import settings  
 from django.conf.urls.static import static  
   
 urlpatterns = [  
     path('admin/', admin.site.urls),  
-    path('', include('django_herobiz_ds.urls')),  
+    path('', include('django_herobiz_dental.urls')),  
 ] + static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
 ```
 
 ---
 #### Composition
 
-프로젝트 내의 \_data 폴더 안에 herobizds.py 파일을 생성하고 다음과 같은 형식으로 작성한다.(예제 파일 참조)
+프로젝트 내의 \_data 폴더 안에 herobizdental.py 파일을 생성하고 다음과 같은 형식으로 작성한다.(예제 파일 참조)
 
 ```
 context = {
     "color": '-orange',  # ['', '-blue', '-green', '-orange', '-purple', '-red', '-pink']
     "hero_type": 'fullscreen',  # ['animated', 'carousel', 'fullscreen', 'static']
 }
```

