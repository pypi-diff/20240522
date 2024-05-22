# Comparing `tmp/gene4mvcf-1.1.3.tar.gz` & `tmp/gene4mvcf-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene4mvcf-1.1.3.tar", last modified: Mon May 20 15:12:42 2024, max compression
+gzip compressed data, was "gene4mvcf-1.1.4.tar", last modified: Wed May 22 16:28:20 2024, max compression
```

## Comparing `gene4mvcf-1.1.3.tar` & `gene4mvcf-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 15:12:42.759353 gene4mvcf-1.1.3/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2417 2024-05-20 15:12:42.759353 gene4mvcf-1.1.3/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1967 2024-05-20 12:34:41.000000 gene4mvcf-1.1.3/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 15:12:42.755353 gene4mvcf-1.1.3/gene4mVCF/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:07:18.000000 gene4mvcf-1.1.3/gene4mVCF/__init__.py
--rwxrwxr-x   0 ws2024    (1000) ws2024    (1000)     5149 2024-05-20 15:04:08.000000 gene4mvcf-1.1.3/gene4mVCF/fetchgenes.py
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 15:12:42.759353 gene4mvcf-1.1.3/gene4mVCF.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2417 2024-05-20 15:12:42.000000 gene4mvcf-1.1.3/gene4mVCF.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      264 2024-05-20 15:12:42.000000 gene4mvcf-1.1.3/gene4mVCF.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 15:12:42.000000 gene4mvcf-1.1.3/gene4mVCF.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       56 2024-05-20 15:12:42.000000 gene4mvcf-1.1.3/gene4mVCF.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       78 2024-05-20 15:12:42.000000 gene4mvcf-1.1.3/gene4mVCF.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-05-20 15:12:42.000000 gene4mvcf-1.1.3/gene4mVCF.egg-info/top_level.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-20 15:12:42.759353 gene4mvcf-1.1.3/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1343 2024-05-20 15:12:23.000000 gene4mvcf-1.1.3/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-22 16:28:20.568721 gene4mvcf-1.1.4/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2798 2024-05-22 16:28:20.568721 gene4mvcf-1.1.4/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     2348 2024-05-22 16:27:06.000000 gene4mvcf-1.1.4/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-22 16:28:20.564721 gene4mvcf-1.1.4/gene4mVCF/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:07:18.000000 gene4mvcf-1.1.4/gene4mVCF/__init__.py
+-rwxrwxr-x   0 ws2024    (1000) ws2024    (1000)     6323 2024-05-22 16:20:58.000000 gene4mvcf-1.1.4/gene4mVCF/fetchgenes.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-22 16:28:20.568721 gene4mvcf-1.1.4/gene4mVCF.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2798 2024-05-22 16:28:20.000000 gene4mvcf-1.1.4/gene4mVCF.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      264 2024-05-22 16:28:20.000000 gene4mvcf-1.1.4/gene4mVCF.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-22 16:28:20.000000 gene4mvcf-1.1.4/gene4mVCF.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       56 2024-05-22 16:28:20.000000 gene4mvcf-1.1.4/gene4mVCF.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       78 2024-05-22 16:28:20.000000 gene4mvcf-1.1.4/gene4mVCF.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-05-22 16:28:20.000000 gene4mvcf-1.1.4/gene4mVCF.egg-info/top_level.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-22 16:28:20.568721 gene4mvcf-1.1.4/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1343 2024-05-22 16:27:50.000000 gene4mvcf-1.1.4/setup.py
```

### Comparing `gene4mvcf-1.1.3/PKG-INFO` & `gene4mvcf-1.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene4mVCF
-Version: 1.1.3
+Version: 1.1.4
 Summary: Description of your package
 Home-page: https://github.com/VJ-Ulaganathan/gene4mVCF
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Description-Content-Type: text/markdown
 Requires-Dist: pysam>=0.16.0.1
 Requires-Dist: pandas>=1.0.0
