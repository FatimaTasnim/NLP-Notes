Stemming and lemmatization are very two very popular ideas that are used to reduce the vocabulary size of corpus.
## Lemmatization
Lemmatization is the task of determining that two words have the same root,
despite their surface differences. The words am, are, and is have the shared lemma
be; the words dinner and dinners both have the lemma dinner.


Spacy has Lemmatization but no stemming facility as stemming is not a overall good idea. SpaCy does lemmatization by default when the text is processed as an object. lemma also makes Appels to appels.

Lemmatization is aware of the linguistic role that words play in context. "Meeting" is converted to "meet" because it's a verb. spaCy does expose part of speech tagging and other linguistic features for us to use

