# Data preprocessing

The original CGED corpora is sourced from the writing section of the HSK (Pinyin of *Hanyu Shuiping Kaoshi*, Test of Chinese Level) (Cui et al, 2011; Zhang et al, 2013). Native Chinese speakers were trained to manually annotate grammatical errors in Chinese sentences written by Chinese as a foreign language (CFL) learners and provide corrections and corresponding error types. The input sentence may contain one or more such errors. 

Such errors are defined as: 
-	Redundant words (R)
-	Missing words (M)
-	Word selection errors (S)
-	Word ordering errors (W). 

The raw data has already been uniformly converted to simplified Chinese characters. Some samples that were removed from the original datasets contain the following problems: (1) too short (less than 7 words); (2) have significant annotation issues; (3) contain only punctuation mistakes, which barely contributes to the grammaticality judgement.  

For each entry in the dataset, we extract sentence pairs and their corresponding list of error types  from the raw data. This process results in a structured list of sentence data with 41,490 sentence pairs, prepared for subsequent model evaluation.
