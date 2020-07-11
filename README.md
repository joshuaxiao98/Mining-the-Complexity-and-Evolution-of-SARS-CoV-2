# Mining-the-Complexity-and-Evolution-of-SARS-CoV-2

1. Important_functions.ipynb contains the code for all the functions needed to calculate transition probability matrix, entropy rate, fractal dimension and processing of the sequence files acquired from GISAID.

2. For Clade Analysis, please use the file ‘Clade_Analysis/nextstrain_ncov_global_metadata_June.csv’ to acquire 20A, 20B, 19A, 19B, 20C clade samples from GISAID and store them in the folder Clade_Analysis as 20A.fasta, 20B.fasta, 19A.fasta, 19B.fasta, 20C.fasta. These files can be generated using the code ‘file_generate_clade.ipynb’. 
The code for 	
(i) pairwise classifier of Clades is Clade_Classification.ipynb
(ii) multiclassification of Clades is Clade_Analysis_multiclassification.ipynb
(iii) region based mutation detection is mutation_detection_region.ipynb

3. All the GISAID samples listed in other csv files (that read as gisaid*.csv) were used to analyze the evolution trends for different clades shown in Figure 5.

4. Samples listed in files – 
- USA/gisaid_hcov19_acknowledgement_table_2020_05_11_15_USA.csv and 
- Europe/gisaid_hcov-19_acknowledgement_table_2020_05_12_19_Europe.csv 
are used to generate variability plots for USA and Europe respectively. The code for computing the variable transitions is Variability.ipynb
Note that for this analysis, you will need to create two folders with name USA and Europe respectively. Inside each of these folders, you will need to store sequences for each day in files labeled as ‘2020-mm-dd.fasta’ which will store sequences for the respective day. The python code file_generate_date.ipynb can be used to achieve that.