@@ -26,37 +26,47 @@
 After installation please download the four required bed files and place inside the folder /gene4mVCF
 <br>'hg19.ensGene.bed' --> https://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/genes/hg19.ensGene.gtf.gz </br>
 <br>'hg19.ncbiRefSeq.bed' --> https://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/genes/hg19.ncbiRefSeq.gtf.gz </br>
 <br>'hg38.ensGene.bed' --> https://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/genes/hg38.ensGene.gtf.gz </br>
 <br>'hg38.ncbiRefSeq.bed'--> https://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/genes/hg38.ncbiRefSeq.gtf.gz </br>
 
 ## Usage
-usage: `$ gene4mVCF [-h] -i INPUT -g GENE`
-
 Extract variant entries for a specific gene or list of genes from a VCF file.
+<br>usage: `$ gene4mVCF [-h] -i INPUT -g GENE [-r REFERENCE]`</br>
+
+Needed arguments:
+ <br>`-i INPUT, --input INPUT, is bgzip compressed VCF file`</br>
+ <br>`-g GENE, --genes GENE, is either a Gene name, Ensembl gene ID, or path to a genelist file with *.txt extension`</br>
 
-optional arguments:
-  -h, --help            show this help message and exit
-  -i INPUT, --input INPUT
-                        Input bgzip compressed VCF file
-  -g GENES, --genes GENES
-                        Gene name, Ensembl gene ID, or path to a gene list file
 
+<br>optional arguments:</br>
+   <br>`-h, --help show this help message and exit`</br>
+   <br>`-r REFERENCE, --ref REFERENCE, is 37 or 38, based on the reference genome used for creating the VCF file`</br>
+  
 ## Examples
 Extract variants for a single gene using gene name:
 `$ gene4mVCF -i input.vcf.gz -g EGFR`
 
 Extract variants for a single using ensembl gene id:
 `$ gene4mVCF -i input.vcf.gz -g ENSG00000168878`
 
 Extract variants for multiple genes listed in a file:
-`$ gene4mVCF -i input.vcf.gz -g genes.txt`
+`$ gene4mVCF -i input.vcf.gz -g acmg-genes.txt`
 
 For more options and details, refer to the help message.
 
+**Example showing extraction of variants of ACTB gene**
+
+<br>input command</br>
+![Example Image](images/input.png)
+
+<br>Output file in the tab-separated format</br>
+![Example Image](images/ACTB.png)
+
+
 ## Support
 For any issues or inquiries, please open an issue on the GitHub repository https://github.com/VJ-Ulaganathan/gene4mVCF
 
 
 ## Installation
 
 Installation via pip:
```

### Comparing `gene4mvcf-1.1.3/README.md` & `gene4mvcf-1.1.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -12,37 +12,47 @@
 After installation please download the four required bed files and place inside the folder /gene4mVCF
 <br>'hg19.ensGene.bed' --> https://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/genes/hg19.ensGene.gtf.gz </br>
 <br>'hg19.ncbiRefSeq.bed' --> https://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/genes/hg19.ncbiRefSeq.gtf.gz </br>
 <br>'hg38.ensGene.bed' --> https://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/genes/hg38.ensGene.gtf.gz </br>
 <br>'hg38.ncbiRefSeq.bed'--> https://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/genes/hg38.ncbiRefSeq.gtf.gz </br>
 
 ## Usage
-usage: `$ gene4mVCF [-h] -i INPUT -g GENE`
-
 Extract variant entries for a specific gene or list of genes from a VCF file.
+<br>usage: `$ gene4mVCF [-h] -i INPUT -g GENE [-r REFERENCE]`</br>
+
+Needed arguments:
+ <br>`-i INPUT, --input INPUT, is bgzip compressed VCF file`</br>
+ <br>`-g GENE, --genes GENE, is either a Gene name, Ensembl gene ID, or path to a genelist file with *.txt extension`</br>
 
-optional arguments:
-  -h, --help            show this help message and exit
-  -i INPUT, --input INPUT
-                        Input bgzip compressed VCF file
-  -g GENES, --genes GENES
-                        Gene name, Ensembl gene ID, or path to a gene list file
 
