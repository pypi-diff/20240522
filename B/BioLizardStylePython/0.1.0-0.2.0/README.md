# Comparing `tmp/biolizardstylepython-0.1.0.tar.gz` & `tmp/biolizardstylepython-0.2.0.tar.gz`

## Comparing `biolizardstylepython-0.1.0.tar` & `biolizardstylepython-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,111 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 biolizardstylepython-0.1.0/src/BioLizardStylePython/__init__.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 biolizardstylepython-0.1.0/src/BioLizardStylePython/lizard_style.mplstyle
--rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 biolizardstylepython-0.1.0/src/BioLizardStylePython/utils.py
--rw-r--r--   0        0        0    18462 2020-02-02 00:00:00.000000 biolizardstylepython-0.1.0/src/BioLizardStylePython/logo/BiolizardLogo.png
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 biolizardstylepython-0.1.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 biolizardstylepython-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biolizardstylepython-0.1.0/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 biolizardstylepython-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 biolizardstylepython-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0   131914 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/An_Iris_Plot.pdf
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0   876501 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/example.ipynb
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0   110420 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0    52356 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/doctrees/example.doctree
+-rw-r--r--   0        0        0    13763 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/.buildinfo
+-rw-r--r--   0        0        0    46405 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/example.html
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/genindex.html
+-rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/index.html
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/objects.inv
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/search.html
+-rw-r--r--   0        0        0    10372 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/searchindex.js
+-rw-r--r--   0        0        0    93836 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/0b62c5d77832e640292907e786b9e94a81637b91291dfb320c90506892318d07.png
+-rw-r--r--   0        0        0    27849 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/19308f5bdbc9e63735bdbdb049919fec4293ede53e5dfc1f32afd55501923b38.png
+-rw-r--r--   0        0        0    92699 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/2147426cd8cb9356b1f20f52b821c3b9f9567b6c809d01005a168570ade96178.png
+-rw-r--r--   0        0        0    23130 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/333c2671c9a22cd7206e31154806dce3965dd8db2564c3797698dea05494befb.png
+-rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/33bf448d38c18d5aef32e418d40c5ceafce7090c5f21ee87ee4632790d64e991.png
+-rw-r--r--   0        0        0    42506 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/37f906bbf66861e679185b6a16ecf57474a2df12e1e79a7e39a30ba05bb4d910.png
+-rw-r--r--   0        0        0    30875 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/42347cb44762cf256eab64bef7799ac910a925808bcb68d2a0b1da40d9fd6b44.png
+-rw-r--r--   0        0        0    42675 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/498a0750907b8420a4f68866aa2431ea84b991d0426e5c70c3cd2d459c98c6ac.png
+-rw-r--r--   0        0        0    38780 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/5196919949527e58e158422dd3aac6b970c50bb378a1e7498c0435a536339b6a.png
+-rw-r--r--   0        0        0    13946 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/5346d1f8a5ddaa1e3053a224d6d4f64671b2f8fa0b4279b4e51b3268214ada54.png
+-rw-r--r--   0        0        0    24406 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/6667099494a9e2a8781deb2699c2d588b6b34cc6d562aadbcbd1a8998b87a2b4.png
+-rw-r--r--   0        0        0    40800 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/6c4670c6cc47869a1b1bdd06a0dbb63d14cde8b230382bee7dbf249322dce7da.png
+-rw-r--r--   0        0        0    47429 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/a64cfc2da9d7de9a042d16e0d7c3bd280dc9de9c282d38fcfa7d00365c5e0c5e.png
+-rw-r--r--   0        0        0    15866 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/b8ca0027099c5da56fedc334a1f73357da86c9d46cf062dcc9ca95128c3235bd.png
+-rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/be891a2e155538d052ab0f79b67d1f78e9f1afa88f2f2bd049bbbf21b2ac334f.png
+-rw-r--r--   0        0        0    14334 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/c95df1ae33d8434db90767ea013463cceaff120ebd5a4b31656e3b3c7bc54b68.png
+-rw-r--r--   0        0        0    36503 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/e0eb9efbbb5d6c2edfa6e2e5eae32a1095e863a1e7ea7882ab17bc688ead946a.png
+-rw-r--r--   0        0        0    19952 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/e4d4d95c9b8c8eebb77f7f7bc9a2e9a3a7fbfdf094d7369e155a4ca19f5dc640.png
+-rw-r--r--   0        0        0    22099 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_images/ee4d9b21369f8f804d953b040ea44e26df1667d24a7e172d43dce6bcdba29a4c.png
+-rw-r--r--   0        0        0   604621 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_sources/example.ipynb.txt
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_sources/index.md.txt
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/basic.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/doctools.js
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/file.png
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/jquery.js
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0        0        0    39364 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0   135314 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0        0        0    93836 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/0b62c5d77832e640292907e786b9e94a81637b91291dfb320c90506892318d07.png
+-rw-r--r--   0        0        0    27849 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/19308f5bdbc9e63735bdbdb049919fec4293ede53e5dfc1f32afd55501923b38.png
+-rw-r--r--   0        0        0    92699 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/2147426cd8cb9356b1f20f52b821c3b9f9567b6c809d01005a168570ade96178.png
+-rw-r--r--   0        0        0    23130 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/333c2671c9a22cd7206e31154806dce3965dd8db2564c3797698dea05494befb.png
+-rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/33bf448d38c18d5aef32e418d40c5ceafce7090c5f21ee87ee4632790d64e991.png
+-rw-r--r--   0        0        0    42506 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/37f906bbf66861e679185b6a16ecf57474a2df12e1e79a7e39a30ba05bb4d910.png
+-rw-r--r--   0        0        0    30875 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/42347cb44762cf256eab64bef7799ac910a925808bcb68d2a0b1da40d9fd6b44.png
+-rw-r--r--   0        0        0    42675 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/498a0750907b8420a4f68866aa2431ea84b991d0426e5c70c3cd2d459c98c6ac.png
+-rw-r--r--   0        0        0    38780 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/5196919949527e58e158422dd3aac6b970c50bb378a1e7498c0435a536339b6a.png
+-rw-r--r--   0        0        0    13946 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/5346d1f8a5ddaa1e3053a224d6d4f64671b2f8fa0b4279b4e51b3268214ada54.png
+-rw-r--r--   0        0        0    24406 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/6667099494a9e2a8781deb2699c2d588b6b34cc6d562aadbcbd1a8998b87a2b4.png
+-rw-r--r--   0        0        0    40800 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/6c4670c6cc47869a1b1bdd06a0dbb63d14cde8b230382bee7dbf249322dce7da.png
+-rw-r--r--   0        0        0    47429 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/a64cfc2da9d7de9a042d16e0d7c3bd280dc9de9c282d38fcfa7d00365c5e0c5e.png
+-rw-r--r--   0        0        0    15866 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/b8ca0027099c5da56fedc334a1f73357da86c9d46cf062dcc9ca95128c3235bd.png
+-rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/be891a2e155538d052ab0f79b67d1f78e9f1afa88f2f2bd049bbbf21b2ac334f.png
+-rw-r--r--   0        0        0    14334 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/c95df1ae33d8434db90767ea013463cceaff120ebd5a4b31656e3b3c7bc54b68.png
+-rw-r--r--   0        0        0    36503 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/e0eb9efbbb5d6c2edfa6e2e5eae32a1095e863a1e7ea7882ab17bc688ead946a.png
+-rw-r--r--   0        0        0    19952 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/e4d4d95c9b8c8eebb77f7f7bc9a2e9a3a7fbfdf094d7369e155a4ca19f5dc640.png
+-rw-r--r--   0        0        0    22099 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/ee4d9b21369f8f804d953b040ea44e26df1667d24a7e172d43dce6bcdba29a4c.png
+-rw-r--r--   0        0        0   604620 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/docs/_build/jupyter_execute/example.ipynb
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/src/BioLizardStylePython/__init__.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/src/BioLizardStylePython/lizard_style.mplstyle
+-rw-r--r--   0        0        0     9065 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/src/BioLizardStylePython/utils.py
+-rw-r--r--   0        0        0    18462 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/src/BioLizardStylePython/logo/BiolizardLogo.png
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/tests/test_palettes.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/tests/test_plots.py
+-rw-r--r--   0        0        0    10389 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/tests/baseline_images/test_plots/div_cmapplot.png
+-rw-r--r--   0        0        0    37488 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/tests/baseline_images/test_plots/irisplot.png
+-rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/tests/baseline_images/test_plots/irisplot_box.png
+-rw-r--r--   0        0        0    43620 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/tests/baseline_images/test_plots/irisplot_dens.png
+-rw-r--r--   0        0        0    47190 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/tests/baseline_images/test_plots/lineplot.png
+-rw-r--r--   0        0        0    10116 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/tests/baseline_images/test_plots/seq_cmapplot.png
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/README.md
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 biolizardstylepython-0.2.0/PKG-INFO
```

### Comparing `biolizardstylepython-0.1.0/src/BioLizardStylePython/lizard_style.mplstyle` & `biolizardstylepython-0.2.0/src/BioLizardStylePython/lizard_style.mplstyle`

 * *Files 15% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 ## ***************************************************************************
 ## * PATCHES                                                                 *
 ## ***************************************************************************
 ## Patches are graphical objects that fill 2D space, like polygons or circles.
 
 patch.linewidth: 0 # edge width in points.
-patch.facecolor: 348ABD  # blue
+patch.facecolor: 01a086  # BLZ green
 patch.edgecolor: EEEEEE
 patch.antialiased: True # render patches in antialiased (no jaggies)
 
 ## ***************************************************************************
 ## * FONT                                                                    *
 ## ***************************************************************************
 font.family: sans-serif
-font.sans-serif: Avenir LT Std
+font.sans-serif: Lato
 font.size: 14
 
 ## ***************************************************************************
 ## * AXES                                                                    *
 ## ***************************************************************************
 
 axes.facecolor: white # axes background color
@@ -37,20 +37,16 @@
 axes.titlelocation: left   # alignment of the title: {left, right, center}
 axes.labelsize: 15 # font size of the x and y labels
 axes.spines.top:    False #Axis line at top of plot
 axes.spines.right:  False #Axis line at right of plot
 
 
 #Biolizard qualitative color palette (e.g. when plotting multiple lines)
-#Starts of with 'biolizard' dark gray -> green -> yellow, followed by other colors in palette
-#This palette is inspired by Martin Krzywinski's "12-COLOR PALETTE FOR COLORBLINESS"
-#and is infused with the signature house colors of Biolizard for the first three shades.
-#Tailored to be inclusive, it is friendly for those with the prevalent form of color blindness: Deuteranopia (Red-Green Color Blindness).
 
-axes.prop_cycle: cycler('color', ['1e2237', '01a086', 'e9b940','00C2F9', 'FF6E3A', '8400CD', 'FFB2FD', 'A40122','008DF9','00FCCF','E20134','FF5AAF','A40122'])
+axes.prop_cycle: cycler('color', ['01a086', '1e2237', 'e9b940','105144', '6CC7B7', '233E60', '666666', 'D6D6D6'])
 
 #TICKS
 
 xtick.color: 555555
 xtick.direction: out # direction: {in, out, inout}
 ytick.color: 555555
 ytick.direction: out # direction: {in, out, inout}
```

