# Comparing `tmp/foxesscloud-2.2.6.tar.gz` & `tmp/foxesscloud-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-p061ai77\foxesscloud-2.2.6.tar", last modified: Fri May 17 11:13:17 2024, max compression
+gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-2t3nm83_\foxesscloud-2.2.7.tar", last modified: Wed May 22 17:33:54 2024, max compression
```

## Comparing `foxesscloud-2.2.6.tar` & `foxesscloud-2.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/
--rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.6/LICENCE
--rw-rw-rw-   0        0        0    41597 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    41042 2024-05-17 11:01:10.000000 foxesscloud-2.2.6/README.md
--rw-rw-rw-   0        0        0      635 2024-05-16 18:18:41.000000 foxesscloud-2.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/src/foxesscloud/
--rw-rw-rw-   0        0        0   177033 2024-05-17 11:02:52.000000 foxesscloud-2.2.6/src/foxesscloud/foxesscloud.py
--rw-rw-rw-   0        0        0   171254 2024-05-17 11:03:22.000000 foxesscloud-2.2.6/src/foxesscloud/openapi.py
-drwxrwxrwx   0        0        0        0 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/src/foxesscloud.egg-info/
--rw-rw-rw-   0        0        0    41597 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/src/foxesscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/src/foxesscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/src/foxesscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/src/foxesscloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/
+-rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.7/LICENCE
+-rw-rw-rw-   0        0        0    41962 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    41407 2024-05-22 17:15:35.000000 foxesscloud-2.2.7/README.md
+-rw-rw-rw-   0        0        0      635 2024-05-19 11:23:16.000000 foxesscloud-2.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/src/foxesscloud/
+-rw-rw-rw-   0        0        0   180405 2024-05-22 17:29:15.000000 foxesscloud-2.2.7/src/foxesscloud/foxesscloud.py
+-rw-rw-rw-   0        0        0   174609 2024-05-22 17:29:15.000000 foxesscloud-2.2.7/src/foxesscloud/openapi.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/src/foxesscloud.egg-info/
+-rw-rw-rw-   0        0        0    41962 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/src/foxesscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/src/foxesscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/src/foxesscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/src/foxesscloud.egg-info/top_level.txt
```

### Comparing `foxesscloud-2.2.6/LICENCE` & `foxesscloud-2.2.7/LICENCE`

 * *Files identical despite different names*

### Comparing `foxesscloud-2.2.6/PKG-INFO` & `foxesscloud-2.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.2.6
+Version: 2.2.7
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -345,25 +345,25 @@
 + updates your battery charge settings (if update_settings is not 0)
 + gets the current work mode and updates this if timed work mode changes are configured
 
 ### Configuration Parameters
 
 The following parameters and default values are used to configure charge_needed and may be updated if required using name=value:
 ```
-contingency: 20               # % of consumption to allow as contingency
+contingency: [20,10,5,10]     # % of consumption. Single or [winter, spring, summer, autumn] values
 capacity: None                # Battery capacity in kWh (over-rides generated value if set)
 charge_current: None          # max battery charge current setting in A. None uses a value derrived from the inverter model
 discharge_current: None       # max battery discharge current setting in A. None uses a value derrived from the inverter model
-export_limit: None            # maximum export power. None uses the inverter power rating
+export_limit: None            # maximum export power in kW. None uses the inverter power rating
 discharge_loss: 0.97          # loss converting battery discharge power to grid power
 pv_loss: 0.95                 # loss converting PV power to battery charge power
 grid_loss: 0.97               # loss converting grid power to battery charge power
 charge_loss: None             # loss converting charge power to residual
-inverter_power: None          # inverter power consumption W (dynamically set)
-bms_power: 25                 # BMS power consumption W
+inverter_power: None          # inverter power consumption in W (dynamically set)
+bms_power: 25                 # BMS power consumption in W
 bat_resistance: 0.070         # internal resistance of a battery in ohms
 volt_curve: lifepo4_curve     # battery OCV from 0% to 100% SoC
 nominal_soc: 55               # SoC for nominal open circuit voltage
 generation_days: 3            # number of days to use for average generation (1-7)
 consumption_days: 3           # number of days to use for average consumption (1-7)
 consumption_span: 'week'      # 'week' = last 7 days or 'weekday' = last 7 weekdays e.g. Saturdays
 use_today: 21.0               # hour when today's generation and consumption data will be used
@@ -686,15 +686,19 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.6<br>
+2.2.7<br>
+Updated contingency to allow seasonal values for winter, spring, summer and autumn.
+Update strategy mode to support ForceCharge and ForceDischarge work modes.
+Update so min_soc setting in charge_needed() over-rides min_soc in the tariff strategy.
+Fix force charge strategy mode in charge_neded() to set min_soc correctly.
 Implement 2 second delay between calls that change inverter settings.
 Added strategy mode (timed_mode=2) to charge_needed().
 Added set_strategy() and charge_strategy() to manage charging schedules and work mode changes.
 Refactor debug messaging.
 Simplify charge_needed() output.
 Added 'target_soc' to charge_needed() settings
 Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50 where there is no battery
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.6 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.7 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -248,92 +248,93 @@
 available now and the expected charging or discharging of the battery to
 forecast the battery state + works out if there is a deficit (i.e. when the
 battery would be discharged below your min_soc) + reports the charge needed
 (deficit) or the minimum expected battery level + updates your battery charge
 settings (if update_settings is not 0) + gets the current work mode and updates
 this if timed work mode changes are configured ### Configuration Parameters The
 following parameters and default values are used to configure charge_needed and
-may be updated if required using name=value: ``` contingency: 20 # % of
-consumption to allow as contingency capacity: None # Battery capacity in kWh
-(over-rides generated value if set) charge_current: None # max battery charge
-current setting in A. None uses a value derrived from the inverter model
-discharge_current: None # max battery discharge current setting in A. None uses
-a value derrived from the inverter model export_limit: None # maximum export
-power. None uses the inverter power rating discharge_loss: 0.97 # loss
-converting battery discharge power to grid power pv_loss: 0.95 # loss
-converting PV power to battery charge power grid_loss: 0.97 # loss converting
-grid power to battery charge power charge_loss: None # loss converting charge
-power to residual inverter_power: None # inverter power consumption W
-(dynamically set) bms_power: 25 # BMS power consumption W bat_resistance: 0.070
-# internal resistance of a battery in ohms volt_curve: lifepo4_curve # battery
-OCV from 0% to 100% SoC nominal_soc: 55 # SoC for nominal open circuit voltage
-generation_days: 3 # number of days to use for average generation (1-7)
-consumption_days: 3 # number of days to use for average consumption (1-7)
-consumption_span: 'week' # 'week' = last 7 days or 'weekday' = last 7 weekdays
-e.g. Saturdays use_today: 21.0 # hour when today's generation and consumption
-data will be used min_hours: 0.25 # minimum charge time to set (in decimal
-hours) min_kwh: 0.5 # minimum charge to add in kwh solcast_adjust: 100 # %
-adjustment to make to Solcast forecast solar_adjust: 100 # % adjustment to make
-to Solar forecast forecast_selection: 1 # 1 = only update charge times if
-forecast is available, 0 = use best available data. Default is 1.
-annual_consumption: None # optional annual consumption in kWh. If set, this
-replaces consumption history timed_mode: 0 # 0 = None, 1 = use timed work mode,
-2 = strategy mode special_contingency: 30 # contingency for special days when
-consumption might be higher special_days: ['12-25', '12-26', '01-01']
-full_charge: None # day of month (1-28) to do full charge or 'daily' or day of
-week: 'Mon', 'Tue' etc derate_temp: 21 # battery temperature in C when derating
-charge current is applied derate_step: 5 # step size for derating e.g. 21, 16,
-11 derating: [24, 15, 10, 2] # derated charge current for each temperature step
-e.g. 21C, 16C, 11C, 6C force: 1 # 1 = disable strategy periods when setting
-charge. 0 = fail if strategy period has been set. data_wrap: 6 # data items to
-show per line target_soc: None # target soc for charging ``` These values are
-stored / available in f.charge_config. The default battery open circuit voltage
-curve versus SoC from 0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30,
-52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ``` When operating in
-strategy mode (timed_mode=2), charge_needed will create a schedule that
-includes the strategy for the tariff with additional time segments added to
-charge from grid and (optionall) to stop the battery discharging. In other
-modes, charge_needed() will disable any schedules and set the battery charge
-times. This example shows the results reported by charge needed: ![image]
-(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-
-b165-20d806b1e7e8) ## Battery Info Provides detailed information on the current
-state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
-(interval, run, log, save, count) ``` battery_info() prints information on the
-battery and cells: + count: optional over-ride. The default is based on
-factorising the number of cells reported by 16 or 18 to work out the number of
-batteries. + plot: 1 plot the cell voltages for each battery, 2 plot the cell
-temperatueres, 0 don't plot. The default is 1 + log: see below. Default is 0
-battery_monitor() runs battery_info() in log mode on a schedule to provide
-information on the battery status over a period of time: + interval: the time
-in minutes between log entries. The default is 30 minutes + run: the number of
-log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
-total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
-cell temps. The default is 1 + save: name of a CSV file to write log data to +
-count: optional over-ride for the number of batteries This is an example of the
-output from battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/
-assets/63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ```
-f.date_list(s, e, limit, span, today) ``` Returns a list of dates in the format
-'YYYY-MM-DD'. This function will not return dates in the future. The last date
-will be yesterday or today (if today is True). All parameters are optional: +
-s: start date + e: end date + limit: maximum number of days. The default is 200
-+ span: the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
-'weekday' + today: 1 allows today to be included, 2 allows future dates to be
-included. Default is 0, date list will stop at yesterday You can use 'span' as
-follows: + 'day' provides a single day + 'week' will provide the dates of 7
-consequetive days + 'month' will provide the dates of the days up to the same
-date in the preceeding (or follwing) month + '2days' will provide the dates of
-yesterday and today + 'weekday' will provide the dates of the same day of the
-week, going backwards (or forwards) up to 7 weeks ``` f.british_summer_time(d)
-# 1 if d is in Britsh Summer Time, 0 if not ``` ## Time Periods Times and time
-period settings are held as decimal hours. Functions for working with time
-strings with the format 'HH:MM:SS' and decimal hours include: ``` f.time_hours
-(t, d=None) # convert time to decimal hours. t is a time string ('HH:MM' or
-'HH:MM:SS'), d is optional and is the default time if s is None f.hours_time(h,
-mm=True, ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm =
-include minutes, ss = include seconds, day = include /n for day when hours > 24
+may be updated if required using name=value: ``` contingency: [20,10,5,10] # %
+of consumption. Single or [winter, spring, summer, autumn] values capacity:
+None # Battery capacity in kWh (over-rides generated value if set)
+charge_current: None # max battery charge current setting in A. None uses a
+value derrived from the inverter model discharge_current: None # max battery
+discharge current setting in A. None uses a value derrived from the inverter
+model export_limit: None # maximum export power in kW. None uses the inverter
+power rating discharge_loss: 0.97 # loss converting battery discharge power to
+grid power pv_loss: 0.95 # loss converting PV power to battery charge power
+grid_loss: 0.97 # loss converting grid power to battery charge power
+charge_loss: None # loss converting charge power to residual inverter_power:
+None # inverter power consumption in W (dynamically set) bms_power: 25 # BMS
+power consumption in W bat_resistance: 0.070 # internal resistance of a battery
+in ohms volt_curve: lifepo4_curve # battery OCV from 0% to 100% SoC
+nominal_soc: 55 # SoC for nominal open circuit voltage generation_days: 3 #
+number of days to use for average generation (1-7) consumption_days: 3 # number
+of days to use for average consumption (1-7) consumption_span: 'week' # 'week'
+= last 7 days or 'weekday' = last 7 weekdays e.g. Saturdays use_today: 21.0 #
+hour when today's generation and consumption data will be used min_hours: 0.25
+# minimum charge time to set (in decimal hours) min_kwh: 0.5 # minimum charge
+to add in kwh solcast_adjust: 100 # % adjustment to make to Solcast forecast
+solar_adjust: 100 # % adjustment to make to Solar forecast forecast_selection:
+1 # 1 = only update charge times if forecast is available, 0 = use best
+available data. Default is 1. annual_consumption: None # optional annual
+consumption in kWh. If set, this replaces consumption history timed_mode: 0 # 0
+= None, 1 = use timed work mode, 2 = strategy mode special_contingency: 30 #
+contingency for special days when consumption might be higher special_days:
+['12-25', '12-26', '01-01'] full_charge: None # day of month (1-28) to do full
+charge or 'daily' or day of week: 'Mon', 'Tue' etc derate_temp: 21 # battery
+temperature in C when derating charge current is applied derate_step: 5 # step
+size for derating e.g. 21, 16, 11 derating: [24, 15, 10, 2] # derated charge
+current for each temperature step e.g. 21C, 16C, 11C, 6C force: 1 # 1 = disable
+strategy periods when setting charge. 0 = fail if strategy period has been set.
+data_wrap: 6 # data items to show per line target_soc: None # target soc for
+charging ``` These values are stored / available in f.charge_config. The
+default battery open circuit voltage curve versus SoC from 0% to 100% is: ```
+lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9,
+53.1, 53.50] ``` When operating in strategy mode (timed_mode=2), charge_needed
+will create a schedule that includes the strategy for the tariff with
+additional time segments added to charge from grid and (optionall) to stop the
+battery discharging. In other modes, charge_needed() will disable any schedules
+and set the battery charge times. This example shows the results reported by
+charge needed: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
+63789168/8b77956b-c326-43cd-b165-20d806b1e7e8) ## Battery Info Provides
+detailed information on the current state of the batteries: ``` f.battery_info
+(count, plot, log) f.battery_monitor(interval, run, log, save, count) ```
+battery_info() prints information on the battery and cells: + count: optional
+over-ride. The default is based on factorising the number of cells reported by
+16 or 18 to work out the number of batteries. + plot: 1 plot the cell voltages
+for each battery, 2 plot the cell temperatueres, 0 don't plot. The default is 1
++ log: see below. Default is 0 battery_monitor() runs battery_info() in log
+mode on a schedule to provide information on the battery status over a period
+of time: + interval: the time in minutes between log entries. The default is 30
+minutes + run: the number of log entries to create. The default is 48 i.e.
+every 30 minues for 24 hours in total + log: 0 = display, 1 = log battery info,
+2 = add cell volts, 3 = add cell temps. The default is 1 + save: name of a CSV
+file to write log data to + count: optional over-ride for the number of
+batteries This is an example of the output from battery_info(): ![image](https:
+//github.com/TonyM1958/FoxESS-Cloud/assets/63789168/a8eb52b6-ce3f-4b58-bb76-
+5483d5e40fa7) ## Date Ranges ``` f.date_list(s, e, limit, span, today) ```
+Returns a list of dates in the format 'YYYY-MM-DD'. This function will not
+return dates in the future. The last date will be yesterday or today (if today
+is True). All parameters are optional: + s: start date + e: end date + limit:
+maximum number of days. The default is 200 + span: the range of dates. One of
+'day', 'week', 'month' or 'year', '2days' or 'weekday' + today: 1 allows today
+to be included, 2 allows future dates to be included. Default is 0, date list
+will stop at yesterday You can use 'span' as follows: + 'day' provides a single
+day + 'week' will provide the dates of 7 consequetive days + 'month' will
+provide the dates of the days up to the same date in the preceeding (or
+follwing) month + '2days' will provide the dates of yesterday and today +
+'weekday' will provide the dates of the same day of the week, going backwards
+(or forwards) up to 7 weeks ``` f.british_summer_time(d) # 1 if d is in Britsh
+Summer Time, 0 if not ``` ## Time Periods Times and time period settings are
+held as decimal hours. Functions for working with time strings with the format
+'HH:MM:SS' and decimal hours include: ``` f.time_hours(t, d=None) # convert
+time to decimal hours. t is a time string ('HH:MM' or 'HH:MM:SS'), d is
+optional and is the default time if s is None f.hours_time(h, mm=True,
+ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm = include
+minutes, ss = include seconds, day = include /n for day when hours > 24
 f.hours_in(h, {'start': a, 'end': b}) # True if decimal hour h is in the time
 period a -> b ``` ## Tariffs Tariffs configure when your battery can be charged
 and provide time of use (TOU) periods to split your grid import and export into
 peak, off-peak and shoulder times when data is uploaded to PV Ouptut. There are
 a number of different pre-configured tariffs: + Octopus Flux: off-peak from 02:
 00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed
 work mode change to Self Use at 7am and Feed In First at 4pm. + Intelligent
@@ -478,25 +479,29 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.6
-Implement 2 second delay between calls that change inverter settings. Added
-strategy mode (timed_mode=2) to charge_needed(). Added set_strategy() and
-charge_strategy() to manage charging schedules and work mode changes. Refactor
-debug messaging. Simplify charge_needed() output. Added 'target_soc' to
-charge_needed() settings Fix bat_info() giving incorrect temperatures when API
-returns 0 instead of -50 where there is no battery Fix key error when accessing
-cell volts and temps using an agent / installer account. Ensure output is
-generated if get_battery() fails using battery_info(). Update f.avg() to
-include calculation of averages in lists containng None values. Added
-'data_wrap' to charge_config. 2.1.9
+(verbose) # Version Info 2.2.7
+Updated contingency to allow seasonal values for winter, spring, summer and
+autumn. Update strategy mode to support ForceCharge and ForceDischarge work
+modes. Update so min_soc setting in charge_needed() over-rides min_soc in the
+tariff strategy. Fix force charge strategy mode in charge_neded() to set
+min_soc correctly. Implement 2 second delay between calls that change inverter
+settings. Added strategy mode (timed_mode=2) to charge_needed(). Added
+set_strategy() and charge_strategy() to manage charging schedules and work mode
+changes. Refactor debug messaging. Simplify charge_needed() output. Added
+'target_soc' to charge_needed() settings Fix bat_info() giving incorrect
+temperatures when API returns 0 instead of -50 where there is no battery Fix
+key error when accessing cell volts and temps using an agent / installer
+account. Ensure output is generated if get_battery() fails using battery_info
+(). Update f.avg() to include calculation of averages in lists containng None
+values. Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

### Comparing `foxesscloud-2.2.6/README.md` & `foxesscloud-2.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -331,25 +331,25 @@
 + updates your battery charge settings (if update_settings is not 0)
 + gets the current work mode and updates this if timed work mode changes are configured
 
 ### Configuration Parameters
 
 The following parameters and default values are used to configure charge_needed and may be updated if required using name=value:
 ```
-contingency: 20               # % of consumption to allow as contingency
+contingency: [20,10,5,10]     # % of consumption. Single or [winter, spring, summer, autumn] values
 capacity: None                # Battery capacity in kWh (over-rides generated value if set)
 charge_current: None          # max battery charge current setting in A. None uses a value derrived from the inverter model
 discharge_current: None       # max battery discharge current setting in A. None uses a value derrived from the inverter model
-export_limit: None            # maximum export power. None uses the inverter power rating
+export_limit: None            # maximum export power in kW. None uses the inverter power rating
 discharge_loss: 0.97          # loss converting battery discharge power to grid power
 pv_loss: 0.95                 # loss converting PV power to battery charge power
 grid_loss: 0.97               # loss converting grid power to battery charge power
 charge_loss: None             # loss converting charge power to residual
-inverter_power: None          # inverter power consumption W (dynamically set)
-bms_power: 25                 # BMS power consumption W
+inverter_power: None          # inverter power consumption in W (dynamically set)
+bms_power: 25                 # BMS power consumption in W
 bat_resistance: 0.070         # internal resistance of a battery in ohms
 volt_curve: lifepo4_curve     # battery OCV from 0% to 100% SoC
 nominal_soc: 55               # SoC for nominal open circuit voltage
 generation_days: 3            # number of days to use for average generation (1-7)
 consumption_days: 3           # number of days to use for average consumption (1-7)
 consumption_span: 'week'      # 'week' = last 7 days or 'weekday' = last 7 weekdays e.g. Saturdays
 use_today: 21.0               # hour when today's generation and consumption data will be used
@@ -672,15 +672,19 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.6<br>
+2.2.7<br>
+Updated contingency to allow seasonal values for winter, spring, summer and autumn.
+Update strategy mode to support ForceCharge and ForceDischarge work modes.
+Update so min_soc setting in charge_needed() over-rides min_soc in the tariff strategy.
+Fix force charge strategy mode in charge_neded() to set min_soc correctly.
 Implement 2 second delay between calls that change inverter settings.
 Added strategy mode (timed_mode=2) to charge_needed().
 Added set_strategy() and charge_strategy() to manage charging schedules and work mode changes.
 Refactor debug messaging.
 Simplify charge_needed() output.
 Added 'target_soc' to charge_needed() settings
 Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50 where there is no battery
```

#### html2text {}

```diff
@@ -241,92 +241,93 @@
 available now and the expected charging or discharging of the battery to
 forecast the battery state + works out if there is a deficit (i.e. when the
 battery would be discharged below your min_soc) + reports the charge needed
 (deficit) or the minimum expected battery level + updates your battery charge
 settings (if update_settings is not 0) + gets the current work mode and updates
 this if timed work mode changes are configured ### Configuration Parameters The
 following parameters and default values are used to configure charge_needed and
-may be updated if required using name=value: ``` contingency: 20 # % of
-consumption to allow as contingency capacity: None # Battery capacity in kWh
-(over-rides generated value if set) charge_current: None # max battery charge
-current setting in A. None uses a value derrived from the inverter model
-discharge_current: None # max battery discharge current setting in A. None uses
-a value derrived from the inverter model export_limit: None # maximum export
-power. None uses the inverter power rating discharge_loss: 0.97 # loss
-converting battery discharge power to grid power pv_loss: 0.95 # loss
-converting PV power to battery charge power grid_loss: 0.97 # loss converting
-grid power to battery charge power charge_loss: None # loss converting charge
-power to residual inverter_power: None # inverter power consumption W
-(dynamically set) bms_power: 25 # BMS power consumption W bat_resistance: 0.070
-# internal resistance of a battery in ohms volt_curve: lifepo4_curve # battery
-OCV from 0% to 100% SoC nominal_soc: 55 # SoC for nominal open circuit voltage
-generation_days: 3 # number of days to use for average generation (1-7)
-consumption_days: 3 # number of days to use for average consumption (1-7)
-consumption_span: 'week' # 'week' = last 7 days or 'weekday' = last 7 weekdays
-e.g. Saturdays use_today: 21.0 # hour when today's generation and consumption
-data will be used min_hours: 0.25 # minimum charge time to set (in decimal
-hours) min_kwh: 0.5 # minimum charge to add in kwh solcast_adjust: 100 # %
-adjustment to make to Solcast forecast solar_adjust: 100 # % adjustment to make
-to Solar forecast forecast_selection: 1 # 1 = only update charge times if
-forecast is available, 0 = use best available data. Default is 1.
-annual_consumption: None # optional annual consumption in kWh. If set, this
-replaces consumption history timed_mode: 0 # 0 = None, 1 = use timed work mode,
-2 = strategy mode special_contingency: 30 # contingency for special days when
-consumption might be higher special_days: ['12-25', '12-26', '01-01']
-full_charge: None # day of month (1-28) to do full charge or 'daily' or day of
-week: 'Mon', 'Tue' etc derate_temp: 21 # battery temperature in C when derating
-charge current is applied derate_step: 5 # step size for derating e.g. 21, 16,
-11 derating: [24, 15, 10, 2] # derated charge current for each temperature step
-e.g. 21C, 16C, 11C, 6C force: 1 # 1 = disable strategy periods when setting
-charge. 0 = fail if strategy period has been set. data_wrap: 6 # data items to
-show per line target_soc: None # target soc for charging ``` These values are
-stored / available in f.charge_config. The default battery open circuit voltage
-curve versus SoC from 0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30,
-52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ``` When operating in
-strategy mode (timed_mode=2), charge_needed will create a schedule that
-includes the strategy for the tariff with additional time segments added to
-charge from grid and (optionall) to stop the battery discharging. In other
-modes, charge_needed() will disable any schedules and set the battery charge
-times. This example shows the results reported by charge needed: ![image]
-(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-
-b165-20d806b1e7e8) ## Battery Info Provides detailed information on the current
-state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
-(interval, run, log, save, count) ``` battery_info() prints information on the
-battery and cells: + count: optional over-ride. The default is based on
-factorising the number of cells reported by 16 or 18 to work out the number of
-batteries. + plot: 1 plot the cell voltages for each battery, 2 plot the cell
-temperatueres, 0 don't plot. The default is 1 + log: see below. Default is 0
-battery_monitor() runs battery_info() in log mode on a schedule to provide
-information on the battery status over a period of time: + interval: the time
-in minutes between log entries. The default is 30 minutes + run: the number of
-log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
-total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
-cell temps. The default is 1 + save: name of a CSV file to write log data to +
-count: optional over-ride for the number of batteries This is an example of the
-output from battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/
-assets/63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ```
-f.date_list(s, e, limit, span, today) ``` Returns a list of dates in the format
-'YYYY-MM-DD'. This function will not return dates in the future. The last date
-will be yesterday or today (if today is True). All parameters are optional: +
-s: start date + e: end date + limit: maximum number of days. The default is 200
-+ span: the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
-'weekday' + today: 1 allows today to be included, 2 allows future dates to be
-included. Default is 0, date list will stop at yesterday You can use 'span' as
-follows: + 'day' provides a single day + 'week' will provide the dates of 7
-consequetive days + 'month' will provide the dates of the days up to the same
-date in the preceeding (or follwing) month + '2days' will provide the dates of
-yesterday and today + 'weekday' will provide the dates of the same day of the
-week, going backwards (or forwards) up to 7 weeks ``` f.british_summer_time(d)
-# 1 if d is in Britsh Summer Time, 0 if not ``` ## Time Periods Times and time
-period settings are held as decimal hours. Functions for working with time
-strings with the format 'HH:MM:SS' and decimal hours include: ``` f.time_hours
-(t, d=None) # convert time to decimal hours. t is a time string ('HH:MM' or
-'HH:MM:SS'), d is optional and is the default time if s is None f.hours_time(h,
-mm=True, ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm =
-include minutes, ss = include seconds, day = include /n for day when hours > 24
+may be updated if required using name=value: ``` contingency: [20,10,5,10] # %
+of consumption. Single or [winter, spring, summer, autumn] values capacity:
+None # Battery capacity in kWh (over-rides generated value if set)
+charge_current: None # max battery charge current setting in A. None uses a
+value derrived from the inverter model discharge_current: None # max battery
+discharge current setting in A. None uses a value derrived from the inverter
+model export_limit: None # maximum export power in kW. None uses the inverter
+power rating discharge_loss: 0.97 # loss converting battery discharge power to
+grid power pv_loss: 0.95 # loss converting PV power to battery charge power
+grid_loss: 0.97 # loss converting grid power to battery charge power
+charge_loss: None # loss converting charge power to residual inverter_power:
+None # inverter power consumption in W (dynamically set) bms_power: 25 # BMS
+power consumption in W bat_resistance: 0.070 # internal resistance of a battery
+in ohms volt_curve: lifepo4_curve # battery OCV from 0% to 100% SoC
+nominal_soc: 55 # SoC for nominal open circuit voltage generation_days: 3 #
+number of days to use for average generation (1-7) consumption_days: 3 # number
+of days to use for average consumption (1-7) consumption_span: 'week' # 'week'
+= last 7 days or 'weekday' = last 7 weekdays e.g. Saturdays use_today: 21.0 #
+hour when today's generation and consumption data will be used min_hours: 0.25
+# minimum charge time to set (in decimal hours) min_kwh: 0.5 # minimum charge
+to add in kwh solcast_adjust: 100 # % adjustment to make to Solcast forecast
+solar_adjust: 100 # % adjustment to make to Solar forecast forecast_selection:
+1 # 1 = only update charge times if forecast is available, 0 = use best
+available data. Default is 1. annual_consumption: None # optional annual
+consumption in kWh. If set, this replaces consumption history timed_mode: 0 # 0
+= None, 1 = use timed work mode, 2 = strategy mode special_contingency: 30 #
+contingency for special days when consumption might be higher special_days:
+['12-25', '12-26', '01-01'] full_charge: None # day of month (1-28) to do full
+charge or 'daily' or day of week: 'Mon', 'Tue' etc derate_temp: 21 # battery
+temperature in C when derating charge current is applied derate_step: 5 # step
+size for derating e.g. 21, 16, 11 derating: [24, 15, 10, 2] # derated charge
+current for each temperature step e.g. 21C, 16C, 11C, 6C force: 1 # 1 = disable
+strategy periods when setting charge. 0 = fail if strategy period has been set.
+data_wrap: 6 # data items to show per line target_soc: None # target soc for
+charging ``` These values are stored / available in f.charge_config. The
+default battery open circuit voltage curve versus SoC from 0% to 100% is: ```
+lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9,
+53.1, 53.50] ``` When operating in strategy mode (timed_mode=2), charge_needed
+will create a schedule that includes the strategy for the tariff with
+additional time segments added to charge from grid and (optionall) to stop the
+battery discharging. In other modes, charge_needed() will disable any schedules
+and set the battery charge times. This example shows the results reported by
+charge needed: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
+63789168/8b77956b-c326-43cd-b165-20d806b1e7e8) ## Battery Info Provides
+detailed information on the current state of the batteries: ``` f.battery_info
+(count, plot, log) f.battery_monitor(interval, run, log, save, count) ```
+battery_info() prints information on the battery and cells: + count: optional
+over-ride. The default is based on factorising the number of cells reported by
+16 or 18 to work out the number of batteries. + plot: 1 plot the cell voltages
+for each battery, 2 plot the cell temperatueres, 0 don't plot. The default is 1
++ log: see below. Default is 0 battery_monitor() runs battery_info() in log
+mode on a schedule to provide information on the battery status over a period
+of time: + interval: the time in minutes between log entries. The default is 30
+minutes + run: the number of log entries to create. The default is 48 i.e.
+every 30 minues for 24 hours in total + log: 0 = display, 1 = log battery info,
+2 = add cell volts, 3 = add cell temps. The default is 1 + save: name of a CSV
+file to write log data to + count: optional over-ride for the number of
+batteries This is an example of the output from battery_info(): ![image](https:
+//github.com/TonyM1958/FoxESS-Cloud/assets/63789168/a8eb52b6-ce3f-4b58-bb76-
+5483d5e40fa7) ## Date Ranges ``` f.date_list(s, e, limit, span, today) ```
+Returns a list of dates in the format 'YYYY-MM-DD'. This function will not
+return dates in the future. The last date will be yesterday or today (if today
+is True). All parameters are optional: + s: start date + e: end date + limit:
+maximum number of days. The default is 200 + span: the range of dates. One of
+'day', 'week', 'month' or 'year', '2days' or 'weekday' + today: 1 allows today
+to be included, 2 allows future dates to be included. Default is 0, date list
+will stop at yesterday You can use 'span' as follows: + 'day' provides a single
+day + 'week' will provide the dates of 7 consequetive days + 'month' will
+provide the dates of the days up to the same date in the preceeding (or
+follwing) month + '2days' will provide the dates of yesterday and today +
+'weekday' will provide the dates of the same day of the week, going backwards
+(or forwards) up to 7 weeks ``` f.british_summer_time(d) # 1 if d is in Britsh
+Summer Time, 0 if not ``` ## Time Periods Times and time period settings are
+held as decimal hours. Functions for working with time strings with the format
+'HH:MM:SS' and decimal hours include: ``` f.time_hours(t, d=None) # convert
+time to decimal hours. t is a time string ('HH:MM' or 'HH:MM:SS'), d is
+optional and is the default time if s is None f.hours_time(h, mm=True,
+ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm = include
+minutes, ss = include seconds, day = include /n for day when hours > 24
 f.hours_in(h, {'start': a, 'end': b}) # True if decimal hour h is in the time
 period a -> b ``` ## Tariffs Tariffs configure when your battery can be charged
 and provide time of use (TOU) periods to split your grid import and export into
 peak, off-peak and shoulder times when data is uploaded to PV Ouptut. There are
 a number of different pre-configured tariffs: + Octopus Flux: off-peak from 02:
 00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed
 work mode change to Self Use at 7am and Feed In First at 4pm. + Intelligent
@@ -471,25 +472,29 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.6
-Implement 2 second delay between calls that change inverter settings. Added
-strategy mode (timed_mode=2) to charge_needed(). Added set_strategy() and
-charge_strategy() to manage charging schedules and work mode changes. Refactor
-debug messaging. Simplify charge_needed() output. Added 'target_soc' to
-charge_needed() settings Fix bat_info() giving incorrect temperatures when API
-returns 0 instead of -50 where there is no battery Fix key error when accessing
-cell volts and temps using an agent / installer account. Ensure output is
-generated if get_battery() fails using battery_info(). Update f.avg() to
-include calculation of averages in lists containng None values. Added
-'data_wrap' to charge_config. 2.1.9
+(verbose) # Version Info 2.2.7
+Updated contingency to allow seasonal values for winter, spring, summer and
+autumn. Update strategy mode to support ForceCharge and ForceDischarge work
+modes. Update so min_soc setting in charge_needed() over-rides min_soc in the
+tariff strategy. Fix force charge strategy mode in charge_neded() to set
+min_soc correctly. Implement 2 second delay between calls that change inverter
+settings. Added strategy mode (timed_mode=2) to charge_needed(). Added
+set_strategy() and charge_strategy() to manage charging schedules and work mode
+changes. Refactor debug messaging. Simplify charge_needed() output. Added
+'target_soc' to charge_needed() settings Fix bat_info() giving incorrect
+temperatures when API returns 0 instead of -50 where there is no battery Fix
+key error when accessing cell volts and temps using an agent / installer
+account. Ensure output is generated if get_battery() fails using battery_info
+(). Update f.avg() to include calculation of averages in lists containng None
+values. Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

### Comparing `foxesscloud-2.2.6/pyproject.toml` & `foxesscloud-2.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "foxesscloud"
-version = "2.2.6"
+version = "2.2.7"
 authors = [
   {name="Tony Matthews", email="tony@quasair.co.uk"},
 ]
 description = "library for accessing Fox ESS cloud data using Open API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `foxesscloud-2.2.6/src/foxesscloud/foxesscloud.py` & `foxesscloud-2.2.7/src/foxesscloud/foxesscloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud
-Updated:  12 May 2024
+Updated:  22 May 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud web site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2023
 ##################################################################################################
 
-version = "1.3.8"
+version = "1.3.9"
 print(f"FoxESS-Cloud version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -702,28 +702,26 @@
         else:
             output(f"** set_charge(), {errno_message(errno)}")
         return None
     else:
         output(f"success", 2) 
     return battery_settings
 
-def charge_strategy(st1 = None, en1 = None, st2 = None, en2 = None, adjust=0, min_soc=None):
+def charge_strategy(st1 = None, en1 = None, st2 = None, en2 = None, adjust=0, min_soc=10, target_soc=None):
     output(f"\nConfiguring schedule",1)
-    periods = set_strategy()
+    periods = set_strategy(min_soc=min_soc, quiet=0)
     if st1 is not None and en1 is not None and st1 != en1:
         st1 = round_time(time_hours(st1) + adjust)
         en1 = round_time(time_hours(en1) + adjust)
-        output(f"   Force Charge from {hours_time(st1)} to {hours_time(en1)}", 1)
-        periods.append(set_period(start = st1, end = en1, mode = 'ForceCharge'))
+        periods.append(set_period(start = st1, end = en1, mode = 'ForceCharge', min_soc = target_soc, quiet=0))
     if st2 is not None and en2 is not None and st2 != en2:
         st2 = round_time(time_hours(st2) + adjust)
         en2 = round_time(time_hours(en2) + adjust)
         mode = 'SelfUse'
-        output(f"   {mode} from {hours_time(st2)} to {hours_time(en2)} with min_soc = {min_soc}%", 1)
-        periods.append(set_period(start = st2, end = en2, mode = mode, fdsoc = min_soc))
+        periods.append(set_period(start = st2, end = en2, mode = mode, min_soc = target_soc, quiet=0))
     return periods
 
 ##################################################################################################
 # get min soc settings and save in battery_settings
 ##################################################################################################
 
 def get_min():
@@ -748,15 +746,15 @@
     return battery_settings
 
 ##################################################################################################
 # set min soc from battery_settings or parameters
 ##################################################################################################
 
 def set_min(minGridSoc = None, minSoc = None, force = 0):
-    global token, device_sn, battery_settings, debug_setting, messages, default_min_soc
+    global token, device_sn, battery_settings, debug_setting, messages
     if get_device() is None:
         return None
     if get_schedule().get('enable'):
         if force == 0:
             output(f"** set_min(): cannot set min SoC mode when a schedule is enabled")
             return None
         set_schedule(enable=0)
@@ -1162,54 +1160,56 @@
 
 
 ##################################################################################################
 # set schedule
 ##################################################################################################
 
 # create a period structure. Note: end time is exclusive.
-def set_period(start, end, mode=None, min_soc=None, fdsoc=None, fdpwr=None):
-    if type(start) is str:
-        start = time_hours(start)
-    if type(end) is str:
-        end = time_hours(end)
+def set_period(start, end, mode=None, min_soc=None, fdsoc=None, fdpwr=None, quiet=1):
+    start = time_hours(start)
+    end = time_hours(end)
     if start is None or end is None:
         return None
+    end = round_time(end - 1/60)        # adjust exclusive time to inclusive
     mode = 'SelfUse' if mode is None else mode
     if mode not in work_modes:
         output(f"** mode must be one of {work_modes}")
         return None
     min_soc = 10 if min_soc is None else min_soc
-    fdsoc = 10 if fdsoc is None else fdsoc
+    fdsoc = min_soc if fdsoc is None else fdsoc
     fdpwr = 0 if fdpwr is None else fdpwr
-    device_power = device.get('power') if device is not None else None
-    if device_power is None:
-        device_power = 12000
-    if fdpwr < 0 or fdpwr > 12000:
-        output(f"** fdpwr must be between 0 and {device_power}")
+    if min_soc < 10 or min_soc > 100:
+        output(f"** min_soc must be between 10 and 100")
+        return None
+    if fdpwr < 0 or fdpwr > 6000:
+        output(f"** fdpwr must be between 0 and 6000")
         return None
-    if fdsoc < 10 or fdsoc > 100:
-        output(f"** fdsoc must between 10 and 100")
+    if fdsoc < min_soc or fdsoc > 100:
+        output(f"** fdsoc must between {min_soc} and 100")
         return None
+    if quiet == 0:
+        output(f"   {hours_time(start)} to {hours_time(end)}: {mode} with min_soc = {min_soc}%" + (f", fdPwr = {fdpwr}W and fdSoC = {fdsoc}%" if mode == 'ForceDischarge' else ""), 1)
     start_h, start_m = split_hours(start)
-    end_h, end_m = split_hours(end - 1/60)
+    end_h, end_m = split_hours(end)
     period = {'startH': start_h, 'startM': start_m, 'endH': end_h, 'endM': end_m, 'workMode': mode, 'minSocOnGrid': min_soc, 'fdSoc': fdsoc, 'fdPwr': fdpwr}
     return period
 
 # create periods from a list of strategy times:
-def set_strategy(strategy=None):
+def set_strategy(strategy=None, min_soc=10, quiet=1):
     global tariff
     if strategy is None and tariff is not None:
         strategy = tariff.get('strategy')
     if strategy is None:
         return []
     if type(strategy) is not list:
         strategy = [strategy]
     periods = []
     for s in strategy:
-        p = set_period(s['start'], s['end'], s['mode'], s.get('min_soc'), s.get('fdsoc'), s.get('fdpwr'))
+        min_soc = s['min_soc'] if s.get('min_soc') is not None and s['min_soc'] > min_soc else min_soc
+        p = set_period(s['start'], s['end'], s['mode'], min_soc, s.get('fdsoc'), s.get('fdpwr'), quiet=quiet)
         if p is not None:
             periods.append(p)
     return periods
 
 # set a schedule from a period or list of periods
 def set_schedule(periods=None, template=None, enable=1):
     global token, device_sn, debug_setting, messages, schedule, templates
@@ -1813,14 +1813,16 @@
     minutes = int (h % 1 * 60 + 0.5)
     return (hours, minutes)
 
 # convert time string HH:MM:SS to decimal hours (range 0 to 24)
 # If BST time zone is included, convert to GMT (range -1 to 23)
 def time_hours(t, d = None):
     if t is None:
+        if d is None:
+            return None
         t = d
     if type(t) is float:
         return t
     if type(t) is int:
         return float(t)
     offset = 1 if 'BST' in t else 0
     t = t[0:8]
@@ -1845,33 +1847,55 @@
         h -= 24
         d += 1
     suffix = ""
     if day:
         suffix = f"/{d:0}"
     return f"{int(h):02}:{int(h * 60 % 60):02}:{int(h * 3600 % 60):02}"[:n] + suffix
 
-# True if a decimal hour is within a time period
+# True if a decimal hour falls within a time period
 def hour_in(h, period):
     if period is None:
         return False
-    s = period['start']
-    e = period['end']
+    s = period.get('start')
+    e = period.get('end')
     if s is None or e is None or s == e:
         return False
     while h < 0:
         h += 24
     while h >= 24:
         h -= 24
     if s > e:
         # e.g. 16:00 - 07:00
         return h >= s or h < e
     else:
         # e.g. 02:00 - 05:00
         return h >= s and h < e
 
+# Time in a decimal hour that falls within a time period
+def duration_in(h, period):
+    if period is None:
+        return None
+    duration = 1.0
+    s = period.get('start')
+    e = period.get('end')
+    if s is None or e is None:
+        return None
+    if s == e:
+        return 0.0
+    if e > s and (h >= e or (h + 1) <= s):    # normal time
+            return 0.0
+    if e < s and (h >= e and (h + 1) <= s):   # wrap around time
+            return 0.0
+    if s > h and s < (h + 1):
+        duration -= (s - h)
+    if e > h and e < (h + 1):
+        duration -= (h + 1 - e)
+    duration = 1.0 if duration > 1.0 else 0.0 if duration < 0.0 else duration
+    return duration
+
 # Return the hours in a time period with optional value check
 def period_hours(period, check = None, value = 1):
     if period is None:
         return 0
     if check is not None and period[check] != value:
         return 0
     return round_time(period['end'] - period['start'])
@@ -1925,16 +1949,17 @@
     'name': 'Octopus Flux',
     'off_peak1': {'start': 2.0, 'end': 5.0, 'force': 1},        # off-peak period 1 / am charging period
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},        # off-peak period 2 / pm charging period
     'peak': {'start': 16.0, 'end': 19.0 },                      # peak period 1
     'peak2': {'start': 0.0, 'end': 0.0 },                       # peak period 2
     'forecast_times': [22, 23],                                 # hours in a day to get a forecast
     'strategy': [                                               # timed work mode settings
-        {'start': 5, 'end': 12, 'mode': 'SelfUse'},
-        {'start': 16, 'end': 23, 'mode': 'Feedin'}]
+        {'start': 0, 'end': 2, 'mode': 'Feedin'},
+        {'start': 5, 'end': 6, 'mode': 'SelfUse'},
+        {'start': 16, 'end': 24, 'mode': 'Feedin'}]
     }
 
 # time periods for Intelligent Octopus
 intelligent_octopus = {
     'name': 'Intelligent Octopus',
     'off_peak1': {'start': 23.5, 'end': 5.5, 'force': 1},
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},
@@ -2189,15 +2214,15 @@
         gmt = ' GMT' if tariff['off_peak1'].get('gmt') is not None else ''
     print(f"\n{tariff['name']} {am_pm} charging period: {hours_time(start)} to {hours_time(end)}{gmt}")
     return 1
 
 # set tariff and AM/PM charge time period
 def set_tariff(find, update=1, start_at=None, end_by=None, duration=None, times=None, forecast_times=None, strategy=None, d=None, **settings):
     global debug_setting, agile_octopus, tariff, tariff_list
