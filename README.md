# Sentence-Classificaion-Thesis-Codes

**Purpose**

(1) Classify sentences of research paper into various categories using hybrid approach

(2) Comparison of machine learning approaches to a hybrid approach 

(3) Evaluation of previous research, the model, architecture and result to compare with the 
model developed by this research

(4) Evaluation of the neuro-symbolic approach with other hybrid approaches.


**DATA**

SSBJ dataset (df_sentences_with_cite): The corpus of scientific articles based on information system which 
comprises of 7,304 scientific articles from the senior scholars' basket of journals, published 
between 1989 and September 2021 (Assiciation for Information Systems, 2021)

test_data: The test dataset is derived from a research paper that is found on a variety of internet 
platforms that provide free access to scholarly literature. The data for this study was extracted 
from ArXiv.

Cue Phrases dataset: the cue phrases that corresponds to the specific category. The cue phrases were taken from the 
website's Academic phrase library (REF-N-WRITE), which contains 20,000 academic phrase 
templates. 

keyword_vocab: Contains keywords and the specific class it belongs to. The keywords is selected based on domain 
knowledge, the Academic phrase bank of the website (REF-N-WRITE) that provides 20,000 
academic phrase templates and other research paper selected from ArXiv.

(RB) rule_train_data: training data including the output from rule based function

(RB) rule_test_data: testing data including the output from rule based function

(NRB) preprocessed_train:  training data without the output from rule based function

(NRB) preprocessed_test:  testing data without the output from rule based function



**Data Labelling and Augmentation**

annotation.ipynb: The notebook includes the creation of rule-based fuction which is used to annonate the data

Nlpaug.ipynb:  To minimize the chance of misclassification rate, the data was oversampled using 
Nlpaug. Nlpaug is a data augmentation technique to generate additional data using the data in 
hand. 

data_preprocessing.ipynb: The sentences in the dataset which are in the textual form was pre-processed before 
representing the text.  The packages such as ‘re’ and ‘nltk’ was used to pre-process the texts. 

Rule_test_data.ipynb: Test dataset adding output from rule-based function 

rule_train_data. ipynb: Train dataset adding output from rule-based function


**Baseline Model**

Baseline.ipynb: The non-rulebased dataset (NRB) were train and tested on baseline models

Baseline-rule_based.ipynb: The rulebased dataset (RB) were train and tested on baseline models


**CNN Models**

cnn_yoon_kim.ipynb: Using model by (Kim, 2014) to test on our NRB dataset to find the best embedding technique

cnn_yoon_kim-rulebased: ipynb Using model by (Kim, 2014) to test on our RB dataset to find the best embedding technique

norules_multichanne.ipynb: Multi-channel CNN model on NRB dataset

CNN 1d_norules-main.ipynb: Single-channel CNN model on NRB dataset

neurosymbolic_multichannel.ipynb: Multi-channel CNN model on RB dataset 

CNN 1d_rules-main.ipynb Single-channel:  CNN model on RB dataset