+<br>optional arguments:</br>
+   <br>`-h, --help show this help message and exit`</br>
+   <br>`-r REFERENCE, --ref REFERENCE, is 37 or 38, based on the reference genome used for creating the VCF file`</br>
+  
 ## Examples
 Extract variants for a single gene using gene name:
 `$ gene4mVCF -i input.vcf.gz -g EGFR`
 
 Extract variants for a single using ensembl gene id:
 `$ gene4mVCF -i input.vcf.gz -g ENSG00000168878`
 
 Extract variants for multiple genes listed in a file:
-`$ gene4mVCF -i input.vcf.gz -g genes.txt`
+`$ gene4mVCF -i input.vcf.gz -g acmg-genes.txt`
 
 For more options and details, refer to the help message.
 
+**Example showing extraction of variants of ACTB gene**
+
+<br>input command</br>
+![Example Image](images/input.png)
+
+<br>Output file in the tab-separated format</br>
+![Example Image](images/ACTB.png)
+
+
 ## Support
 For any issues or inquiries, please open an issue on the GitHub repository https://github.com/VJ-Ulaganathan/gene4mVCF
 
 
 ## Installation
 
 Installation via pip:
```

### Comparing `gene4mvcf-1.1.3/gene4mVCF/fetchgenes.py` & `gene4mvcf-1.1.4/gene4mVCF/fetchgenes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 import argparse
 import subprocess
 import os
 import gzip
 from tqdm import tqdm
 
 def parse_bed_file(gene_identifier, genome_version):
-    if "GRCh38" in genome_version:
+    if genome_version == "hg38" or "GRCh38" in genome_version:
         if gene_identifier.startswith("ENSG"):
             bed_file = "hg38.ensGene.bed"
         else:
             bed_file = "hg38.ncbiRefSeq.bed"
-    elif "GRCh37" in genome_version or "hg19" in genome_version:
+    elif genome_version == "hg19" or "GRCh37" in genome_version:
         if gene_identifier.startswith("ENSG"):
             bed_file = "hg19.ensGene.bed"
         else:
             bed_file = "hg19.ncbiRefSeq.bed"
     else:
         # Default to hg19 if genome version cannot be determined
         if gene_identifier.startswith("ENSG"):
             bed_file = "hg19.ensGene.bed"
         else:
             bed_file = "hg19.ncbiRefSeq.bed"
     
-    #print("Detected genome version:", genome_version)
     print("Selected BED file:", bed_file)  # Add this line for debugging
 
     gene_regions = {}
+    gene_chromosomes = {}
     with open(bed_file, 'r') as file:
-        for line in file:
+        lines = file.readlines()
+        for line in tqdm(lines, desc="Reading BED file"):
             fields = line.strip().split('\t')
             chrom = fields[0].lstrip("chr")
             start = int(fields[1])
             end = int(fields[2])
             gene_name = fields[3]
             feature = fields[7]
 
             if gene_identifier.startswith("ENSG"):
                 if fields[3] == gene_identifier:
                     gene_regions[(chrom, start, end)] = (gene_name, feature)
+                    gene_chromosomes[gene_identifier] = chrom
             else:
                 if fields[3] == gene_identifier:
                     gene_regions[(chrom, start, end)] = (gene_name, feature)
+                    gene_chromosomes[gene_identifier] = chrom
 
     if not gene_regions:
         raise ValueError(f"Gene {gene_identifier} not found in {bed_file}")
-    return gene_regions
+    return gene_regions, gene_chromosomes
 
 def get_reference_genome(vcf_path):
     reference_genome = None
     with gzip.open(vcf_path, 'rt') as file:
         for line in file:
             if line.startswith("##contig="):
                 if "assembly=gnomAD_GRCh38" in line:
                     reference_genome = "GRCh38"
                 elif "assembly=GRCh38" in line:
                     reference_genome = "GRCh38"
                 break
             elif line.startswith("#CHROM"):
-                reference_genome = "GRCh38"  # Default to GRCh37, as genome version could not be determine from the given vcf file
+                reference_genome = "GRCh37"  # Default to GRCh37, as genome version could not be determined from the given vcf file
                 break
                 
     if reference_genome is None:
         # Default to GRCh37 if genome version cannot be determined
         reference_genome = "GRCh37"
         print("Reference genome could not be determined from the VCF file, defaulting to GRCh37")
 