-    print(f"\n---------------- set_tariff -----------------")
+    output(f"\n---------------- set_tariff -----------------", 1)
     # validate parameters
     args = locals()
     s = ""
     for k in [k for k in args.keys() if args[k] is not None and k != 'settings']:
         s += f"\n  {k} = {args[k]}"
     # store settings:
     for key, value in settings.items():
@@ -2237,20 +2262,21 @@
         if type(forecast_times) is not list:
             forecast_times = [forecast_times]
         forecast_hours = []
         for i, t in enumerate(forecast_times):
             forecast_times[i] = hours_time(t)
             forecast_hours.append(time_hours(t))
         use['forecast_times'] = forecast_hours
-        output(f"\nForecast times set to {forecast_times}")
+        output(f"Forecast times set to {forecast_times}")
     if strategy is not None:
         if type(strategy) is not list:
             strategy = [strategy]
         use['strategy'] = strategy
-        output(f"\nStrategy set to {strategy}")
+        output(f"Strategy updated")
+        set_strategy(strategy, quiet=0)
     if update == 1:
         tariff = use
         output(f"\nTariff set to {tariff['name']}")
     else:
         output(f"\nNo changes made to current tariff", 1)
     return None
 
@@ -2341,32 +2367,53 @@
     for h in range(0, 24):
         profile.append(c_float(forecast.daily[tomorrow]['hourly'].get(int(round_time(h - time_offset)))))
     timed = []
     for h in range(int(hour_now), 24):
         timed.append(c_float(forecast.daily[today]['hourly'].get(int(round_time(h - time_offset)))))
     return (timed + profile + profile)[:run_time]
 
