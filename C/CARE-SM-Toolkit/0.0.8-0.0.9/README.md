# Comparing `tmp/CARE-SM-Toolkit-0.0.8.tar.gz` & `tmp/CARE-SM-Toolkit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CARE-SM-Toolkit-0.0.8.tar", last modified: Wed Feb 14 11:18:35 2024, max compression
+gzip compressed data, was "CARE-SM-Toolkit-0.0.9.tar", last modified: Wed Mar 13 08:45:35 2024, max compression
```

## Comparing `CARE-SM-Toolkit-0.0.8.tar` & `CARE-SM-Toolkit-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2024-02-14 11:18:35.017251 CARE-SM-Toolkit-0.0.8/
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2024-02-14 11:18:35.017251 CARE-SM-Toolkit-0.0.8/CARE_SM_Toolkit.egg-info/
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      311 2024-02-14 11:18:34.000000 CARE-SM-Toolkit-0.0.8/CARE_SM_Toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      233 2024-02-14 11:18:34.000000 CARE-SM-Toolkit-0.0.8/CARE_SM_Toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2024-02-14 11:18:34.000000 CARE-SM-Toolkit-0.0.8/CARE_SM_Toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2024-02-14 11:18:34.000000 CARE-SM-Toolkit-0.0.8/CARE_SM_Toolkit.egg-info/top_level.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      311 2024-02-14 11:18:35.017251 CARE-SM-Toolkit-0.0.8/PKG-INFO
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     2531 2024-01-17 14:08:18.000000 CARE-SM-Toolkit-0.0.8/README.md
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2024-02-14 11:18:35.017251 CARE-SM-Toolkit-0.0.8/setup.cfg
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      369 2024-02-14 11:18:05.000000 CARE-SM-Toolkit-0.0.8/setup.py
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2024-02-14 11:18:35.017251 CARE-SM-Toolkit-0.0.8/toolkit/
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2024-01-17 14:08:18.000000 CARE-SM-Toolkit-0.0.8/toolkit/__init__.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    31350 2024-02-14 10:32:34.000000 CARE-SM-Toolkit-0.0.8/toolkit/main.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     7540 2024-01-17 14:08:18.000000 CARE-SM-Toolkit-0.0.8/toolkit/test_pytest.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2024-03-13 08:45:35.482484 CARE-SM-Toolkit-0.0.9/
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2024-03-13 08:45:35.482484 CARE-SM-Toolkit-0.0.9/CARE_SM_Toolkit.egg-info/
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      311 2024-03-13 08:45:35.000000 CARE-SM-Toolkit-0.0.9/CARE_SM_Toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      253 2024-03-13 08:45:35.000000 CARE-SM-Toolkit-0.0.9/CARE_SM_Toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2024-03-13 08:45:35.000000 CARE-SM-Toolkit-0.0.9/CARE_SM_Toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2024-03-13 08:45:35.000000 CARE-SM-Toolkit-0.0.9/CARE_SM_Toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      311 2024-03-13 08:45:35.482484 CARE-SM-Toolkit-0.0.9/PKG-INFO
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     2641 2024-03-13 08:23:50.000000 CARE-SM-Toolkit-0.0.9/README.md
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2024-03-13 08:45:35.482484 CARE-SM-Toolkit-0.0.9/setup.cfg
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      369 2024-03-13 08:44:43.000000 CARE-SM-Toolkit-0.0.9/setup.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2024-03-13 08:45:35.482484 CARE-SM-Toolkit-0.0.9/toolkit/
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2024-01-17 14:08:18.000000 CARE-SM-Toolkit-0.0.9/toolkit/__init__.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    11894 2024-03-13 08:23:50.000000 CARE-SM-Toolkit-0.0.9/toolkit/main.py
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    27492 2024-03-13 08:23:50.000000 CARE-SM-Toolkit-0.0.9/toolkit/template.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     7540 2024-01-17 14:08:18.000000 CARE-SM-Toolkit-0.0.9/toolkit/test_pytest.py
```

### Comparing `CARE-SM-Toolkit-0.0.8/README.md` & `CARE-SM-Toolkit-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CARE-SM-Toolkit
+# CARE-SM Toolkit
 
 **CSV datatable toolkit for CARE semantic model implementation**
 
 The implementation of the Clinical And Registry Entries (CARE) Semantic Model for CSV data entails a meticulous and technically advanced workflow. By leveraging the power of the CARE-SM, YARRRML templates and incorporating the critical curation step executed by the CARE-SM toolkit, this implementation achieves robustness, accuracy, and reliability in generating RDF-based CDE-oriented patient data.
 
 The toolkit serves as a module dedicated to performing a curation step prior to the conversion of data into RDF. The primary transformations carried out by the toolkit include:
 
