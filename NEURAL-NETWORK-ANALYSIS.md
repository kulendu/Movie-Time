This file contains all the ***Neural Network Analysis*** information. 
- `Dataset analysis`: Here the dataset used is the ***IMDB dataset***. The dataset contains 25000 movies reviews from IMDB, labeled by sentiment (*positive/negative*). Reviews have been preprocessed, and each review is encoded as a list of word indexes (integers). For convenience, words are indexed by overall frequency in the dataset, so that for instance the integer "3" encodes the 3rd most frequent word in the data. This allows for quick filtering operations such as: "only consider the top 10,000 most common words, but eliminate the top 20 most common words".

As a convention, "0" does not stand for a specific word, but instead is used to encode any unknown word. [The dataset can be found here](https://ai.stanford.edu/~amaas/data/sentiment/)

- `Building and analysing the neural network`: The neural network used here is a three layered NN. It goes as follows:
	- First layer (*input layer*) : Densely connected with the second layer, with input shape(10000, ) and with 16 neurons/units per layer. A	ctivation function used: 'relu' - Re	ctified Linear unit.
	- Second layer (*hidden layer*) : Densely connected with the second layer, with input shape(10000, ). Activation function used: 'relu' - 	Rectified Linear unit, with the same 16 units/neurons per layer.
	- Third layer (*final output layer)* : This is the final layer with 1 unit (uni-class output or the probabilitic value) and with an activ	ation funciton of 'sigmoid'. 

	<img src="https://github.com/kulendu/Movie-Time/blob/master/assets/Neural%20net.png">

- `Brief on the activation functions` : 
![](https://github.com/kulendu/Movie-Time/blob/master/assets/1_Xu7B5y9gp0iL5ooBj7LtWw.png)
### SIGMOID FUNCTION 
This formula for *Sigmoid function* is : ![]()
