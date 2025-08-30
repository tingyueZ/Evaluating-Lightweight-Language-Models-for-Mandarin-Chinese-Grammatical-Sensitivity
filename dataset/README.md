# Data preprocessing

We conduct our experiments using a cleaned and reformatted version of the Chinese Grammatical Error Diagnosis (CGED) corpus, originally released as part of the NLP-TEA shared tasks (Rao et al., 2020). The original CGED corpora were sourced from the writing section of the HSK (Pinyin of Hanyu Shuiping Kaoshi, Test of Chinese Level) (Cui et al, 2011; Zhang et al, 2013). The CGED dataset consists of sentences written by learners of Chinese as a foreign language (CFL), manually annotated by native speakers to mark grammatical errors, their types, and corresponding corrections. 
The file is provided in JSONL (JSON Lines) format, where each line is a valid JSON object that contains the three items:
 
- text: the original sentence potentially containing one or more grammatical errors;
- correct: the corrected version of the sentence, provided by human annotators;
- error: a list of error annotations, specifying the type and location of errors in the original sentence. The annotated error types include: R (Redundant words), M (Missing words), S (Selection errors) and W (Word ordering errors).

All sentences are in simplified Chinese, and the dataset has been preprocessed to exclude samples with low utility that might contain the following problems: (1) sentences shorter than 7 words; (2) significant annotation problems; (3) errors consisting solely of punctuation, which contribute little to grammaticality judgment.