+# take a strategy and return a timed profile:
+def strategy_timed(timed_mode, hour_now, run_time, min_soc=10):
+    global tariff
+    profile = []
+    for h in range(0, 24):
+        profile.append({'mode': 'SelfUse', 'min_soc': min_soc, 'fdpwr': 0, 'fdsoc': min_soc, 'duration': 1.0})
+        if tariff is None or tariff.get('strategy') is None or timed_mode == 0:
+            continue
+        for d in tariff['strategy']:
+            if hour_in(h, d):
+                profile[h]['mode'] = d['mode']
+                if d.get('min_soc') is not None:
+                    profile[h]['min_soc'] = d['min_soc'] if d['min_soc'] > min_soc else min_soc
+                if d.get('fdsoc') is not None:
+                    profile[h]['fdsoc'] = d['fdsoc'] if d['fdsoc'] > min_soc else min_soc
+                if d.get('fdpwr') is not None:
+                    profile[h]['fdpwr'] = d['fdpwr']
+                profile[h]['duration'] = duration_in(h, d)
+    output(f"work mode profile = {profile}", 2)
+    return (profile[int(hour_now):] + profile + profile)[:run_time]
+
 # Battery open circuit voltage (OCV) from 0% to 100% SoC
 #                 0%     10%    20%    30%    40%    50%    60%    70%    80%    90%   100%
 lifepo4_curve = [51.00, 51.50, 52.00, 52.30, 52.60, 52.80, 52.90, 53.00, 53.10, 53.30, 54.00]
 
 # charge_needed settings
 charge_config = {
-    'contingency': 20,                # % of consumption to allow as contingency
+    'contingency': [20,10,5,15],      # % of consumption. Single value or [winter, spring, summer, autumn]
     'capacity': None,                 # Battery capacity (over-ride)
     'min_soc': None,                  # Minimum Soc (over-ride)
     'charge_current': None,           # max battery charge current setting in A
     'discharge_current': None,        # max battery discharge current setting in A
-    'export_limit': None,             # maximum export power
+    'export_limit': None,             # maximum export power in kW
     'discharge_loss': 0.97,           # loss converting battery discharge power to grid power
     'pv_loss': 0.95,                  # loss converting PV power to battery charge power
     'grid_loss': 0.95,                # loss converting grid power to battery charge power
     'charge_loss': None,              # loss converting charge power to residual
-    'inverter_power': None,           # Inverter power consumption W
-    'bms_power': 27,                  # BMS power consumption W
+    'inverter_power': None,           # Inverter power consumption in W
+    'bms_power': 27,                  # BMS power consumption in W
     'bat_resistance': 0.072,          # internal resistance of a battery
     'volt_curve': lifepo4_curve,      # battery OCV range from 0% to 100% SoC
     'nominal_soc': 60,                # SoC for nominal open circuit battery voltage
     'generation_days': 3,             # number of days to use for average generation (1-7)
     'consumption_days': 3,            # number of days to use for average consumption (1-7)
     'consumption_span': 'week',       # 'week' = last n days or 'weekday' = last n weekdays
     'use_today': 21.0,                # hour when todays consumption and generation can be used
@@ -2398,15 +2445,15 @@
 #  show_plot: 1 plots battery SoC, 2 plots battery residual. Default = 1
 #  run_after: 0 over-rides 'forecast_times'. The default is 1.
 #  forecast_times: list of hours when forecast can be fetched
 #  force_charge: 1 = set force charge, 2 = charge for whole period
 
 def charge_needed(forecast=None, update_settings=0, timed_mode=None, show_data=None, show_plot=None, run_after=None,
         forecast_times=None, force_charge=None, test_time=None, test_soc=None, test_charge=None, **settings):
-    global device, seasonality, solcast_api_key, debug_setting, tariff, solar_arrays, legend_location, time_shift, default_min_soc
+    global device, seasonality, solcast_api_key, debug_setting, tariff, solar_arrays, legend_location, time_shift, timed_strategy
     print(f"\n---------------- charge_needed ----------------")
     # validate parameters
     args = locals()
     s = ""
     for k in [k for k in args.keys() if args[k] is not None and k != 'settings']:
         s += f"\n  {k} = {args[k]}"
     # store settings:
@@ -2451,28 +2498,28 @@
     force_charge = 0 if force_charge is None else force_charge
     start_am = time_hours(tariff['off_peak1']['start'] if tariff is not None else 2.0)
     end_am = time_hours(tariff['off_peak1']['end'] if tariff is not None else 5.0)
     # adjust charge times for Economy 7 in BST
     if time_offset > 0 and tariff is not None and tariff['off_peak1'].get('gmt') is not None:
         start_am += 1
         end_am += 1
-    force_charge_am = 0 if tariff is not None and tariff['off_peak1']['force'] == 0 or force_charge == 0 else force_charge
+    force_charge_am = 0 if (tariff is not None and tariff['off_peak1']['force'] == 0) or force_charge == 0 else 1
     time_to_am = round_time(start_am - base_hour)
     start_pm = time_hours(tariff['off_peak2']['start'] if tariff is not None else 0.0)
     end_pm = time_hours(tariff['off_peak2']['end'] if tariff is not None else 0.0)
-    force_charge_pm = 0 if tariff is not None and tariff['off_peak2']['force'] == 0 or force_charge == 0 else 1
+    force_charge_pm = 0 if (tariff is not None and tariff['off_peak2']['force'] == 0) or force_charge == 0 else 1
     time_to_pm = round_time(start_pm - base_hour) if start_pm > 0 else None
     no_go1 = time_to_am is not None and hour_in(hour_now, {'start': round_time(start_am - 0.25), 'end': round_time(end_am + 0.25)})
     no_go2 = time_to_pm is not None and hour_in(hour_now, {'start': round_time(start_pm - 0.25), 'end': round_time(end_pm + 0.25)})
     if (no_go1 or no_go2) and update_settings > 0:
         output(f"\nInverter settings will not be changed less than 15 minutes before or after a charging period")
         update_settings = 0
     # choose and configure parameters for next charge time period
     charge_pm = time_to_pm is not None and time_to_pm < time_to_am
-    force_charge = force_charge_pm if charge_pm else force_charge_am
+    force_charge = force_charge_pm if charge_pm else force_charge if force_charge_am == 1 else 0
     start_at = start_pm if charge_pm else start_am
     end_by = end_pm if charge_pm else end_am
     charge_time = round_time(end_by - start_at)
     time_to_start = time_to_pm if charge_pm else time_to_am
     start_hour = base_hour + time_to_start
     time_to_next = int(time_to_start)
     start_part_hour = time_to_start % 1
@@ -2720,106 +2767,117 @@
         if charge_config['forecast_selection'] == 1 and update_settings > 0:
             output(f"\nSettings will not be updated when forecast is not available")
             update_settings = 0
     # produce time lines for main charge and discharge (after losses)
     charge_timed = [x * charge_config['pv_loss'] for x in generation_timed]
     discharge_timed = [x / charge_config['discharge_loss'] for x in consumption_timed]
     # adjust charge and discharge time lines for work mode, force charge and power limits
-    work_mode = current_mode
+    work_mode_timed = strategy_timed(timed_mode, hour_now, run_time, min_soc)
+    work_mode = work_mode_timed[0]['mode'] if current_mode is None else current_mode
     for i in range(0, run_time):
         h = base_hour + i
         # get work mode and check for changes
-        new_work_mode = timed_work_mode(h, current_mode) if timed_mode > 0 else current_mode
-        if new_work_mode is not None and new_work_mode != work_mode:
+        new_work_mode = work_mode_timed[i]['mode']
+        if new_work_mode != work_mode:
             output(f"  {hours_time(h)}: {new_work_mode} work mode", 2)
             work_mode = new_work_mode
         # cap charge / discharge power
         charge_timed[i] = charge_limit if charge_timed[i] > charge_limit else charge_timed[i]
         discharge_timed[i] = discharge_limit if discharge_timed[i] > discharge_limit else discharge_timed[i]
-        if force_charge_am == 1 and hour_in(h, {'start': start_am, 'end': end_am}):
+        # apply changes due to work mode
+        duration = work_mode_timed[i]['duration']
+        if timed_mode > 0 and work_mode == 'ForceCharge':
+            (discharge_timed[i], charge_timed[i]) = (discharge_timed[i] * (1.0 - duration),
+                charge_limit * duration + charge_timed[i] * (1.0 - duration))
+        elif timed_mode > 0 and work_mode == 'ForceDischarge':
+            fdpwr = work_mode_timed[i]['fdpwr'] / charge_config['discharge_loss']
+            fdpwr = min([discharge_limit, export_limit * 1000 + discharge_timed[i], fdpwr])
+            (discharge_timed[i], charge_timed[i]) = (fdpwr * duration + discharge_timed[i] * (1.0 - duration) - charge_timed[i] * duration,
+                charge_timed[i] * (1.0 - duration))
+        elif force_charge_am > 0 and hour_in(h, {'start': start_am, 'end': end_am}):
             discharge_timed[i] = operating_loss if charge_timed[i] == 0.0 else 0.0
-        elif force_charge_pm == 1 and hour_in(h, {'start': start_pm, 'end': end_pm}):
+        elif force_charge_pm > 0 and hour_in(h, {'start': start_pm, 'end': end_pm}):
             discharge_timed[i] = operating_loss if charge_timed[i] == 0.0 else 0.0
         elif timed_mode > 0 and work_mode == 'Backup':
             discharge_timed[i] = operating_loss if charge_timed[i] == 0.0 else 0.0
         elif timed_mode > 0 and work_mode == 'Feedin':
             (discharge_timed[i], charge_timed[i]) = (bms_loss if (charge_timed[i] >= discharge_timed[i]) else (discharge_timed[i] - charge_timed[i]),
-                0.0 if (charge_timed[i] <= export_limit + discharge_timed[i]) else (charge_timed[i] - export_limit - discharge_timed[i]))
+                0.0 if (charge_timed[i] <= export_limit * 1000 + discharge_timed[i]) else (charge_timed[i] - export_limit * 1000 - discharge_timed[i]))
         else: # work_mode == 'SelfUse'
             (discharge_timed[i], charge_timed[i]) = (bms_loss if (charge_timed[i] >= discharge_timed[i]) else (discharge_timed[i] - charge_timed[i]),
                 0.0 if (charge_timed[i] <= discharge_timed[i]) else (charge_timed[i] - discharge_timed[i]))
     # track the battery residual over the run time (if we don't add any charge)
     # adjust residual from hour_now to what it was at the start of current hour
     h = base_hour
     kwh_timed = [charge * charge_loss - discharge for charge, discharge in zip(charge_timed, discharge_timed)]
     kwh_current = residual - kwh_timed[0] * (hour_now - h)
     bat_timed = []
