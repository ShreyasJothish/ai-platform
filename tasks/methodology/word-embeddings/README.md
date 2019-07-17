# Word Embeddings using Word2Vec.

### Procedure

1) I shall be working with [Fake News data](https://www.kaggle.com/mrisdal/fake-news)
from Kaggle as an example for Word Embedding.
This data set has sufficient data containing documents to train the model on.

2) Clean/Tokenize the documents in the data set.

3) Vectorize the model using Word2Vec and explore the results like finding most similar
words and finding similarity.

[gensim](https://radimrehurek.com/gensim/) package is used for Word2Vec functionality.

### Running Locally

python tasks/methodology/word-embeddings/word_embeddings.py **word1** **word2** **topn**

where:
word1 - First word used to find similar words within the documents.
word2 - Second word used to find similar words within the documents.
Note : word1 is also compared with word2 to find similarity between them.
topn - Number of similar words to be listed.

Example:
python tasks/methodology/word-embeddings/word_embeddings.py trump mayor 10

### Output
ML Flow shall be used to log input parameters.
* word1
* word2
* topn

ML Flow shall be used to record similar words as tags.
* word1_most_similar
* word2_most_similar

ML Flow shall be used to log metrics.
* vocabulary_size
* similarity_score between word1 and word2


