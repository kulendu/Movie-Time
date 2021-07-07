This file contains all the ***Neural Network Analysis*** information. 
- `Dataset analysis`: Here the dataset used is the ***IMDB dataset***. The dataset contains 25000 movies reviews from IMDB, labeled by sentiment (*positive/negative*). Reviews have been preprocessed, and each review is encoded as a list of word indexes (integers). For convenience, words are indexed by overall frequency in the dataset, so that for instance the integer "3" encodes the 3rd most frequent word in the data. This allows for quick filtering operations such as: "only consider the top 10,000 most common words, but eliminate the top 20 most common words".

As a convention, "0" does not stand for a specific word, but instead is used to encode any unknown word. [The dataset can be found here](https://ai.stanford.edu/~amaas/data/sentiment/)

- `Building and analysing the neural network`: The neural network used here is a three layered NN. It goes as follows:
	- **First layer (*input layer*)** : Densely connected with the second layer, with input shape(10000, ) and with 16 neurons/units per layer. A	ctivation function used: 'relu' - Re	ctified Linear unit.
	- **Second layer (*hidden layer*)** : Densely connected with the second layer, with input shape(10000, ). Activation function used: 'relu' - 	Rectified Linear unit, with the same 16 units/neurons per layer.
	- **Third layer (*final output layer*)** : This is the final layer with 1 unit (uni-class output or the probabilitic value) and with an activ	ation funciton of 'sigmoid'. 

<p align='center'>
	<img src="https://github.com/kulendu/Movie-Time/blob/master/assets/Neural%20net.png">
</p>

- `Brief on the activation functions` : Activation fucntions are used to introduce non-linearity into our neural-network<br>
- ### SIGMOID FUNCTION 
<p align='center'>
	<img src = 'https://github.com/kulendu/Movie-Time/blob/master/assets/formula.png' height=50px width=350px> <br>
</p>

As the formula suggests the  *sigmoid function* is used to normalize the data into binary constraints, and in our case it is used in the final output layer to normalize the output values between the constraints {0,1}.
<p align='center'>
	<img src='https://github.com/kulendu/Movie-Time/blob/master/assets/1_Xu7B5y9gp0iL5ooBj7LtWw.png' height=250px width=400px>
</p>
<br>

- ### RELU FUNCTION 
<p align='center'>
	<img src = 'https://github.com/kulendu/Movie-Time/blob/master/assets/Annotation%202021-06-01%20235544.png'  height=300px width=400px> <br>
</p>

Also know as Recified Linear Unit (ReLU). This function basically satisfies the condition : `if num > 0 = positive , and if num <= 0 = 0`. This best fits in our scenario as we want our network to not train on any -ve values and this is the best fit.
<br>

Here's a clear difference between the two activation functions.
<p align='center'>
	<img src = 'https://github.com/kulendu/Movie-Time/blob/master/assets/1_XxxiA0jJvPrHEJHD4z893g.png'> <br>
</p>

- `Analysing the evaluation` :

![](https://github.com/kulendu/Movie-Time/blob/master/assets/acc-VS-loss.png)
![](https://github.com/kulendu/Movie-Time/blob/master/assets/accurcay-VS-val_acc.png)
![](https://github.com/kulendu/Movie-Time/blob/master/assets/loss-VS-val_loss.png)
