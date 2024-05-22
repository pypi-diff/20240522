# Comparing `tmp/vbpy-2.2.0.tar.gz` & `tmp/vbpy-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbpy-2.2.0.tar", last modified: Wed May 22 09:16:33 2024, max compression
+gzip compressed data, was "vbpy-2.2.1.tar", last modified: Wed May 22 09:47:01 2024, max compression
```

## Comparing `vbpy-2.2.0.tar` & `vbpy-2.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 09:16:33.530000 vbpy-2.2.0/
--rw-rw-rw-   0        0        0      122 2024-05-22 09:16:34.000000 vbpy-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-22 09:16:34.000000 vbpy-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0      536 2024-05-22 09:16:18.000000 vbpy-2.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:16:33.570000 vbpy-2.2.0/vbpy/
--rw-rw-rw-   0        0        0      265 2024-05-22 09:16:04.000000 vbpy-2.2.0/vbpy/__init__.py
--rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.2.0/vbpy/combine_data_file.py
--rw-rw-rw-   0        0        0     1006 2024-05-22 08:23:28.000000 vbpy-2.2.0/vbpy/load_channel_data_file.py
--rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.2.0/vbpy/load_claim_auto_file.py
--rw-rw-rw-   0        0        0    18225 2024-05-22 09:16:10.000000 vbpy-2.2.0/vbpy/load_open_claim_auto_file.py
--rw-rw-rw-   0        0        0    14873 2024-05-22 07:54:10.000000 vbpy-2.2.0/vbpy/load_revenue_auto_file.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:16:33.610000 vbpy-2.2.0/vbpy.egg-info/
--rw-rw-rw-   0        0        0      122 2024-05-22 09:16:34.000000 vbpy-2.2.0/vbpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-05-22 09:16:34.000000 vbpy-2.2.0/vbpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 09:16:34.000000 vbpy-2.2.0/vbpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-22 09:16:34.000000 vbpy-2.2.0/vbpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 09:47:01.210000 vbpy-2.2.1/
+-rw-rw-rw-   0        0        0      122 2024-05-22 09:47:02.000000 vbpy-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-22 09:47:02.000000 vbpy-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      536 2024-05-22 09:46:58.000000 vbpy-2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:47:01.240000 vbpy-2.2.1/vbpy/
+-rw-rw-rw-   0        0        0      265 2024-05-22 09:16:04.000000 vbpy-2.2.1/vbpy/__init__.py
+-rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.2.1/vbpy/combine_data_file.py
+-rw-rw-rw-   0        0        0     1006 2024-05-22 08:23:28.000000 vbpy-2.2.1/vbpy/load_channel_data_file.py
+-rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.2.1/vbpy/load_claim_auto_file.py
+-rw-rw-rw-   0        0        0    16408 2024-05-22 09:46:12.000000 vbpy-2.2.1/vbpy/load_open_claim_auto_file.py
+-rw-rw-rw-   0        0        0    14873 2024-05-22 07:54:10.000000 vbpy-2.2.1/vbpy/load_revenue_auto_file.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:47:01.280000 vbpy-2.2.1/vbpy.egg-info/
+-rw-rw-rw-   0        0        0      122 2024-05-22 09:47:02.000000 vbpy-2.2.1/vbpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-05-22 09:47:02.000000 vbpy-2.2.1/vbpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 09:47:02.000000 vbpy-2.2.1/vbpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 09:47:02.000000 vbpy-2.2.1/vbpy.egg-info/top_level.txt
```

### Comparing `vbpy-2.2.0/setup.py` & `vbpy-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     
     name='vbpy',
-    version='2.2.0',
+    version='2.2.1',
     packages=find_packages(),
     # description='Your library description',
     # long_description=open('README.md').read(),
     # long_description_content_type='text/markdown',
     author='Nguyen Ha Tuan Long',
     author_email='tuanlongnguyenha@gmail.com',
     # url='https://github.com/yourusername/your_library_name',
```

### Comparing `vbpy-2.2.0/vbpy/combine_data_file.py` & `vbpy-2.2.1/vbpy/combine_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.2.0/vbpy/load_channel_data_file.py` & `vbpy-2.2.1/vbpy/load_channel_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.2.0/vbpy/load_claim_auto_file.py` & `vbpy-2.2.1/vbpy/load_claim_auto_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.2.0/vbpy/load_open_claim_auto_file.py` & `vbpy-2.2.1/vbpy/load_open_claim_auto_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,95 +37,61 @@
                         elif pd.notna(df.iloc[0, col]) and pd.isna(df.iloc[1, col]):
                             headers.append(df.iloc[0, col])
                         else:
                             print(f'No headers found for {col}')
 
                     # Set the determined headers as column names
                     df.columns = headers
