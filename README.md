# Quora_QA
Fine tuning and evaluating models for Question Answer Task based on Quora QA dataset.

Libraries used: 
1. Numpy
2. Pandas
3. tensorflow
4. nltk
5. sklearn
6. torch
7. transformers
8. MatPlotLib

Data Cleaning: 
1. Null values removal
2. Duplicate rows removal
3. Stop word removal
4. Punctuation removal
5. Abbreviation expansion

Stemming, Lemmitization provided as options within the preprocess_text() function. 

Train-test split used from sklearn. 80-20 split.

Tokenisation through custom tokens for individual models to avoid loss of information

Models used - BERT, T5, GPT2

Trained on a subset of train split for faster processing
Tested on a small subset of test split for faster processing

Evaluation Metrics - ROUGE, BLEU, F1

Scores: 
ROUGE
  T5 - 'rouge1': 0.0363, 'rouge2': 0.00719, 'rougeL': 0.03323
  BERT - 'rouge1': 0.03531, 'rouge2': 0.0057, 'rougeL': 0.03077
  GPT - 'rouge1': 0.08987, 'rouge2': 0.01239, 'rougeL': 0.07646

BLEU
  T5 - 1.2770167793782132e-80
  BERT - 9.818196498280712e-06
  GPT - 0.0017485099706965135



Suggested Novel Improvements: 
1. Tokenisation: Word based; delimiter: .,!?  ; Sentence based
2. Emoji removal
3. Translate non-Latin script languages and non-English languages into English - Latin script
4. Obtaining context from wider sources to enable fact checking and BERT.
5. Increasing the dataset used for training and use of more extensive computing resources
   