@@ -14,31 +14,33 @@
 
 * Conducting a quality control among `age`/`date`, `stardate` and `enddate` columns to ensure data consistency and validity.
 
 * Eliminating any row that lacks of the minimal required data to minimize the generation of incomplete RDF transformations.
 
 * Creation of the column called `uniqid` that assigns a unique identifier to each observation. This prevents the RDF instances from overlapping with one another, ensuring their distinctiveness and integrity.
 
-## Dockerized implementation:
+## Dockerized implementation
 
 There's a Docker-based implementation controlled via API (using FastAPI) that you can use for mounting this data transformation step as a part of your CARE-SM implementation. Use our docker compose to control your Docker image, ports where its located and volumes in order to pass your CSV-based patient data:
 
 ```yaml
 version: "3.3"
 
 services:
   api:
-    image: pabloalarconm/care-sm-toolkit:0.0.1 # check for latest version
+    image: pabloalarconm/care-sm-toolkit:latest # check for latest version
     ports:
       - "8000:8000"
     volumes:
       - ./data:/code/data
 ```
 
-## Local implementation:
+## Local implementation
+
+If you are not interested on running Docker image, you can install the Pyhton module for local implementation.
 
 ###  Installation:
 
 ```bash
 pip install CARE-SM-Toolkit
 ```
 **Requirements:**
@@ -49,10 +51,10 @@
 
 ```py
 import pandas as pd
 from main import Toolkit
 
 test= Toolkit()
 
-test_done = test.whole_quality_control(input_data="etoolkit/exemplar_data/preCARE.csv")
+test_done = test.whole_quality_control(input_data="toolkit/exemplar_data/preCARE.csv")
 test_done.to_csv ("toolkit/exemplar_data/CARE.csv", index = False, header=True)
 ```
