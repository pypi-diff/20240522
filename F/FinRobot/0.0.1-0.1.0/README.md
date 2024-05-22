# Comparing `tmp/FinRobot-0.0.1.tar.gz` & `tmp/FinRobot-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinRobot-0.0.1.tar", last modified: Thu Feb 29 19:28:58 2024, max compression
+gzip compressed data, was "FinRobot-0.1.0.tar", last modified: Wed May 22 12:07:20 2024, max compression
```

## Comparing `FinRobot-0.0.1.tar` & `FinRobot-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-02-29 19:28:58.156293 FinRobot-0.0.1/
-drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-02-29 19:28:58.155979 FinRobot-0.0.1/FinRobot.egg-info/
--rw-r--r--   0 bruce      (501) staff       (20)      949 2024-02-29 19:28:58.000000 FinRobot-0.0.1/FinRobot.egg-info/PKG-INFO
--rw-r--r--   0 bruce      (501) staff       (20)      185 2024-02-29 19:28:58.000000 FinRobot-0.0.1/FinRobot.egg-info/SOURCES.txt
--rw-r--r--   0 bruce      (501) staff       (20)        1 2024-02-29 19:28:58.000000 FinRobot-0.0.1/FinRobot.egg-info/dependency_links.txt
--rw-r--r--   0 bruce      (501) staff       (20)       54 2024-02-29 19:28:58.000000 FinRobot-0.0.1/FinRobot.egg-info/requires.txt
--rw-r--r--   0 bruce      (501) staff       (20)        1 2024-02-29 19:28:58.000000 FinRobot-0.0.1/FinRobot.egg-info/top_level.txt
--rw-r--r--   0 bruce      (501) staff       (20)     1078 2024-02-27 02:32:37.000000 FinRobot-0.0.1/LICENSE
--rw-r--r--   0 bruce      (501) staff       (20)      949 2024-02-29 19:28:58.156181 FinRobot-0.0.1/PKG-INFO
--rw-r--r--   0 bruce      (501) staff       (20)      181 2024-02-29 19:24:39.000000 FinRobot-0.0.1/README.md
--rw-r--r--   0 bruce      (501) staff       (20)       38 2024-02-29 19:28:58.156339 FinRobot-0.0.1/setup.cfg
--rw-r--r--   0 bruce      (501) staff       (20)     1506 2024-02-29 19:28:38.000000 FinRobot-0.0.1/setup.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-05-22 12:07:20.644713 FinRobot-0.1.0/
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-05-22 12:07:20.644278 FinRobot-0.1.0/FinRobot.egg-info/
+-rw-r--r--   0 bruce      (501) staff       (20)     1400 2024-05-22 12:07:20.000000 FinRobot-0.1.0/FinRobot.egg-info/PKG-INFO
+-rw-r--r--   0 bruce      (501) staff       (20)      185 2024-05-22 12:07:20.000000 FinRobot-0.1.0/FinRobot.egg-info/SOURCES.txt
+-rw-r--r--   0 bruce      (501) staff       (20)        1 2024-05-22 12:07:20.000000 FinRobot-0.1.0/FinRobot.egg-info/dependency_links.txt
+-rw-r--r--   0 bruce      (501) staff       (20)      178 2024-05-22 12:07:20.000000 FinRobot-0.1.0/FinRobot.egg-info/requires.txt
+-rw-r--r--   0 bruce      (501) staff       (20)        1 2024-05-22 12:07:20.000000 FinRobot-0.1.0/FinRobot.egg-info/top_level.txt
+-rw-r--r--   0 bruce      (501) staff       (20)     1083 2024-04-25 06:26:20.000000 FinRobot-0.1.0/LICENSE
+-rw-r--r--   0 bruce      (501) staff       (20)     1400 2024-05-22 12:07:20.644521 FinRobot-0.1.0/PKG-INFO
+-rw-r--r--   0 bruce      (501) staff       (20)    11360 2024-05-22 12:03:48.000000 FinRobot-0.1.0/README.md
+-rw-r--r--   0 bruce      (501) staff       (20)       38 2024-05-22 12:07:20.644766 FinRobot-0.1.0/setup.cfg
+-rw-r--r--   0 bruce      (501) staff       (20)     1553 2024-05-22 12:07:07.000000 FinRobot-0.1.0/setup.py
```

### Comparing `FinRobot-0.0.1/LICENSE` & `FinRobot-0.1.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 AI4Finance Foundation
+Copyright (c) 2024 AI4Finance Foundation Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

