This file contains all the ***Neural Network Analysis*** information. 
- `Dataset analysis`: Here the dataset used is the ***IMDB dataset***. The dataset contains 25000 movies reviews from IMDB, labeled by sentiment (*positive/negative*). Reviews have been preprocessed, and each review is encoded as a list of word indexes (integers). For convenience, words are indexed by overall frequency in the dataset, so that for instance the integer "3" encodes the 3rd most frequent word in the data. This allows for quick filtering operations such as: "only consider the top 10,000 most common words, but eliminate the top 20 most common words".

As a convention, "0" does not stand for a specific word, but instead is used to encode any unknown word. [The dataset can be found here](https://ai.stanford.edu/~amaas/data/sentiment/)

- `Building and analysing the ***neural network***`: 
