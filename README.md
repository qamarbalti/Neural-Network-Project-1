Contents
Problem 1........................................................................................................................................ 2
Problem 2........................................................................................................................................ 2
a. .................................................................................................................................................. 2
b................................................................................................................................................... 4
Problem 3........................................................................................................................................ 4
Problem 4........................................................................................................................................ 5
a. .................................................................................................................................................. 5
b................................................................................................................................................... 5
Problem 5........................................................................................................................................ 6
Iran University of Science & Technology
School of Computer Engineering 
Neural Networks, Assignment #1
Page 2 of 6
Problem 1
As presented in the classroom material where we've explored logic functions such as AND and 
OR, let's now delve into the NOR logic function using the following data.
Consider the NOR logic function described in the following table:
X1 X2 Y
0 0 1
0 1 0
1 0 0
1 1 0
Attempt to design a single artificial neuron that uses a threshold of -0.5 to solve the NOR logic 
function. Utilize the neuron's weight values in conjunction with the specified threshold to achieve 
correct predictions.
(10 points)
Problem 2
a.
Your challenge involves constructing an ADALINE1
capable of precisely solving the OR logic 
function. In the context of this task, the learning rate is specified as 0.1 and a bias of 1 is established
and also the initial weights are: b=0.2, w1=0.3, w2=0.1
Your primary goal is to lay out, in comprehensive detail, the sequential steps necessary to craft an 
ADALINE neuron that effectively learns, refines its weights, and reliably predicts the behavior of 
the OR logic function. Emphasize the iterative nature of the training process across a span of three
steps. Calculate the weights considering following activation functions.
1- Step function (hard limiter)
𝑜𝑢𝑡 = {
1 𝑖𝑓 𝑦 >= 0
−1 𝑖𝑓 𝑦 <= 0
1 Adaptive Linear Neuron
Neural Networks, Assignment #1
Page 3 of 6
2- ReLU 
 𝑜𝑢𝑡 = max (0, 𝑥)
3- Sigmoid
𝑜𝑢𝑡 =
1
1 + 𝑒
−𝑥
Calculate Gradient Decent and Stochastic Gradient Decent for section 1. Explain and compare the 
two methods (SGD and GD). Write down your calculations.
X1 X2 Y
0 0 0
0 1 1
1 0 1
1 1 1
(20 points)
Neural Networks, Assignment #1
Page 4 of 6
b.
Refer to Problem2.ipynb in the assignment folder. Complete parts A and B to implement an 
Adaline and Madaline for classifying mentioned dataset. Explain and compare the results.
(20 points)
Problem 3
Consider the following MLP. Calculate the forward pass and backpropagation in this MLP.
• All calculations should be written for two epochs.
(20 points)
𝑯𝟏
𝑯𝟐
𝑶𝟏
𝑿𝟏=1
𝑿𝟐=0
𝑿𝟑=1
𝜽 = −𝟎. 𝟒
𝜽 = 𝟎. 𝟐
𝜽 = 𝟎. 𝟏
Y = 1
Neural Networks, Assignment #1
Page 5 of 6
Problem 4
a.
Implement a Multi-Layer Perceptron (MLP) neural network from scratch based on the following 
structure. Train and test the MLP using the MNIST dataset.
• Input layer:
o Number of Neurons: 784 (28*28) 
• Hidden layer:
o Number of Neurons: 800
o Activation Function: Sigmoid
• Output layer:
o Number of Neurons: 10
o Activation Function: Softmax
(15 points)
b.
Design and implement a Dynamic Multi-Layer Perceptron (MLP) neural network from scratch. 
Keep in mind that your design must take inputs such as the number of layers, the number of 
neurons in each layer, the activation function, the number of epochs and input samples. Then, train 
the network on some data and finally test it.
Notice: Your MLP will be tested using random data by the TA.
(20 points)
Neural Networks, Assignment #1
Page 6 of 6
Problem 5
Discuss the potential issue (overfitting or underfitting) in the following scenarios and propose 
solutions for each one of them.
• Your team is working on a financial fraud detection system using machine learning. 
The model seems to have poor detection performance on new transactions.
• In the field of natural language processing, your text summarization model produces 
summaries that are overly generic and fail to capture important details from the source 
text.
• You are developing a deep learning model for image denoising, aiming to remove noise 
from medical X-ray images. While the model performs exceptionally well on the 
training dataset, it fails to generalize to new X-ray images from different hospitals and 
machines.
(15 points
