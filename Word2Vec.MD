## BUILDING Word2Vec
### VOCABULARY BUILDING STAGE TECHNIQUES
- Optimization Technique
- Loosy Counting
### LOOSY COUNTING
The lossy count algorithm is used to identify elements in a dataset whose frequency count exceeds a user-given threshold. It's useful for large corpus when rarely used words can be kept out of consideration to narrow down the vocabulary size to speedup the execution time.
- Input:  data streams 
- Periodically removes very low-count elements from the frequency table
- Threshold: User's choice

## CONTEXT BUILDING STAGE TECHNIQUES
- Dynamic Window Scaling
- Subsampling
- Pruning

### DYNAMIC WINDOW SCALING
In this technique the words that are near to the target word are more important than the distant words. Here, uniform weight are assigned to the nearby words of the target word. 
#### Assigning Weight to Nearby Words
A window size K will be chosen in between 0 to L (length)
then the nearest word will be assigned with a weight of k/k
then the 2nd nearest word will be assigned as k-1/k.........
the kth nearest word will be assigned as 1/k

### SUBSAMPLING
Subsampling is the method that removes the most frequent words. This technique is very useful for removing stop words. These techniques also remove words randomly, and these randomly chosen words occur in the corpus more frequently. So, words that are removed are more frequent than some threshold t with a probability of p, where f marks the words corpus frequency and we use t = 10−5 in our experiments. Refer to the following equation 
 ```
 P = 1 - sqrt(1/f)
```

### PRUNING
Pruning is also used when we are building word pairs for training purposes using context builder. Size of the total vocabulary can be restricted by using the max_vocab_size parameter given in the Python gensim library.

## EXTENSION of THE word2vec CONCEPT
The word2vec concept can be extended to different levels of text. Here are the following extended concepts built by using the word2vec concept:

- Para2vec
- Doc2vec
- gloVe

### Para2Vec
Para2vec stands for paragraph vector. The paragraph vector is an unsupervised algorithm that uses fixed-length feature representation. It derives this feature representation from variable-length pieces of texts such as sentences, paragraphs, and documents.

### Doc2vec
 is an extension of word2vec. It learns to correlate document labels and words, rather than words with other words. Here, you need document tags. You are able to represent an entire sentence using a fixed-length vector. 

### GloVe
GloVe stands for global vector. GloVe is an unsupervised learning algorithm. This algorithm generates vector representations for words. Here, training is performed by using an aggregated global word-word co-occurrence matrix and other statistics from a corpus, and the resulting representations give you interesting linear substructures of the word vector space. So the co-occurrence matrix is the input of GloVe.

GloVe uses cosine similarity or the Euclidean distance to get an idea of similar words. Glove gives you fresh aspects and proves that if you take the nearest neighbor, then you can see such kinds of words that are very rare in terms of their frequent usage. 