-                    df = df.drop([0, 1])
+                    df = df.drop([0])
                     df.reset_index(drop = True, inplace=True)
                     print(f'   Rows = {df.shape[0]}')
                     # print(f'Columns = {df.shape[1]}')
             
             
                     """ RENAME COLUMNS"""
                     print("--------------------------------------------------------------------------\nRenaming Columns:")
                     df_clm_dict = {
-                        'mã đơn vị quản lý': 'MA_DVI',
-                        'Mã đơn vị xử lý': 'MA_DVI_XL',
-                        'Mã khai thác': 'MA_KT',
-                        'Mã khách hàng': 'MA_KH',
-                        'Số hồ sơ': 'SO_HSBT',
+                        'Số hồ sơ': 'SO_HSBT', 
                         'Ngày mở HSBT': 'NGAY_MO_HSBT',
                         'Ngày thông báo': 'NGAY_THONG_BAO',
                         'Ngày xảy ra': 'NGAY_XAY_RA',
-                        'Số ngày tồn': 'SO_NGAY_TON',
-                        'Ngày giải quyết': 'NGAY_GIAI_QUYET',
                         'Phòng': 'PHONG_BT',
                         'Cán bộ bồi thường': 'CAN_BO_BT',
                         'Nghiệp vụ': 'MA_LHNV',
-                        'Tên LHNV': 'TEN_LHNV',
                         'Số hợp đồng': 'SO_HD',
+                        'Mã khai thác': 'MA_KT',
+                        'Mã khách hàng': 'MA_KH',
                         'Tên khách hàng': 'TEN_KH',
-                        'Địa chỉ': 'DIA_CHI',
-                        'Nguồn KT': 'NGUON_KT',
-                        'Số GCN': 'SO_GCN',
-                        'Biển xe': 'SO_BIEN_XE',
-                        'Số khung/Số máy': 'SO_KHUNG/SO_MAY',
                         'Đối tượng bảo hiểm': 'TEN_DTBH',
-                        'Tuổi xe': 'TUOI_XE',
                         'Ngày cấp': 'NGAY_CAP',
                         'Ngày HL': 'NGAY_HL',
                         'Ngày KT': 'NGAY_KT',
-                        'Mã NT': 'MA_NGUYEN_TE',
-                        'Số tiền bảo hiểm': 'STBH',
-                        'Phí bảo hiểm VNĐ': 'PHI_BH',
                         'Nhóm': 'NHOM_XE', 
-                        'Loại xe': 'LOAI_XE',
                         'Nguyên nhân': 'NGUYEN_NHAN_BT',
                         'Số tiền tổn thất': 'STTT',
-                        'Số tiền bồi thường': 'STBT', 
-                        'Ngày thanh toán bồi thường': 'NGAY_TT_BT',
-                        'Gara': 'GARA',
-                        'Hạch toán': 'HACH_TOAN',
-                        'Ghi chú': 'GHI_CHU'
+                        'Số tiền bồi thường': 'STBT'
                     }
 
                     df.rename(columns={col: df_clm_dict[col] for col in df.columns if col in df_clm_dict}, inplace=True)
 
                             
                     """ REMOVE UNNECESSARY COLUMNS"""
                     print("--------------------------------------------------------------------------\nRemoving Unneeded Columns:")
                     removed_cols = [
-                        'Lĩnh vực kinh doanh',
-                        'Cán bộ cấp đơn',
-                        'Tổng giảm trừ', 
                         'STT',
-                        'Số CV KN',
-                        'Ngày hồ sơ đầy đủ', 
-                        'Khu vực', 
-                        'Điện thoại', 
-                        'Danh mục cơ sở', 
-                        'Email', 
-                        'Số tiền bảo hiểm đưa vào tái',  
-                        'Ngày thanh toán phí',
+                        'Cán bộ cấp đơn',
+                        'Thu hồi bồi thường',
+                        'Phí giám định'
                         'Kiểu ĐBH', 
                         'Tỷ lệ ĐBH', 
                         'Thu đòi đồng BH', 
                         'Tỷ lệ tái CĐ', 
                         'Thu đòi tái bảo hiểm CĐ', 
                         'Tỷ lệ tái TT', 
-                        'Thu đòi tái bảo hiểm TT',
-                        'Giảm trừ tỷ lệ bảo hiểm',
-                        'Giảm trừ khấu hao',
-                        'Giảm trừ chế tài',
-                        'Giảm trừ khác',
-                        'Miễn thường',
-                        'Thu hồi bồi thường',
-                        'Phí giám định'
+                        'Thu đòi tái bảo hiểm TT'
                     ]
 
                     # Removing columns, check if the columns exist
                     for col in removed_cols:
                         if col in df.columns:
                             df.drop(columns=col, inplace=True)
                         else:
```

### Comparing `vbpy-2.2.0/vbpy/load_revenue_auto_file.py` & `vbpy-2.2.1/vbpy/load_revenue_auto_file.py`

 * *Files identical despite different names*