-    kwh_min = kwh_current
-    min_hour = h
-    reserve_drain = reserve
+    kwh_min = capacity
+    reserve_drain_now = reserve
+    min_soc_now = min_soc
     for i in range(0, run_time):
-        if kwh_current <= reserve and i <= time_to_next:
+        reserve_now = capacity * min_soc_now / 100
+        reserve_drain = capacity * (min_soc_now - 4) / 100
+        reserve_drain_now = reserve_now if reserve_drain_now > reserve_now or reserve_drain_now < reserve_drain else reserve_drain_now
+#        print(f"h={h}, min_soc_now={min_soc_now}, reserve_now={reserve_now}, kwh_current={kwh_current}")
+        if kwh_current <= reserve_now and i <= time_to_next:
             # battery is empty
-            if reserve_drain < (capacity * 6 / 100):
-                reserve_drain = reserve           # force charge to restore reserve
-            kwh_current = reserve_drain           # stop discharge below reserve
-            reserve_drain -= bms_loss             # allow for BMS drain
+            kwh_current = reserve_drain_now        # stop discharge below reserve
+            reserve_drain_now -= bms_loss          # allow for BMS drain
         else:
-            reserve_drain = reserve                # reset drain
+            reserve_drain_now = reserve_now           # reset drain
         if kwh_current > capacity:
             # battery is full
             kwh_current = capacity
         bat_timed.append(kwh_current)
-        if kwh_current < kwh_min:       # track minimum and time
+        if kwh_current < kwh_min and i >= time_to_next:       # track minimum after next charge
             kwh_min = kwh_current
-            min_hour = h
         kwh_current += kwh_timed[i]
+        min_soc_now = work_mode_timed[i]['fdsoc'] if work_mode_timed[i]['mode'] =='ForceDischarge' else work_mode_timed[i]['min_soc']
         h += 1
     # work out what we need to add to stay above reserve and provide contingency or to hit target_soc
     contingency = charge_config['special_contingency'] if tomorrow[-5:] in charge_config['special_days'] else charge_config['contingency']
+    contingency = contingency[quarter] if type(contingency) is list else contingency
     kwh_contingency = consumption * contingency / 100
     kwh_needed = reserve + kwh_contingency - kwh_min
     start_residual = interpolate(time_to_start, bat_timed)      # residual when charging starts
-    target_soc = charge_config['target_soc'] if charge_config.get('target_soc') is not None else 0
-    target_kwh = capacity if target_soc > 100 else target_soc / 100 * capacity
+    target_soc = charge_config['target_soc'] if charge_config.get('target_soc') is not None else 10
+    target_soc = 100 if target_soc > 100 else 10 if target_soc < 10 else target_soc
+    target_kwh = target_soc / 100 * capacity
     if target_kwh > (start_residual + kwh_needed):
         kwh_needed = target_kwh - start_residual
