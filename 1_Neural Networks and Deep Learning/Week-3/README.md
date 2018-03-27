## Neural Networks 

### Hidden Layers 

>
![alt text](../images/multipleNN.png "multipleNN")

>
![alt text](../images/recap.png "recap")

### Why tanh activation funciton?
tanh function ranges from -1 to 1, so the mean comes out to be 0. Hence, this centralised the data which help model to learn little bit easier, as compared to mean 0.5 in sigmoid function (ranges from 0 to 1).

<br>
Note : Sigmoid function is used rarely. One exception is, it is used in output layer, as we want output to be either 0 or 1
(Binary classification).

>
![alt text](../images/tanhAF.png "tanhAF")

### Why ReLu function?
As Z increases, it decreases slope, hence slows down the gradient descent. So, we defined ReLu function in which, derivative(slope) is 1 if Z is +ve and derivative is 0, is Z is -ve.

>
![alt text](../images/reluAF.png "reluAF")

**If you dont know what activation function you should use, then go for ReLU ACtivation Function.**

### Activation Functions 
>
![alt text](../images/AFunction.png "AFunction")

### Why non-linear activation function?
If we have neural network consiting of hidden layers, then using linear activation funciton, turns out to be similar to neural network having only one layer. So going deep into hidden layers will be of no use. Hence we use non-linear AF, so that hidden layers play major role in computing output. 

>
![alt text](../images/nlAF.png "nlAF")


### Derivatives of Activation functions
>
![alt text](../images/sigmoid.png "sigmoid ")

>
![alt text](../images/tanh.png "tanh ")

>
![alt text](../images/relu.png "relu ")


### Formulaes used in BackPropogation 
>
![alt text](../images/formulaesBP.png "formulaesBP ")


### Backpropogation intuition

**RECAP**

>
![alt text](../images/recapYahh.png "recapYahh ")


>
![alt text](../images/derivations.png "derivations ")

>
![alt text](../images/summary.png "summary ")


### Why Randomization?
Suppose you have built a neural network. You decide to initialize the weights and biases to be zero. 
<br>
In that case, each neuron in the first hidden layer will perform the same computation. So even after multiple iterations of gradient descent each neuron in the layer will be computing the same thing as other neurons. Therefore, randomization is very important in which we initialize weights to some random numbers, instead of initializing them to zero.




