# Predicting the Emergence of SARS-CoV-2 Clades

1. Important_functions.ipynb contains the code for all the functions needed to calculate transition probability matrix, entropy rate and processing of the sequence files acquired from GISAID.

2. For Figures 3 and 4, please use the file ‘Clade_Analysis/nextstrain_ncov_global_metadata_June.csv’ to acquire 20A, 20B, 19A, 19B, 20C clade samples from GISAID and store them in the folder Clade_Analysis as 20A.fasta, 20B.fasta, 19A.fasta, 19B.fasta, 20C.fasta. These files can be generated using the code ‘file_generate_clade.ipynb’. 
The code for 	
(i) pairwise classifier of Clades is Clade_Classification.ipynb
(ii) multiclassification of Clades is Clade_Analysis_multiclassification.ipynb
(iii) region based mutation detection is mutation_detection_region.ipynb

3. All the GISAID samples (~23000) listed in csv files (that read as gisaid_hcov-19*.csv) were used to analyze the evolution trends for different clades shown in Figure 5. There are two major preprocessing steps needed here:
- First the clade for each of the samples is identified. This can be done either by using the software provided by nextstrain.org (https://github.com/nextstrain/ncov) or the multiclassifier we built in obtaining Figure 3. 
- Second, for a given clade (for example 19A), samples are required to be separated on the basis of months so that they can be put into different classes for machine learning classification within a clade on the basis of months.

After obtaining the separation of classes based on months for each clade, the code for the learning based classifier is the same as the ML() and build_model() functions used in Clade_Classification.ipynb.