-    day_when = 'today' if min_hour < 24 else 'tomorrow' if min_hour <= 48 else 'day after tomorrow'
     if kwh_min > reserve and kwh_needed < charge_config['min_kwh'] and full_charge is None and test_charge is None:
-        output(f"\nNo charging is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh)")
+        output(f"\nNo charging is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh, contingency = {kwh_contingency:.1f}kWh)")
         charge_message = "no charge needed"
         kwh_needed = 0.0
         hours = 0.0
         end1 = start_at
         end_soc = int(start_residual / capacity * 100 + 0.5)
         output(f"   Expected SoC at {hours_time(start_at)} is {end_soc}%")
     else:
         charge_message = "with charge added"
         if test_charge is None:
-            min_hour_adjust = min_hour - hour_adjustment if min_hour >= change_hour else 0
-            output(f"\nCharge of {kwh_needed:.2f}kWh is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh)")
+            output(f"\nCharge of {kwh_needed:.2f}kWh is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh, contingency = {kwh_contingency:.1f}kWh)")
         else:
             output(f"\nTest charge of {test_charge}kWh")
             charge_message = "** test charge **"
             kwh_needed = test_charge
         # work out time to add kwh_needed to battery
         taper_time = 10/60 if (start_residual + kwh_needed) >= (capacity * 0.95) else 0
         hours = round_time(kwh_needed / (charge_limit * charge_loss + discharge_timed[time_to_next]) + taper_time)
         # full charge if requested or charge time exceeded or charge needed exceeds capacity
-        if full_charge is not None or force_charge == 2 or hours > charge_time or (start_residual + kwh_needed) > (capacity * 1.05):
+        if full_charge is not None or force_charge == 2 or hours > charge_time or (start_residual + kwh_needed) > (capacity * 1.01):
             kwh_needed = capacity - start_residual
-            hours = round_time(kwh_needed / (charge_limit * charge_loss + discharge_timed[time_to_next]) + taper_time)
-            if full_charge is not None or force_charge == 2 or hours > charge_time:
-                hours = charge_time
-                output(f"  Full charge time used")
+            hours = charge_time
+            output(f"  Full charge time used")
         elif hours < charge_config['min_hours']:
             hours = charge_config['min_hours']
 #            output(f"  Minimum charge time used")
         end1 = round_time(start_at + hours)
-        # rework charge and discharge and work out grid consumption
+        # rework charge and discharge
         start_timed = time_to_start      # relative start and end time 
         end_timed = start_timed + hours
         charge_timed_old = [x for x in charge_timed]
         discharge_timed_old = [x for x in discharge_timed]
         for i in range(time_to_next, int(time_to_next + hours + 2)):
             j = i + 1
             # work out time (fraction of hour) when charging in hour from i to j
@@ -2841,52 +2899,53 @@
         # rebuild the battery residual with the charge added
         # adjust residual from hour_now to what it was at the start of current hour
         h = base_hour
         kwh_timed = [charge * charge_loss - discharge for charge, discharge in zip(charge_timed, discharge_timed)]
         kwh_current = residual - kwh_timed[0] * (hour_now - h)
         bat_timed_old = [x for x in bat_timed]     # save for before / after comparison
         bat_timed = []
-        reserve_drain = reserve
+        reserve_drain_now = reserve
         for i in range(0, run_time):
-            if kwh_current <= reserve:
+            reserve_now = capacity * min_soc_now / 100
+            reserve_drain = capacity * (min_soc_now - 4) / 100
+            reserve_drain_now = reserve_now if reserve_drain_now > reserve_now or reserve_drain_now < reserve_drain else reserve_drain_now 
+            if kwh_current <= reserve_now and i <= time_to_next:
                 # battery is empty
-                if reserve_drain < (capacity * 6 / 100):
-                    reserve_drain = reserve           # force charge by BMS
-                kwh_current = reserve_drain           # stop discharge below reserve
-                reserve_drain -= bms_loss             # BMS drain
+                kwh_current = reserve_drain_now        # stop discharge below reserve
+                reserve_drain_now -= bms_loss          # allow for BMS drain
             else:
-                reserve_drain = reserve                # reset drain
+                reserve_drain_now = reserve_now           # reset drain
             if kwh_current > capacity:
                 # battery is full
                 kwh_current = capacity
             bat_timed.append(kwh_current)
             kwh_current += kwh_timed[i]
+            min_soc_now = work_mode_timed[i]['fdsoc'] if work_mode_timed[i]['mode'] =='ForceDischarge' else work_mode_timed[i]['min_soc']
             h += 1
         time_to_end = int(start_timed + hours) + 1
         kwh_added = bat_timed[time_to_end] - bat_timed_old[time_to_end]
         end_part_hour = end_timed - int(end_timed)
         old_residual = interpolate(end_timed, bat_timed_old)
         new_residual = capacity if old_residual + kwh_added > capacity else old_residual + kwh_added
         net_added = new_residual - start_residual
         end_soc = int(new_residual / capacity * 100 + 0.5)
-#        output(f"  Charging for {int(hours * 60)} minutes adds {net_added:.2f}kWh")
         output(f"  Start SoC: {start_residual / capacity * 100:3.0f}% at {hours_time(start_at)} ({start_residual:.2f}kWh)")
         output(f"  End SoC:   {end_soc:3.0f}% at {hours_time(end1)} ({new_residual:.2f}kWh)")
     if show_data > 2:
         output(f"\nTime, Generation, Charge, Consumption, Discharge, Residual, kWh")
         for i in range(0, run_time):
             h = base_hour + i
             output(f"  {hours_time(h)}, {generation_timed[i]:6.3f}, {charge_timed[i]:6.3f}, {consumption_timed[i]:6.3f}, {discharge_timed[i]:6.3f}, {bat_timed[i]:6.3f}")
         if kwh_needed > 0 and show_data > 3:
             output(f"\nTime, Generation, Charge, Consumption, Discharge, Residual, kWh (before charging)")
             for i in range(0, run_time):
                 h = base_hour + i
                 output(f"  {hours_time(h)}, {generation_timed[i]:6.3f}, {charge_timed_old[i]:6.3f}, {consumption_timed[i]:6.3f}, {discharge_timed_old[i]:6.3f}, {bat_timed_old[i]:6.3f}")
     if show_data > 0:
-        data_wrap = charge_config['data_wrap']
+        data_wrap = charge_config['data_wrap'] if charge_config.get('data_wrap') is not None else 6
         s = f"\nBattery Energy kWh:\n" if show_data == 2 else f"\nBattery SoC %:\n"
         s += " " * (18 if show_data == 2 else 17) * (base_hour % data_wrap)
         h = base_hour
         for r in bat_timed:
             s += "\n" if h > hour_now and h % data_wrap == 0 else ""
             s += f"  {hours_time(h - (hour_adjustment if h >= change_hour else 0), day=True)}"
             s += f" = {r:5.2f}," if show_data == 2 else f" = {r / capacity * 100:3.0f}%,"
@@ -2914,27 +2973,26 @@
         plt.grid()
         if show_plot > 1:
             plt.legend(fontsize=8, loc="upper right")
         plot_show()
     if test_charge is not None:
         return None
     # work out charge periods settings
-    start2 = round_time(start_at if hours == 0 else end1 + 1 / 60)       # add 1 minute to end time
-    if force_charge == 1 and hour_in(start2, {'start':start_at, 'end': end_by}):
+    start2 = round_time(start_at if hours == 0 else end1)
+    if force_charge > 0 and hour_in(start2, {'start':start_at, 'end': end_by}):
         end2 = end_by
     else:
             end2 = start2
     # setup charging
     if update_settings == 1:
         # adjust times for clock changes
         adjust = hour_adjustment if hour_adjustment != 0 and start_hour > change_hour else 0
         if timed_mode > 1:
-            schedule = charge_strategy(st1 = start_at, en1 = end1, st2 = start2, en2 = end2, adjust = adjust, min_soc = end_soc)
-            output(f"Schedule = {schedule}", 2)
-            set_schedule(periods = schedule)
+            periods = charge_strategy(st1 = start_at, en1 = end1, st2 = start2, en2 = end2, adjust = adjust, min_soc = min_soc, target_soc = end_soc if target_soc <= 10 else target_soc)
+            set_schedule(periods = periods)
         else:
             set_charge(ch1 = True, st1 = start_at, en1 = end1, ch2 = False, st2 = start2, en2 = end2, adjust = adjust, force = charge_config['force'])
     else:
         print(f"\nNo changes made to charge settings")
     output_close(plot=show_plot)
     return None
```

### Comparing `foxesscloud-2.2.6/src/foxesscloud/openapi.py` & `foxesscloud-2.2.7/src/foxesscloud/openapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud using Open API
-Updated:  12 May 2024
+Updated:  22 May 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud api site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2024
 ##################################################################################################
 
-version = "2.2.6"
+version = "2.2.7"
 print(f"FoxESS-Cloud Open API version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -653,28 +653,25 @@
         else:
             output(f"** set_charge(), {errno_message(response)}")
         return None
     else:
         output(f"success", 2) 
     return battery_settings
 
-def charge_strategy(st1 = None, en1 = None, st2 = None, en2 = None, adjust=0, min_soc=None):
+def charge_strategy(st1 = None, en1 = None, st2 = None, en2 = None, adjust=0, min_soc=10, target_soc=None):
     output(f"\nConfiguring schedule", 1)
-    periods = set_strategy()
+    periods = set_strategy(min_soc = min_soc, quiet=0)
     if st1 is not None and en1 is not None and st1 != en1:
         st1 = round_time(time_hours(st1) + adjust)
         en1 = round_time(time_hours(en1) + adjust)
-        output(f"   Force Charge from {hours_time(st1)} to {hours_time(en1)}", 1)
-        periods.append(set_group(start = st1, end = en1, mode = 'ForceCharge'))
+        periods.append(set_group(start = st1, end = en1, mode = 'ForceCharge', min_soc = target_soc, quiet=0))
     if st2 is not None and en2 is not None and st2 != en2:
         st2 = round_time(time_hours(st2) + adjust)
         en2 = round_time(time_hours(en2) + adjust)
-        mode = 'SelfUse'
-        output(f"   {mode} from {hours_time(st2)} to {hours_time(en2)} with min_soc = {min_soc}%", 1)
-        periods.append(set_group(start = st2, end = en2, mode = mode, fdsoc = min_soc))
+        periods.append(set_group(start = st2, end = en2, mode = 'SelfUse', min_soc = target_soc, quiet=0))
     return periods
 
 ##################################################################################################
 # get min soc settings and save in battery_settings
 ##################################################################################################
 
 def get_min():
@@ -1046,55 +1043,59 @@
     return schedule
 
 ##################################################################################################
 # set schedule
 ##################################################################################################
 
 # create time segment structure. Note: end time is exclusive.
-def set_group(start, end, mode=None, min_soc=None, fdsoc=None, fdpwr=None, enable=1):
-    if start is None or end is None:
-        return None
+def set_group(start, end, mode=None, min_soc=None, fdsoc=None, fdpwr=None, enable=1, quiet=1):
     start = time_hours(start)
     end = time_hours(end)
+    if start is None or end is None:
+        return None
+    end = round_time(end - 1/60)        # adjust exclusive time to inclusive
     mode = 'SelfUse' if mode is None else mode
-    min_soc = 10 if min_soc is None else min_soc
-    fdsoc = 10 if fdsoc is None else fdsoc
-    fdpwr = 0 if fdpwr is None else fdpwr
     if mode not in work_modes:
         output(f"** mode must be one of {work_modes}")
         return None
-    device_power = device.get('power') if device is not None else None
-    if device_power is None:
-        device_power = 12000
-    if fdpwr < 0 or fdpwr > 12000:
-        output(f"** fdpwr must be between 0 and {device_power}")
+    min_soc = 10 if min_soc is None else min_soc
+    fdsoc = min_soc if fdsoc is None else fdsoc
+    fdpwr = 0 if fdpwr is None else fdpwr
+    if min_soc < 10 or min_soc > 100:
+        output(f"** min_soc must be between 10 and 100")
+        return None
+    if fdpwr < 0 or fdpwr > 6000:
+        output(f"** fdpwr must be between 0 and 6000")
         return None
-    if fdsoc < 10 or fdsoc > 100:
-        output(f"** fdsoc must between 10 and 100")
+    if fdsoc < min_soc or fdsoc > 100:
+        output(f"** fdsoc must between {min_soc} and 100")
         return None
+    if quiet == 0:
+        output(f"   {hours_time(start)} to {hours_time(end)}: {mode} with min_soc = {min_soc}%" + (f", fdPwr = {fdpwr/1000:.3f}kW and fdSoC = {fdsoc}%" if mode == 'ForceDischarge' else ""), 1)
     start_hour, start_minute = split_hours(start)
-    end_hour, end_minute = split_hours(end - 1/60)
+    end_hour, end_minute = split_hours(end)
     group = {'enable': enable, 'startHour': start_hour, 'startMinute': start_minute, 'endHour': end_hour, 'endMinute': end_minute, 'workMode': mode, 'minSocOnGrid': min_soc, 'fdSoc': fdsoc, 'fdPwr': fdpwr}
     return group
 
 # create groups from a list of strategy periods
-def set_strategy(strategy=None):
+def set_strategy(strategy=None, min_soc=10, quiet=1):
     global tariff
     if strategy is None and tariff is not None:
         strategy = tariff.get('strategy')
     if strategy is None:
         return []
     if type(strategy) is not list:
         strategy = [strategy]
-    groups = []
+    periods = []
     for s in strategy:
-        p = set_group(s['start'], s['end'], s.get('mode'), s.get('min_soc'), s.get('fdsoc'), s.get('fdpwr'))
+        min_soc = s['min_soc'] if s.get('min_soc') is not None and s['min_soc'] > min_soc else min_soc
+        p = set_group(s['start'], s['end'], s['mode'], min_soc, s.get('fdsoc'), s.get('fdpwr'), quiet=quiet)
         if p is not None:
-            groups.append(p)
-    return groups
+            periods.append(p)
+    return periods
 
 # set a schedule from a period or list of time segment groups
 def set_schedule(groups=None, enable=1):
     global token, device_sn, debug_setting, schedule
     if get_flag() is None:
         return None
     output(f"set_schedule(): enable = {enable}, groups = {groups}", 2)
@@ -1686,14 +1687,16 @@
     minutes = int (h % 1 * 60 + 0.5)
     return (hours, minutes)
 
 # convert time string HH:MM:SS to decimal hours (range 0 to 24)
 # If BST time zone is included, convert to GMT (range -1 to 23)
 def time_hours(t, d = None):
     if t is None:
+        if d is None:
+            return None
         t = d
     if type(t) is float:
         return t
     if type(t) is int:
         return float(t)
     offset = 1 if 'BST' in t else 0
     t = t[0:8]
@@ -1718,33 +1721,55 @@
         h -= 24
         d += 1
     suffix = ""
     if day:
         suffix = f"/{d:0}"
     return f"{int(h):02}:{int(h * 60 % 60):02}:{int(h * 3600 % 60):02}"[:n] + suffix
 
-# True if a decimal hour is within a time period
+# True if a decimal hour falls within a time period
 def hour_in(h, period):
     if period is None:
         return False
-    s = period['start']
-    e = period['end']
+    s = period.get('start')
+    e = period.get('end')
     if s is None or e is None or s == e:
         return False
     while h < 0:
         h += 24
     while h >= 24:
         h -= 24
     if s > e:
         # e.g. 16:00 - 07:00
         return h >= s or h < e
     else:
         # e.g. 02:00 - 05:00
         return h >= s and h < e
 
+# Time in a decimal hour that falls within a time period
+def duration_in(h, period):
+    if period is None:
+        return None
+    duration = 1.0
+    s = period.get('start')
+    e = period.get('end')
+    if s is None or e is None:
+        return None
+    if s == e:
+        return 0.0
+    if e > s and (h >= e or (h + 1) <= s):    # normal time
+            return 0.0
+    if e < s and (h >= e and (h + 1) <= s):   # wrap around time
+            return 0.0
+    if s > h and s < (h + 1):
+        duration -= (s - h)
+    if e > h and e < (h + 1):
+        duration -= (h + 1 - e)
+    duration = 1.0 if duration > 1.0 else 0.0 if duration < 0.0 else duration
+    return duration
+
 # Return the hours in a time period with optional value check
 def period_hours(period, check = None, value = 1):
     if period is None:
         return 0
     if check is not None and period[check] != value:
         return 0
     return round_time(period['end'] - period['start'])
@@ -1798,16 +1823,17 @@
     'name': 'Octopus Flux',
     'off_peak1': {'start': 2.0, 'end': 5.0, 'force': 1},        # off-peak period 1 / am charging period
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},        # off-peak period 2 / pm charging period
     'peak': {'start': 16.0, 'end': 19.0 },                      # peak period 1
     'peak2': {'start': 0.0, 'end': 0.0 },                       # peak period 2
     'forecast_times': [22, 23],                                 # hours in a day to get a forecast
     'strategy': [                                               # timed work mode settings
-        {'start': 5, 'end': 12, 'mode': 'SelfUse'},
-        {'start': 16, 'end': 23, 'mode': 'Feedin'}]
+        {'start': 0, 'end': 2, 'mode': 'Feedin'},
+        {'start': 5, 'end': 6, 'mode': 'SelfUse'},
+        {'start': 16, 'end': 24, 'mode': 'Feedin'}]
     }
 
 # time periods for Intelligent Octopus
 intelligent_octopus = {
     'name': 'Intelligent Octopus',
     'off_peak1': {'start': 23.5, 'end': 5.5, 'force': 1},
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},
@@ -2056,79 +2082,80 @@
     if charge_pm:
         tariff['off_peak2']['start'] = start
         tariff['off_peak2']['end'] = end
     else:
         tariff['off_peak1']['start'] = start
         tariff['off_peak1']['end'] = end
         gmt = " GMT" if tariff['off_peak1'].get('gmt') is not None else ""
