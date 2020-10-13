# SRPC-2020
Code for Student Research Paper Competition 2020.

### Clustering of English texts on the basis of extraction of key properties

To ran the code, you need to download the corresponding jupyter notebook "REALEC_clustering.ipynb" and unzip the dataset "REALEC_cleaned.zip" in the same directory.

Next, you need to set the parameters that will be used in the work in a string format:

1. data_type - the data we want to analyze, can be set to:
* 'unknown_data' - the unlabeled data to which you should set path to folder with essay
(example: folder = "datasets/REALEC_clean/exam/Exam2018")
* 'test_graph' - labeled data which is used to draw the representations of graph descriptions from Exam2017 for test results
* 'test_essay' - labeled data which is used to draw the representations of opinion essays from Exam2017 for test results

2. method - method for receiving embeddings, can take the following values:
* 'tf-idf' - sklearn TF-IDF method
* 'bm25' - weighted TD-IDF
* 'dm' - 'dm' realization of doc2vec PV
* 'dbow' - 'dbow' realization of doc2vec PV

After analysis of values of internal measures, you should set the optimal number of clusters ('best_k' - by default set to 4) that will be used for all subsequent clustering algorithms and for keywords extraction for the corresponding groups.

Dataset REALEC: https://yadi.sk/d/AVFzedaVtSporg 
