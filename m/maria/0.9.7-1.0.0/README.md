# Comparing `tmp/maria-0.9.7.tar.gz` & `tmp/maria-1.0.0.tar.gz`

## Comparing `maria-0.9.7.tar` & `maria-1.0.0.tar`

### file list

```diff
@@ -1,70 +1,100 @@
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 maria-0.9.7/.codecov.yml
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 maria-0.9.7/.cookiecutter-maria.yaml
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 maria-0.9.7/.coveragerc
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 maria-0.9.7/.flake8
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 maria-0.9.7/.gitattributes
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 maria-0.9.7/.isort.cfg
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 maria-0.9.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 maria-0.9.7/CONTRIBUTING.rst
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 maria-0.9.7/pytest.ini
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 maria-0.9.7/setup.cfg
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 maria-0.9.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 maria-0.9.7/.github/workflows/docs.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 maria-0.9.7/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 maria-0.9.7/.github/workflows/release.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 maria-0.9.7/maria/__init__.py
--rw-r--r--   0        0        0    18472 2020-02-02 00:00:00.000000 maria-0.9.7/maria/_version.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 maria-0.9.7/maria/base.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 maria-0.9.7/maria/coords.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maria-0.9.7/maria/errors.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 maria-0.9.7/maria/noise.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 maria-0.9.7/maria/sim.py
--rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 maria-0.9.7/maria/array/__init__.py
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 maria-0.9.7/maria/array/arrays.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 maria-0.9.7/maria/array/band.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 maria-0.9.7/maria/array/dets.py
--rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 maria-0.9.7/maria/atmosphere/__init__.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 maria-0.9.7/maria/atmosphere/engine.py
--rw-r--r--   0        0        0    11592 2020-02-02 00:00:00.000000 maria-0.9.7/maria/atmosphere/turbulent_layer.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 maria-0.9.7/maria/atmosphere/spectra/__init__.py
--rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 maria-0.9.7/maria/atmosphere/weather/__init__.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 maria-0.9.7/maria/cmb/__init__.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 maria-0.9.7/maria/configs/default_params.yml
--rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 maria-0.9.7/maria/map/__init__.py
--rw-r--r--   0        0        0     8718 2020-02-02 00:00:00.000000 maria-0.9.7/maria/map/mappers.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 maria-0.9.7/maria/map/maps.csv
--rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 maria-0.9.7/maria/pointing/__init__.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 maria-0.9.7/maria/pointing/patterns.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 maria-0.9.7/maria/pointing/pointings.yml
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 maria-0.9.7/maria/site/__init__.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 maria-0.9.7/maria/site/regions.csv
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 maria-0.9.7/maria/site/sites.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maria-0.9.7/maria/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maria-0.9.7/maria/tests/conftest.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 maria-0.9.7/maria/tests/test_atmosphere.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 maria-0.9.7/maria/tests/test_coordinates.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 maria-0.9.7/maria/tests/test_map_obs.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 maria-0.9.7/maria/tests/test_mappers.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 maria-0.9.7/maria/tests/test_noise_sims.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 maria-0.9.7/maria/tests/test_objects.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 maria-0.9.7/maria/tests/test_pipeline.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 maria-0.9.7/maria/tests/test_simulation.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 maria-0.9.7/maria/tests/test_spectra.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 maria-0.9.7/maria/tests/test_tod.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 maria-0.9.7/maria/tests/test_weather.py
--rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 maria-0.9.7/maria/tod/__init__.py
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 maria-0.9.7/maria/utils/__init__.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 maria-0.9.7/maria/utils/beam.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 maria-0.9.7/maria/utils/constants.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 maria-0.9.7/maria/utils/functions.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 maria-0.9.7/maria/utils/io.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 maria-0.9.7/maria/utils/linalg.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 maria-0.9.7/maria/utils/tod.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 maria-0.9.7/maria/utils/units.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 maria-0.9.7/maria/utils/weather.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 maria-0.9.7/.gitignore
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 maria-0.9.7/AUTHORS.rst
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 maria-0.9.7/LICENSE
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 maria-0.9.7/README.rst
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 maria-0.9.7/pyproject.toml
--rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 maria-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 maria-1.0.0/.codecov.yml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 maria-1.0.0/.cookiecutter-maria.yaml
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 maria-1.0.0/.coveragerc
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 maria-1.0.0/.flake8
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 maria-1.0.0/.gitattributes
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 maria-1.0.0/.isort.cfg
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 maria-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 maria-1.0.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 maria-1.0.0/pytest.ini
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 maria-1.0.0/setup.cfg
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 maria-1.0.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 maria-1.0.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 maria-1.0.0/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 maria-1.0.0/.github/workflows/testing.yml
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 maria-1.0.0/maria/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 maria-1.0.0/maria/_version.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 maria-1.0.0/maria/constants.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 maria-1.0.0/maria/errors.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 maria-1.0.0/maria/functions.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 maria-1.0.0/maria/io.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 maria-1.0.0/maria/units.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 maria-1.0.0/maria/atmosphere/__init__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 maria-1.0.0/maria/atmosphere/engine.py
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 maria-1.0.0/maria/atmosphere/sim.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 maria-1.0.0/maria/atmosphere/spectrum.py
+-rw-r--r--   0        0        0    12015 2020-02-02 00:00:00.000000 maria-1.0.0/maria/atmosphere/turbulent_layer.py
+-rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 maria-1.0.0/maria/atmosphere/weather.py
+-rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 maria-1.0.0/maria/cmb/__init__.py
+-rw-r--r--   0        0        0    12421 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/__init__.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/beams.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/configs.yml
+-rw-r--r--   0        0        0    10447 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/bands/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/bands/format.csv
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/bands/configs/abs.yml
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/bands/configs/act.yml
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/bands/configs/alma.yml
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/bands/configs/atlast.yml
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/bands/configs/mustang2.yml
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/bands/passbands/mustang2/f093.csv
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/__init__.py
+-rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/aca.cfg
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle1.csv
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle1.f043.csv
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle1.f078.csv
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle1.f100.csv
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle1.f144.csv
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle1.f187.csv
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle1.f243.csv
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle1.f324.csv
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle1.f447.csv
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle1.f661.csv
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle1.f869.csv
+-rw-r--r--   0        0        0    24598 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle1.total.csv
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle10.2.cfg
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle10.3.cfg
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle10.4.cfg
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle10.5.cfg
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle10.6.cfg
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle10.7.cfg
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 maria-1.0.0/maria/instrument/detectors/arrays/alma/alma.cycle10.8.cfg
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 maria-1.0.0/maria/map/Planck_Parchment_RGB.txt
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 maria-1.0.0/maria/map/__init__.py
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 maria-1.0.0/maria/map/map.py
+-rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 maria-1.0.0/maria/map/mappers.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 maria-1.0.0/maria/map/maps.csv
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 maria-1.0.0/maria/noise/__init__.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 maria-1.0.0/maria/noise/levels.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 maria-1.0.0/maria/noise/results_of_instrument_simulation.csv
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 maria-1.0.0/maria/plan/__init__.py
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 maria-1.0.0/maria/plan/patterns.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 maria-1.0.0/maria/plan/plans.yml
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 maria-1.0.0/maria/sim/__init__.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 maria-1.0.0/maria/sim/base.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 maria-1.0.0/maria/sim/params.yml
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 maria-1.0.0/maria/site/__init__.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 maria-1.0.0/maria/site/regions.csv
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 maria-1.0.0/maria/site/sites.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maria-1.0.0/maria/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maria-1.0.0/maria/tests/conftest.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 maria-1.0.0/maria/tests/test_atmosphere.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 maria-1.0.0/maria/tests/test_cmb.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 maria-1.0.0/maria/tests/test_coordinates.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 maria-1.0.0/maria/tests/test_instruments.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 maria-1.0.0/maria/tests/test_mappers.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 maria-1.0.0/maria/tests/test_noise.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 maria-1.0.0/maria/tests/test_pipeline.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 maria-1.0.0/maria/tests/test_plans.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 maria-1.0.0/maria/tests/test_simulation.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 maria-1.0.0/maria/tests/test_sites.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 maria-1.0.0/maria/tests/test_tod.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 maria-1.0.0/maria/utils/__init__.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 maria-1.0.0/maria/utils/linalg.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 maria-1.0.0/maria/utils/signal.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 maria-1.0.0/.gitignore
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 maria-1.0.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 maria-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 maria-1.0.0/README.rst
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 maria-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 maria-1.0.0/PKG-INFO
```

### Comparing `maria-0.9.7/.pre-commit-config.yaml` & `maria-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `maria-0.9.7/CONTRIBUTING.rst` & `maria-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `maria-0.9.7/.github/workflows/ci.yml` & `maria-1.0.0/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `maria-0.9.7/.github/workflows/docs.yml` & `maria-1.0.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `maria-0.9.7/maria/__init__.py` & `maria-1.0.0/maria/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 # AVE MARIA, gratia plena, Dominus tecum.
 # Benedicta tu in mulieribus, et benedictus fructus ventris tui, Iesus.
 # Sancta Maria, Mater Dei, ora pro nobis peccatoribus, nunc, et in hora mortis nostrae.
 