-    print(f"\n{tariff['name']} {am_pm} charging period: {hours_time(start)} to {hours_time(end)}{gmt}")
+    output(f"\n{tariff['name']} {am_pm} charging period: {hours_time(start)} to {hours_time(end)}{gmt}")
     return 1
 
 # set tariff and AM/PM charge time period
 def set_tariff(find, update=1, start_at=None, end_by=None, duration=None, times=None, forecast_times=None, strategy=None, d=None, **settings):
     global debug_setting, agile_octopus, tariff, tariff_list
-    print(f"\n---------------- set_tariff -----------------")
+    output(f"\n---------------- set_tariff -----------------", 1)
     # validate parameters
     args = locals()
     s = ""
     for k in [k for k in args.keys() if args[k] is not None and k != 'settings']:
         s += f"\n  {k} = {args[k]}"
     # store settings:
     for key, value in settings.items():
         if key not in tariff_config:
             print(f"** unknown configuration parameter: {key}")
         else:
             tariff_config[key] = value
             s += f"\n  {key} = {value}"
-    if len(s) > 0 and debug_setting > 1:
-        print(f"Parameters: {s}")
+    if len(s) > 0:
+        output(f"Parameters: {s}", 2)
     found = []
     if find in tariff_list:
         found = [find]
     elif type(find) is str:
         for dict in tariff_list:
             if find.lower() in dict['name'].lower():
                 found.append(dict)
     if len(found) != 1:
-        print(f"** set_tariff(): {find} must identify one of the available tariffs:")
+        output(f"** set_tariff(): {find} must identify one of the available tariffs:")
         for x in tariff_list:
             print(f"  {x['name']}")
         return None
     use = found[0]
     if times is None:
         times = [(start_at, end_by, duration)] if start_at is not None or end_by is not None or duration is not None else [(None, None, 3)]
     elif type(times) is not list:
         times = [times]
     if len(times) > 2:
-        print(f"** set_tariff(): one AM (11pm - 11am) and one PM (11am - 11pm) charge time can be set. times = {times}")
+        output(f"** set_tariff(): one AM (11pm - 11am) and one PM (11am - 11pm) charge time can be set. times = {times}")
         return None
     set_proc = set_agile_period if use == agile_octopus else set_tariff_period
     for t in times:
         result = set_proc(period={'start': t[0], 'end': t[1], 'duration': t[2]}, tariff=use, d=d)
         if result is None:
             return None
     if forecast_times is not None:
         if type(forecast_times) is not list:
             forecast_times = [forecast_times]
         forecast_hours = []
         for i, t in enumerate(forecast_times):
             forecast_times[i] = hours_time(t)
             forecast_hours.append(time_hours(t))
         use['forecast_times'] = forecast_hours
-        print(f"\nForecast times set to {forecast_times}")
+        output(f"Forecast times set to {forecast_times}", 1)
     if strategy is not None:
         if type(strategy) is not list:
             strategy = [strategy]
         use['strategy'] = strategy
-        print(f"\nStrategy set to {strategy}")
+        output(f"Strategy updated")
+        set_strategy(strategy, quiet=0)
     if update == 1:
         tariff = use
-        print(f"\nTariff set to {tariff['name']}")
+        output(f"\nTariff set to {tariff['name']}", 1)
     elif debug_setting > 0:
-        print(f"\nNo changes made to current tariff")
+        output(f"\nNo changes made to current tariff", 1)
     return None
 
 # get work mode for a time of day based on the tariff:
 def timed_work_mode(h, default = 'SelfUse'):
     if tariff is None or tariff.get('strategy') is None:
         return default
     for d in tariff['strategy']:
@@ -2214,32 +2241,53 @@
     for h in range(0, 24):
         profile.append(c_float(forecast.daily[tomorrow]['hourly'].get(int(round_time(h - time_offset)))))
     timed = []
     for h in range(int(hour_now), 24):
         timed.append(c_float(forecast.daily[today]['hourly'].get(int(round_time(h - time_offset)))))
     return (timed + profile + profile)[:run_time]
 
+# take a strategy and return a timed profile:
+def strategy_timed(timed_mode, hour_now, run_time, min_soc=10):
+    global tariff
+    profile = []
+    for h in range(0, 24):
+        profile.append({'mode': 'SelfUse', 'min_soc': min_soc, 'fdpwr': 0, 'fdsoc': min_soc, 'duration': 1.0})
+        if tariff is None or tariff.get('strategy') is None or timed_mode == 0:
+            continue
+        for d in tariff['strategy']:
+            if hour_in(h, d):
+                profile[h]['mode'] = d['mode']
+                if d.get('min_soc') is not None:
+                    profile[h]['min_soc'] = d['min_soc'] if d['min_soc'] > min_soc else min_soc
+                if d.get('fdsoc') is not None:
+                    profile[h]['fdsoc'] = d['fdsoc'] if d['fdsoc'] > min_soc else min_soc
+                if d.get('fdpwr') is not None:
+                    profile[h]['fdpwr'] = d['fdpwr']
+                profile[h]['duration'] = duration_in(h, d)
+    output(f"work mode profile = {profile}", 2)
+    return (profile[int(hour_now):] + profile + profile)[:run_time]
+
 # Battery open circuit voltage (OCV) from 0% to 100% SoC
 #                 0%     10%    20%    30%    40%    50%    60%    70%    80%    90%   100%
 lifepo4_curve = [51.00, 51.50, 52.00, 52.30, 52.60, 52.80, 52.90, 53.00, 53.10, 53.30, 54.00]
 
 # charge_needed settings
 charge_config = {
-    'contingency': 20,                # % of consumption to allow as contingency
+    'contingency': [20,10,5,15],      # % of consumption. Value or [winter, spring, summer, autumn]
     'capacity': None,                 # Battery capacity (over-ride)
     'min_soc': None,                  # Minimum Soc (over-ride)
     'charge_current': None,           # max battery charge current setting in A
     'discharge_current': None,        # max battery discharge current setting in A
-    'export_limit': None,             # maximum export power
+    'export_limit': None,             # maximum export power in kW
     'discharge_loss': 0.97,           # loss converting battery discharge power to grid power
     'pv_loss': 0.95,                  # loss converting PV power to battery charge power
     'grid_loss': 0.95,                # loss converting grid power to battery charge power
     'charge_loss': None,              # loss converting charge power to residual
-    'inverter_power': None,           # Inverter power consumption W
-    'bms_power': 27,                  # BMS power consumption W
+    'inverter_power': None,           # Inverter power consumption in W
+    'bms_power': 27,                  # BMS power consumption in W
     'bat_resistance': 0.072,          # internal resistance of a battery
     'volt_curve': lifepo4_curve,      # battery OCV range from 0% to 100% SoC
     'nominal_soc': 60,                # SoC for nominal open circuit battery voltage
     'generation_days': 3,             # number of days to use for average generation (1-7)
     'consumption_days': 3,            # number of days to use for average consumption (1-7)
     'consumption_span': 'week',       # 'week' = last n days or 'weekday' = last n weekdays
     'use_today': 21.0,                # hour when todays consumption and generation can be used
@@ -2272,14 +2320,15 @@
 #  run_after: 0 over-rides 'forecast_times'. The default is 1.
 #  forecast_times: list of hours when forecast can be fetched
 #  force_charge: 1 = set force charge, 2 = charge for whole period
 
 def charge_needed(forecast=None, update_settings=0, timed_mode=None, show_data=None, show_plot=None, run_after=None,
         forecast_times=None, force_charge=None, test_time=None, test_soc=None, test_charge=None, **settings):
     global device, seasonality, solcast_api_key, debug_setting, tariff, solar_arrays, legend_location, time_shift, default_min_soc, charge_needed_app_key
+    global timed_strategy
     print(f"\n---------------- charge_needed ----------------")
     # validate parameters
     args = locals()
     s = ""
     for k in [k for k in args.keys() if args[k] is not None and k != 'settings']:
         s += f"\n  {k} = {args[k]}"
     # store settings:
@@ -2324,28 +2373,28 @@
     force_charge = 0 if force_charge is None else force_charge
     start_am = time_hours(tariff['off_peak1']['start'] if tariff is not None else 2.0)
     end_am = time_hours(tariff['off_peak1']['end'] if tariff is not None else 5.0)
     # adjust times for Economy 7 in BST
     if time_offset > 0 and tariff is not None and tariff['off_peak1'].get('gmt') is not None:
         start_am += 1
         end_am += 1
-    force_charge_am = 0 if tariff is not None and tariff['off_peak1']['force'] == 0 or force_charge == 0 else force_charge
+    force_charge_am = 0 if (tariff is not None and tariff['off_peak1']['force'] == 0) or force_charge == 0 else 1
     time_to_am = round_time(start_am - base_hour)
     start_pm = time_hours(tariff['off_peak2']['start'] if tariff is not None else 0.0)
     end_pm = time_hours(tariff['off_peak2']['end'] if tariff is not None else 0.0)
-    force_charge_pm = 0 if tariff is not None and tariff['off_peak2']['force'] == 0 or force_charge == 0 else 1
+    force_charge_pm = 0 if (tariff is not None and tariff['off_peak2']['force'] == 0) or force_charge == 0 else 1
     time_to_pm = round_time(start_pm - base_hour) if start_pm > 0 else None
     no_go1 = time_to_am is not None and hour_in(hour_now, {'start': round_time(start_am - 0.25), 'end': round_time(end_am + 0.25)})
     no_go2 = time_to_pm is not None and hour_in(hour_now, {'start': round_time(start_pm - 0.25), 'end': round_time(end_pm + 0.25)})
     if (no_go1 or no_go2) and update_settings > 0:
         print(f"\nInverter settings will not be changed less than 15 minutes before or after a charging period")
         update_settings = 0
     # choose and configure parameters for next charge time period
     charge_pm = time_to_pm is not None and time_to_pm < time_to_am
-    force_charge = force_charge_pm if charge_pm else force_charge_am
+    force_charge = force_charge_pm if charge_pm else force_charge if force_charge_am == 1 else 0
     start_at = start_pm if charge_pm else start_am
     end_by = end_pm if charge_pm else end_am
     charge_time = round_time(end_by - start_at)
     time_to_start = time_to_pm if charge_pm else time_to_am
     start_hour = base_hour + time_to_start
     time_to_next = int(time_to_start)
     start_part_hour = time_to_start % 1
@@ -2590,106 +2639,117 @@
         if charge_config['forecast_selection'] == 1 and update_settings > 0:
             output(f"\nSettings will not be updated when forecast is not available")
             update_settings = 0
     # produce time lines for main charge and discharge (after losses)
     charge_timed = [x * charge_config['pv_loss'] for x in generation_timed]
     discharge_timed = [x / charge_config['discharge_loss'] for x in consumption_timed]
     # adjust charge and discharge time lines for work mode, force charge and power limits
-    work_mode = current_mode
+    work_mode_timed = strategy_timed(timed_mode, hour_now, run_time, min_soc)
+    work_mode = work_mode_timed[0]['mode'] if current_mode is None else current_mode
     for i in range(0, run_time):
         h = base_hour + i
         # get work mode and check for changes
-        new_work_mode = timed_work_mode(h, current_mode) if timed_mode > 0 else current_mode
-        if new_work_mode is not None and new_work_mode != work_mode:
+        new_work_mode = work_mode_timed[i]['mode']
+        if new_work_mode != work_mode:
             output(f"  {hours_time(h)}: {new_work_mode} work mode", 2)
             work_mode = new_work_mode
         # cap charge / discharge power
         charge_timed[i] = charge_limit if charge_timed[i] > charge_limit else charge_timed[i]
         discharge_timed[i] = discharge_limit if discharge_timed[i] > discharge_limit else discharge_timed[i]
-        if force_charge_am == 1 and hour_in(h, {'start': start_am, 'end': end_am}):
+        # apply changes due to work mode
+        duration = work_mode_timed[i]['duration']
+        if timed_mode > 0 and work_mode == 'ForceCharge':
+            (discharge_timed[i], charge_timed[i]) = (discharge_timed[i] * (1.0 - duration),
+                charge_limit * duration + charge_timed[i] * (1.0 - duration))
+        elif timed_mode > 0 and work_mode == 'ForceDischarge':
+            fdpwr = work_mode_timed[i]['fdpwr'] / charge_config['discharge_loss']
+            fdpwr = min([discharge_limit, export_limit * 1000 + discharge_timed[i], fdpwr])
+            (discharge_timed[i], charge_timed[i]) = (fdpwr * duration + discharge_timed[i] * (1.0 - duration) - charge_timed[i] * duration,
+                charge_timed[i] * (1.0 - duration))
+        elif force_charge_am == 1 and hour_in(h, {'start': start_am, 'end': end_am}):
             discharge_timed[i] = operating_loss if charge_timed[i] == 0.0 else 0.0
         elif force_charge_pm == 1 and hour_in(h, {'start': start_pm, 'end': end_pm}):
             discharge_timed[i] = operating_loss if charge_timed[i] == 0.0 else 0.0
         elif timed_mode > 0 and work_mode == 'Backup':
             discharge_timed[i] = operating_loss if charge_timed[i] == 0.0 else 0.0
         elif timed_mode > 0 and work_mode == 'Feedin':
             (discharge_timed[i], charge_timed[i]) = (bms_loss if (charge_timed[i] >= discharge_timed[i]) else (discharge_timed[i] - charge_timed[i]),
-                0.0 if (charge_timed[i] <= export_limit + discharge_timed[i]) else (charge_timed[i] - export_limit - discharge_timed[i]))
+                0.0 if (charge_timed[i] <= export_limit * 1000 + discharge_timed[i]) else (charge_timed[i] - export_limit * 1000 - discharge_timed[i]))
         else: # work_mode == 'SelfUse'
             (discharge_timed[i], charge_timed[i]) = (bms_loss if (charge_timed[i] >= discharge_timed[i]) else (discharge_timed[i] - charge_timed[i]),
                 0.0 if (charge_timed[i] <= discharge_timed[i]) else (charge_timed[i] - discharge_timed[i]))
     # track the battery residual over the run time (if we don't add any charge)
     # adjust residual from hour_now to what it was at the start of current hour
     h = base_hour
     kwh_timed = [charge * charge_loss - discharge for charge, discharge in zip(charge_timed, discharge_timed)]
     kwh_current = residual - kwh_timed[0] * (hour_now - h)
     bat_timed = []
