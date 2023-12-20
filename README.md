# DeepLearning_Assignment

Submitted by -
- Yashwanth S Gowda
* 4NI20IS126
+ VII sem ISE 'B' sec
- Topic - Feed-Forward Networks

## Introduction

Feedforward neural networks, also known as multilayer perceptrons (MLPs), are a type of artificial neural network architecture. In a feedforward network, information flows in one direction—from the input layer through one or more hidden layers to the output layer—without forming cycles or loops. This forward flow of information is where the term "feedforward" originates.

Here are the key components and characteristics of feedforward networks:

Layers:-

-Input Layer: The first layer of the network, where the input data is introduced.
-Hidden Layers: Intermediate layers between the input and output layers. Each layer consists of nodes (neurons), and the term "hidden" refers to the fact that these layers do not directly interact with the external environment or provide the final output.
-Output Layer: The final layer that produces the network's output.

1. Neurons (Nodes):-
Each node in the network is a computational unit that processes information.
Nodes in the input layer represent features of the input data.
Nodes in hidden layers perform computations based on weighted inputs from the previous layer and apply activation functions.
Nodes in the output layer produce the final output of the network.

2. Connections (Weights):-
Each connection between nodes is associated with a weight, representing the strength of the connection.
Weights are adjusted during the training process to enable the network to learn from data.

3. Activation Functions:-
Neurons in the hidden layers typically apply activation functions to introduce non-linearities into the network, enabling it to learn complex relationships in the data.
Common activation functions include sigmoid, hyperbolic tangent (tanh), and rectified linear unit (ReLU).

4. Training:-
Feedforward networks are trained using supervised learning, where they learn to map input data to desired output labels.
During training, the network adjusts its weights through backpropagation, minimizing the difference between predicted and actual outputs (loss or error).

Feedforward networks are versatile and have been successfully applied to various tasks, including pattern recognition, image classification, natural language processing, and regression problems. While they lack feedback loops and dynamic memory, which are present in recurrent neural networks, their simplicity and effectiveness make them a fundamental building block in the field of artificial neural networks.

## This Repository

Its an example on how to implement Feedforward Neural networks with Keras and Tensorflow on MNIST dataset. Everything about dataset, model and its working is mentioned in the comments. We are intending to create a model that can predict the number on the handwritten image. The activation function used here is ReLU. After training the model the evaluation of this came out about 95.2% which is pretty good. 

## Saving and using the model

keras_model_path='C:\\Users\\admin'
model.save(keras_model_path)

restored_keras_model = tf.keras.models.load_model(keras_model_path)
