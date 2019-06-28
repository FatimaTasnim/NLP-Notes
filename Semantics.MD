# Semantics
An utterance or text in the form of a series of sentences. So, the meaning of a text is called its semantics.

## Distributional semantics
 Quantify and categorize semantic similarities between linguistic items based on their distributional properties in large samples of text data.
 - Latent Semantic Analysis
 - Word2Vec

## word2vec
word2vec is a representation of words in a vector where the words are placed in a specific manner so that it can give the word a meaningful value.
- What is the Specific Manner?
    - There is a very famous quote by a famous linguist John Firth to understand the concept of it-
    "You shall know the word by the company it keeps."

word2vec  converts each word to some vector in some sophisticated space, which usually have several hundred dimensions. To learn the word embedding, Word2vec uses nearby words. Basically, different words, which often are used in the same context, will be very close in these vectoring representation, which, of course, will benefit our models. Furthermore, there are some prominent examples showing that we can apply basic operations like addition and subtraction on these vectors and expect results of such operations to be interpretable. example: if we do [(king - man) + woman] result will be queen

So, to vectorize the word we need to know the other words that are associate with the target word and their distribution. 


The distributional representation of a word is a vector form in which the word can be represented. Words are expressed in the form of a dense vector, and the dense vector has to be chosen so that it will be good at predicting other words that appear in the context of this word. Now, each of those other words that we are making predictions about also have other words attached to them, so we use a similarity measure, such as the vector dot product. This is a kind of recursive approach, where each word will predict the other words that can appear in the same context, and other predicted words also perform the same operation by predicting some other words. So, we need a clever algorithm to perform this kind of recursive operation & the major point here is to generate the vector for a word that also carries the significance of similarity measure so that you can understand the contextual meaning of the word. 

### Usage of Word2Vec
- sentiment analysis: word2vec gives an idea about how words are spread across the dataset, and then       parameters can be customized such as context window size, subsampling, and so on. At first generate      bag of words (BOW) and then start to train word2vec on that BOW and generate word vectors. These         vectors can be fed as input features for the ML algorithm, then generate sentiment analysis output.

- Document classification. word2vec implementation gives you more good results, as it preserves semantic   similarity.