@@ -73,57 +76,75 @@
             return gene_name, feature
     return "", ""
 
 def main():
     parser = argparse.ArgumentParser(description='Extract variant entries for a specific gene or list of genes from a VCF file.')
     parser.add_argument('-i', '--input', required=True, help='Input VCF file')
     parser.add_argument('-g', '--genes', required=True, help='Gene name, Ensembl gene ID, or path to a gene list file')
+    parser.add_argument('-r', '--ref', choices=['37', '38'], help='Reference genome version (optional)')
 
     args = parser.parse_args()
 
-    genome_version = get_reference_genome(args.input)
+    if args.ref:
+        genome_version = "hg19" if args.ref == "37" else "hg38"
+    else:
+        genome_version = get_reference_genome(args.input)
 
     if genome_version:
-        print(f"Reference genome version of the input vcf file: {genome_version}")
+        print(f"Reference genome version: {genome_version}")
 
     if args.genes.endswith('.txt'):
         with open(args.genes, 'r') as gene_list_file:
             gene_list = [line.strip() for line in gene_list_file]
     else:
         gene_list = [args.genes]
 
     gene_regions = {}
-    for gene_identifier in gene_list:
-        gene_regions.update(parse_bed_file(gene_identifier, genome_version))
+    gene_chromosomes = {}
+    for gene_identifier in tqdm(gene_list, desc="Processing genes"):
+        regions, chromosomes = parse_bed_file(gene_identifier, genome_version)
+        gene_regions.update(regions)
+        gene_chromosomes.update(chromosomes)
 
     # Create index file for the input VCF file
     index_file = args.input + ".tbi"
     if not os.path.exists(index_file):
         subprocess.run(["tabix", "-p", "vcf", args.input], check=True)
 
-    output_vcf = f"{os.path.splitext(args.input)[0]}_{'_'.join(gene_list)}.vcf"
+    output_prefix = f"{os.path.splitext(args.input)[0]}_{'_'.join(gene_list)}_{genome_version}"
+    output_vcf = f"{output_prefix}.vcf"
     region = ','.join([f'{chrom}:{start}-{end}' for (chrom, start, end) in gene_regions])
     cmd = f"bcftools view -r {region} -o {output_vcf} {args.input}"
     subprocess.run(cmd, shell=True, check=True)
 
     # Count the number of variants in the output VCF file
     variant_count = sum(1 for line in open(output_vcf) if not line.startswith("#"))
 
-    output_tsv = f"{os.path.splitext(output_vcf)[0]}.tsv"
+    output_tsv = f"{output_prefix}.tsv"
     with open(output_tsv, 'w') as tsv_out:
         tsv_out.write("#CHROM\tPOS\tID\tREF\tALT\tQUAL\tFILTER\tINFO\tGene_Name\tFeature\n")
         with open(output_vcf, 'r') as vcf_in:
-            for line in vcf_in:
+            lines = vcf_in.readlines()
+            for line in tqdm(lines, desc="Processing VCF file"):
                 if not line.startswith("#"):  # Skip header lines
                     fields = line.strip().split('\t')
                     chrom = fields[0]
                     pos = int(fields[1])
                     gene_name, feature = get_gene_info(chrom, pos, gene_regions)
                     tsv_out.write(f"{chrom}\t{pos}\t{fields[2]}\t{fields[3]}\t{fields[4]}\t{fields[5]}\t{fields[6]}\t{fields[7]}\t{gene_name}\t{feature}\n")
 
     os.remove(output_vcf)
 
-    print(f"{variant_count} variants were found in the genes {', '.join(gene_list)} in the given input file.")
+    if variant_count == 0:
+        missing_genes = [gene for gene in gene_list if gene not in gene_regions]
+        if missing_genes:
+            missing_chromosomes = {gene: gene_chromosomes.get(gene, "unknown") for gene in missing_genes}
+            for gene, chrom in missing_chromosomes.items():
+                print(f"Gene {gene} is located in chromosome {chrom}, not found in the input VCF file.")
+        else:
+            print(f"0 variants were found in the genes {', '.join(gene_list)} in the given input file.")
+    else:
+        print(f"{variant_count} variants were found in the genes {', '.join(gene_list)} in the given input file.")
 
 if __name__ == '__main__':
     main()
