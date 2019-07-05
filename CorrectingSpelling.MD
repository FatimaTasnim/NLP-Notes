Good Read on Correcting Spelling [Peter Norvig's Spell Correct](https://norvig.com/spell-correct.html).

Tow Packages
- FuzzyWuzzy: is easy to use. It gives a simple similarity score between two strings, capped to 100. Higher numbers mean that the words are more similar.
- Jellyfish supports six edit distance functions and four phonetic encoding options that you can use as per your use case.

- **Phonetic Word Encoding**
We can convert a word into a representation of its pronunciation. Of course, this might vary by accents, and by the conversion technique as well.

## Runtime Complexity
O(n^2) where n = number of unique words.

The alternative is to use a standard dictionary and expand the same for your corpus. If the dictionary has m unique words, this process now will be O(m∗n). Assuming that m<< n*m<< n2, this will be much faster than the previous approach
