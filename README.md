# Predicting the Emergence of SARS-CoV-2 Clades

1. Important_functions.ipynb contains the code for all the functions needed to calculate transition probability matrix, entropy rate and processing of the sequence files acquired from GISAID.

2. For Figures 3 and 4, please use the file ‘Clade_Analysis/nextstrain_ncov_global_metadata_June.csv’ to acquire 20A, 20B, 19A, 19B, 20C clade samples from GISAID and store them in the folder Clade_Analysis as 20A.fasta, 20B.fasta, 19A.fasta, 19B.fasta, 20C.fasta. These files can be generated using the code ‘file_generate_clade.ipynb’. 
The code for 	
(i) pairwise classifier of Clades is Clade_Classification.ipynb
(ii) multiclassification of Clades is Clade_Analysis_multiclassification.ipynb
(iii) region based mutation detection is mutation_detection_region.ipynb

3. All the GISAID samples (~20000) listed in other csv files (that read as gisaid_hcov-19*.csv) were used to analyze the evolution trends for different clades shown in Figure 5. For a given clade, samples from different months are required to be put in different classes for machine learning classification. The code for the learning based classifier is the same as provided in ML() and build_model() functions in Clade_Classification.ipynb.