### Comparing `biolizardstylepython-0.1.0/src/BioLizardStylePython/utils.py` & `biolizardstylepython-0.2.0/src/BioLizardStylePython/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,203 +1,236 @@
-import os
-import io
-import numpy as np
-from PIL import Image
-import matplotlib.pyplot as plt
-import matplotlib.colors
-import colorspace
-
-def lizard_style(font_name='Nunito Sans 10pt'):
-    """
-    Load and apply the lizard_style for matplotlib plots.
-
-    Parameters:
-    -----------
-    font_name : str, optional
-        The name of the font to be used for the plots. By default, it uses 'Nunito Sans 10pt'.
-        If you want to use your own local installation of Nunito Sans or any other font,
-        specify the font name using this parameter. For more details on how to use
-        the font_name parameter, refer to the 'In_Action' file on GitHub.
-
-    Example:
-    --------
-    #>>> lizard_style(font_name='Nunito')
-
-    Notes:
-    ------
-    Ensure that the specified font is installed on your system and is recognized by matplotlib.
-
-    """
-    style_path = os.path.join(os.path.dirname(__file__), 'lizard_style.mplstyle')
-    plt.style.use(style_path)
-    plt.rcParams['font.sans-serif'] = [font_name]
-
-
-
-def biolizard_qualitative_pal():
-    """
-    Generate a qualitative colormap for matplotlib.
-
-    This colormap is inspired by Martin Krzywinski's "12-COLOR PALETTE FOR COLORBLINDNESS"
-    and incorporates the signature house colors of BioLizard for the first three shades.
-    Specifically designed to be inclusive, it is suitable for individuals with the most
-    common form of color blindness: Deuteranopia (Red-Green Color Blindness).
-
-    Returns:
-        matplotlib.colors.ListedColormap: A colormap object suitable for use with matplotlib plots.
-
-    Example:
-        #>>> bar_colors = [biolizard_qualitative_pal(i) for i in range(len(categories))]
-        #>>> bars = plt.bar(categories, values, color=bar_colors)
-        #>>> plt.show()
-    """
-    return matplotlib.colors.ListedColormap([
-        "#01a086", "#1e2237", "#e9b940", "#00C2F9", "#FF6E3A", "#00FCCF",
-        "#8400CD", "#E20134", "#008DF9","#FFB2FD", "#FF5AAF", "#A40122"
-    ])
-
-#Sequential and divergent color map
-#These two color maps will be registered as 'biolizard_<sequential/divergent>_pal' when installing the package.
-
-#Internal function
-def create_and_register_colormap(palette, name):
-    """
-    Create and register a colormap with matplotlib.
-
-    This function generates a colormap from a given palette and registers it with
-    matplotlib under the specified name.
-
-    Parameters:
-    - palette (function): A function that returns a list of colors.
-    - name (str): The name under which the colormap will be registered with matplotlib.
-
-    Example:
-    #>>> biolizard_sequential_pal = colorspace.sequential_hcl(h=170, c=[40,0,75], l=[35,90], power=1)
-    #>>> create_and_register_colormap(biolizard_sequential_pal, "biolizard_sequential_pal")
-    """
-    colors = palette(256)
-    rgbcolors = [matplotlib.colors.to_rgb(color) for color in colors]
-    cmap = matplotlib.colors.LinearSegmentedColormap.from_list(name, rgbcolors)
-    if name == "biolizard_sequential_pal":
-        cmap = cmap.reversed() # Reverse the order of the colors
-    matplotlib.colormaps.register(name=name, cmap=cmap)
-
-# Sequential Biolizard Color Map
-#
-# This colormap applies the sequential Biolizard palette.
-#
-# Details:
-# The sequential palette represents underlying values using a consistent sequence of increasing luminance.
-# The hue is derived from the Biolizard green. The palette utilizes gradients within the HCL-spectrum for perceptual uniformity.
-# The chroma follows a triangular progression to help differentiate the middle range values from the extreme values.
-biolizard_sequential_pal = colorspace.sequential_hcl(h=170, c=[40,0,75], l=[35,90], power=1)
-create_and_register_colormap(biolizard_sequential_pal, "biolizard_sequential_pal")
-
-# Divergent Biolizard Color Map
-#
-# This colormap applies the divergent Biolizard palette for scenarios where color corresponds to categories with a natural midpoint.
-#
-# Details:
-# This divergent palette codes underlying numeric values by a triangular luminance sequence with different hues
-# in the left and in the right "arms" of the palette. Specifically:
-# (a) a single hue is used for each arm of the palette,
-# (b) chroma and luminance trajectory are balanced between the two arms,
-# (c) the neutral central value has zero chroma.
-# The palette is crafted using hue 291 and hue 170, which is the distinctive biolizard green.
-# This unique hue pairing produces a palette that remains accessible for all major forms of color blindness.
-biolizard_divergent_pal = colorspace.diverging_hcl(h=[291, 170], c=80, l=[35, 95], power=1)
-create_and_register_colormap(biolizard_divergent_pal, "biolizard_divergent_pal")
-
-def finalise_lizardplot(plot, source_text, fontsize=12, pdf=False, output_name="TempLizardPlot", save_filepath=None):
-    """
-   Finalise and save a plot with custom adjustments and a source text.
-
-   This function takes a provided plot, adjusts its layout, and appends a footer
-   at the bottom containing a source text and a logo. The combined image is then saved
-   either as a PNG or a PDF.
-
-   Parameters:
-   - plot (matplotlib.figure.Figure): The input plot to be finalized.
-   - source_text (str): The source text to be displayed at the bottom of the plot.
-   - fontsize (int, optional): Font size of the source text. Defaults to 12.
-   - pdf (bool, optional): If True, saves the output as a PDF. Otherwise, saves as a PNG. Defaults to False.
-   - output_name (str, optional): Name of the output file (without extension). Defaults to "TempLizardPlot".
-   - save_filepath (str, optional): Full path to save the output (with extension). If specified, it takes precedence over output_name.
-
-   Returns:
-   None. The combined image is saved to the specified location or the current working directory.
-
-   Example:
-   #>>> fig, ax = plt.subplots()
-   #>>> ax.plot([0, 1], [0, 1])
-   #>>> finalise_lizardplot(fig, "Source: BioLizard Data", pdf=True)
-   """
-    # Adjust the provided plot
-    plot.subplots_adjust(left=0.11, bottom=0.13, right=0.95)
-
-    # Save the adjusted plot to a temporary buffer
-    buf = io.BytesIO()
-    dpi = 300  # Increased DPI for higher resolution
-    plot.savefig(buf, format='png', pad_inches=0.1, dpi=dpi)
-    buf.seek(0)
-    img2 = Image.open(buf)
-
-    # Get the width of the saved plot in pixels
-    swarmplot_width, _ = img2.size
-
-    # Adjust the width and height of the custom figure to match the width of the plot in pixels
-    custom_fig_width_inches = swarmplot_width / dpi
-    custom_fig_height_inches = 0.4  # Reduced height
-
-    fig1 = plt.figure(figsize=(custom_fig_width_inches, custom_fig_height_inches))
-    ax = fig1.add_axes([0, 0, 1, 1])
-    ax.plot([0, 1], [1, 1], color='black', linewidth=1.5, transform=ax.transAxes)
-
-    font_name = plt.rcParams['font.sans-serif'][0]
-
-    ax.text(0.05, 0.5, source_text, verticalalignment='center', transform=ax.transAxes, fontsize=fontsize,
-            fontname=font_name)
-
-    ax_image = fig1.add_axes([0.90, -0.09, 0.10, 1], anchor='NE', zorder=-1)
-
-    # Get the directory of the current script
-    current_directory = os.path.dirname(os.path.abspath(__file__))
-    # Construct the path to the image
-    image_path = os.path.join(current_directory, 'logo', 'BiolizardLogo.png')
-    # Read the image
-    img = plt.imread(image_path)
-
-    ax_image.imshow(img)
-    ax_image.axis('off')
-    ax.axis('off')
-
-    # Save the custom figure to a temporary buffer
-    buf1 = io.BytesIO()
-    fig1.savefig(buf1, format='png', pad_inches=0.1, dpi=dpi)
-    buf1.seek(0)
-    img1 = Image.open(buf1)
-    plt.close(fig1)
-
-    # Concatenate the two images vertically
-    combined_img = Image.new('RGB', (swarmplot_width, img1.height + img2.height))
-    combined_img.paste(img2, (0, 0))
-    combined_img.paste(img1, (0, img2.height))
-
-    # Save the concatenated image
-    if pdf:
-        if save_filepath:
-            filename = save_filepath
-        else:
-            filename = output_name + '.pdf'
-        combined_img.save(filename, "PDF", resolution=100.0)
-    else:
-        if save_filepath:
-            filename = save_filepath
-        else:
-            filename = output_name + '.png'
-        combined_img.save(filename)
-
-
-
-
-
-
+import os
+import io
+# import numpy as np
+from PIL import Image
+from pathlib import Path
+import matplotlib.pyplot as plt
+import matplotlib.colors
+from matplotlib import font_manager
+import colorspace
+
+# the three basic colors
+blz_green = "#01a086"
+blz_blue = "#1e2237"
+blz_yellow = "#e9b940"
+
+
+def lizard_style():
+    """
+    Load and apply the lizard_style for matplotlib plots.
+
+    Parameters:
+    -----------
+    font_name : str, optional
+        The name of the font to be used for the plots. By default, it uses 'Lato'.
+        If you want to use your own local installation of Lato or any other font,
+        specify the font name using this parameter. For more details on how to use
+        the font_name parameter, refer to the 'In_Action' file on GitHub.
+
+    Example:
+    --------
+    #>>> lizard_style()
+
+    Notes:
+    ------
+    Ensure that the specified font is installed on your system and is recognized by matplotlib.
+
+    """
+    style_path = os.path.join(os.path.dirname(__file__), 'lizard_style.mplstyle')
+    plt.style.use(style_path)
+    from BioLizardStylePython import lato_localname
+    plt.rcParams['font.sans-serif'] = [lato_localname]
+
+
+def biolizard_qualitative_pal():
+    """
+    Generate a qualitative colormap for matplotlib.
+
+    Specifically designed to be inclusive, it is suitable for individuals with the most
+    common form of color blindness: Deuteranopia (Red-Green Color Blindness).
+
+    Returns:
+        matplotlib.colors.ListedColormap: A colormap object suitable for use with matplotlib plots.
+
+    Example:
+        #>>> bar_colors = [biolizard_qualitative_pal(i) for i in range(len(categories))]
+        #>>> bars = plt.bar(categories, values, color=bar_colors)
+        #>>> plt.show()
+    """
+    return matplotlib.colors.ListedColormap([
+        "#01a086", "#1e2237", "#e9b940","#105144",
+        "#6CC7B7", "#233E60", "#666666", "#D6D6D6"
+    ])
+
+def biolizard_qualitative_pal_r():
+    """
+    Generate a qualitative colormap for matplotlib. Colors are reversed compared to biolizard_qualitative_pal.
+
+    Specifically designed to be inclusive, it is suitable for individuals with the most
+    common form of color blindness: Deuteranopia (Red-Green Color Blindness).
+
+    Returns:
+        matplotlib.colors.ListedColormap: A colormap object suitable for use with matplotlib plots.
+
+    Example:
+        #>>> bar_colors = [biolizard_qualitative_pal(i) for i in range(len(categories))]
+        #>>> bars = plt.bar(categories, values, color=bar_colors)
+        #>>> plt.show()
+    """
+    cmap = matplotlib.colors.ListedColormap([
+        "#01a086", "#1e2237", "#e9b940","#105144",
+        "#6CC7B7", "#233E60", "#666666", "#D6D6D6"
+    ])
+
+    return cmap.reversed()
+
+#Sequential and divergent color map
+#These two color maps will be registered as 'biolizard_<sequential/divergent>_pal' when installing the package.
+
+#Internal function
+def _create_and_register_colormap(palette, name, reverse=False):
+    """
+    Create and register a colormap with matplotlib.
+
+    This function generates a colormap from a given palette and registers it with
+    matplotlib under the specified name.
+
+    Parameters:
+    - palette (function): A function that returns a list of colors.
+    - name (str): The name under which the colormap will be registered with matplotlib.
+
+    Example:
+    #>>> biolizard_sequential_pal = colorspace.sequential_hcl(h=170, c=[40,0,75], l=[35,90], power=1)
+    #>>> create_and_register_colormap(biolizard_sequential_pal, "biolizard_sequential_pal")
+    """
+    colors = palette(256)
+    rgbcolors = [matplotlib.colors.to_rgb(color) for color in colors]
+    cmap = matplotlib.colors.LinearSegmentedColormap.from_list(name, rgbcolors)
+    if reverse:
+        cmap = cmap.reversed()
+    matplotlib.colormaps.register(name=name, cmap=cmap)
+
+
+# Sequential Biolizard Color Map
+#
+# This colormap applies the sequential Biolizard palette.
+#
+# Details:
+# The sequential palette represents underlying values using a consistent sequence of increasing luminance.
+# The hue is derived from the Biolizard green. The palette utilizes gradients within the HCL-spectrum for perceptual uniformity.
+# The chroma follows a triangular progression to help differentiate the middle range values from the extreme values.
+biolizard_sequential_pal = colorspace.sequential_hcl(h=170, c=[0,75,40], l=[90,35], power=1)
+_create_and_register_colormap(biolizard_sequential_pal, "biolizard_sequential_pal")
+_create_and_register_colormap(biolizard_sequential_pal, "biolizard_sequential_pal_r", reverse=True)
+
+
+# Divergent Biolizard Color Map
+#
+# This colormap applies the divergent Biolizard palette for scenarios where color corresponds to categories with a natural midpoint.
+#
+# Details:
+# This divergent palette codes underlying numeric values by a triangular luminance sequence with different hues
+# in the left and in the right "arms" of the palette. Specifically:
+# (a) a single hue is used for each arm of the palette,
+# (b) chroma and luminance trajectory are balanced between the two arms,
+# (c) the neutral central value has zero chroma.
+# The palette is crafted using hue 291 and hue 170, which is the distinctive biolizard green.
+# This unique hue pairing produces a palette that remains accessible for all major forms of color blindness.
+biolizard_divergent_pal = colorspace.diverging_hcl(h=[60, 170], c=80, l=[50, 95], power=1)
+_create_and_register_colormap(biolizard_divergent_pal, "biolizard_divergent_pal")
+_create_and_register_colormap(biolizard_divergent_pal, "biolizard_divergent_pal_r", reverse=True)
+
+
+def finalise_lizardplot(plot, source_text, fontsize=12, pdf=False, output_name="TempLizardPlot", save_filepath=None):
+    """
+   Finalise and save a plot with custom adjustments and a source text.
+
+   This function takes a provided plot, adjusts its layout, and appends a footer
+   at the bottom containing a source text and a logo. The combined image is then saved
+   either as a PNG or a PDF.
+
+   Parameters:
+   - plot (matplotlib.figure.Figure): The input plot to be finalized.
+   - source_text (str): The source text to be displayed at the bottom of the plot.
+   - fontsize (int, optional): Font size of the source text. Defaults to 12.
+   - pdf (bool, optional): If True, saves the output as a PDF. Otherwise, saves as a PNG. Defaults to False.
+   - output_name (str, optional): Name of the output file (without extension). Defaults to "TempLizardPlot".
+   - save_filepath (str, optional): Full path to save the output (with extension). If specified, it takes precedence over output_name.
+
+   Returns:
+   None. The combined image is saved to the specified location or the current working directory.
+
+   Example:
+   #>>> fig, ax = plt.subplots()
+   #>>> ax.plot([0, 1], [0, 1])
+   #>>> finalise_lizardplot(fig, "Source: BioLizard Data", pdf=True)
+   """
+    # Adjust the provided plot
+    plot.subplots_adjust(left=0.11, bottom=0.13, right=0.95)
+
+    # Save the adjusted plot to a temporary buffer
+    buf = io.BytesIO()
+    dpi = 300  # Increased DPI for higher resolution
+    plot.savefig(buf, format='png', pad_inches=0.1, dpi=dpi)
+    buf.seek(0)
+    img2 = Image.open(buf)
+
+    # Get the width of the saved plot in pixels
+    swarmplot_width, _ = img2.size
+
+    # Adjust the width and height of the custom figure to match the width of the plot in pixels
+    custom_fig_width_inches = swarmplot_width / dpi
+    custom_fig_height_inches = 0.4  # Reduced height
+
+    fig1 = plt.figure(figsize=(custom_fig_width_inches, custom_fig_height_inches))
+    ax = fig1.add_axes([0, 0, 1, 1])
+    ax.plot([0, 1], [1, 1], color='black', linewidth=1.5, transform=ax.transAxes)
+
+    font_name = plt.rcParams['font.sans-serif'][0]
+
+    ax.text(0.05, 0.5, source_text, verticalalignment='center', transform=ax.transAxes, fontsize=fontsize,
+            fontname=font_name)
+
+    ax_image = fig1.add_axes([0.90, -0.09, 0.10, 1], anchor='NE', zorder=-1)
+
+    # Get the directory of the current script
+    current_directory = os.path.dirname(os.path.abspath(__file__))
+    # Construct the path to the image
+    image_path = os.path.join(current_directory, 'logo', 'BiolizardLogo.png')
+    # Read the image
+    img = plt.imread(image_path)
+
+    ax_image.imshow(img)
+    ax_image.axis('off')
+    ax.axis('off')
+
+    # Save the custom figure to a temporary buffer
+    buf1 = io.BytesIO()
+    fig1.savefig(buf1, format='png', pad_inches=0.1, dpi=dpi)
+    buf1.seek(0)
+    img1 = Image.open(buf1)
+    plt.close(fig1)
+
+    # Concatenate the two images vertically
+    combined_img = Image.new('RGB', (swarmplot_width, img1.height + img2.height))
+    combined_img.paste(img2, (0, 0))
+    combined_img.paste(img1, (0, img2.height))
+
+    # Save the concatenated image
+    if pdf:
+        if save_filepath:
+            filename = save_filepath
+        else:
+            filename = output_name + '.pdf'
+        combined_img.save(filename, "PDF", resolution=100.0)
+    else:
+        if save_filepath:
+            filename = save_filepath
+        else:
+            filename = output_name + '.png'
+        combined_img.save(filename)
+
+
+
+
+
+
```

### Comparing `biolizardstylepython-0.1.0/src/BioLizardStylePython/logo/BiolizardLogo.png` & `biolizardstylepython-0.2.0/src/BioLizardStylePython/logo/BiolizardLogo.png`

 * *Files identical despite different names*

### Comparing `biolizardstylepython-0.1.0/LICENSE` & `biolizardstylepython-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
- Copyright (c) 2023 BioLizard
-
- Permission is hereby granted, free of charge, to any person
- obtaining a copy of this software and associated documentation
- files (the "Software"), to deal in the Software without
- restriction, including without limitation the rights to use,
- copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the
- Software is furnished to do so, subject to the following
- conditions:
-
- The above copyright notice and this permission notice shall be
- included in all copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
- EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
- OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
- NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
- HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
- WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
- FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+ Copyright (c) 2023 BioLizard
+
+ Permission is hereby granted, free of charge, to any person
+ obtaining a copy of this software and associated documentation
+ files (the "Software"), to deal in the Software without
+ restriction, including without limitation the rights to use,
+ copy, modify, merge, publish, distribute, sublicense, and/or sell
+ copies of the Software, and to permit persons to whom the
+ Software is furnished to do so, subject to the following
+ conditions:
+
+ The above copyright notice and this permission notice shall be
+ included in all copies or substantial portions of the Software.
+
+ THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+ EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
+ OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+ NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
+ HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
+ WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+ FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `biolizardstylepython-0.1.0/pyproject.toml` & `biolizardstylepython-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,36 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "BioLizardStylePython"
-version = "0.1.0"
-authors = [
-  { name = "BioLizard"},
-  { name = "Robbe Neirynck", email = "robbe.neirynck1@hotmail.com" }
-]
-description = "Enhance plots with the signature Biolizard aesthetic for matplotlib and seaborn."
-readme = "README.md"
-requires-python = ">=3.9"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-dependencies = [
-    "matplotlib>=3.7.1",
-    "numpy>=1.24.30",
-    "Pillow>=9.4.0"
-]
-
-
-[project.urls]
-"Homepage" = "https://github.com/lizard-bio/nature-grade-visualization-playground/tree/main"
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "BioLizardStylePython"
+version = "0.2.0"
+authors = [
+  { name = "BioLizard", email = "contact@lizard.bio"},
+  { name = "Aniko Meijer", email = "aniko.meijer@lizard.bio"},
+  { name = "Robbe Neirynck" },
+]
+maintainers = [
+  { name = "Alexander Koch", email = "alexander.koch@lizard.bio"},
+  { name = "Aniko Meijer", email = "aniko.meijer@lizard.bio"}
+]
+description = "Enhance plots with the signature Biolizard aesthetic for matplotlib and seaborn."
+readme = "README.md"
+changelog_file = "CHANGELOG.md" 
+requires-python = ">=3.9"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+dependencies = [
+    "matplotlib>=3.7.1",
+    "Pillow>=9.4.0",
+    "fonts>=0.0.3",
+    "font-lato>=0.0.1"
+]
+
+
+[project.urls]
+"Homepage" = "https://github.com/lizard-bio/nature-grade-visualization-playground/tree/main"
```

