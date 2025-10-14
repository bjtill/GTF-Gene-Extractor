# GTF-Gene-Extractor
A tool to generate a BED file containing the chromosome, beginning and ending coordinates of a gene, given a list of genes and a genome annotation GTF file.  
_____________________________________________________________________________________________________________________________________________________________

Use at your own risk. I cannot provide support. All information obtained/inferred with this code is without any implied warranty of fitness for any purpose or use whatsoever.

ABOUT: 

This program generates a downloadable BED file for a list of genes based on information within a genome annotation GTF file.  The program searches for gene names in a case-insensitive manner, but having an exact match.  For example if the gene actin is provided, it will generate a bed file for actin or ACTIN, but not actin-like.  The input gene list should contain one gene per line.  The program will report the smallest and largest nucleotide positions within the GTF file that are associated with the name.  Names that are not found in the GTF file are reported in a downloadable log file.  

RATIONAL: 

Extracting genomic coordinates from a genome build has potentially many uses. While relatively simple to achieve, this web-tool automates the process, supports evaluation of many genes, and provides information on genes not discovered.  The tool was originally built for in-house whole genome sequence analysis pipelines and as an input to the BLAST-based Genome coordinate Converter (a cross-genome all-purpose tool similar to liftover). A link to this converter will be added shortly. 

SCREENSHOTS:  

Input files

<img width="936" height="843" alt="Screenshot from 2025-10-14 14-29-28" src="https://github.com/user-attachments/assets/4b06e0cf-bd5a-4521-b5e2-9d264e293707" />

Green check marks and file names appear when files have been selected

<img width="989" height="873" alt="Screenshot from 2025-10-14 14-39-39" src="https://github.com/user-attachments/assets/84128929-7f14-455d-9caf-b505bf635315" />

When finished, the program creates a log of how many genes were found, a list of any genes not found and the coordinates of genes found. The log file and associated BED file of found genes can be downloaded. 

<img width="1056" height="653" alt="Screenshot from 2025-10-09 15-29-04" src="https://github.com/user-attachments/assets/36ed17bd-147e-4917-92bc-0a1218f2bbab" />