-    kwh_min = kwh_current
-    min_hour = h
-    reserve_drain = reserve
+    kwh_min = capacity
+    reserve_drain_now = reserve
+    min_soc_now = min_soc
     for i in range(0, run_time):
-        if kwh_current <= reserve and i <= time_to_next:
+        reserve_now = capacity * min_soc_now / 100
+        reserve_drain = capacity * (min_soc_now - 4) / 100
+        reserve_drain_now = reserve_now if reserve_drain_now > reserve_now or reserve_drain_now < reserve_drain else reserve_drain_now
+        if kwh_current <= reserve_now and i <= time_to_next:
             # battery is empty
-            if reserve_drain < (capacity * 6 / 100):
-                reserve_drain = reserve           # force charge to restore reserve
-            kwh_current = reserve_drain           # stop discharge below reserve
-            reserve_drain -= bms_loss             # allow for BMS drain
+            kwh_current = reserve_drain_now       # stop discharge below reserve
+            reserve_drain_now -= bms_loss         # allow for BMS drain
         else:
-            reserve_drain = reserve                # reset drain
+            reserve_drain_now = reserve_now       # reset drain
         if kwh_current > capacity:
             # battery is full
             kwh_current = capacity
         bat_timed.append(kwh_current)
-        if kwh_current < kwh_min:       # track minimum and time
+        if kwh_current < kwh_min and i >= time_to_next:       # track minimum after next charge
             kwh_min = kwh_current
             min_hour = h
         kwh_current += kwh_timed[i]
+        min_soc_now = work_mode_timed[i]['fdsoc'] if work_mode_timed[i]['mode'] =='ForceDischarge' else work_mode_timed[i]['min_soc']
         h += 1
     # work out what we need to add to stay above reserve and provide contingency or to hit target_soc
     contingency = charge_config['special_contingency'] if tomorrow[-5:] in charge_config['special_days'] else charge_config['contingency']
+    contingency = contingency[quarter] if type(contingency) is list else contingency
     kwh_contingency = consumption * contingency / 100
     kwh_needed = reserve + kwh_contingency - kwh_min
     start_residual = interpolate(time_to_start, bat_timed)      # residual when charging starts
-    target_soc = charge_config['target_soc'] if charge_config.get('target_soc') is not None else 0
-    target_kwh = capacity if target_soc > 100 else target_soc / 100 * capacity
+    target_soc = charge_config['target_soc'] if charge_config.get('target_soc') is not None else 10
+    target_soc = 100 if target_soc > 100 else 10 if target_soc < 10 else target_soc
+    target_kwh = target_soc / 100 * capacity
     if target_kwh > (start_residual + kwh_needed):
         kwh_needed = target_kwh - start_residual
-    day_when = 'today' if min_hour < 24 else 'tomorrow' if min_hour <= 48 else 'day after tomorrow'
     if kwh_min > reserve and kwh_needed < charge_config['min_kwh'] and full_charge is None and test_charge is None:
-        output(f"\nNo charging is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh)")
+        output(f"\nNo charging is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh, contingency = {kwh_contingency:.1f}kWh)")
         charge_message = "no charge needed"
         kwh_needed = 0.0
         hours = 0.0
         end1 = start_at
         end_soc = int(start_residual / capacity * 100 + 0.5)
         output(f"   Expected SoC at {hours_time(start_at)} is {end_soc}%")
     else:
         charge_message = "with charge added"
         if test_charge is None:
-            min_hour_adjust = min_hour - hour_adjustment if min_hour >= change_hour else 0
-            output(f"\nCharge of {kwh_needed:.2f}kWh is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh)")
+            output(f"\nCharge of {kwh_needed:.2f}kWh is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh, contingency = {kwh_contingency:.1f}kWh)")
         else:
             output(f"\nTest charge of {test_charge}kWh")
             charge_message = "** test charge **"
             kwh_needed = test_charge
         # work out time to add kwh_needed to battery
         taper_time = 10/60 if (start_residual + kwh_needed) >= (capacity * 0.95) else 0
         hours = round_time(kwh_needed / (charge_limit * charge_loss + discharge_timed[time_to_next]) + taper_time)
         # full charge if requested or charge time exceeded or charge needed exceeds capacity
-        if full_charge is not None or force_charge == 2 or hours > charge_time or (start_residual + kwh_needed) > (capacity * 1.05):
+        if full_charge is not None or force_charge == 2 or hours > charge_time or (start_residual + kwh_needed) > (capacity * 1.01):
             kwh_needed = capacity - start_residual
-            hours = round_time(kwh_needed / (charge_limit * charge_loss + discharge_timed[time_to_next]) + taper_time)
-            if full_charge is not None or force_charge == 2 or hours > charge_time:
-                hours = charge_time
-                output(f"  Full charge time used")
+            hours = charge_time
+            output(f"  Full charge time used")
         elif hours < charge_config['min_hours']:
             hours = charge_config['min_hours']
 #            output(f"  Minimum charge time used")
         end1 = round_time(start_at + hours)
-        # rework charge and discharge and work out grid consumption
+        # rework charge and discharge
         start_timed = time_to_start      # relative start and end time 
         end_timed = start_timed + hours
         charge_timed_old = [x for x in charge_timed]
         discharge_timed_old = [x for x in discharge_timed]
         for i in range(time_to_next, int(time_to_next + hours + 2)):
             j = i + 1
             # work out time (fraction of hour) when charging in hour from i to j
@@ -2710,52 +2770,53 @@
         # rebuild the battery residual with the charge added
         # adjust residual from hour_now to what it was at the start of current hour
         h = base_hour
         kwh_timed = [charge * charge_loss - discharge for charge, discharge in zip(charge_timed, discharge_timed)]
         kwh_current = residual - kwh_timed[0] * (hour_now - h)
         bat_timed_old = [x for x in bat_timed]     # save for before / after comparison
         bat_timed = []
-        reserve_drain = reserve
+        reserve_drain_now = reserve
         for i in range(0, run_time):
-            if kwh_current <= reserve:
+            reserve_now = capacity * min_soc_now / 100
+            reserve_drain = capacity * (min_soc_now - 4) / 100
+            reserve_drain_now = reserve_now if reserve_drain_now > reserve_now or reserve_drain_now < reserve_drain else reserve_drain_now 
+            if kwh_current <= reserve_now and i <= time_to_next:
                 # battery is empty
-                if reserve_drain < (capacity * 6 / 100):
-                    reserve_drain = reserve           # force charge by BMS
-                kwh_current = reserve_drain           # stop discharge below reserve
-                reserve_drain -= bms_loss             # BMS drain
+                kwh_current = reserve_drain_now       # stop discharge below reserve
+                reserve_drain_now -= bms_loss         # BMS drain
             else:
-                reserve_drain = reserve                # reset drain
+                reserve_drain_now = reserve_now       # reset drain
             if kwh_current > capacity:
                 # battery is full
                 kwh_current = capacity
             bat_timed.append(kwh_current)
             kwh_current += kwh_timed[i]
+            min_soc_now = work_mode_timed[i]['fdsoc'] if work_mode_timed[i]['mode'] =='ForceDischarge' else work_mode_timed[i]['min_soc']
             h += 1
         time_to_end = int(start_timed + hours) + 1
         kwh_added = bat_timed[time_to_end] - bat_timed_old[time_to_end]
         end_part_hour = end_timed - int(end_timed)
         old_residual = interpolate(end_timed, bat_timed_old)
         new_residual = capacity if old_residual + kwh_added > capacity else old_residual + kwh_added
         net_added = new_residual - start_residual
         end_soc = int(new_residual / capacity * 100 + 0.5)
-#        output(f"  Charging for {int(hours * 60)} minutes adds {net_added:.2f}kWh")
         output(f"  Start SoC: {start_residual / capacity * 100:3.0f}% at {hours_time(start_at)} ({start_residual:.2f}kWh)")
         output(f"  End SoC:   {end_soc:3.0f}% at {hours_time(end1)} ({new_residual:.2f}kWh)")
     if show_data > 2:
         output(f"\nTime, Generation, Charge, Consumption, Discharge, Residual, kWh")
         for i in range(0, run_time):
             h = base_hour + i
             output(f"  {hours_time(h)}, {generation_timed[i]:6.3f}, {charge_timed[i]:6.3f}, {consumption_timed[i]:6.3f}, {discharge_timed[i]:6.3f}, {bat_timed[i]:6.3f}")
         if kwh_needed > 0 and show_data > 3:
             output(f"\nTime, Generation, Charge, Consumption, Discharge, Residual, kWh (before charging)")
             for i in range(0, run_time):
                 h = base_hour + i
                 output(f"  {hours_time(h)}, {generation_timed[i]:6.3f}, {charge_timed_old[i]:6.3f}, {consumption_timed[i]:6.3f}, {discharge_timed_old[i]:6.3f}, {bat_timed_old[i]:6.3f}")
     if show_data > 0:
-        data_wrap = charge_config['data_wrap']
+        data_wrap = charge_config['data_wrap'] if charge_config.get('data_wrap') is not None else 6
         s = f"\nBattery Energy kWh:\n" if show_data == 2 else f"\nBattery SoC %:\n"
         s += " " * (18 if show_data == 2 else 17) * (base_hour % data_wrap)
         h = base_hour
         for r in bat_timed:
             s += "\n" if h > hour_now and h % data_wrap == 0 else ""
             s += f"  {hours_time(h - (hour_adjustment if h >= change_hour else 0), day=True)}"
             s += f" = {r:5.2f}," if show_data == 2 else f" = {r / capacity * 100:3.0f}%,"
@@ -2783,27 +2844,26 @@
         plt.grid()
         if show_plot > 1:
             plt.legend(fontsize=8, loc="upper right")
         plot_show()
     if test_charge is not None:
         return None
     # work out charge periods settings
-    start2 = round_time(start_at if hours == 0 else end1 + 1 / 60)       # add 1 minute to end time
-    if force_charge == 1 and hour_in(start2, {'start':start_at, 'end': end_by}):
+    start2 = round_time(start_at if hours == 0 else end1)
+    if force_charge > 0 and hour_in(start2, {'start':start_at, 'end': end_by}):
         end2 = end_by
     else:
         end2 = start2
     # setup charging
     if update_settings == 1:
         # adjust times for clock changes
         adjust = hour_adjustment if hour_adjustment != 0 and start_hour > change_hour else 0
         if timed_mode > 1:
-            schedule = charge_strategy(st1 = start_at, en1 = end1, st2 = start2, en2 = end2, adjust = adjust, min_soc = end_soc)
-            output(f"Schedule = {schedule}", 2)
-            set_schedule(schedule)
+            groups = charge_strategy(st1 = start_at, en1 = end1, st2 = start2, en2 = end2, adjust = adjust, min_soc = min_soc, target_soc = end_soc if target_soc <= 10 else target_soc)
+            set_schedule(groups)
         else:
             set_charge(ch1 = True, st1 = start_at, en1 = end1, ch2 = False, st2 = start2, en2 = end2, adjust = adjust, force = charge_config['force'])
     else:
         output(f"\nNo changes made to charge settings")
     output_close(plot=show_plot)
     return None