```

### Comparing `CARE-SM-Toolkit-0.0.8/toolkit/main.py` & `CARE-SM-Toolkit-0.0.9/toolkit/template.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,1037 +1,905 @@
-import pandas as pd
-from perseo.main import milisec
-import sys
-
-class Toolkit:
-
-    def import_your_data_from_csv(self, input_data):
-      try:
-          data = pd.read_csv(input_data)
-
-          return data
-      except FileNotFoundError:
-          print(f"File not found: {input_data}")
-          return None
-      except pd.errors.EmptyDataError:
-          print(f"The CSV file is empty: {input_data}")
-          return None
-      except pd.errors.ParserError:
-          print(f"Error parsing the CSV file: {input_data}")
-          return None
-      
-    ## Check the status of the columns
-    def check_status_column_names(self, data):
-        column_names = ["model","pid","event_id","value","age","value_datatype","valueIRI","activity","unit","input","target","intensity","protocol_id","frequency_type","frequency_value","agent","route","startdate","enddate","comments"]
-        for name in column_names:
-            if name not in data.columns:
-                return False
-        return data
-
-    def check_for_duplicated_titles_among_row(self, data):
-        count = 0
-        for value in data["model"]:
-            if value == "model":
-                count += 1
-        return count > 0
-        
-    ## Add ontological columns
-    def add_columns_from_template(self,data):
-        print("Transforming and Validating....")
-
-        data = data.where(pd.notnull(data), None)
-
-        temp = Template.template_model
-        final_df = pd.DataFrame()
-        row_df = dict()
-
-        for row in data.iterrows():
-            milisec_point = milisec()
-
-            # Tag each row with the new of the model 
-            new_row = {milisec_point : {"model": row[1]["model"]}}
-            row_df.update(new_row)
-
-            # Include columns related to ontological terms:
-            for cde in temp.items():
-                if cde[0] == row_df[milisec_point]["model"]:
-                    row_df[milisec_point].update(cde[1])
-
-            # Include columns from input CSV table:
-            for title, val in row[1].items():
-                if not val == None:
-                    row_df[milisec_point].update({title:val})
-
-            # Concate rows:
-            final_row_df = pd.DataFrame(row_df[milisec_point], index=[1])
-            # final_df = pd.append([final_df, final_row_df])
-            if not final_row_df.empty and not final_row_df.isna().all().all():
-                final_df = pd.concat([final_df, final_row_df], ignore_index=True)
-
-        final_df = final_df.reset_index(drop=True)
-
-        final_df = final_df.where(pd.notnull(final_df), None)
-        return final_df
-      
-      
-      
-    def transform_shape_based_on_config(self, configuration, data):
-        
-        # Import static template for all CDE terms:
-        temp = Template.template_model
-        
-        # Empty objects:
-        final_df = pd.DataFrame()
-        row_df = {}
-
-        # Iterate each row from data input
-        # check each YAML object from configuration file to set the parameters
-        for row in data.iterrows():
-
-            for config in configuration.items():
-
-                # Create a unique stamp per new row to about them to colapse:
-                milisec_point = milisec()
-
-                row_df.update({milisec_point: {'model':config[1]["cde"]}})
-                
-                # Add YAML template static information
-                for cde in temp.items():
-                    if cde[0] == row_df[milisec_point]["model"]:
-                        row_df[milisec_point].update(cde[1])
-
-                # Relate each YAML parameter with original data input
-                for element in config[1]["columns"].items():
-                    for r in row[1].index:
-                        if r == element[1]:
-                            dict_element = {element[0]:row[1][r]}
-                            row_df[milisec_point].update(dict_element)
-                            
-
-                # Store formed element into the final table:
-                final_row_df = pd.DataFrame(row_df[milisec_point], index=[1])
-                if not final_row_df.empty and not final_row_df.isna().all().all():
-                    final_df = pd.concat([final_df, final_row_df], ignore_index=True)
-        final_df = final_df.reset_index(drop=True)
-
-        final_df = final_df.where(pd.notnull(final_df), None)
-        return final_df
-
-    ## Value edition
-    def value_edition(self, data):
-        
-        for index, row in data.iterrows():
-            
-            data = data.where(pd.notnull(data), None)
-            
-            # Based on the value_datatype, add value
-            if row["value_datatype"] == "xsd:string":
-                data.at[index, "value_string"] = data["value"][index] #.astype('str')
-
-            if row["value_datatype"] == "xsd:float":
-                data.at[index, "value_float"] = data["value"][index] #.astype('float64')
-
-            if row["value_datatype"] == "xsd:integer":
-                data.at[index, "value_integer"] = data["value"][index] #.astype('int64')
-
-            if row["value_datatype"] == "xsd:date":
-                data.at[index, "value_date"] = data["value"][index] #.astype({'date': 'datetime64[ns]'})
-
-            ## ValueIRI/value edition
-            
-            if row["model"] in ["Sex","Status","Diagnosis","Symptom","Clinical_trial", "Body_measurement"]:
-                data.at[index, "attribute_type"] = data["valueIRI"][index]
-
-            if row["model"] in ["Genetic","Imaging"]:
-                data.at[index, "output_id"] = data["valueIRI"][index]
-                
-            if row["model"] in ["Zygosity"]:
-                data.at[index, "output_type"] = data["valueIRI"][index]
-                
-            if row["model"] in ["Aminoacid"]:
-                data.at[index, "input_id"] = data["valueIRI"][index]
-                
-            if row["model"] in ["Medication"]:
-                data.at[index, "concentration_value"] = data["value"][index]
-                
-            ## Target edition
-            data = data.where(pd.notnull(data), None)
-
-            
-            if row["model"] in ["Zygosity","Genetic"]:
-                data.at[index, "target_id"] = data["target"][index]
-            
-            if row["model"] in ["Aminoacid","Lab_measurement","Biobank","Surgical","Imaging","Questionnaire"]:
-                data.at[index, "target_type"] = data["target"][index]
-                
-            if row["model"] in ["Biobank","Clinical_trial"]:
-                data.at[index, "agent_id"] = data["agent"][index]
-                
-            if row["model"] in ["Medication","Surgery"]:
-                data.at[index, "substance_id"] = data["agent"][index]
-
-            data = data.where(pd.notnull(data), None)
-
-        return data     
-
-    # Time edition
-    def time_edition(self, data):
-        
-        data = data.where(pd.notnull(data), None)
-
-        for index, row in data.iterrows():
-            ## From startdate to enddate
-            
-            if type(row['enddate']) == float or row['enddate'] == None: #TODO work on nan values to filter them better
-                data.at[index, 'enddate'] = row['startdate']
-                
-            # print(data["enddate"][index])
-
-        return data
-
-    ## Clean rows with no value
-    def clean_empty_rows(self, data):
-
-        for row_final in data.iterrows():
-            if row_final[1]["value"] == None and row_final[1]["valueIRI"] == None and row_final[1]["activity"] == None and row_final[1]["target"] == None and row_final[1]["model"] not in ["Biobank", "Consent_used", "Consent_contacted"]:
-                data = data.drop(row_final[0])
-        return data
-    
-    def delete_extra_columns(self, data):
-
-        del data["value"]
-        del data["valueIRI"]
-        del data["target"]
-        del data["agent"]
-
-        return data
-    
-    def unique_id_generation(self,data):
-        data['uniqid'] = ""
-
-        for i in data.index:
-            data.at[i, "uniqid"] = milisec()
-        
-        return data
-
-    def whole_quality_control(self,input_data):
-
-        imported_file = self.import_your_data_from_csv(input_data)
-        if imported_file is not None:
-            print("CSV file imported successfully.")
-        else:
-            print("CSV file import failed. Please check the file path and format.")
-
-        columns_names_conformation = self.check_status_column_names(imported_file)
-        if columns_names_conformation is not None:
-            print("Every CSV columns present.")
-        else:
-            print("CSV file quality control failed. Please check the columns names, every required column is not present")
-
-        # table_without_extra_head = self.check_for_duplicated_titles_among_row(columns_names_conformation)
-        # if table_without_extra_head is not None:
-        #     print("CSV without title duplcations done.")
-        # else:
-        #     print("CSV file quiality control failed. Please check the data content, looks like their multiple head rows with title in you CSV.")
-
-        table_with_template_addition = self.add_columns_from_template(imported_file)
-
-        table_with_value_edited = self.value_edition(table_with_template_addition)
-
-        table_with_time_corrected = self.time_edition(table_with_value_edited)
-
-        table_with_blanks_cleaned = self.clean_empty_rows(table_with_time_corrected)
-
-        table_extra_column_deleted = self.delete_extra_columns(table_with_blanks_cleaned)
-
-        table_with_uniqid = self.unique_id_generation(table_extra_column_deleted)
-
-        if table_with_uniqid is not None:
-            print("CSV data transformation done.")
-        else:
-            sys.exit("CSV file quiality control failed. Please check the columns names, every required column is not present")
-
-        return table_with_uniqid
-      
-      
-    def yaml_quality_control(self,input_data,configuration):
-
-        imported_file = self.import_your_data_from_csv(input_data)
-        if imported_file is not None:
-            print("CSV file imported successfully.")
-        else:
-            print("CSV file import failed. Please check the file path and format.")
-
-        columns_names_conformation = self.check_status_column_names(imported_file)
-        if columns_names_conformation is not None:
-            print("Every CSV columns present.")
-        else:
-            sys.exit("CSV file quiality control failed. Please check the columns names, every required column is not present")
-
-        # table_without_extra_head= self.check_for_duplicated_titles_among_row(columns_names_conformation)
-        # if table_without_extra_head is not None:
-        #     print("CSV without title duplcations done.")
-        # else:
-        #     print("CSV file quiality control failed. Please check the data content, looks like their multiple head rows with title in you CSV.")
-
-        table_with_template_addition = self.transform_shape_based_on_config(configuration=configuration, data=imported_file)
-
-        table_with_value_edited = self.value_edition(table_with_template_addition)
-    
-
-        table_with_time_corrected = self.time_edition(table_with_value_edited)
-
-        table_with_blanks_cleaned = self.clean_empty_rows(table_with_time_corrected)
-
-        table_extra_column_deleted = self.delete_extra_columns(table_with_blanks_cleaned)
-
-        table_with_uniqid = self.unique_id_generation(table_extra_column_deleted)
-
-        if table_with_uniqid is not None:
-            print("CSV data transformation done.")
-        else:
-            print("CSV data transformation failed. Something went wrong during transformation.")
-
-        return table_with_uniqid
-    
-   
 class Template:
 
   template_model = dict(
 
     Birthdate = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
-      output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C68615",
-      attribute_type2 = None,
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:date",
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
-
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
+        attribute_type = "http://purl.obolibrary.org/obo/NCIT_C6861",
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/NCIT_C70856", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:date",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
     
     Birthyear = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
-      output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C83164",
-      attribute_type2 = None,
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:integer",
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
-
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
+        attribute_type = "http://purl.obolibrary.org/obo/NCIT_C83164",
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/NCIT_C70856", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:integer",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-
-    Deathdate = dict( 
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
-      output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C70810",
-      attribute_type2 = None,
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,    
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:date",
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
+        
+    Deathdate = dict(
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
+        attribute_type = "http://purl.obolibrary.org/obo/NCIT_C70810",
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/NCIT_C70856", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:date",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-
+        
     First_visit = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
-      output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C164021",
-      attribute_type2 = None,
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:date",
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
+        attribute_type = "http://purl.obolibrary.org/obo/NCIT_C164021",
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/NCIT_C70856", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:date",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-
-    Sex = dict( 
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
-      output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = None,
-      attribute_type2 = "http://purl.obolibrary.org/obo/NCIT_C28421",
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:string",
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
+        
+    Symptoms_onset = dict(
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
+        attribute_type = "http://purl.obolibrary.org/obo/NCIT_C124353",
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/NCIT_C70856", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:date",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-
+    
+    Sex = dict(
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
+        attribute_type = None,
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/NCIT_C160908", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:string",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
+    ),
+        
+        
     Status = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
-      output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = None,
-      attribute_type2 = "http://purl.obolibrary.org/obo/NCIT_C166244",
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:string",
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
+        attribute_type = None,
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/NCIT_C164628", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:string",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-
+    
+    Education = dict(
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
+        attribute_type = "http://purl.obolibrary.org/obo/NCIT_C17953",
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/NCIT_C70856", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = "http://purl.obolibrary.org/obo/NCIT_C73537",        
+        protocol_id = "https://www.wikidata.org/wiki/Q1390351", 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:integer",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
+    ),
+    
+        
+        
     Diagnosis = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type = "http://purl.obolibrary.org/obo/NCIT_C18020",
-      output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = None,
-      attribute_type2 = "http://purl.obolibrary.org/obo/NCIT_C2991",
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:string",
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C18020",
+        attribute_type = None,
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/NCIT_C154625", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:string",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-
-    Symptom = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type = "http://purl.obolibrary.org/obo/NCIT_C18020",
-      output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = None,
-      attribute_type2 = "http://purl.obolibrary.org/obo/NCIT_C100104",
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:string",
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
+        
+        
+    Phenotype = dict(
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C18020",
+        attribute_type = None,
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/NCIT_C16977", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:string",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-
-    Genetic = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type= "http://purl.obolibrary.org/obo/NCIT_C15709",
-      output_type= "http://purl.obolibrary.org/obo/NCIT_C45766",
-      attribute_type= None,
-      attribute_type2 = None,
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = "http://purl.obolibrary.org/obo/NCIT_C16612",
-      target_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:string",  
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
+        
+        
+    Genotype = dict(
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C15709",
+        attribute_type = None,
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = "http://purl.obolibrary.org/obo/NCIT_C45766",
+        target_id = None,     
+        output_type = None, 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:string",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-    
+        
+        
     Zygosity = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type= "http://purl.obolibrary.org/obo/NCIT_C15709",
-      output_type= None,
-      attribute_type= None,
-      attribute_type2 = None,
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = "http://purl.obolibrary.org/obo/NCIT_C45766",
-      target_id = None,
-      activity = "http://purl.obolibrary.org/obo/NCIT_C181350",
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:string",  
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C15709",
+        attribute_type = "http://purl.obolibrary.org/obo/NCIT_C181350",
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = "http://purl.obolibrary.org/obo/NCIT_C45766",
+        target_id = None,     
+        output_type = None, 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:string",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-    
-    Aminoacid = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type= "http://purl.obolibrary.org/obo/NCIT_C15709",
-      output_type= "http://purl.obolibrary.org/obo/NCIT_C164371",
-      attribute_type= None,
-      attribute_type2 = None,
-      agent_id = None,
-      substance_id = None,
-      input = "http://purl.obolibrary.org/obo/NCIT_C17021",
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:integer",  
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
+        
+        
+    Protein = dict(
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C18962",
+        attribute_type = None,
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = "http://purl.obolibrary.org/obo/NCIT_C165059",
+        target_id = None,     
+        output_type = None, 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:string",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-
+        
+        
     Consent_contacted = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type= "http://purl.obolibrary.org/obo/OBI_0000810",
-      output_type = "http://purl.obolibrary.org/obo/OBIB_0000488",
-      attribute_type= None,
-      attribute_type2 = None,
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:string",
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/OBI_0000810",
+        attribute_type = None,
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/OBIB_0000488", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:string",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-
+        
+        
     Consent_used = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type= "http://purl.obolibrary.org/obo/OBI_0000810",
-      output_type = "http://purl.obolibrary.org/obo/DUO_0000001",
-      attribute_type= None,
-      attribute_type2 = None,
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:string",
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/OBI_0000810",
+        attribute_type = None,
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/DUO_0000001", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:string",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-
+        
+        
     Biobank = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type= "http://purl.obolibrary.org/obo/OMIABIS_0000061",
-      output_type= "http://purl.obolibrary.org/obo/NCIT_C115570",
-      attribute_type= None,
-      attribute_type2 = None,
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = "http://purl.obolibrary.org/obo/OBIB_0000616",
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:string",
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/OMIABIS_0000061",
+        attribute_type = None,
+        agent_type = "http://purl.obolibrary.org/obo/OBIB_0000616",
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/NCIT_C115570", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:string",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-
-    Questionnaire = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type = "http://purl.obolibrary.org/obo/NCIT_C91102",
-      output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = None,
-      attribute_type2 = None,
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:float",
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
+    
+    XXX = dict(
+        pid = None,
+        process_type = None,
+        attribute_type = None,
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = None, 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:string",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
+    
 
+    Disability = dict(
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C91102",
+        attribute_type = "http://purl.obolibrary.org/obo/NCIT_C21007",
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/NCIT_C70856", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:float",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
+    ),
+    
     Body_measurement = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type = "http://purl.obolibrary.org/obo/NCIT_C142470" ,
-      output_type = "http://purl.obolibrary.org/obo/NCIT_C70856" ,
-      attribute_type = None,
-      attribute_type2 = "http://purl.obolibrary.org/obo/NCIT_C25447" ,
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:float" ,
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
+        attribute_type = None,
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/NCIT_C70856", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:float",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-
-
+    
     Lab_measurement = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type = "http://purl.obolibrary.org/obo/NCIT_C25294" ,
-      output_type = "http://purl.obolibrary.org/obo/NCIT_C70856" ,
-      attribute_type = None,
-      attribute_type2 = None,
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype= "xsd:float" ,
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C25294",
+        attribute_type = None,
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/NCIT_C70856", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:float",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-
+    
     Imaging = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type = "http://purl.obolibrary.org/obo/NCIT_C17369",
-      output_type =  "http://purl.obolibrary.org/obo/NCIT_C81289",
-      attribute_type = None,
-      attribute_type2 = None,
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = None,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:string" ,
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C17369",
+        attribute_type = None,
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/NCIT_C81289", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:string",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-
+    
     Surgery = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type = "http://purl.obolibrary.org/obo/NCIT_C15329",
-      output_type = None,
-      attribute_type = None,
-      attribute_type2 = None,
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = "http://purl.obolibrary.org/obo/NCIT_C177929",
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:string" ,
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
-    ),
-
-    Clinical_trial = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type = "http://purl.obolibrary.org/obo/NCIT_C71104" ,
-      output_type=  "http://purl.obolibrary.org/obo/NCIT_C115575" ,
-      attribute_type = None,
-      attribute_type2 = "http://purl.obolibrary.org/obo/NCIT_C2991",
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = "http://purl.obolibrary.org/obo/NCIT_C16696" ,
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:string",
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
-
-
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C15329",
+        attribute_type = None,
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = None, 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = "http://purl.obolibrary.org/obo/NCIT_C73537",        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:string",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     ),
-
+    
     Medication = dict(
-      pid = None,
-      event_id = None,
-      comments = None,
-      process_type = "http://purl.obolibrary.org/obo/NCIT_C70962",
-      output_type = None ,
-      attribute_type = None,
-      attribute_type2 = None,
-      agent_id = None,
-      substance_id = None,
-      input = None,
-      input_id = None,
-      target_type = None,
-      target_id = None,
-      output_id = None,
-      activity = None,
-      intensity = None,
-      unit = None,
-      agent_type = "http://purl.obolibrary.org/obo/NCIT_C177929",
-      frequency_type = None,
-      frequency_value = None,
-      route = None,
-      concentration_value = None,
-      value_date = None,
-      value_integer = None,
-      value_string = None,
-      value_float = None,
-      value_datatype = "xsd:float",
-      age = None,
-      protocol_id = None,
-      startdate = None,
-      enddate = None,
-      uniqid = None,
-
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C25409",
+        attribute_type = None,
+        agent_type = None,
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = None, 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = "http://purl.obolibrary.org/obo/NCIT_C73537",        
+        protocol_id = None, 
+        substance_type = "http://purl.obolibrary.org/obo/NCIT_C177929",      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = "http://purl.obolibrary.org/obo/NCIT_C25488",
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:float",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
+    ),
+    
+    
+    Clinical_trial = dict(
+        pid = None,
+        process_type = "http://purl.obolibrary.org/obo/NCIT_C71104",
+        attribute_type = None,
+        agent_type = "http://purl.obolibrary.org/obo/NCIT_C16696",
+        agent_id = None,
+        input_type = None,
+        #input_id = None,
+        target_type = None,
+        target_id = None,     
+        output_type = "http://purl.obolibrary.org/obo/NCIT_C115575", 
+        output_id = None,
+        unit_type = None,
+        specific_process_type = None,
+        protocol_type = None,        
+        protocol_id = None, 
+        substance_type = None,      
+        substance_id = None,
+        activity_type = None,
+        frequency_type = None,
+        frequency_value = None,        
+        concentration_type = None,
+        concentration_value = None,
+        concentration_unit_type = None,
+        value_date = None,
+        value_integer = None,
+        value_string = None,
+        value_float = None,
+        value_datatype = "xsd:string",
+        comments = None,
+        startdate = None,
+        enddate = None,
+        age = None,
+        uniqid = None,
+        event_id = None
     )
+
   )
```

### Comparing `CARE-SM-Toolkit-0.0.8/toolkit/test_pytest.py` & `CARE-SM-Toolkit-0.0.9/toolkit/test_pytest.py`

 * *Files identical despite different names*

