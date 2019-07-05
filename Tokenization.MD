- Split by whitespace
- Alphanumeric extraction

## SpaCy for tokenization
Download in terminal 
```cmd
python -m spacy download en
```

Using SpaCy 

```Python
import spacy
nlp = spacy.load('en')
doc = nlp(text) # spacy object -> doc. stores precalculated languistic features including tokens.
```

## Sentence Tokenization
SpaCy can also extract a sentence instrad of word.

## Stop Word Removal
at first need to convert our text in toSmall format and then pass it to spacy. spacy has prebuilt is_stop token to find out stopping words. We can also add custom words as stopword
```Python
domain_stop_words = ["NLP", "Processing", "AGI"]
for word in domain_stop_words:
   STOP_WORDS.add(word)
```