```

### Comparing `foxesscloud-2.2.6/src/foxesscloud.egg-info/PKG-INFO` & `foxesscloud-2.2.7/src/foxesscloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.2.6
+Version: 2.2.7
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -345,25 +345,25 @@
 + updates your battery charge settings (if update_settings is not 0)
 + gets the current work mode and updates this if timed work mode changes are configured
 
 ### Configuration Parameters
 
 The following parameters and default values are used to configure charge_needed and may be updated if required using name=value:
 ```
-contingency: 20               # % of consumption to allow as contingency
+contingency: [20,10,5,10]     # % of consumption. Single or [winter, spring, summer, autumn] values
 capacity: None                # Battery capacity in kWh (over-rides generated value if set)
 charge_current: None          # max battery charge current setting in A. None uses a value derrived from the inverter model
 discharge_current: None       # max battery discharge current setting in A. None uses a value derrived from the inverter model
-export_limit: None            # maximum export power. None uses the inverter power rating
+export_limit: None            # maximum export power in kW. None uses the inverter power rating
 discharge_loss: 0.97          # loss converting battery discharge power to grid power
 pv_loss: 0.95                 # loss converting PV power to battery charge power
 grid_loss: 0.97               # loss converting grid power to battery charge power
 charge_loss: None             # loss converting charge power to residual
-inverter_power: None          # inverter power consumption W (dynamically set)
-bms_power: 25                 # BMS power consumption W
+inverter_power: None          # inverter power consumption in W (dynamically set)
+bms_power: 25                 # BMS power consumption in W
 bat_resistance: 0.070         # internal resistance of a battery in ohms
 volt_curve: lifepo4_curve     # battery OCV from 0% to 100% SoC
 nominal_soc: 55               # SoC for nominal open circuit voltage
 generation_days: 3            # number of days to use for average generation (1-7)
 consumption_days: 3           # number of days to use for average consumption (1-7)
 consumption_span: 'week'      # 'week' = last 7 days or 'weekday' = last 7 weekdays e.g. Saturdays
 use_today: 21.0               # hour when today's generation and consumption data will be used
@@ -686,15 +686,19 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.6<br>
+2.2.7<br>
+Updated contingency to allow seasonal values for winter, spring, summer and autumn.
+Update strategy mode to support ForceCharge and ForceDischarge work modes.
+Update so min_soc setting in charge_needed() over-rides min_soc in the tariff strategy.
+Fix force charge strategy mode in charge_neded() to set min_soc correctly.
 Implement 2 second delay between calls that change inverter settings.
 Added strategy mode (timed_mode=2) to charge_needed().
 Added set_strategy() and charge_strategy() to manage charging schedules and work mode changes.
 Refactor debug messaging.
 Simplify charge_needed() output.
 Added 'target_soc' to charge_needed() settings
 Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50 where there is no battery
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.6 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.7 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -248,92 +248,93 @@
 available now and the expected charging or discharging of the battery to
 forecast the battery state + works out if there is a deficit (i.e. when the
 battery would be discharged below your min_soc) + reports the charge needed
 (deficit) or the minimum expected battery level + updates your battery charge
 settings (if update_settings is not 0) + gets the current work mode and updates
 this if timed work mode changes are configured ### Configuration Parameters The
 following parameters and default values are used to configure charge_needed and
-may be updated if required using name=value: ``` contingency: 20 # % of
-consumption to allow as contingency capacity: None # Battery capacity in kWh
-(over-rides generated value if set) charge_current: None # max battery charge
-current setting in A. None uses a value derrived from the inverter model
-discharge_current: None # max battery discharge current setting in A. None uses
-a value derrived from the inverter model export_limit: None # maximum export
-power. None uses the inverter power rating discharge_loss: 0.97 # loss
-converting battery discharge power to grid power pv_loss: 0.95 # loss
-converting PV power to battery charge power grid_loss: 0.97 # loss converting
-grid power to battery charge power charge_loss: None # loss converting charge
-power to residual inverter_power: None # inverter power consumption W
-(dynamically set) bms_power: 25 # BMS power consumption W bat_resistance: 0.070
-# internal resistance of a battery in ohms volt_curve: lifepo4_curve # battery
-OCV from 0% to 100% SoC nominal_soc: 55 # SoC for nominal open circuit voltage
-generation_days: 3 # number of days to use for average generation (1-7)
-consumption_days: 3 # number of days to use for average consumption (1-7)
-consumption_span: 'week' # 'week' = last 7 days or 'weekday' = last 7 weekdays
-e.g. Saturdays use_today: 21.0 # hour when today's generation and consumption
-data will be used min_hours: 0.25 # minimum charge time to set (in decimal
-hours) min_kwh: 0.5 # minimum charge to add in kwh solcast_adjust: 100 # %
-adjustment to make to Solcast forecast solar_adjust: 100 # % adjustment to make
-to Solar forecast forecast_selection: 1 # 1 = only update charge times if
-forecast is available, 0 = use best available data. Default is 1.
-annual_consumption: None # optional annual consumption in kWh. If set, this
-replaces consumption history timed_mode: 0 # 0 = None, 1 = use timed work mode,
-2 = strategy mode special_contingency: 30 # contingency for special days when
-consumption might be higher special_days: ['12-25', '12-26', '01-01']
-full_charge: None # day of month (1-28) to do full charge or 'daily' or day of
-week: 'Mon', 'Tue' etc derate_temp: 21 # battery temperature in C when derating
-charge current is applied derate_step: 5 # step size for derating e.g. 21, 16,
-11 derating: [24, 15, 10, 2] # derated charge current for each temperature step
-e.g. 21C, 16C, 11C, 6C force: 1 # 1 = disable strategy periods when setting
-charge. 0 = fail if strategy period has been set. data_wrap: 6 # data items to
-show per line target_soc: None # target soc for charging ``` These values are
-stored / available in f.charge_config. The default battery open circuit voltage
-curve versus SoC from 0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30,
-52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ``` When operating in
-strategy mode (timed_mode=2), charge_needed will create a schedule that
-includes the strategy for the tariff with additional time segments added to
-charge from grid and (optionall) to stop the battery discharging. In other
-modes, charge_needed() will disable any schedules and set the battery charge
-times. This example shows the results reported by charge needed: ![image]
-(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-
-b165-20d806b1e7e8) ## Battery Info Provides detailed information on the current
-state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
-(interval, run, log, save, count) ``` battery_info() prints information on the
-battery and cells: + count: optional over-ride. The default is based on
-factorising the number of cells reported by 16 or 18 to work out the number of
-batteries. + plot: 1 plot the cell voltages for each battery, 2 plot the cell
-temperatueres, 0 don't plot. The default is 1 + log: see below. Default is 0
-battery_monitor() runs battery_info() in log mode on a schedule to provide
-information on the battery status over a period of time: + interval: the time
-in minutes between log entries. The default is 30 minutes + run: the number of
-log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
-total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
-cell temps. The default is 1 + save: name of a CSV file to write log data to +
-count: optional over-ride for the number of batteries This is an example of the
-output from battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/
-assets/63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ```
-f.date_list(s, e, limit, span, today) ``` Returns a list of dates in the format
-'YYYY-MM-DD'. This function will not return dates in the future. The last date
-will be yesterday or today (if today is True). All parameters are optional: +
-s: start date + e: end date + limit: maximum number of days. The default is 200
-+ span: the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
-'weekday' + today: 1 allows today to be included, 2 allows future dates to be
-included. Default is 0, date list will stop at yesterday You can use 'span' as
-follows: + 'day' provides a single day + 'week' will provide the dates of 7
-consequetive days + 'month' will provide the dates of the days up to the same
-date in the preceeding (or follwing) month + '2days' will provide the dates of
-yesterday and today + 'weekday' will provide the dates of the same day of the
-week, going backwards (or forwards) up to 7 weeks ``` f.british_summer_time(d)
-# 1 if d is in Britsh Summer Time, 0 if not ``` ## Time Periods Times and time
-period settings are held as decimal hours. Functions for working with time
-strings with the format 'HH:MM:SS' and decimal hours include: ``` f.time_hours
-(t, d=None) # convert time to decimal hours. t is a time string ('HH:MM' or
-'HH:MM:SS'), d is optional and is the default time if s is None f.hours_time(h,
-mm=True, ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm =
-include minutes, ss = include seconds, day = include /n for day when hours > 24
+may be updated if required using name=value: ``` contingency: [20,10,5,10] # %
+of consumption. Single or [winter, spring, summer, autumn] values capacity:
+None # Battery capacity in kWh (over-rides generated value if set)
+charge_current: None # max battery charge current setting in A. None uses a
+value derrived from the inverter model discharge_current: None # max battery
+discharge current setting in A. None uses a value derrived from the inverter
+model export_limit: None # maximum export power in kW. None uses the inverter
+power rating discharge_loss: 0.97 # loss converting battery discharge power to
+grid power pv_loss: 0.95 # loss converting PV power to battery charge power
+grid_loss: 0.97 # loss converting grid power to battery charge power
+charge_loss: None # loss converting charge power to residual inverter_power:
+None # inverter power consumption in W (dynamically set) bms_power: 25 # BMS
+power consumption in W bat_resistance: 0.070 # internal resistance of a battery
+in ohms volt_curve: lifepo4_curve # battery OCV from 0% to 100% SoC
+nominal_soc: 55 # SoC for nominal open circuit voltage generation_days: 3 #
+number of days to use for average generation (1-7) consumption_days: 3 # number
+of days to use for average consumption (1-7) consumption_span: 'week' # 'week'
+= last 7 days or 'weekday' = last 7 weekdays e.g. Saturdays use_today: 21.0 #
+hour when today's generation and consumption data will be used min_hours: 0.25
+# minimum charge time to set (in decimal hours) min_kwh: 0.5 # minimum charge
+to add in kwh solcast_adjust: 100 # % adjustment to make to Solcast forecast
+solar_adjust: 100 # % adjustment to make to Solar forecast forecast_selection:
+1 # 1 = only update charge times if forecast is available, 0 = use best
+available data. Default is 1. annual_consumption: None # optional annual
+consumption in kWh. If set, this replaces consumption history timed_mode: 0 # 0
+= None, 1 = use timed work mode, 2 = strategy mode special_contingency: 30 #
+contingency for special days when consumption might be higher special_days:
+['12-25', '12-26', '01-01'] full_charge: None # day of month (1-28) to do full
+charge or 'daily' or day of week: 'Mon', 'Tue' etc derate_temp: 21 # battery
+temperature in C when derating charge current is applied derate_step: 5 # step
+size for derating e.g. 21, 16, 11 derating: [24, 15, 10, 2] # derated charge
+current for each temperature step e.g. 21C, 16C, 11C, 6C force: 1 # 1 = disable
+strategy periods when setting charge. 0 = fail if strategy period has been set.
+data_wrap: 6 # data items to show per line target_soc: None # target soc for
+charging ``` These values are stored / available in f.charge_config. The
+default battery open circuit voltage curve versus SoC from 0% to 100% is: ```
+lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9,
+53.1, 53.50] ``` When operating in strategy mode (timed_mode=2), charge_needed
+will create a schedule that includes the strategy for the tariff with
+additional time segments added to charge from grid and (optionall) to stop the
+battery discharging. In other modes, charge_needed() will disable any schedules
+and set the battery charge times. This example shows the results reported by
+charge needed: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
+63789168/8b77956b-c326-43cd-b165-20d806b1e7e8) ## Battery Info Provides
+detailed information on the current state of the batteries: ``` f.battery_info
+(count, plot, log) f.battery_monitor(interval, run, log, save, count) ```
+battery_info() prints information on the battery and cells: + count: optional
+over-ride. The default is based on factorising the number of cells reported by
+16 or 18 to work out the number of batteries. + plot: 1 plot the cell voltages
+for each battery, 2 plot the cell temperatueres, 0 don't plot. The default is 1
++ log: see below. Default is 0 battery_monitor() runs battery_info() in log
+mode on a schedule to provide information on the battery status over a period
+of time: + interval: the time in minutes between log entries. The default is 30
+minutes + run: the number of log entries to create. The default is 48 i.e.
+every 30 minues for 24 hours in total + log: 0 = display, 1 = log battery info,
+2 = add cell volts, 3 = add cell temps. The default is 1 + save: name of a CSV
+file to write log data to + count: optional over-ride for the number of
+batteries This is an example of the output from battery_info(): ![image](https:
+//github.com/TonyM1958/FoxESS-Cloud/assets/63789168/a8eb52b6-ce3f-4b58-bb76-
+5483d5e40fa7) ## Date Ranges ``` f.date_list(s, e, limit, span, today) ```
+Returns a list of dates in the format 'YYYY-MM-DD'. This function will not
+return dates in the future. The last date will be yesterday or today (if today
+is True). All parameters are optional: + s: start date + e: end date + limit:
+maximum number of days. The default is 200 + span: the range of dates. One of
+'day', 'week', 'month' or 'year', '2days' or 'weekday' + today: 1 allows today
+to be included, 2 allows future dates to be included. Default is 0, date list
+will stop at yesterday You can use 'span' as follows: + 'day' provides a single
+day + 'week' will provide the dates of 7 consequetive days + 'month' will
+provide the dates of the days up to the same date in the preceeding (or
+follwing) month + '2days' will provide the dates of yesterday and today +
+'weekday' will provide the dates of the same day of the week, going backwards
+(or forwards) up to 7 weeks ``` f.british_summer_time(d) # 1 if d is in Britsh
+Summer Time, 0 if not ``` ## Time Periods Times and time period settings are
+held as decimal hours. Functions for working with time strings with the format
+'HH:MM:SS' and decimal hours include: ``` f.time_hours(t, d=None) # convert
+time to decimal hours. t is a time string ('HH:MM' or 'HH:MM:SS'), d is
+optional and is the default time if s is None f.hours_time(h, mm=True,
+ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm = include
+minutes, ss = include seconds, day = include /n for day when hours > 24
 f.hours_in(h, {'start': a, 'end': b}) # True if decimal hour h is in the time
 period a -> b ``` ## Tariffs Tariffs configure when your battery can be charged
 and provide time of use (TOU) periods to split your grid import and export into
 peak, off-peak and shoulder times when data is uploaded to PV Ouptut. There are
 a number of different pre-configured tariffs: + Octopus Flux: off-peak from 02:
 00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed
 work mode change to Self Use at 7am and Feed In First at 4pm. + Intelligent
@@ -478,25 +479,29 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.6
-Implement 2 second delay between calls that change inverter settings. Added
-strategy mode (timed_mode=2) to charge_needed(). Added set_strategy() and
-charge_strategy() to manage charging schedules and work mode changes. Refactor
-debug messaging. Simplify charge_needed() output. Added 'target_soc' to
-charge_needed() settings Fix bat_info() giving incorrect temperatures when API
-returns 0 instead of -50 where there is no battery Fix key error when accessing
-cell volts and temps using an agent / installer account. Ensure output is
-generated if get_battery() fails using battery_info(). Update f.avg() to
-include calculation of averages in lists containng None values. Added
-'data_wrap' to charge_config. 2.1.9
+(verbose) # Version Info 2.2.7
+Updated contingency to allow seasonal values for winter, spring, summer and
+autumn. Update strategy mode to support ForceCharge and ForceDischarge work
+modes. Update so min_soc setting in charge_needed() over-rides min_soc in the
+tariff strategy. Fix force charge strategy mode in charge_neded() to set
+min_soc correctly. Implement 2 second delay between calls that change inverter
+settings. Added strategy mode (timed_mode=2) to charge_needed(). Added
+set_strategy() and charge_strategy() to manage charging schedules and work mode
+changes. Refactor debug messaging. Simplify charge_needed() output. Added
+'target_soc' to charge_needed() settings Fix bat_info() giving incorrect
+temperatures when API returns 0 instead of -50 where there is no battery Fix
+key error when accessing cell volts and temps using an agent / installer
+account. Ensure output is generated if get_battery() fails using battery_info
+(). Update f.avg() to include calculation of averages in lists containng None
+values. Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

