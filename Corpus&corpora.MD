# NATURAL LANGUAGE PROCESSING
## CORPUS
corpus is a collection of written or spoken natural language to find out how a language works.

## CORPORA 
When there is more than one corpus it's called corpora.

There are 2 types of corpus

- Text Data: written materials
- Speech Data: spoken material

## CORPUS ANALYSIS
Most NLP task needs some basic corpus analysis to understand the corpus well. **nltk** provides some inbuilt corpus.

## nltk CORPORA
nltk has 4 types of corpora
- Isolate Corpus: collection of text. Example: gutenberg, webtext.

- Categorized Corpus; collection of text that are grouped into different types of categories. Ex: **Brown** corpus. (categories: news, hobbies.....)

- Overlapping Corpus: Collection of texts which are categorized and categories can overlap with each other. Ex: reuters corpus.

- Temporal Corpus: This type of corpus is a collection of the usages of natural language over a period of time. EX: inaugural address corpus.

## nltk API
The Python code has basic commands of how to access corpus using the nltk API. 

![API Attributes](/NLP-images/API-attributes.png)

## Types of data attributes
- categorical = ordinal & nominal
- Numeric: Continous & discrete

## CORPORA FORMATES
usual data formats such as txt, csv, tsv, xml, json and LibSVM

### LibSVM: 
 allows for sparse training data. The non-zero values are the only ones that are included in the training dataset. Hence, the index specifies the column of the instance data (feature index). To convert from a conventional dataset, just iterate over the data, and if the value of X(i,j) is non-zero, print j + 1: X(i,j).

## PREPROCESSING THE DATASET
- **Formating:** switch to comfortable data formet.
- **Cleaning:** Clean the data for missing valus.
- **Sampling:** one can figure out which of the available data attributes our present dataset has and which of the data attributes can be derived by us. We are also trying to figure out what the most important data attributes are as per our application. 
- **Trandsforming Data:** Feature engineering techniques that help to convert the text data into numeric data so the machine can understand the dataset and try to find out the pattern in the dataset. So, this stage is basically a data manipulation stage. In the NLP domain, for the transformation stage,  some encoding and vectorization techniques can be used. 

