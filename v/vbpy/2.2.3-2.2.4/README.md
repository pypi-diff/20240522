# Comparing `tmp/vbpy-2.2.3.tar.gz` & `tmp/vbpy-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbpy-2.2.3.tar", last modified: Wed May 22 09:53:22 2024, max compression
+gzip compressed data, was "vbpy-2.2.4.tar", last modified: Wed May 22 09:58:30 2024, max compression
```

## Comparing `vbpy-2.2.3.tar` & `vbpy-2.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 09:53:22.780000 vbpy-2.2.3/
--rw-rw-rw-   0        0        0      122 2024-05-22 09:53:24.000000 vbpy-2.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-22 09:53:24.000000 vbpy-2.2.3/setup.cfg
--rw-rw-rw-   0        0        0      536 2024-05-22 09:53:14.000000 vbpy-2.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:53:22.820000 vbpy-2.2.3/vbpy/
--rw-rw-rw-   0        0        0      265 2024-05-22 09:16:04.000000 vbpy-2.2.3/vbpy/__init__.py
--rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.2.3/vbpy/combine_data_file.py
--rw-rw-rw-   0        0        0     1006 2024-05-22 08:23:28.000000 vbpy-2.2.3/vbpy/load_channel_data_file.py
--rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.2.3/vbpy/load_claim_auto_file.py
--rw-rw-rw-   0        0        0    16428 2024-05-22 09:53:06.000000 vbpy-2.2.3/vbpy/load_open_claim_auto_file.py
--rw-rw-rw-   0        0        0    14873 2024-05-22 07:54:10.000000 vbpy-2.2.3/vbpy/load_revenue_auto_file.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:53:22.860000 vbpy-2.2.3/vbpy.egg-info/
--rw-rw-rw-   0        0        0      122 2024-05-22 09:53:24.000000 vbpy-2.2.3/vbpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-05-22 09:53:24.000000 vbpy-2.2.3/vbpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 09:53:24.000000 vbpy-2.2.3/vbpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-22 09:53:24.000000 vbpy-2.2.3/vbpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 09:58:29.990000 vbpy-2.2.4/
+-rw-rw-rw-   0        0        0      122 2024-05-22 09:58:32.000000 vbpy-2.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-22 09:58:32.000000 vbpy-2.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      536 2024-05-22 09:58:22.000000 vbpy-2.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:58:30.030000 vbpy-2.2.4/vbpy/
+-rw-rw-rw-   0        0        0      265 2024-05-22 09:16:04.000000 vbpy-2.2.4/vbpy/__init__.py
+-rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.2.4/vbpy/combine_data_file.py
+-rw-rw-rw-   0        0        0     1006 2024-05-22 08:23:28.000000 vbpy-2.2.4/vbpy/load_channel_data_file.py
+-rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.2.4/vbpy/load_claim_auto_file.py
+-rw-rw-rw-   0        0        0    10327 2024-05-22 09:58:00.000000 vbpy-2.2.4/vbpy/load_open_claim_auto_file.py
+-rw-rw-rw-   0        0        0    14873 2024-05-22 07:54:10.000000 vbpy-2.2.4/vbpy/load_revenue_auto_file.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:58:30.070000 vbpy-2.2.4/vbpy.egg-info/
+-rw-rw-rw-   0        0        0      122 2024-05-22 09:58:30.000000 vbpy-2.2.4/vbpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-05-22 09:58:30.000000 vbpy-2.2.4/vbpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 09:58:30.000000 vbpy-2.2.4/vbpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 09:58:30.000000 vbpy-2.2.4/vbpy.egg-info/top_level.txt
```

### Comparing `vbpy-2.2.3/setup.py` & `vbpy-2.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     
     name='vbpy',
-    version='2.2.3',
+    version='2.2.4',
     packages=find_packages(),
     # description='Your library description',
     # long_description=open('README.md').read(),
     # long_description_content_type='text/markdown',
     author='Nguyen Ha Tuan Long',
     author_email='tuanlongnguyenha@gmail.com',
     # url='https://github.com/yourusername/your_library_name',
```

### Comparing `vbpy-2.2.3/vbpy/combine_data_file.py` & `vbpy-2.2.4/vbpy/combine_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.2.3/vbpy/load_channel_data_file.py` & `vbpy-2.2.4/vbpy/load_channel_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.2.3/vbpy/load_claim_auto_file.py` & `vbpy-2.2.4/vbpy/load_claim_auto_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.2.3/vbpy/load_open_claim_auto_file.py` & `vbpy-2.2.4/vbpy/load_revenue_auto_file.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import pandas as pd
 import numpy as np
 pd.set_option('display.max_rows', None) 
 pd.set_option('display.max_columns', None)  
+
 import os
 import re
 from tqdm import tqdm
 
-def load_open_claim_auto(directory, skip_rows=12, lhnv = None):
+def load_revenue_auto(directory, skip_rows=13, lhnv = None):
     # Regular expression to find a four-digit year in the file name
-    pattern = re.compile(r'\b(\d{2})-(\d{4})\b')
+    year_pattern = re.compile(r'\b(\d{4})\b')
 
     # List to keep track of the names of the DataFrames stored as globals
     global_df_names = []
 
     # Iterate through each file in the specified directory
     for file in sorted(os.listdir(directory)):
         if file.endswith('.xlsx') and not file.startswith('~$'):
             
             # Find the year in the file name