-from ._version import get_versions
-
-__version__ = get_versions()["version"]
-del get_versions
-
-from . import utils  # noqa F401
-from .array import all_arrays, get_array  # noqa F401
-from .map import Map, mappers  # noqa F401
-from .pointing import all_pointings, get_pointing  # noqa F401
-from .sim import Simulation  # noqa F401
-from .site import all_regions, all_sites, get_site  # noqa F401
-from .tod import TOD  # noqa F401
+from . import utils  # noqa
+from ._version import __version__, __version_tuple__  # noqa
+from .instrument import all_instruments, get_instrument  # noqa
+from .map import Map, mappers  # noqa
+from .plan import all_plans, get_plan  # noqa
+from .sim import Simulation  # noqa
+from .site import all_regions, all_sites, get_site  # noqa
```

### Comparing `maria-0.9.7/maria/array/dets.py` & `maria-1.0.0/maria/instrument/detectors/arrays.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,177 +1,182 @@
-from collections.abc import Mapping
+import os
+import warnings
 
-import matplotlib as mpl
 import numpy as np
 import pandas as pd
+from scipy.spatial import ConvexHull
+from scipy.spatial.distance import cdist
 
-from .band import Band
+from ..bands import Band
+from ..beams import compute_angular_fwhm
 
-HEX_CODE_LIST = [
-    mpl.colors.to_hex(mpl.colormaps.get_cmap("Paired")(t))
-    for t in [*np.linspace(0.05, 0.95, 12)]
-]
-
-REQUIRED_DET_CONFIG_KEYS = ["n", "band_center", "band_width"]
-
-det_columns = {
-    "band": "str",
-    "offset_x": "float",
-    "offset_y": "float",
-    "baseline_x": "float",
-    "baseline_y": "float",
-    "baseline_z": "float",
-    "pol_angle": "float",
-}
-
-
-def generate_array_offsets(geometry, field_of_view, n):
-    valid_array_types = ["flower", "hex", "square"]
-
-    if geometry == "flower":
-        phi = np.pi * (3.0 - np.sqrt(5.0))  # golden angle in radians
-        dzs = np.zeros(n).astype(complex)
-        for i in range(n):
-            dzs[i] = np.sqrt((i / (n - 1)) * 2) * np.exp(1j * phi * i)
-        od = np.abs(np.subtract.outer(dzs, dzs))
-        dzs *= field_of_view / od.max()
-        return np.c_[np.real(dzs), np.imag(dzs)]
-    if geometry == "hex":
-        return generate_hex_offsets(n, field_of_view)
-    if geometry == "square":
-        dxy_ = np.linspace(-field_of_view, field_of_view, int(np.ceil(np.sqrt(n)))) / (
-            2 * np.sqrt(2)
+here, this_filename = os.path.split(__file__)
+
+SUPPORTED_ARRAY_PACKINGS = ["hex", "square", "sunflower"]
+SUPPORTED_ARRAY_SHAPES = ["hex", "square", "circle"]
+
+
+def generate_2d_offsets(n, packing="hex", shape="circle", normalize=False):
+    """
+    Generate a scatter of $n$ points with some pattern.
+    These points are spread such that each is a unit of distance away from its nearest neighbor.
+    """
+
+    n = int(np.maximum(n, 1))
+    bigger_n = 2 * n
+
+    if packing == "square":
+        s = int(np.ceil(np.sqrt(bigger_n)))
+        side = np.arange(-s, s + 1, dtype=float)
+        x, y = [foo.ravel() for foo in np.meshgrid(side, side)]
+
+    elif packing == "hex":
+        s = int(np.ceil((np.sqrt(12 * bigger_n - 3) + 3) / 6))
+        side = np.arange(-s, s + 1, dtype=float)
+        x, y = np.meshgrid(side, side)
+        y[:, ::2] -= 0.5
+        x *= np.sqrt(3) / 2
+        x, y = x.ravel(), y.ravel()
+
+    elif packing == "sunflower":
+        i = np.arange(bigger_n)
+        golden_angle = np.pi * (3.0 - np.sqrt(5.0))
+        x = 0.5966 * np.sqrt(i) * np.cos(golden_angle * i)
+        y = 0.5966 * np.sqrt(i) * np.sin(golden_angle * i)
+
+    else:
+        raise ValueError(
+            "Supported offset packings are ['square', 'hex', or 'sunflower']."
         )
-        DX, DY = np.meshgrid(dxy_, dxy_)
-        return np.c_[DX.ravel()[:n], DY.ravel()[:n]]
 
-    raise ValueError(
-        "Please specify a valid array type. Valid array types are:\n"
-        + "\n".join(valid_array_types)
-    )
+    n_sides = {"square": 4, "hex": 6, "circle": 256}[shape]
 
+    r = np.sqrt(x**2 + y**2)
+    p = np.arctan2(y, x)
+    ngon_distance = r * np.cos(np.arcsin(np.sin(n_sides / 2 * p)) * 2 / n_sides)
 
-def generate_hex_offsets(n, d):
-    angles = np.linspace(0, 2 * np.pi, 6 + 1)[1:] + np.pi / 2
-    zs = np.array([0])
-    layer = 0
-    while len(zs) < n:
-        for angle in angles:
-            for z in layer * np.exp(1j * angle) + np.arange(layer) * np.exp(
-                1j * (angle + 2 * np.pi / 3)
-            ):
-                zs = np.append(zs, z)
-        layer += 1
-    zs -= zs.mean()
-    zs *= 0.5 * d / np.abs(zs).max()
-
-    return np.c_[np.real(np.array(zs[:n])), np.imag(np.array(zs[:n]))]
-
-
-class Detectors:
-    @classmethod
-    def generate(
-        cls,
-        bands: Mapping,
-        field_of_view: float = 1,
-        geometry: str = "hex",
-        baseline: float = 0,
-        offsets: np.array = None,
-    ):
-        ubands = {}
-        det_params = {
-            col: []
-            for col in [
-                "band",
-                "offset_x",
-                "offset_y",
-                "baseline_x",
-                "baseline_y",
-                "baseline_z",
-                "pol_angle",
-            ]
-        }
-
-        for band_key, band_config in bands.items():
-            if not all(key in band_config.keys() for key in REQUIRED_DET_CONFIG_KEYS):
-                raise ValueError(f"Each band must have keys {REQUIRED_DET_CONFIG_KEYS}")
-
-            band_name = band_config.get("band_name", band_key)
-
-            n = band_config["n"]
-
-            det_params["band"].extend(n * [band_name])
-
-            ubands[band_key] = Band(
-                name=band_name,
-                center=band_config["band_center"],
-                width=band_config["band_width"],
-            )
+    subset_index = np.argsort(ngon_distance)[:n]
 
-            det_offsets_radians = np.radians(
-                generate_array_offsets(geometry, field_of_view, n)
-            )
+    offsets = np.c_[x[subset_index], y[subset_index]]
 
-            # should we make another function for this?
-            det_baselines_meters = generate_array_offsets(geometry, baseline, n)
-
-            # if randomize_offsets:
-            #     np.random.shuffle(offsets_radians)  # this is a stupid function.
-
-            det_params["offset_x"].extend(det_offsets_radians[:, 0])
-            det_params["offset_y"].extend(det_offsets_radians[:, 1])
-            det_params["baseline_x"].extend(det_baselines_meters[:, 0])
-            det_params["baseline_y"].extend(det_baselines_meters[:, 1])
-            det_params["baseline_z"].extend(0 * det_baselines_meters[:, 1])
+    if normalize:
+        hull_pts = (
+            offsets[ConvexHull(offsets).vertices] if len(offsets) > 16 else offsets
+        )
+        span = cdist(hull_pts, hull_pts, metric="euclidean").max()
+        offsets /= span if span > 0 else 1.0
 
-            det_params["pol_angle"].extend(n * [0.0])
+    return offsets
 
-        return cls(det_params, bands=ubands)
 
-    @property
-    def band_center(self):
-        centers = np.zeros(shape=self.n)
-        for band_name, band in self.bands.items():
-            centers[self.band == band_name] = band.center
+def generate_2d_offsets_from_diameter(
+    diameter, packing="hex", shape="circle", tol=1e-2, max_iterations=32
+):
+    n = np.square(diameter)
+    span = 0
+
+    for _ in range(max_iterations):
+        offsets = generate_2d_offsets(n=n, packing=packing, shape=shape)
+        hull_pts = (
+            offsets[ConvexHull(offsets).vertices] if len(offsets) > 16 else offsets
+        )
+        span = cdist(hull_pts, hull_pts, metric="euclidean").max()
 
-        return centers
+        n *= np.square(diameter / span)
 
-    @property
-    def band_width(self):
-        widths = np.zeros(shape=self.n)
-        for band_name, band in self.bands.items():
-            widths[self.band == band_name] = band.width
+        if np.abs(span - diameter) / diameter < tol:
+            return offsets
 
-        return widths
+    return offsets
 
-    def __init__(self, params: dict = {}, bands: dict = {}):
-        self.bands = bands
-        self.params = params
 
-        for k, v in self.params.items():
-            setattr(self, k, np.array(v))
+def generate_array(
+    bands: list,
+    n: int = None,
+    primary_size: float = 10.0,
+    field_of_view: float = 0.0,
+    beam_spacing: float = 1.0,
+    array_packing: tuple = "hex",
+    array_shape: tuple = "circle",
+    array_offset: tuple = (0.0, 0.0),
+    baseline_diameter: float = 0,
+    baseline_packing: str = "sunflower",
+    baseline_shape: str = "circle",
+    baseline_offset: tuple = (0.0, 0.0, 0.0),
+    polarization: bool = False,
+    bath_temp: float = 0,
+    file: str = None,
+):
+    dets = pd.DataFrame()
+
+    bands = [Band.from_config(name=k, config=v) for k, v in bands.items()]
+
+    band_centers = [band.center for band in bands]
+    resolutions = [
+        compute_angular_fwhm(primary_size, z=np.inf, f=1e9 * band.center)
+        for band in bands
+    ]
+    detector_spacing = beam_spacing * np.max(resolutions)
+
+    if n is None:
+        topological_diameter = np.radians(field_of_view) / detector_spacing
+        if topological_diameter > 1:
+            offsets = detector_spacing * generate_2d_offsets_from_diameter(
+                diameter=topological_diameter, packing=array_packing, shape=array_shape
+            )
+        else:
+            n = 1  # what?
 
-        self.n = len(self.band)
+    if n is not None:
+        if field_of_view is not None:
+            offsets = np.radians(field_of_view) * generate_2d_offsets(
+                n=n, packing=array_packing, shape=array_shape, normalize=True
+            )
+        else:
+            if len(resolutions) > 1:
+                warnings.warn(
+                    "Subarray has more than one band. "
+                    f"Generating detector spacing based on the lowest frequency ({np.min(band_centers):.01f}) GHz."
+                )
+            offsets = detector_spacing * generate_2d_offsets(
+                n=n, packing=array_packing, shape=array_shape
+            )
 
-    @property
-    def df(self):
-        df = pd.DataFrame(columns=det_columns, dtype="float")
+    baselines = baseline_diameter * generate_2d_offsets(
+        n=len(offsets), packing=baseline_packing, shape=baseline_shape, normalize=True
+    )
 
-        for col, dtype in det_columns.items():
-            df.loc[:, col] = self.params[col]
-            df.loc[:, col] = df.loc[:, col].astype(dtype)
+    if polarization:
+        # generate random polarization angles and double each detector
+        pol_angles = np.random.uniform(low=0, high=2 * np.pi, size=len(offsets))
+        pol_labels = np.r_[["A" for _ in pol_angles], ["B" for _ in pol_angles]]
+        pol_angles = np.r_[pol_angles, (pol_angles + np.pi / 2) % (2 * np.pi)]
+        offsets = np.r_[offsets, offsets]
+        baselines = np.r_[baselines, baselines]
+
+    else:
+        pol_angles = np.zeros(len(offsets))
+        pol_labels = ["A" for i in pol_angles]
+
+    for band in bands:
+        band_dets = pd.DataFrame(
+            index=np.arange(len(offsets)),
+            dtype=float,
+        )
 
-        return df
+        band_dets.loc[:, "band_name"] = band.name
+        band_dets.loc[:, "sky_x"] = np.radians(array_offset[0]) + offsets[:, 0]
+        band_dets.loc[:, "sky_y"] = np.radians(array_offset[1]) + offsets[:, 1]
 
-    @property
-    def ubands(self):
-        return list(self.bands.keys())
+        band_dets.loc[:, "baseline_x"] = baseline_offset[0] + baselines[:, 0]
+        band_dets.loc[:, "baseline_y"] = baseline_offset[1] + baselines[:, 1]
+        band_dets.loc[:, "baseline_z"] = baseline_offset[2]
 
-    def passband(self, nu):
-        _nu = np.atleast_1d(nu)
+        band_dets.loc[:, "bath_temp"] = bath_temp
+        band_dets.loc[:, "pol_angle"] = pol_angles
+        band_dets.loc[:, "pol_label"] = pol_labels
 
-        PB = np.zeros((len(self.df), len(_nu)))
+        band_dets.loc[:, "primary_size"] = primary_size
 
-        for band_name, band in self.bands.items():
-            PB[self.band == band_name] = band.passband(_nu)
+        dets = pd.concat([dets, band_dets])
 
-        return PB
+    return dets
```

### Comparing `maria-0.9.7/maria/atmosphere/engine.py` & `maria-1.0.0/maria/atmosphere/engine.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-import os
-
+import dask.array as da
 import numpy as np
 
-# how do we do the bands? this is a great question.
-# because all practical telescope instrumentation assume a constant band
-
-here, this_filename = os.path.split(__file__)
-
 
 def extrude(
     values: np.array,
     A: np.array,
     B: np.array,
     n_steps: int,
     n_i: int,
     n_j: int,
     i_sample_index: int,
     j_sample_index: int,
 ):
     # muy rapido
     BUFFER = np.zeros((n_steps + n_i) * n_j)
+    BUFFER = da.random.random(size=((n_steps + n_i) * n_j))
     BUFFER[n_steps * n_j :] = values
 
     # remember that (e, c) -> n_c * e + c
     for buffer_index in np.arange(n_steps)[::-1]:
         BUFFER[buffer_index * n_j + np.arange(n_j)] = A @ BUFFER[
             n_j * (buffer_index + 1 + i_sample_index) + j_sample_index
         ] + B @ np.random.standard_normal(size=n_j)
```

### Comparing `maria-0.9.7/maria/atmosphere/turbulent_layer.py` & `maria-1.0.0/maria/atmosphere/turbulent_layer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,136 +1,140 @@
+import dask.array as da
 import numpy as np
 import scipy as sp
+from todder.coords import Coordinates, get_center_phi_theta
 
 from .. import utils
-from ..array import Array
-from ..coords import Coordinates, get_center_phi_theta
+from ..functions import approximate_normalized_matern
+from ..instrument import Instrument
+from ..instrument.beams import construct_beam_filter, separably_filter
 from .weather import Weather
 
 MIN_SAMPLES_PER_RIBBON = 2
 RIBBON_SAMPLE_DECAY = 2
 JITTER_LEVEL = 1e-4
 
-matern_callback = utils.functions.approximate_normalized_matern
-# matern_callback = utils.functions.normalized_matern
+matern_callback = approximate_normalized_matern
 
 
 class TurbulentLayer:
     """
     The simplest possible atmospheric model.
     This model is only appropriate for single instruments, i.e. when the baseline is zero.
     """
 
     def __init__(
         self,
-        array: Array,
+        instrument: Instrument,
         boresight: Coordinates,
         weather: Weather,
         depth: float,
         res: float,
-        turbulent_outer_scale: float,
+        turbulent_outer_scale: float = 500,
         verbose: bool = False,
+        timestep: float = 0.05,
         **kwargs,
     ):
-        self.array = array
-        self.boresight = boresight
+        self.instrument = instrument
+        self.boresight = boresight.downsample(timestep=timestep)
         self.weather = weather
         self.depth = depth
         self.res = res
+        self.timestep = timestep
+
+        self.sim_time = self.boresight.time.compute()
+        self.sim_az = self.boresight.az.compute()
+        self.sim_el = self.boresight.el.compute()
 
         # this is approximately correct
-        # self.depth = self.depth / np.sin(np.mean(self.pointing.el))
+        # self.depth = self.depth / np.sin(np.mean(self.plan.el))
 
         # this might change
         self.angular_outer_scale = turbulent_outer_scale / self.depth
 
         # returns the beam fwhm for each detector at the layer distance
-        # self.physical_beam_fwhm = self.array.physical_fwhm(self.depth)
+        # self.physical_beam_fwhm = self.instrument.physical_fwhm(self.depth)
         # self.angular_beam_fwhm = self.physical_beam_fwhm / self.depth
 
         self.angular_resolution = self.res / self.depth
 
         if verbose:
             print(f"{self.angular_resolution = }")
 
-        self.layer_altitude = self.weather.altitude + self.depth / np.sin(
-            self.boresight.el
-        )
+        self.layer_altitude = self.weather.altitude + self.depth / np.sin(self.sim_el)
 
         layer_wind_north = sp.interpolate.interp1d(
             self.weather.altitude_levels, self.weather.wind_north, axis=0
         )(self.layer_altitude)
         layer_wind_east = sp.interpolate.interp1d(
             self.weather.altitude_levels, self.weather.wind_east, axis=0
         )(self.layer_altitude)
 
         angular_velocity_x = (
-            +layer_wind_east * np.cos(self.boresight.az)
-            - layer_wind_north * np.sin(self.boresight.az)
+            +layer_wind_east * np.cos(self.sim_az)
+            - layer_wind_north * np.sin(self.sim_az)
         ) / self.depth
 
         angular_velocity_y = (
-            -layer_wind_east * np.sin(self.boresight.az)
-            + layer_wind_north * np.cos(self.boresight.az)
+            -layer_wind_east * np.sin(self.sim_az)
+            + layer_wind_north * np.cos(self.sim_az)
         ) / self.depth
 
         if verbose:
             print(f"{(layer_wind_east, layer_wind_north) = }")
 
         # compute the offset with respect to the center of the scan
-        center_az, center_el = get_center_phi_theta(
-            self.boresight.az, self.boresight.el
-        )
+        center_az, center_el = get_center_phi_theta(self.sim_az, self.sim_el)
         dx, dy = self.boresight.offsets(frame="az_el", center=(center_az, center_el))
 
-        # the angular position of each detector over time WRT the atmosphere
-        # this has dimensions (det index, time index)
+        # the angular position of the boresight over time WRT the atmosphere
+        # this has dimensions (2, time index)
         self.boresight_angular_position = np.c_[
-            dx
-            + np.cumsum(angular_velocity_x * np.gradient(self.boresight.time), axis=-1),
-            dy
-            + np.cumsum(angular_velocity_y * np.gradient(self.boresight.time), axis=-1),
+            dx + np.cumsum(angular_velocity_x * np.gradient(self.sim_time)),
+            dy + np.cumsum(angular_velocity_y * np.gradient(self.sim_time)),
         ]
 
         # find the detector offsets which form a convex hull
-        self.detector_offsets = np.c_[self.array.offset_x, self.array.offset_y]
+        self.detector_offsets = np.radians(
+            np.c_[self.instrument.sky_x, self.instrument.sky_y]
+        )
 
-        # add a small circle of offsets to account for pesky zeros
+        # add a small circle of offsets to account for the beams
         unit_circle_complex = np.exp(1j * np.linspace(0, 2 * np.pi, 64 + 1)[:-1])
         unit_circle_offsets = np.c_[
             np.real(unit_circle_complex), np.imag(unit_circle_complex)
         ]
 
-        # this is a convex hull for the array if it's staring
+        # this is a convex hull for the instrument if it's staring
         stare_convex_hull = sp.spatial.ConvexHull(
             (
                 self.detector_offsets[None, :, None]
-                + self.array.angular_fwhm(depth)[:, None, None]
+                + self.instrument.angular_fwhm(depth)[:, None, None]
                 * unit_circle_offsets[None]
             ).reshape(-1, 2)
         )
-        stare_convex_hull_points = stare_convex_hull.points.reshape(-1, 2)[
+        stare_convex_hull_points = stare_convex_hull.points[
             stare_convex_hull.vertices
-        ]
+        ].reshape(-1, 2)
 
         # convex hull downsample index, to get to 1 second
         chds_index = [
             *np.arange(
                 0,
-                len(self.boresight.time),
-                int(np.maximum(np.gradient(self.boresight.time).mean(), 1)),
+                len(self.sim_time),
+                int(np.maximum(np.median(np.diff(self.sim_time)), 1)),
             ),
             -1,
         ]
 
         # this is a convex hull for the atmosphere
         atmosphere_hull = sp.spatial.ConvexHull(
             (
-                stare_convex_hull_points[None, :, None]
-                + self.boresight_angular_position[None, chds_index]
+                self.boresight_angular_position[chds_index, None]
+                + stare_convex_hull_points[None]
             ).reshape(-1, 2)
         )
         self.atmosphere_hull_points = atmosphere_hull.points.reshape(-1, 2)[
             atmosphere_hull.vertices
         ]
 
         # R takes us from the real (dx, dy) to a more compact (cross_section, extrusion) frame
@@ -275,14 +279,16 @@
         # compute the weights
         self.A = COV_LE_S @ inv_COV_S_S
         self.B = np.linalg.cholesky(COV_LE_LE - self.A @ COV_LE_S.T)
         self.shaped_values = np.zeros(
             (self.n_extrusion, self.n_cross_section), dtype=np.float32
         )
 
+        self.shaped_values = da.from_array(self.shaped_values)
+
         self.atmosphere_detector_points = (
             self.detector_offsets[:, None] + self.boresight_angular_position[None]
         ) @ self.R.T
 
     def generate(self):
         n_steps = self.n_extrusion
 
@@ -299,29 +305,32 @@
 
         self.shaped_values = extruded_values.reshape(
             self.n_extrusion, self.n_cross_section
         )
 
     def sample(self):
         detector_values = np.zeros(self.atmosphere_detector_points.shape[:-1])
-        for band in self.array.ubands:
+        for band in self.instrument.bands:
             # we assume the atmosphere looks the same for every nu in the band
-            band_mask = self.array.dets.band == band
 
-            band_angular_fwhm = self.array.angular_fwhm(z=self.depth)[band_mask].mean()
-
-            F = utils.beam.make_beam_filter(
-                band_angular_fwhm, self.angular_resolution, self.array.beam_profile
+            band_index = self.instrument.dets.subset(band_name=band.name).index
+            band_angular_fwhm = self.instrument.angular_fwhm(z=self.depth)[
+                band_index
+            ].mean()
+
+            F = construct_beam_filter(
+                fwhm=band_angular_fwhm,
+                res=self.angular_resolution,
+                beam_profile=self.instrument.beam_profile,
             )
+            FILTERED_VALUES = separably_filter(self.shaped_values, F)
 
-            FILTERED_VALUES = utils.beam.separably_filter(self.shaped_values, F)
-
-            detector_values[band_mask] = sp.interpolate.RegularGridInterpolator(
+            detector_values[band_index] = sp.interpolate.RegularGridInterpolator(
                 (self.cross_section_side, self.extrusion_side), FILTERED_VALUES.T
-            )(self.atmosphere_detector_points[band_mask])
+            )(self.atmosphere_detector_points[band_index])
 
         return detector_values
 
     # def simulate_integrated_water_vapor(self):
     #     detector_values = self.simulate_normalized_effective_water_vapor()
 
     #     # this is "zenith-scaled"
```

### Comparing `maria-0.9.7/maria/atmosphere/weather/__init__.py` & `maria-1.0.0/maria/atmosphere/weather.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 import os
-from dataclasses import dataclass, field
 from datetime import datetime
 
 import h5py
 import numpy as np
 import pytz
 import scipy as sp
 
-from ...site import InvalidRegionError, all_regions, supported_regions_table
-from ...utils import get_utc_day_hour, get_utc_year_day
-from ...utils.constants import g
-from .. import utils
+from ..constants import g
+from ..io import fetch_cache
+from ..site import InvalidRegionError, all_regions, supported_regions_table
+from ..utils import get_utc_day_hour, get_utc_year_day
 
 here, this_filename = os.path.split(__file__)
 
-WEATHER_DATA_DIRECTORY = f"{here}/data"
-WEATHER_DATA_CACHE_DIRECTORY = "/tmp/maria_data_cache/weather"
-WEATHER_DATA_URL_BASE = "https://github.com/thomaswmorris/maria/raw/master/maria/atmosphere/weather/data"  # noqa F401
-MAX_CACHE_AGE_SECONDS = 86400
+WEATHER_CACHE_BASE = "/tmp/maria-data/weather"
+WEATHER_SOURCE_BASE = "https://github.com/thomaswmorris/maria-data/raw/master/atmosphere/weather"  # noqa F401
 
 
 def get_vapor_pressure(air_temp, rel_hum):  # units are (°K, %)
     T = air_temp - 273.15  # in °C
     a, b, c = 611.21, 17.67, 238.88  # units are Pa, ., °C
     gamma = np.log(1e-2 * rel_hum) + b * T / (c + T)
     return a * np.exp(gamma)
@@ -49,64 +46,64 @@
     return 1e-2 * rel_hum * get_saturation_pressure(air_temp) / (461.5 * air_temp)
 
 
 def absolute_to_relative_humidity(air_temp, abs_hum):
     return 1e2 * 461.5 * air_temp * abs_hum / get_saturation_pressure(air_temp)
 
 
-@dataclass
 class Weather:
-    region: str = "chajnantor"
-    t: float = 0
-    altitude: float = None
-    utc_time: str = ""
-    local_time: str = ""
-    time_zone: str = ""
-    quantiles: dict = field(default_factory=dict)
-    override: dict = field(default_factory=dict)
-    source: str = "era5"
-    from_cache: bool = None
-
-    def __post_init__(self):
-        if self.region not in all_regions:
+    def __init__(
+        self,
+        region: str = "chajnantor",
+        t: float = 0,
+        altitude: float = None,
+        utc_time: str = "",
+        local_time: str = "",
+        time_zone: str = "",
+        quantiles: dict = {},
+        override: dict = {},
+        source: str = "era5",
+        refresh_cache: bool = False,
+    ):
+        if region not in all_regions:
             raise InvalidRegionError(self.region)
 
-        self.source_path = f"{WEATHER_DATA_DIRECTORY}/{self.source}/{self.region}.h5"
-
-        # if the data isn't in the module, default to use the cache
-        self.from_cache = (
-            self.from_cache
-            if self.from_cache is not None
-            else not os.path.exists(self.source_path)
+        self.region = region
+        self.t = t
+        self.altitude = altitude
+        self.utc_time = utc_time
+        self.local_time = local_time
+        self.time_zone = time_zone
+        self.quantiles = quantiles
+        self.override = override
+        self.source = source
+
+        self.cache_path = f"{WEATHER_CACHE_BASE}/{source}/{region}.h5"
+        self.source_url = f"{WEATHER_SOURCE_BASE}/{source}/{region}.h5"
+
+        fetch_cache(
+            source_url=self.source_url,
+            cache_path=self.cache_path,
+            max_age=30 * 86400,
+            refresh=refresh_cache,
         )
 
-        # if we don't have the data, download and cache it
-        if self.from_cache:
-            self.source_path = (
-                f"{WEATHER_DATA_CACHE_DIRECTORY}/{self.source}/{self.region}.h5"
-            )
-            utils.io.fetch_cache(
-                source_url=f"{WEATHER_DATA_URL_BASE}/{self.source}/{self.region}.h5",
-                cache_path=self.source_path,
-            )
-            self.from_cache = True
-
         if self.altitude is None:
             self.altitude = supported_regions_table.loc[self.region, "altitude"]
 
         self.t = np.round(self.t, 0)
         self.altitude = np.round(self.altitude, 0)
         self.time_zone = supported_regions_table.loc[self.region, "timezone"]
         self.utc_datetime = datetime.fromtimestamp(self.t).astimezone(pytz.utc)
         self.utc_time = self.utc_datetime.ctime()
         self.local_time = self.utc_datetime.astimezone(
             pytz.timezone(self.time_zone)
         ).ctime()
 
-        with h5py.File(self.source_path, "r") as f:
+        with h5py.File(self.cache_path, "r") as f:
             self.utc_day_hour = get_utc_day_hour(self.t)
             self.utc_year_day = get_utc_year_day(self.t)
 
             self.quantile_levels = f["quantile_levels"][:]
             self.pressure_levels = f["pressure_levels"][:]
 
             self.fields = list(f["data"].keys())
```

### Comparing `maria-0.9.7/maria/configs/default_params.yml` & `maria-1.0.0/maria/sim/params.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,35 @@
 # this is a master list of parameters that can be passed to a total simulation, along with default values
 # repeated parameters like "description" or "documentation" are not preserved in the simulation class.
 
-array: # defaults to a small test array
-  array_description:
-  detector_config:
-    f090:
-      n: 60
-      band_center: 90
-      band_width: 10
-    f150:
-      n: 60
-      band_center: 150
-      band_width: 20
-  field_of_view: 0.8
-  baseline: 0 # meters
-  geometry: hex
+instrument: # defaults to a small test instrument
+  instrument_description: str
+  instrument_documentation: str
   primary_size: 6
+  dets: dict
   az_bounds: [0,  360]
   el_bounds: [20,  90]
   max_az_vel: 3
   max_el_vel: 2
   max_az_acc: 1
   max_el_acc: 0.25
-  array_documentation: ''
 
-pointing: # defaults to a 45 degree stare due north
-  pointing_description: ''
+plan: # defaults to a 45 degree stare due north
+  plan_description: ''
   start_time: 2022-02-10T06:00:00
-  integration_time: 60 # in seconds
+  duration: 60 # in seconds
   pointing_frame: az_el
   degrees: True
   sample_rate: 20
   scan_pattern: daisy
   scan_center: [10, 4.5]
-  scan_options: {}
+  scan_options: mapping
 
 site: # default to the ALMA site
-  site_description: ''
+  description: ''
   region: 'chajnantor'
   latitude: -23.0294
   longitude: -67.7548
   altitude: 5064
   site_documentation: ''
   weather_quantiles: {}
 
@@ -50,20 +39,21 @@
   min_atmosphere_beam_res: 4
   min_atmosphere_height: 500
   max_atmosphere_height: 5000
   turbulent_outer_scale: 800
   pwv_rms_frac: 0.03
   pwv:
 
+noise:
+  noise: True
+
 map:
   map_file: ''
   map_frame: ra_dec
   map_center: [10, 4.5]
   map_res: 0.5
   map_inbright:
   map_units: K_RJ
   map_freqs: [150]
 
-noise:
-  white_noise_level: 1.e-2 # in Kelvin Rayleigh-Jeans equivalent
-  pink_noise_level: 1.e-2 # in Kelvin Rayleigh-Jeans equivalent amplitude in fourier domain
-  pink_noise_slope: 0.5
+cmb:
+  cmb_source: planck
```

### Comparing `maria-0.9.7/maria/map/__init__.py` & `maria-1.0.0/maria/map/mappers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,255 +1,275 @@
-from dataclasses import dataclass
-from typing import List, Tuple
+import os
+from typing import Sequence, Tuple
 
-import astropy as ap
-import matplotlib.pyplot as plt
 import numpy as np
 import scipy as sp
 from astropy.io import fits
-from astropy.wcs import WCS
-from tqdm import tqdm
+from todder import TOD
 
-from .. import utils
+from .. import units, utils
+from .map import Map
 
+np.seterr(invalid="ignore")
 
-@dataclass
-class Map:
-    """
-    We define height and width, which determines the shape of the
-
-    This means that there might be non-square pixels
-    """
-
-    freqs: List[float]
-    center: Tuple[float, float]
-    width: float = 1
-    height: float = 1
-    degrees: bool = True
-    inbright: float = 1
-    header: ap.io.fits.header.Header = None
-    frame: str = "ra_dec"
-    units: str = "K"
-    data: np.array = None  # 3D array
-
-    def __post_init__(self):
-        assert len(self.freqs) == self.n_freqs
+here, this_filename = os.path.split(__file__)
 
-        assert self.data is not None
 
-        self.width = self.res * self.n_x
-        self.height = self.res * self.n_y
+class BaseMapper:
+    """
+    The base class for mapping.
+    """
 
-    @property
-    def res(self):
-        """
-        TODO: don't do this
-        """
-        return self.x_res
+    def __init__(
+        self,
+        center: Tuple[float, float] = (0, 0),
+        width: float = 1,
+        height: float = 1,
+        res: float = 0.01,
+        frame: str = "ra_dec",
+        units: str = "K_RJ",
+        degrees: bool = True,
+        calibrate: bool = False,
+        tods: Sequence[TOD] = [],
+    ):
+        self.res = np.radians(res) if degrees else res
+        self.center = np.radians(center) if degrees else center
+        self.width = np.radians(width) if degrees else width
+        self.height = np.radians(height) if degrees else height
+        self.degrees = degrees
+        self.calibrate = calibrate
+        self.frame = frame
+        self.units = units
+
+        self.n_x = int(np.maximum(1, self.width / self.res))
+        self.n_y = int(np.maximum(1, self.height / self.res))
+
+        self.x_bins = np.linspace(-0.5 * self.width, 0.5 * self.width, self.n_x + 1)
+        self.y_bins = np.linspace(-0.5 * self.height, 0.5 * self.height, self.n_y + 1)
+
+        self.tods = list(np.atleast_1d(tods))
+
+    def plot(self):
+        if not hasattr(self, "map"):
+            raise RuntimeError("Mapper has not been run yet.")
+        self.map.plot()
 
     @property
-    def x_res(self):
-        return self.width / self.n_x
+    def n_maps(self):
+        return len(self.maps)
 
-    @property
-    def y_res(self):
-        return self.height / self.n_y
+    def add_tods(self, tods):
+        for tod in np.atleast_1d(tods):
+            self.tods.append(tod)
+
+    def save_maps(self, filepath):
+        self.header = self.tods[0].header
+        self.header["comment"] = "Made Synthetic observations via maria code"
+        self.header["comment"] = "Overwrote resolution and size of the output map"
+
+        self.header["CDELT1"] = np.rad2deg(self.res)
+        self.header["CDELT2"] = np.rad2deg(self.res)
+
+        self.header["CRPIX1"] = self.n_x / 2
+        self.header["CRPIX2"] = self.n_y / 2
+
+        self.header["CRVAL1"] = np.rad2deg(self.center[0])
+        self.header["CRVAL2"] = np.rad2deg(self.center[1])
+
+        self.header["CTYPE1"] = "RA---SIN"
+        self.header["CTYPE2"] = "DEC--SIN"
+        self.header["CUNIT1"] = "deg     "
+        self.header["CUNIT2"] = "deg     "
+        self.header["CTYPE3"] = "FREQ    "
+        self.header["CUNIT3"] = "Hz      "
+        self.header["CRPIX3"] = 1.000000000000e00
+
+        self.header["comment"] = "Overwrote pointing location of the output map"
+        self.header["comment"] = "Overwrote spectral position of the output map"
+
+        self.header["BTYPE"] = "Intensity"
+
+        if self.map.units == "Jy/pixel":
+            self.header["BUNIT"] = "Jy/pixel "
+        elif self.map.units == "K_RJ":
+            self.header["BUNIT"] = "Kelvin RJ"  # tods are always in Kelvin
+        else:
+            raise ValueError(f"Units {self.map.units} not implemented.")
+
+        save_maps = np.zeros((len(self.map.frequency), self.n_x, self.n_y))
+
+        for i, key in enumerate(self.band_data.keys()):
+            self.header["CRVAL3"] = self.band_data[key]["band_center"] * 1e9
+            self.header["CDELT3"] = self.band_data[key]["band_width"] * 1e9
+
+            save_maps[i] = self.map.data[i]
+
+            if self.map.units == "Jy/pixel":
+                save_maps[i] *= units.KbrightToJyPix(
+                    self.header["CRVAL3"], self.header["CDELT1"], self.header["CDELT2"]
+                )
 
-    @property
-    def n_freqs(self):
-        return self.data.shape[0]
+        fits.writeto(
+            filename=filepath,
+            data=save_maps,
+            header=self.header,
+            overwrite=True,
+        )
 
-    @property
-    def n_x(self):
-        return self.data.shape[2]
 
-    @property
-    def n_y(self):
-        return self.data.shape[1]
+class BinMapper(BaseMapper):
+    def __init__(
+        self,
+        center: Tuple[float, float] = (0, 0),
+        width: float = 1,
+        height: float = 1,
+        res: float = 0.01,
+        frame: str = "ra_dec",
+        units: str = "K_RJ",
+        degrees: bool = True,
+        calibrate: bool = False,
+        tod_postprocessing: dict = {},
+        map_postprocessing: dict = {},
+        tods: Sequence[TOD] = [],
+    ):
+        super().__init__(
+            center=center,
+            width=width,
+            height=height,
+            res=res,
+            frame=frame,
+            degrees=degrees,
+            calibrate=calibrate,
+            tods=tods,
+            units=units,
+        )
 
-    @property
-    def x_side(self):
-        x = self.res * np.arange(self.n_x)
-        return x - x.mean()
+        self.tod_postprocessing = tod_postprocessing
+        self.map_postprocessing = map_postprocessing
 
-    @property
-    def y_side(self):
-        y = self.res * np.arange(self.n_y)
-        return y - y.mean()
-
-    def plot(self, cmap="plasma", units="degrees", **kwargs):
-        for i_freq, freq in enumerate(self.freqs):
-            header = fits.header.Header()
-
-            header["RESTFRQ"] = freq
-
-            res_degrees = self.res if self.degrees else np.degrees(self.res)
-            center_degrees = self.center if self.degrees else np.degrees(self.center)
-
-            header["CDELT1"] = res_degrees  # degree
-            header["CDELT2"] = res_degrees  # degree
-
-            header["CRPIX1"] = self.n_x / 2
-            header["CRPIX2"] = self.n_y / 2
-
-            header["CTYPE1"] = "RA---SIN"
-            header["CUNIT1"] = "deg     "
-            header["CTYPE2"] = "DEC--SIN"
-            header["CUNIT2"] = "deg     "
-            header["RADESYS"] = "FK5     "
-
-            header["CRVAL1"] = center_degrees[0]
-            header["CRVAL2"] = center_degrees[1]
-            wcs_input = WCS(header, naxis=2)  # noqa F401
-
-            fig = plt.figure()
-
-            ax = fig.add_subplot(1, 1, 1)  # , projection=wcs_input)
-
-            ax.set_title(f"{freq} GHz")
-
-            map_extent_radians = [
-                -self.width / 2,
-                self.width / 2,
-                -self.height / 2,
-                self.height / 2,
-            ]
-            if self.degrees:
-                map_extent_radians = np.radians(map_extent_radians)
-
-            if units == "degrees":
-                map_extent = np.degrees(map_extent_radians)
-            if units == "arcmin":
-                map_extent = 60 * np.degrees(map_extent_radians)
-            if units == "arcsec":
-                map_extent = 3600 * np.degrees(map_extent_radians)
-
-            vmin, vmax = np.nanpercentile(self.data, q=[5, 95])
-
-            map_im = ax.imshow(
-                self.data.T,
-                cmap=cmap,
-                interpolation="none",
-                extent=map_extent,
-                vmin=vmin,
-                vmax=vmax,
+    def run(self):
+        self.band = sorted(
+            np.unique(
+                [band for tod in self.tods for band in np.unique(tod.dets.band_name)]
             )
+        )
 
-            ax.set_xlabel(rf"$\Delta\,\theta_x$ [{units}]")
-            ax.set_ylabel(rf"$\Delta\,\theta_y$ [{units}]")
-
-            cbar = fig.colorbar(map_im, ax=ax, shrink=1.0)
-            cbar.set_label("mJy km/s/pixel")
-
-
-class MapMixin:
-    """
-    This simulates scanning over celestial sources.
-
-    TODO: add errors
-    """
-
-    def _initialize_map(self):
-        if not self.map_file:
-            return
-
-        self.input_map_file = self.map_file
-        hudl = ap.io.fits.open(self.map_file)
+        self.band_data = {}
 
-        map_data = hudl[0].data
-        if map_data.ndim < 2:
-            raise ValueError()
-        elif map_data.ndim == 2:
-            map_data = map_data[None]
+        self.raw_map_sums = {band: np.zeros((self.n_x, self.n_y)) for band in self.band}
+        self.raw_map_cnts = {band: np.zeros((self.n_x, self.n_y)) for band in self.band}
 
-        map_n_freqs, map_n_y, map_n_x = map_data.shape
+        self.map_data = np.zeros((len(self.band), self.n_y, self.n_x))
+        self.map_weight = np.zeros((len(self.band), self.n_y, self.n_x))
 
-        if map_n_freqs != len(self.map_freqs):
-            raise ValueError()
+        for iband, band in enumerate(np.unique(self.band)):
+            self.band_data[band] = {}
 
-        map_width = self.map_res * map_n_x
-        map_height = self.map_res * map_n_y
+            for tod in self.tods:
+                # compute detector offsets WRT the map
+                dx, dy = tod.coords.offsets(frame=self.frame, center=self.center)
 
-        self.raw_map_data = map_data.copy()
+                band_mask = tod.dets.band_name == band
 
-        res_degrees = self.map_res if self.degrees else np.degrees(self.map_res)
+                if self.calibrate:
+                    D = tod.data_calibrated.copy()[band_mask]
+                else:
+                    D = tod.data.copy()[band_mask]
 
-        if self.map_units == "Jy/pixel":
-            for i, nu in enumerate(self.map_freqs):
-                map_data[i] = map_data[i] / utils.units.KbrightToJyPix(
-                    1e9 * nu, res_degrees, res_degrees
+                # windowing
+                W = np.ones(D.shape[0])[:, None] * sp.signal.windows.tukey(
+                    D.shape[-1], alpha=0.1
                 )
 
-        self.map_data = map_data
-
-        self.input_map = Map(
-            data=map_data,
-            header=hudl[0].header,
-            freqs=np.atleast_1d(self.map_freqs),
-            width=np.radians(map_width) if self.degrees else map_width,
-            height=np.radians(map_height) if self.degrees else map_height,
-            center=np.radians(self.map_center) if self.degrees else map_height,
-            degrees=False,
-            frame=self.pointing_frame,
-            inbright=self.map_inbright,
-            units=self.map_units,
-        )
+                WD = W * sp.signal.detrend(D, axis=-1)
+                del D
 
-        self.input_map.header["HISTORY"] = "History_input_adjustments"
-        self.input_map.header["comment"] = "Changed input CDELT1 and CDELT2"
-        self.input_map.header["comment"] = (
-            "Changed surface brightness units to " + self.input_map.units
-        )
-        self.input_map.header["comment"] = "Repositioned the map on the sky"
+                if "highpass" in self.tod_postprocessing.keys():
+                    WD = utils.signal.highpass(
+                        WD,
+                        fc=self.tod_postprocessing["highpass"]["f"],
+                        fs=tod.fs,
+                        order=self.tod_postprocessing["highpass"].get("order", 1),
+                        method="bessel",
+                    )
+
+                if "remove_modes" in self.tod_postprocessing.keys():
+                    n_modes_to_remove = self.tod_postprocessing["remove_modes"]["n"]
+
+                    U, V = utils.signal.decompose(
+                        WD, downsample_rate=np.maximum(int(tod.fs / 16), 1), mode="uv"
+                    )
+                    WD = U[:, n_modes_to_remove:] @ V[n_modes_to_remove:]
+
+                if "despline" in self.tod_postprocessing.keys():
+                    B = utils.signal.get_bspline_basis(
+                        tod.time.compute(),
+                        dk=self.tod_postprocessing["despline"].get("knot_spacing", 10),
+                        order=self.tod_postprocessing["despline"].get(
+                            "spline_order", 3
+                        ),
+                    )
+
+                    A = np.linalg.inv(B @ B.T) @ B @ WD.T
+
+                    WD -= A.T @ B
+
+                map_sum = sp.stats.binned_statistic_2d(
+                    dx[band_mask].ravel(),
+                    dy[band_mask].ravel(),
+                    WD.ravel(),
+                    bins=(self.x_bins, self.y_bins),
+                    statistic="sum",
+                )[0]
+
+                map_cnt = sp.stats.binned_statistic_2d(
+                    dx[band_mask].ravel(),
+                    dy[band_mask].ravel(),
+                    W.ravel(),
+                    bins=(self.x_bins, self.y_bins),
+                    statistic="sum",
+                )[0]
+
+                self.DATA = WD
+
+                self.raw_map_sums[band] += map_sum
+                self.raw_map_cnts[band] += map_cnt
+
+            self.band_data[band]["band_center"] = tod.dets.band_center.mean()
+            self.band_data[band]["band_width"] = 30
+
+            band_map_numer = self.raw_map_sums[band].copy()
+            band_map_denom = self.raw_map_cnts[band].copy()
+
+            if "gaussian_filter" in self.map_postprocessing.keys():
+                sigma = self.map_postprocessing["gaussian_filter"]["sigma"]
+
+                band_map_numer = sp.ndimage.gaussian_filter(band_map_numer, sigma=sigma)
+                band_map_denom = sp.ndimage.gaussian_filter(band_map_denom, sigma=sigma)
+
+            band_map_data = band_map_numer / band_map_denom
+
+            mask = band_map_denom > 0
+
+            if "median_filter" in self.map_postprocessing.keys():
+                band_map_data = sp.ndimage.median_filter(
+                    band_map_data, size=self.map_postprocessing["median_filter"]["size"]
+                )
 
-        if self.input_map.inbright is not None:
-            self.input_map.data *= self.input_map.inbright / np.nanmax(
-                self.input_map.data
+            self.map_data[iband] = np.where(mask, band_map_numer, np.nan) / np.where(
+                mask, band_map_denom, 1
             )
-            self.input_map.header["comment"] = "Amplitude is rescaled."
 
-    def _run(self, **kwargs):
-        self.sample_maps()
+            self.map_weight[iband] = band_map_denom
 
-    def _sample_maps(self):
-        dx, dy = self.det_coords.offsets(
-            frame=self.map_frame, center=self.input_map.center
+        self.map = Map(
+            data=self.map_data,
+            weight=self.map_weight,
+            frequency=np.array(
+                [self.band_data[band]["band_center"] for band in self.band]
+            ),
+            width=np.degrees(self.width) if self.degrees else self.width,
+            height=np.degrees(self.height) if self.degrees else self.height,
+            center=np.degrees(self.center) if self.degrees else self.center,
+            degrees=self.degrees,
+            units=self.units,
         )
-
-        self.data["map"] = np.zeros((dx.shape))
-
-        freqs = tqdm(self.input_map.freqs) if self.verbose else self.input_map.freqs
-        for i, nu in enumerate(freqs):
-            if self.verbose:
-                freqs.set_description(f"Sampling map at {nu} GHz")
-
-            # nu is in GHz, f is in Hz
-            nu_fwhm = utils.beam.angular_fwhm(
-                fwhm_0=self.array.primary_size, z=np.inf, f=1e9 * nu
-            )
-            nu_map_filter = utils.beam.make_beam_filter(
-                fwhm=nu_fwhm, res=self.input_map.res
-            )
-            filtered_nu_map_data = utils.beam.separably_filter(
-                self.input_map.data[i], nu_map_filter
-            )
-
-            # band_res_radians = 1.22 * (299792458 / (1e9 * nu)) / self.array.primary_size
-            # band_res_pixels = band_res_radians / self.input_map.res
-            # FWHM_TO_SIGMA = 2.355
-            # band_beam_sigma_pixels = band_res_pixels / FWHM_TO_SIGMA
-
-            # # band_beam_filter = self.array.
-
-            # # filtered_map_data = sp.ndimage.convolve()
-            det_freq_response = self.array.passbands(nu=np.array([nu]))[:, 0]
-            det_mask = det_freq_response > -np.inf  # -1e-3
-
-            samples = sp.interpolate.RegularGridInterpolator(
-                (self.input_map.x_side, self.input_map.y_side),
-                filtered_nu_map_data,
-                bounds_error=False,
-                fill_value=0,
-                method="linear",
-            )((dx[det_mask], dy[det_mask]))
-
-            self.data["map"][det_mask] = samples
```

### Comparing `maria-0.9.7/maria/site/__init__.py` & `maria-1.0.0/maria/site/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 from dataclasses import dataclass, field
 
 import pandas as pd
 from astropy.coordinates import EarthLocation
 
-from .. import utils
+from ..io import read_yaml
 
 here, this_filename = os.path.split(__file__)
 
-SITE_CONFIGS = utils.io.read_yaml(f"{here}/sites.yml")
+SITE_CONFIGS = read_yaml(f"{here}/sites.yml")
 SITE_PARAMS = set()
 for key, config in SITE_CONFIGS.items():
     SITE_PARAMS |= set(config.keys())
 
 SITE_DISPLAY_COLUMNS = [
-    "site_description",
+    "description",
     "region",
     "latitude",
     "longitude",
     "altitude",
 ]
 site_data = pd.DataFrame(SITE_CONFIGS).T
 all_sites = list(site_data.index.values)
@@ -47,30 +47,30 @@
 def get_location(site_name):
     site = get_site(site_name)
     return EarthLocation.from_geodetic(
         lon=site.longitude, lat=site.latitude, height=site.altitude
     )
 
 
-def get_site_config(site_name="default", **kwargs):
+def get_site_config(site_name="hoagie_haven", **kwargs):
     if site_name not in SITE_CONFIGS.keys():
         raise InvalidSiteError(site_name)
     SITE_CONFIG = SITE_CONFIGS[site_name].copy()
     for k, v in kwargs.items():
         SITE_CONFIG[k] = v
     return SITE_CONFIG
 
 
-def get_site(site_name="default", **kwargs):
-    return Site(**get_site_config(site_name, **kwargs))
+def get_site(site_name="hoagie_haven", **kwargs):
+    return Site(**get_site_config(site_name=site_name, **kwargs))
 
 
 @dataclass
 class Site:
-    site_description: str = ""
+    description: str = ""
     region: str = "princeton"
     altitude: float = None  # in meters
     seasonal: bool = True
     diurnal: bool = True
     latitude: float = None  # in degrees
     longitude: float = None  # in degrees
     weather_quantiles: dict = field(default_factory=dict)
```

### Comparing `maria-0.9.7/maria/tests/test_coordinates.py` & `maria-1.0.0/maria/tests/test_coordinates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 import pytest
-
-from ..coords import dx_dy_to_phi_theta, phi_theta_to_dx_dy
+from todder.coords import dx_dy_to_phi_theta, phi_theta_to_dx_dy
 
 
 def test_offsets_transform():
     OFFSETS_SIZE = 256
 
     for cphi in np.random.uniform(low=0, high=2 * np.pi, size=16):
         for ctheta in np.random.uniform(low=-np.pi / 2, high=np.pi / 2, size=16):
```

### Comparing `maria-0.9.7/maria/tests/test_pipeline.py` & `maria-1.0.0/maria/tests/test_pipeline.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,84 @@
 import os
 
 import numpy as np
 import pytest
 
+import maria
 from maria import Simulation
 from maria.map.mappers import BinMapper
 
+from ..io import fetch_cache
+
 here, this_filename = os.path.split(__file__)
 
+TEST_MAP_SOURCE_URL = (
+    "https://github.com/thomaswmorris/maria-data/raw/master/maps/cluster.fits"  # noqa
+)
+TEST_MAP_CACHE_PATH = "/tmp/maria-data/maps/test.fits"
+
 
 @pytest.mark.mock_obs
 def test_mustang2():
-    map_size = 0.1
+    fetch_cache(TEST_MAP_SOURCE_URL, TEST_MAP_CACHE_PATH)
 
     pointing_center = (73.5287496858916, 2.961663679507145)
     pixel_size = 8.71452898559111e-05
-    integration_time = 1 * 60.0
+    duration = 1 * 60.0
     sample_rate = 100
     scan_velocity = 38 / 3600
 
-    inputfile = f"{here}/../../data/maps/cluster.fits"
-    outfile_tbl = "/tmp/Cluster_45min_noisy_table.fits"
-    outfile_map = "/tmp/Cluster_45min_noisy_map.fits"
-
-    atm_model = "2d"
-    white_noise_level = 1.3e-2
-    pink_noise_level = 2.4
+    instrument = maria.get_instrument("MUSTANG-2")
+    site = maria.get_site("green_bank")
 
-    sim = Simulation(
-        # Mandatory minimal weither settings
-        # ---------------------
-        array="MUSTANG-2",  # Array type
-        pointing="daisy",  # Scanning strategy
-        site="green_bank",  # Site
-        atmosphere_model=atm_model,  # atmospheric model
-        white_noise_level=white_noise_level,  # white noise level
-        pink_noise_level=pink_noise_level,  # pink noise level
-        # True sky input
-        # ---------------------
-        map_file=inputfile,  # Input files must be a fits file.
-        map_units="Jy/pixel",  # Units of the input map in Kelvin Rayleigh Jeans (K, defeault) or Jy/pixel
-        map_res=pixel_size,  # resolution of the map
-        map_center=pointing_center,  # RA & Dec in degree
-        map_freqs=[93],
-        detector_config={"f093": {"n": 217, "band_center": 93, "band_width": 10}},
-        # MUSTANG-2 Observational setup
-        # ----------------------------s
+    plan = maria.get_plan(
+        "daisy",
         scan_options={
             "radius": 4.0 / 60.0,  # The radius of the Daisy scan in degrees
             "speed": scan_velocity,  # scan velocity in when the scan goes through the center deg/s
         },
-        integration_time=integration_time,  # Seconds
+        duration=duration,  # Seconds
         sample_rate=sample_rate,  # Hz
         scan_center=pointing_center,  # Degrees
-        pointing_frame="ra_dec",  # Frame
+        frame="ra_dec",  # Frame
         start_time="2022-02-11T23:00:00",  # observation date
-        pwv_rms_frac=0.005,  # level of atmospheric fluctuations
+    )
+
+    map = maria.map.from_fits(
+        filename=TEST_MAP_CACHE_PATH,
+        resolution=pixel_size,
+        frequency=90,
+        center=pointing_center,
+    )
+
+    sim = Simulation(
+        instrument=instrument,  # Instrument type
+        site=site,  # Site
+        plan=plan,  # Scanning strategy
+        atmosphere="2d",  # atmospheric model
+        map=map,
     )
 
     tod = sim.run()
 
     mapper = BinMapper(
         center=(tod.coords.center_ra, tod.coords.center_dec),
         frame="ra_dec",
         width=np.radians(10.0 / 60.0),
         height=np.radians(10.0 / 60.0),
-        res=np.radians(2.0 / 3600.0),
+        res=np.radians(4.0 / 3600.0),
         degrees=False,
-        filter_data=True,
-        n_modes_to_remove=1,
+        tod_postprocessing={
+            "remove_modes": {"n": 1},
+            "filter": {"f": 0.08},
+            "despline": {"spacing": 10},
+        },
+        map_postprocessing={
+            "gaussian_filter": {"sigma": 1},
+            "median_filter": {"size": 1},
+        },
+        tods=[tod],
     )
 
-    mapper.add_tods(tod)
     mapper.run()
 
-    mapper.save_maps(outfile_map)
+    mapper.save_maps("/tmp/test-output.fits")
```

### Comparing `maria-0.9.7/maria/utils/beam.py` & `maria-1.0.0/maria/instrument/beams.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import scipy as sp  # noqa F401
 
 
-def angular_fwhm(fwhm_0, z=np.inf, n=1, f=None, l=None):  # noqa F401
+def compute_angular_fwhm(fwhm_0, z=np.inf, n=1, f=None, l=None):  # noqa F401
     """
     Returns the angular full width at half maximum of a Gaussian beam at distance `z` in
     refractive index `n`. Supply either the wavelength `l` in meters or the frequency `f` in Hz.
 
     NOTE: For telescope purposes, `fwhm_0` is the width of the objective/primary.
     """
 
@@ -19,19 +19,19 @@
 
     # Rayleigh range
     z_r = np.pi * w_0**2 * n / l
 
     return 2 * w_0 * np.sqrt(1 / z**2 + 1 / z_r**2)
 
 
-def physical_fwhm(fwhm_0, z=np.inf, n=1, f=None, l=None):  # noqa F401
-    return z * angular_fwhm(fwhm_0=fwhm_0, z=z, n=n, f=f, l=l)
+def compute_physical_fwhm(fwhm_0, z=np.inf, n=1, f=None, l=None):  # noqa F401
+    return z * compute_angular_fwhm(fwhm_0=fwhm_0, z=z, n=n, f=f, l=l)
 
 
-def make_beam_filter(fwhm, res, beam_profile=None, buffer=1):
+def construct_beam_filter(fwhm, res, beam_profile=None, buffer=1):
     """
     Make a beam filter for an image.
     """
 
     if beam_profile is None:
         # beam_profile = lambda r, r0: np.where(r <= r0, 1., 0.)
```

### Comparing `maria-0.9.7/maria/utils/linalg.py` & `maria-1.0.0/maria/utils/linalg.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,14 +38,40 @@
     j0, j1 = np.meshgrid(j, j)
     R[..., j0, j1] = sp.linalg.expm(
         np.array([[0, -1], [+1, 0]]) * shaped_angles[..., None, None]
     )
     return R.reshape(*np.shape(angles), 3, 3)
 
 
+def compute_optimal_rotation(points):
+    if points.ndim != 2:
+        raise ValueError("'points' must be an (n_dim, n_points) array.")
+
+    d = len(points)
+    i, j = np.triu_indices(n=d, k=1)
+
+    def rotation_matrix_from_skew_entries(s):
+        S = np.zeros((d, d))
+        S[i, j] = s
+        return sp.linalg.expm(S + -S.T)
+
+    def loss(x, *args):
+        R = rotation_matrix_from_skew_entries(x)
+        return sum(np.log((R @ args[0]).ptp(axis=1)) * np.array([-1, *np.ones(d - 1)]))
+
+    res = sp.optimize.minimize(
+        loss, x0=np.zeros(int(d * (d - 1) / 2)), args=points, tol=1e-10, method="SLSQP"
+    )
+
+    if not res.success:
+        raise RuntimeError("Could not find optimal rotation.")
+
+    return rotation_matrix_from_skew_entries(res.x)
+
+
 def optimize_area_minimizing_rotation_matrix(points):
     def log_dimension_ratio(a):
         trans_points = points @ get_rotation_matrix_2d(a).T
         log_ratio = np.log(trans_points[:, 0].ptp() / trans_points[:, 1].ptp())
         return log_ratio
 
     test_angles = np.linspace(0, np.pi, 64)[:-1]
```

### Comparing `maria-0.9.7/maria/utils/units.py` & `maria-1.0.0/maria/units.py`

 * *Files identical despite different names*

### Comparing `maria-0.9.7/.gitignore` & `maria-1.0.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# setuptools_scm
+**/_version.py
+
 .DS_Store
 **/.DS_Store
 
 *.png
 *.mp4
 
 notebooks/*
@@ -10,14 +13,16 @@
 # !docs/**.ipynb
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
+docs/build/
+
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
```

### Comparing `maria-0.9.7/LICENSE` & `maria-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maria-0.9.7/README.rst` & `maria-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `maria-0.9.7/pyproject.toml` & `maria-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-vcs", "setuptools_scm"]
 build-backend = "hatchling.build"
 
 [project]
 name = "maria"
-version = "0.9.7"
+dynamic = ["version"]
 description = "Ground-based telescope simulations"
 readme = { file = "README.rst", content-type = "text/x-rst" }
 dependencies = [
   "astropy",
   "cmocean",
+  "dask",
   "h5py",
   "healpy",
   "matplotlib",
   "numpy",
   "pandas",
+  "pytz",
   "reproject",
+  "requests",
   "scipy",
   "tables",
+  "todder",
   "tqdm",
 ]
 requires-python = ">=3.9"
 authors = [
-  { name = "Thomas Morris", email = "thomasmorris@princeton.edu" },
+  { name = "Thomas Morris", email = "thomas.w.morris@yale.edu" },
   { name = "Joshiwa van Marrevijk", email = "joshiwavanmarrewijk@eso.org" }
 ]
 maintainers = [
-  { name = "Thomas Morris", email = "thomasmorris@princeton.edu" },
+  { name = "Thomas Morris", email = "thomas.w.morris@yale.edu" },
   { name = "Joshiwa van Marrevijk", email = "joshiwavanmarrewijk@eso.org" }
 ]
 license = {file = "LICENSE"}
 keywords = ["atmosphere", "cosmology", "astronomy"]  # Optional
 classifiers = [  # Optional
   "Development Status :: 4 - Beta",
   "Intended Audience :: Science/Research",
@@ -75,7 +79,20 @@
 [tool.hatch.build.targets.sdist]
 exclude = [
   "maria/atmosphere/spectra/data/**/*.h5",
   "maria/atmosphere/weather/data/**/*.h5",
   "data",
   "docs",
 ]
+
+[tool.hatch.build.targets.wheel]
+only-include = ["maria"]
+
+[tool.setuptools_scm]
+version_file = "maria/_version.py"
+
+[tool.hatch]
+version.source = "vcs"
+build.hooks.vcs.version-file = "maria/_version.py"
+
+[tool.hatch.version.raw-options]
+local_scheme = "no-local-version"
```

### Comparing `maria-0.9.7/PKG-INFO` & `maria-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: maria
-Version: 0.9.7
+Version: 1.0.0
 Summary: Ground-based telescope simulations
 Project-URL: Homepage, https://github.com/thomaswmorris/maria
 Project-URL: Bug Reports, https://github.com/thomaswmorris/maria/issues
 Project-URL: Source, https://github.com/thomaswmorris/maria/
-Author-email: Thomas Morris <thomasmorris@princeton.edu>, Joshiwa van Marrevijk <joshiwavanmarrewijk@eso.org>
-Maintainer-email: Thomas Morris <thomasmorris@princeton.edu>, Joshiwa van Marrevijk <joshiwavanmarrewijk@eso.org>
+Author-email: Thomas Morris <thomas.w.morris@yale.edu>, Joshiwa van Marrevijk <joshiwavanmarrewijk@eso.org>
+Maintainer-email: Thomas Morris <thomas.w.morris@yale.edu>, Joshiwa van Marrevijk <joshiwavanmarrewijk@eso.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023 Thomas W. Morris
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -46,22 +46,26 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.9
 Requires-Dist: astropy
 Requires-Dist: cmocean
+Requires-Dist: dask
 Requires-Dist: h5py
 Requires-Dist: healpy
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: pytz
 Requires-Dist: reproject
+Requires-Dist: requests
 Requires-Dist: scipy
 Requires-Dist: tables
+Requires-Dist: todder
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: coverage; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: furo; extra == 'dev'
 Requires-Dist: ipykernel; extra == 'dev'
```

