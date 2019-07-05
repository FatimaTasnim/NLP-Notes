# Text to Numbers
## Bag of Words
If there is a bunch of documents then if we consider each of the document as a bag then count the frequency of each word in a bag and assign each word an unique id. So, this unique words are vocabulary with frequency information. Here, this words are feature.

Scikit learn - CountVectorizer creates feature vector. 

### Term Frequency
 This frequency can help us to classify them. But long Docs can influence the solutions. So, a solution of this problem is to divide the frequency with total word count of the doc. This is called TF.
### Inverse Document Frequency (IDF)
 Inverse document frequency is a measure of whether the term is common or rare in all documents.

 We multiply TF with IDF to get our TF-IDF metric, which is always greater than zero. 