```

### Comparing `gene4mvcf-1.1.3/gene4mVCF.egg-info/PKG-INFO` & `gene4mvcf-1.1.4/gene4mVCF.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene4mVCF
-Version: 1.1.3
+Version: 1.1.4
 Summary: Description of your package
 Home-page: https://github.com/VJ-Ulaganathan/gene4mVCF
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Description-Content-Type: text/markdown
 Requires-Dist: pysam>=0.16.0.1
 Requires-Dist: pandas>=1.0.0
@@ -26,37 +26,47 @@
 After installation please download the four required bed files and place inside the folder /gene4mVCF
 <br>'hg19.ensGene.bed' --> https://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/genes/hg19.ensGene.gtf.gz </br>
 <br>'hg19.ncbiRefSeq.bed' --> https://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/genes/hg19.ncbiRefSeq.gtf.gz </br>
 <br>'hg38.ensGene.bed' --> https://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/genes/hg38.ensGene.gtf.gz </br>
 <br>'hg38.ncbiRefSeq.bed'--> https://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/genes/hg38.ncbiRefSeq.gtf.gz </br>
 
 ## Usage
-usage: `$ gene4mVCF [-h] -i INPUT -g GENE`
-
 Extract variant entries for a specific gene or list of genes from a VCF file.
+<br>usage: `$ gene4mVCF [-h] -i INPUT -g GENE [-r REFERENCE]`</br>
+
+Needed arguments:
+ <br>`-i INPUT, --input INPUT, is bgzip compressed VCF file`</br>
+ <br>`-g GENE, --genes GENE, is either a Gene name, Ensembl gene ID, or path to a genelist file with *.txt extension`</br>
 
-optional arguments:
-  -h, --help            show this help message and exit
-  -i INPUT, --input INPUT
-                        Input bgzip compressed VCF file
-  -g GENES, --genes GENES
-                        Gene name, Ensembl gene ID, or path to a gene list file
 
+<br>optional arguments:</br>
+   <br>`-h, --help show this help message and exit`</br>
+   <br>`-r REFERENCE, --ref REFERENCE, is 37 or 38, based on the reference genome used for creating the VCF file`</br>
+  
 ## Examples
 Extract variants for a single gene using gene name:
 `$ gene4mVCF -i input.vcf.gz -g EGFR`
 
 Extract variants for a single using ensembl gene id:
 `$ gene4mVCF -i input.vcf.gz -g ENSG00000168878`
 
 Extract variants for multiple genes listed in a file:
-`$ gene4mVCF -i input.vcf.gz -g genes.txt`
+`$ gene4mVCF -i input.vcf.gz -g acmg-genes.txt`
 
 For more options and details, refer to the help message.
 
+**Example showing extraction of variants of ACTB gene**
+
+<br>input command</br>
+![Example Image](images/input.png)
+
+<br>Output file in the tab-separated format</br>
+![Example Image](images/ACTB.png)
+
+
 ## Support
 For any issues or inquiries, please open an issue on the GitHub repository https://github.com/VJ-Ulaganathan/gene4mVCF
 
 
 ## Installation
 
 Installation via pip:
```

### Comparing `gene4mvcf-1.1.3/setup.py` & `gene4mvcf-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Check if all required commands exist
 if not all(command_exists(cmd) for cmd in required_commands):
     raise RuntimeError("Please install the following dependencies: bcftools, bgzip, tabix")
 
 setup(
     name='gene4mVCF',
-    version='1.1.3',
+    version='1.1.4',
     description='Description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN',
     author_email='vijay-kumar.ulaganathan@uni-tuebingen.de',
     url='https://github.com/VJ-Ulaganathan/gene4mVCF',
     packages=find_packages(),
```