-            match = pattern.search(file)
+            match = year_pattern.search(file)
             if match:
-                quarter = match.group(1)
+                year = match.group(1)
                 file_path = os.path.join(directory, file)
                 try:
                     """ IMPORT DATA"""
                     print(f"\n\n\nxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx\n--------------------------------------------------------------------------\nImporting: {file}")
                     # Load and clean data specifying the engine
                     df = pd.read_excel(file_path, header=None, skiprows=skip_rows, engine='openpyxl')
                     df.drop(df.columns[-1], axis = 1, inplace = True)  # remove na col at the end
@@ -41,104 +42,93 @@
 
                     # Set the determined headers as column names
                     df.columns = headers
                     df = df.drop([0, 1])
                     df.reset_index(drop = True, inplace=True)
                     print(f'   Rows = {df.shape[0]}')
                     # print(f'Columns = {df.shape[1]}')
-                    print(df)
+            
             
                     """ RENAME COLUMNS"""
                     print("--------------------------------------------------------------------------\nRenaming Columns:")
-                    df_clm_dict = {
-                        'Số hồ sơ': 'SO_HSBT', 
-                        'Ngày mở HSBT': 'NGAY_MO_HSBT',
-                        'Ngày thông báo': 'NGAY_THONG_BAO',
-                        'Ngày xảy ra': 'NGAY_XAY_RA',
-                        'Phòng': 'PHONG_BT',
-                        'Cán bộ bồi thường': 'CAN_BO_BT',
-                        'Nghiệp vụ': 'MA_LHNV',
+                    df_rev_dict = {
+                        'Mã đơn vị': 'MA_DVI',
+                        'Mã đơn vị quản lý hợp đồng': 'MA_DVI_QL',
                         'Số hợp đồng': 'SO_HD',
-                        'Mã khai thác': 'MA_KT',
-                        'Mã khách hàng': 'MA_KH',
-                        'Tên khách hàng': 'TEN_KH',
-                        'Đối tượng bảo hiểm': 'TEN_DTBH',
+                        'Đối tượng bảo hiểm': 'SO_BIEN_XE',
+                        'Giấy chứng nhận': 'SO_GCN',
+                        'Giấy chứng nhận gốc': 'SO_GCN_GOC',
+                        'Tuổi xe': 'TUOI_XE',
+                        'Phòng': 'PHONG_BT',
                         'Ngày cấp': 'NGAY_CAP',
                         'Ngày HL': 'NGAY_HL',
-                        'Ngày KT': 'NGAY_KT',
-                        'Nhóm': 'NHOM_XE', 
-                        'Nguyên nhân': 'NGUYEN_NHAN_BT',
-                        'Số tiền tổn thất': 'STTT',
-                        'Số tiền bồi thường': 'STBT'
+                        'Ngày kết thúc': 'NGAY_KT',
+                        'Mã khách hàng': 'MA_KH',
+                        'Tên khách hàng': 'TEN_KH',
+                        'Nguồn KT': 'NGUON_KT',
+                        'LHNV': 'MA_LHNV',
+                        'Tên LHNV': 'TEN_LHNV',
+                        'Nguyên tệ số tiền BH': 'NGUYEN_TE',
+                        'Số tiền bảo hiểm': 'STBH',
+                        'Phí doanh thu': 'PHI_BH',
+                        'Mã đối tượng': 'NHOM_XE',
+                        'Loại': 'NHOM_XE_2',
+                        'Nhóm': 'LOAI_XE',
+                        'Loại KH': 'LOAI_KH',
+                        'Phân khúc': 'PHAN_KHUC_KH',
+                        'Số CMT/MST': 'SO_CMT/MST',
+                        'Đại lý': 'DAI_LY',
+                        'CBQL': 'CAN_BO_QL',
+                        'Giá trị xe': 'GIA_TRI_XE'
                     }
 
-                    df.rename(columns={col: df_clm_dict[col] for col in df.columns if col in df_clm_dict}, inplace=True)
+                    df.rename(columns={col: df_rev_dict[col] for col in df.columns if col in df_rev_dict}, inplace=True)
+
 
-                            
                     """ REMOVE UNNECESSARY COLUMNS"""
                     print("--------------------------------------------------------------------------\nRemoving Unneeded Columns:")
                     removed_cols = [
-                        'STT',
-                        'Cán bộ cấp đơn',
-                        'Thu hồi bồi thường',
-                        'Phí giám định'
+                        'Nhóm KH',
+                        'Người thụ hưởng',
+                        'Ngày bán hàng',
+                        'Ngày kỳ thanh toán',
                         'Kiểu ĐBH', 
-                        'Tỷ lệ ĐBH', 
-                        'Thu đòi đồng BH', 
-                        'Tỷ lệ tái CĐ', 
-                        'Thu đòi tái bảo hiểm CĐ', 
-                        'Tỷ lệ tái TT', 
-                        'Thu đòi tái bảo hiểm TT'
+                        'TL của VBI',
+                        'STT'
                     ]
 
                     # Removing columns, check if the columns exist
-                    for col in removed_cols:
-                        if col in df.columns:
-                            df.drop(columns=col, inplace=True)
-                        else:
-                            print(f"   Column {col} not found in DataFrame.")                       
-
+                    columns_to_remove = [col for col in removed_cols if col in df.columns]
+                    df.drop(columns=columns_to_remove, inplace=True)
+                    
+                    # Remove Reins Columns
+                    try:
+                        phi_bh_index = df.columns.get_loc("PHI_BH")
+                    except KeyError:
+                        print("Column 'PHI_BH' not found in DataFrame")
+                        raise
 
-                    """ ADD COLUMN FOR VALUATION QUARTER"""
-                    print("--------------------------------------------------------------------------\nAdding Column VALU_QUARTER:")
-                    df['VALU_QUARTER'] = quarter
+                    # Step 2: Drop from the next column after "PHI_BH" onwards
+                    df.drop(df.columns[phi_bh_index + 1:], axis=1, inplace=True)
 
 
                     """ FILTER FOR LHNV"""
                     if lhnv:
                         print("--------------------------------------------------------------------------\nFiltering for LHNV:")    
                         rows_b4 = df.shape[0]    
                         df = df[df['MA_LHNV'] == lhnv]
                         print(f'   Removed: {(rows_b4 - df.shape[0]):,.0f} Rows, ({((rows_b4 - df.shape[0])/rows_b4*100):.2f}%)')
 
 
-                    # """ SEPARATE SO MAY and SO KHUNG"""
-                    # print("--------------------------------------------------------------------------\nSeparating SO MAY/SO KHUNG:")
-                    # df['SO_KHUNG/SO_MAY'].fillna('/')
-                    # def get_part(x, index):
-                    #     parts = x.split('/')
-                    #     return parts[index] if len(parts) > index else np.nan
-
-                    # # Apply this function to create the new columns
-                    # df['SO_KHUNG'] = df['SO_KHUNG/SO_MAY'].apply(lambda x: get_part(x, 0))
-                    # df['SO_MAY'] = df['SO_KHUNG/SO_MAY'].apply(lambda x: get_part(x, 1))
-                    # df.drop('SO_KHUNG/SO_MAY', axis = 1, inplace = True)
-                    
-                    
                     """ CONVERT DATE COLUMNS"""           
                     print("--------------------------------------------------------------------------\nReformatting Date Cols:")
                     dates_columns = [
-                        "NGAY_MO_HSBT",
-                        "NGAY_THONG_BAO",
-                        "NGAY_XAY_RA",
-                        "NGAY_GIAI_QUYET",
                         "NGAY_CAP",
                         "NGAY_HL",
-                        "NGAY_KT",
-                        "NGAY_TT_BT"
+                        "NGAY_KT"
                     ]
 
                     for dates_col in dates_columns:
                         if dates_col in df.columns:  # Ensure column exists before converting
                             original_na_count = df[dates_col].isna().sum()
                             df[dates_col] = pd.to_datetime(df[dates_col], errors='coerce', dayfirst=True)
                             new_na_count = df[dates_col].isna().sum()
@@ -151,93 +141,58 @@
 
                     """ CONVERT NUMERICAL COLUMNS"""
                     print("--------------------------------------------------------------------------\nReformatting Num Cols:")
                     num_columns = [
                         'TUOI_XE',
                         'STBH',
                         'PHI_BH',
-                        'STTT',
-                        'STBT'
+                        'GIA_TRI_XE'
                     ]
                     
                     for num_col in num_columns:
                         if num_col in df.columns:  # Ensure column exists before converting
                             original_na_count = df[num_col].isna().sum()
                             df[num_col] = pd.to_numeric(df[num_col], errors='coerce')
                             new_na_count = df[num_col].isna().sum()
                             detected_errors = new_na_count - original_na_count
                             if detected_errors > 0:
                                 print(f"   Detected {detected_errors} Incorrect Values in {num_col}")
                         else:
                             print(f"   Column {num_col} not found in DataFrame.")
                     
-                    
-                    # """ PROCESS DUPLICATED/COINSURED ROWS """
-                    # print("--------------------------------------------------------------------------\nProcessing Dup/Coins Rows:")
-                    # """ Step 1 - Remove Duplicated Transactions and Aggregate """
-                    # _nrows_bf1 = df.shape[0]
-                    # _clms_bf1 = df['STBT'].sum()
-                    # # Identify duplicates that need to be summed
-                    # duplicates_to_sum = df.duplicated(subset=['MA_DVI', 'SO_HSBT', 'STBT'], keep=False)
-                    # df_duplicates = df[duplicates_to_sum]
-
-                    # # Aggregate the data for duplicates
-                    # df_agg = df_duplicates.groupby(['MA_DVI', 'SO_HSBT']).agg({
-                    #     'STBT': 'sum'
-                    # }).reset_index()
-
-                    # # Remove the original duplicated rows from df
-                    # df = df[~duplicates_to_sum]
-
-                    # # Append aggregated results back to the main DataFrame
-                    # df = pd.concat([df, df_agg], ignore_index=True)
-
-                    # print(f"Step 1 - Remove Duplicates\n   -Removed {(_nrows_bf1 - df.shape[0]):,.0f} Rows\n   -Change in Tot Claims = {(_clms_bf1 - df['STBT'].sum()):,.0f} ({((_clms_bf1 - df['STBT'].sum())/_clms_bf1*100):,.0f}%)")
-
-                    # """ Step 2 - Aggregate Claims with Multiple Transactions into One"""  # Policies with same Claim ID, department ID, and different Claim amounts 
-                    # _nrows_bf2 = df.shape[0]
-                    # _clms_bf2 = df['STBT'].sum()
-                    # df['HACH_TOAN'] = df['HACH_TOAN'].astype(bool)
-                    # df_many_trans = df[df.duplicated(subset=['MA_DVI', 'SO_HSBT'], keep = False)]
-                    # df_many_trans_agg = df_many_trans.groupby(by = 'SO_HSBT')[['STBT']].sum()
-                    # _many_trans_chuaht = df.duplicated(subset=['MA_DVI', 'SO_HSBT'], keep = False) & ~df["HACH_TOAN"]
-
-                    # df = df[~_many_trans_chuaht] # Bo nhung dong trung va chua HT (giu da HT lam cot chinh)
-
-                    # for index, row in df_many_trans_agg.iterrows():
-                    #     SO_HSBT = index
-                    #     STBT = row['STBT']
-
-                    #     df.loc[df['SO_HSBT'] == SO_HSBT, ['STBT']] = STBT
-
-                    # print(f"Step 2 - Adjust for Multiple Claims\n   -Removed {(_nrows_bf2 - df.shape[0]):,.0f} Rows\n   -Change in Tot Claims = {(_clms_bf2 - df['STBT'].sum()):,.0f} ({((_clms_bf2 - df['STBT'].sum())/_clms_bf2*100):,.0f}%)")
-
-                    # """ Step 3 - Aggregate Claims with Internal Coinsurance into One """  # Poclies with same Claim ID, different Department ID
-                    # _nrows_bf3 = df.shape[0]
-                    # _clms_bf3 = df['STBT'].sum()
-                    # df["IS_MAIN"] = df.apply(lambda x: x["SO_HSBT"][:3] == x["MA_DVI"], axis=1)
-
-                    # df_many_qly = df[df.duplicated(subset=['SO_HSBT'], keep = False)]
-                    # df_many_qly_agg = df_many_qly.groupby(by = 'SO_HSBT')[['STBT']].sum()
-                    # _many_qly_notmain = df.duplicated(subset=['SO_HSBT'], keep = False) & ~df["IS_MAIN"]
-
-                    # df = df[~_many_qly_notmain] # Bo nhung dong trung va khong phai dvi qly chinh 
-
-                    # for index, row in df_many_qly_agg.iterrows():
-                    #     SO_HSBT = index
-                    #     STBT = row['STBT']
-
-                    #     df.loc[df['SO_HSBT'] == SO_HSBT, ['STBT']] = STBT
-
-                    # print(f"Step 3 - Adjust for Internal Insurance\n   -Removed {(_nrows_bf3 - df.shape[0]):,.0f} Rows\n   -Change in Tot Claims = {(_clms_bf3 - df['STBT'].sum()):,.0f} ({((_clms_bf3 - df['STBT'].sum())/_clms_bf3*100):,.0f}%)")
-
+                    """ PROCESS DUPLICATED/COINSURED ROWS """
+                    if year != '2020':  #SO_GCN was not recorded before 2021.
+                        print("--------------------------------------------------------------------------\nProcessing Dup/Coins Rows:")
+
+                        """ Step 1 - Remove Duplicated Policies """  # Result - Removed Policies with multiple Premium Transactions
+                        _nrows_bf1 = df.shape[0]
+                        _rev_bf1 = df['PHI_BH'].sum()
+                        df = df[~df.duplicated(subset = ['MA_DVI', 'SO_HD', 'SO_GCN', 'SO_BIEN_XE', 'STBH'])] # Policies with the same Pol ID, Department ID, GCN, and SI amount are duplicates
+
+                        print(f"Step 1 - Remove Duplicates\n   -Removed {(_nrows_bf1 - df.shape[0]):,.0f} Rows\n   -Change in Tot Revenue = {(_rev_bf1 - df['PHI_BH'].sum()):,.0f} ({((_rev_bf1 - df['PHI_BH'].sum())/_rev_bf1*100):,.0f}%)")
+
+                        """ Step 2 - Aggregate Claims with Multiple Department IDs """  # Poclies with same Claim ID, different Department ID
+                        _nrows_bf2 = df.shape[0]
+                        _rev_bf2 = df['PHI_BH'].sum()
+                        df["IS_MAIN"] = df.apply(lambda x: x["SO_HD"][:3] == x["MA_DVI"], axis=1)
+                        df = df[df["IS_MAIN"]]
+                        df.drop('IS_MAIN', axis = 1, inplace = True)
+
+                        print(f"Step 2 - Adjust for Internal Coinsurance\n   -Removed {(_nrows_bf2 - df.shape[0]):,.0f} Rows\n   -Change in Tot Revenue = {(_rev_bf2 - df['PHI_BH'].sum()):,.0f} ({((_rev_bf2 - df['PHI_BH'].sum())/_rev_bf2*100):,.0f}%)")
+
+                        """ Step 3 - Remove the rest of the Dups """ 
+                        _nrows_bf3 = df.shape[0] 
+                        _rev_bf3 = df['PHI_BH'].sum()
+                        df = df[~df.duplicated(subset = ['NGAY_HL', 'SO_GCN', 'SO_BIEN_XE', 'SO_HD', 'STBH'])]
+        
+                        print(f"Step 3 - Remove Rest of Duplicates\n   -Removed {(_nrows_bf3 - df.shape[0]):,.0f} Rows\n   -Change in Tot Revenue = {(_rev_bf3 - df['PHI_BH'].sum()):,.0f} ({((_rev_bf3 - df['PHI_BH'].sum())/_rev_bf3*100):,.0f}%)")
                         
                     
                     """ REMOVE ROWs WITH MISSING EFF DATE """
-                    print("--------------------------------------------------------------------------\nRemoving Rows Missing NGAY_HL:")    
+                    print("--------------------------------------------------------------------------\nRemove Rows Missing NGAY_HL:")    
                     rows_b4 = df.shape[0]    
                     df = df[df['NGAY_HL'].notna()]
                     print(f'   Removed: {(rows_b4 - df.shape[0]):,.0f} Rows, ({((rows_b4 - df.shape[0])/rows_b4*100):.2f}%)')
                     
                     
                     " STANDARDIZE PLATE IDs"
                     print("--------------------------------------------------------------------------\nStandardizing SO_BIEN_XE:")    
@@ -249,43 +204,60 @@
                     df.loc[~df['SO_BIEN_XE'].str.match(pattern, na = False), 'SO_BIEN_XE'] = pd.NA
                     
                     print(f'   Changed: {sum(df['SO_BIEN_XE'] == _copy)} values')
                     print(f'   Converted: {df['SO_BIEN_XE'].isna().sum() - _copy.isna().sum()} to NAs')
                     del _copy
                     
                     
+                    """ REPLACE BLANKS WITH NAs """
+                    print("--------------------------------------------------------------------------\nReplacing Blanks:")
+                    def replace_blanks(x):
+                        if isinstance(x, str) and x.strip() == '':
+                            return np.nan
+                        else:
+                            return x
+                        
+                    for col in df.columns:
+                        col_copy = df[col].copy()
+                        df[col] = df[col].apply(replace_blanks)
+                        replaced = (col_copy != df[col]).sum()
+                        if replaced > 0:
+                            print(f"   Converted {replaced} values in {col}")
+                    
+                    del col_copy
+                    
+                    
                     """ PRINT EFF_YEAR COUNTS IN EACH DF"""
                     print("--------------------------------------------------------------------------\nEff Year Count:")
                     df['NAM_HL'] = df['NGAY_HL'].dt.year 
                     print(f"Effective Year Count in CY{year}: {df['NAM_HL'].value_counts()}")
-                        
+                    
                     
                     """ SAVE DF TO GLOBAL VARIABLE"""
                     print("--------------------------------------------------------------------------\nSaving DF:")
                     # Assign DataFrame to a global variable dynamically using the year
-                    df_name = f'df_clm_{year}'
+                    df_name = f'df_rev_{year}'
                     globals()[df_name] = df
                     global_df_names.append(df_name)
-                    print(f"Summary of CY{year}:\n   -NUM CLAIMS = {df.shape[0]:,.0f}\n   -TOTAL CLAIMS = {df['STBT'].sum():,.0f}")
+                    print(f"Summary of CY{year}:\n   -NUM POLS = {df.shape[0]:,.0f}\n   -TOTAL REVENUE = {df['PHI_BH'].sum():,.0f}")
                     print('--------------------------------------------------------------------------\nxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx')
-                    
                 except Exception as e:
                     print(f"Failed to process {file}: {e}")
             else:
                 print(f"No year found in the file name {file}")
 
     # Print all global DataFrame names created
     print("\n\n\n==========================================================================\n==========================================================================\nSuccessfully Imported:", ", ".join(global_df_names))
     
     """ CONCAT INTO ONE DF"""
     all_dataframes = [globals()[name] for name in global_df_names if name in globals()]
-    df_clm = pd.concat(all_dataframes, ignore_index=True)
-    print(f"   Total Rows = {df_clm.shape[0]:,.0f}\n   Total Claims = {df_clm['STBT'].sum():,.0f}")
+    df_rev = pd.concat(all_dataframes, ignore_index=True)
+    print(f"   -NUM POLS = {df_rev.shape[0]:,.0f}\n   -TOTAL REVENUE = {df_rev['PHI_BH'].sum():,.0f}")
     
     print("==========================================================================\n==========================================================================")
     for name in global_df_names:
         del globals()[name]
         
     global_df_names.clear()
     
-    return df_clm
+    return df_rev
```

### Comparing `vbpy-2.2.3/vbpy/load_revenue_auto_file.py` & `vbpy-2.2.4/vbpy/load_open_claim_auto_file.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import pandas as pd
 import numpy as np
 pd.set_option('display.max_rows', None) 
 pd.set_option('display.max_columns', None)  
-
 import os
 import re
 from tqdm import tqdm
 
-def load_revenue_auto(directory, skip_rows=13, lhnv = None):
+def load_open_claim_auto(directory, skip_rows=12, lhnv = None):
     # Regular expression to find a four-digit year in the file name
-    year_pattern = re.compile(r'\b(\d{4})\b')
+    pattern = re.compile(r'\b(\d{2})-(\d{4})\b')
 
     # List to keep track of the names of the DataFrames stored as globals
     global_df_names = []
 
     # Iterate through each file in the specified directory
     for file in sorted(os.listdir(directory)):
         if file.endswith('.xlsx') and not file.startswith('~$'):
             
             # Find the year in the file name
-            match = year_pattern.search(file)
+            match = pattern.search(file)
             if match:
-                year = match.group(1)
+                quarter = match.group(1)
                 file_path = os.path.join(directory, file)
                 try:
                     """ IMPORT DATA"""
                     print(f"\n\n\nxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx\n--------------------------------------------------------------------------\nImporting: {file}")
                     # Load and clean data specifying the engine
                     df = pd.read_excel(file_path, header=None, skiprows=skip_rows, engine='openpyxl')
                     df.drop(df.columns[-1], axis = 1, inplace = True)  # remove na col at the end
@@ -42,90 +41,88 @@
 
                     # Set the determined headers as column names
                     df.columns = headers
                     df = df.drop([0, 1])
                     df.reset_index(drop = True, inplace=True)
                     print(f'   Rows = {df.shape[0]}')
                     # print(f'Columns = {df.shape[1]}')
-            
+                    print(df)
             
                     """ RENAME COLUMNS"""
                     print("--------------------------------------------------------------------------\nRenaming Columns:")
-                    df_rev_dict = {
-                        'Mã đơn vị': 'MA_DVI',
-                        'Mã đơn vị quản lý hợp đồng': 'MA_DVI_QL',
-                        'Số hợp đồng': 'SO_HD',
-                        'Đối tượng bảo hiểm': 'SO_BIEN_XE',
-                        'Giấy chứng nhận': 'SO_GCN',
-                        'Giấy chứng nhận gốc': 'SO_GCN_GOC',
-                        'Tuổi xe': 'TUOI_XE',
+                    df_clm_dict = {
+                        'Số hồ sơ': 'SO_HSBT', 
+                        'Ngày mở HSBT': 'NGAY_MO_HSBT',
+                        'Ngày thông báo': 'NGAY_THONG_BAO',
+                        'Ngày xảy ra': 'NGAY_XAY_RA',
                         'Phòng': 'PHONG_BT',
-                        'Ngày cấp': 'NGAY_CAP',
-                        'Ngày HL': 'NGAY_HL',
-                        'Ngày kết thúc': 'NGAY_KT',
+                        'Cán bộ bồi thường': 'CAN_BO_BT',
+                        'Nghiệp vụ': 'MA_LHNV',
+                        'Số hợp đồng': 'SO_HD',
+                        'Mã khai thác': 'MA_KT',
                         'Mã khách hàng': 'MA_KH',
                         'Tên khách hàng': 'TEN_KH',
-                        'Nguồn KT': 'NGUON_KT',
-                        'LHNV': 'MA_LHNV',
-                        'Tên LHNV': 'TEN_LHNV',
-                        'Nguyên tệ số tiền BH': 'NGUYEN_TE',
-                        'Số tiền bảo hiểm': 'STBH',
-                        'Phí doanh thu': 'PHI_BH',
-                        'Mã đối tượng': 'NHOM_XE',
-                        'Loại': 'NHOM_XE_2',
-                        'Nhóm': 'LOAI_XE',
-                        'Loại KH': 'LOAI_KH',
-                        'Phân khúc': 'PHAN_KHUC_KH',
-                        'Số CMT/MST': 'SO_CMT/MST',
-                        'Đại lý': 'DAI_LY',
-                        'CBQL': 'CAN_BO_QL',
-                        'Giá trị xe': 'GIA_TRI_XE'
+                        'Đối tượng bảo hiểm': 'TEN_DTBH',
+                        'Ngày cấp': 'NGAY_CAP',
+                        'Ngày HL': 'NGAY_HL',
+                        'Ngày KT': 'NGAY_KT',
+                        'Nhóm': 'NHOM_XE', 
+                        'Nguyên nhân': 'NGUYEN_NHAN_BT',
+                        'Số tiền tổn thất': 'STTT',
+                        'Số tiền bồi thường': 'STBT'
                     }
 
-                    df.rename(columns={col: df_rev_dict[col] for col in df.columns if col in df_rev_dict}, inplace=True)
-
+                    df.rename(columns={col: df_clm_dict[col] for col in df.columns if col in df_clm_dict}, inplace=True)
 
+                            
                     """ REMOVE UNNECESSARY COLUMNS"""
                     print("--------------------------------------------------------------------------\nRemoving Unneeded Columns:")
                     removed_cols = [
-                        'Nhóm KH',
-                        'Người thụ hưởng',
-                        'Ngày bán hàng',
-                        'Ngày kỳ thanh toán',
+                        'STT',
+                        'Cán bộ cấp đơn',
+                        'Thu hồi bồi thường',
+                        'Phí giám định',
                         'Kiểu ĐBH', 
-                        'TL của VBI',
-                        'STT'
+                        'Tỷ lệ ĐBH', 
+                        'Thu đòi đồng BH', 
+                        'Tỷ lệ tái CĐ', 
+                        'Thu đòi tái bảo hiểm CĐ', 
+                        'Tỷ lệ tái TT', 
+                        'Thu đòi tái bảo hiểm TT'
                     ]
 
                     # Removing columns, check if the columns exist
-                    columns_to_remove = [col for col in removed_cols if col in df.columns]
-                    df.drop(columns=columns_to_remove, inplace=True)
-                    
-                    # Remove Reins Columns
-                    try:
-                        phi_bh_index = df.columns.get_loc("PHI_BH")
-                    except KeyError:
-                        print("Column 'PHI_BH' not found in DataFrame")
-                        raise
+                    for col in removed_cols:
+                        if col in df.columns:
+                            df.drop(columns=col, inplace=True)
+                        else:
+                            print(f"   Column {col} not found in DataFrame.")                       
 
-                    # Step 2: Drop from the next column after "PHI_BH" onwards
-                    df.drop(df.columns[phi_bh_index + 1:], axis=1, inplace=True)
+
+                    """ ADD COLUMN FOR VALUATION QUARTER"""
+                    print("--------------------------------------------------------------------------\nAdding Column VALU_QUARTER:")
+                    df['VALU_QUARTER'] = quarter
 
 
                     """ FILTER FOR LHNV"""
                     if lhnv:
                         print("--------------------------------------------------------------------------\nFiltering for LHNV:")    
                         rows_b4 = df.shape[0]    
                         df = df[df['MA_LHNV'] == lhnv]
                         print(f'   Removed: {(rows_b4 - df.shape[0]):,.0f} Rows, ({((rows_b4 - df.shape[0])/rows_b4*100):.2f}%)')
 
 
+                    
+                    
                     """ CONVERT DATE COLUMNS"""           
                     print("--------------------------------------------------------------------------\nReformatting Date Cols:")
                     dates_columns = [
+                        "NGAY_MO_HSBT",
+                        "NGAY_THONG_BAO",
+                        "NGAY_XAY_RA",
                         "NGAY_CAP",
                         "NGAY_HL",
                         "NGAY_KT"
                     ]
 
                     for dates_col in dates_columns:
                         if dates_col in df.columns:  # Ensure column exists before converting
@@ -138,126 +135,62 @@
                         else:
                             print(f"   Column {dates_col} not found in DataFrame.")
 
 
                     """ CONVERT NUMERICAL COLUMNS"""
                     print("--------------------------------------------------------------------------\nReformatting Num Cols:")
                     num_columns = [
-                        'TUOI_XE',
-                        'STBH',
-                        'PHI_BH',
-                        'GIA_TRI_XE'
+                        'STTT',
+                        'STBT'
                     ]
                     
                     for num_col in num_columns:
                         if num_col in df.columns:  # Ensure column exists before converting
                             original_na_count = df[num_col].isna().sum()
                             df[num_col] = pd.to_numeric(df[num_col], errors='coerce')
                             new_na_count = df[num_col].isna().sum()
                             detected_errors = new_na_count - original_na_count
                             if detected_errors > 0:
                                 print(f"   Detected {detected_errors} Incorrect Values in {num_col}")
                         else:
                             print(f"   Column {num_col} not found in DataFrame.")
                     
-                    """ PROCESS DUPLICATED/COINSURED ROWS """
-                    if year != '2020':  #SO_GCN was not recorded before 2021.
-                        print("--------------------------------------------------------------------------\nProcessing Dup/Coins Rows:")
-
-                        """ Step 1 - Remove Duplicated Policies """  # Result - Removed Policies with multiple Premium Transactions
-                        _nrows_bf1 = df.shape[0]
-                        _rev_bf1 = df['PHI_BH'].sum()
-                        df = df[~df.duplicated(subset = ['MA_DVI', 'SO_HD', 'SO_GCN', 'SO_BIEN_XE', 'STBH'])] # Policies with the same Pol ID, Department ID, GCN, and SI amount are duplicates
-
-                        print(f"Step 1 - Remove Duplicates\n   -Removed {(_nrows_bf1 - df.shape[0]):,.0f} Rows\n   -Change in Tot Revenue = {(_rev_bf1 - df['PHI_BH'].sum()):,.0f} ({((_rev_bf1 - df['PHI_BH'].sum())/_rev_bf1*100):,.0f}%)")
-
-                        """ Step 2 - Aggregate Claims with Multiple Department IDs """  # Poclies with same Claim ID, different Department ID
-                        _nrows_bf2 = df.shape[0]
-                        _rev_bf2 = df['PHI_BH'].sum()
-                        df["IS_MAIN"] = df.apply(lambda x: x["SO_HD"][:3] == x["MA_DVI"], axis=1)
-                        df = df[df["IS_MAIN"]]
-                        df.drop('IS_MAIN', axis = 1, inplace = True)
-
-                        print(f"Step 2 - Adjust for Internal Coinsurance\n   -Removed {(_nrows_bf2 - df.shape[0]):,.0f} Rows\n   -Change in Tot Revenue = {(_rev_bf2 - df['PHI_BH'].sum()):,.0f} ({((_rev_bf2 - df['PHI_BH'].sum())/_rev_bf2*100):,.0f}%)")
-
-                        """ Step 3 - Remove the rest of the Dups """ 
-                        _nrows_bf3 = df.shape[0] 
-                        _rev_bf3 = df['PHI_BH'].sum()
-                        df = df[~df.duplicated(subset = ['NGAY_HL', 'SO_GCN', 'SO_BIEN_XE', 'SO_HD', 'STBH'])]
-        
-                        print(f"Step 3 - Remove Rest of Duplicates\n   -Removed {(_nrows_bf3 - df.shape[0]):,.0f} Rows\n   -Change in Tot Revenue = {(_rev_bf3 - df['PHI_BH'].sum()):,.0f} ({((_rev_bf3 - df['PHI_BH'].sum())/_rev_bf3*100):,.0f}%)")
                         
                     
                     """ REMOVE ROWs WITH MISSING EFF DATE """
-                    print("--------------------------------------------------------------------------\nRemove Rows Missing NGAY_HL:")    
+                    print("--------------------------------------------------------------------------\nRemoving Rows Missing NGAY_HL:")    
                     rows_b4 = df.shape[0]    
                     df = df[df['NGAY_HL'].notna()]
                     print(f'   Removed: {(rows_b4 - df.shape[0]):,.0f} Rows, ({((rows_b4 - df.shape[0])/rows_b4*100):.2f}%)')
-                    
-                    
-                    " STANDARDIZE PLATE IDs"
-                    print("--------------------------------------------------------------------------\nStandardizing SO_BIEN_XE:")    
-                    pattern = r'^\d{2}[A-Za-z]\d{4,5}$' 
-                    _copy = df['SO_BIEN_XE'].copy()
-                    df.loc[:,'SO_BIEN_XE'] = df['SO_BIEN_XE'].str.replace('[^a-zA-Z0-9]', '', regex=True)
-                    df.loc[:,'SO_BIEN_XE'] = df['SO_BIEN_XE'].str.strip().str.upper()
-                    df.loc[df['SO_BIEN_XE'] == '', 'SO_BIEN_XE'] = pd.NA
-                    df.loc[~df['SO_BIEN_XE'].str.match(pattern, na = False), 'SO_BIEN_XE'] = pd.NA
-                    
-                    print(f'   Changed: {sum(df['SO_BIEN_XE'] == _copy)} values')
-                    print(f'   Converted: {df['SO_BIEN_XE'].isna().sum() - _copy.isna().sum()} to NAs')
-                    del _copy
-                    
-                    
-                    """ REPLACE BLANKS WITH NAs """
-                    print("--------------------------------------------------------------------------\nReplacing Blanks:")
-                    def replace_blanks(x):
-                        if isinstance(x, str) and x.strip() == '':
-                            return np.nan
-                        else:
-                            return x
                         
-                    for col in df.columns:
-                        col_copy = df[col].copy()
-                        df[col] = df[col].apply(replace_blanks)
-                        replaced = (col_copy != df[col]).sum()
-                        if replaced > 0:
-                            print(f"   Converted {replaced} values in {col}")
-                    
-                    del col_copy
-                    
-                    
-                    """ PRINT EFF_YEAR COUNTS IN EACH DF"""
-                    print("--------------------------------------------------------------------------\nEff Year Count:")
-                    df['NAM_HL'] = df['NGAY_HL'].dt.year 
-                    print(f"Effective Year Count in CY{year}: {df['NAM_HL'].value_counts()}")
-                    
+                        
                     
                     """ SAVE DF TO GLOBAL VARIABLE"""
                     print("--------------------------------------------------------------------------\nSaving DF:")
                     # Assign DataFrame to a global variable dynamically using the year
-                    df_name = f'df_rev_{year}'
+                    df_name = f'df_clm_{year}'
                     globals()[df_name] = df
                     global_df_names.append(df_name)
-                    print(f"Summary of CY{year}:\n   -NUM POLS = {df.shape[0]:,.0f}\n   -TOTAL REVENUE = {df['PHI_BH'].sum():,.0f}")
+                    print(f"Summary of CY{year}:\n   -NUM CLAIMS = {df.shape[0]:,.0f}\n   -TOTAL CLAIMS = {df['STBT'].sum():,.0f}")
                     print('--------------------------------------------------------------------------\nxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx')
+                    
                 except Exception as e:
                     print(f"Failed to process {file}: {e}")
             else:
                 print(f"No year found in the file name {file}")
 
     # Print all global DataFrame names created
     print("\n\n\n==========================================================================\n==========================================================================\nSuccessfully Imported:", ", ".join(global_df_names))
     
     """ CONCAT INTO ONE DF"""
     all_dataframes = [globals()[name] for name in global_df_names if name in globals()]
-    df_rev = pd.concat(all_dataframes, ignore_index=True)
-    print(f"   -NUM POLS = {df_rev.shape[0]:,.0f}\n   -TOTAL REVENUE = {df_rev['PHI_BH'].sum():,.0f}")
+    df_clm_open = pd.concat(all_dataframes, ignore_index=True)
+    print(f"   Total Rows = {df_clm_open.shape[0]:,.0f}\n   Total Claims = {df_clm_open['STBT'].sum():,.0f}")
     
     print("==========================================================================\n==========================================================================")
     for name in global_df_names:
         del globals()[name]
         
     global_df_names.clear()
     
-    return df_rev
+    return df_clm_open
```

