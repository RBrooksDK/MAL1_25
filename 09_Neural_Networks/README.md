<h1 align="center">09 Introduction to Neural Networks</h1>

## Preparation

Ch 10 + 11 until (but not including) “Batch Normalization” (pp. 357 – 367). Feel free to ignore the mathematical definitions of the activation functions.

For background and as reference: Ch 12

**Optional:** Look at the [3Blue1Brown videos](#video-lectures) on neural networks. They are not required, but they are a good introduction to the topic and will help you understand the material better. The videos are very well made and provide a great overview of the concepts.


## Material

Session material: In this folder

You will need to install tensorflow and (optionally) tensorboard before this lesson. Specifically, you need tensorflow 2.0 or higher to be able to use all the functionalities in the notebooks. If you don't know whether you have these packages installed, you can open an anaconda prompt and type

```
pip freeze
```

to see which packages you have and which versions.  
You can run the following commands in the anaconda prompt to get the necessary packages:

```
pip install tensorflow  
pip install tensorboard
```
(If you have an older version of tensorflow, you can upgrade with ```pip install tensorflow --upgrade```).

In addition to this, Tensorflow 2 requires you to install this visual studio package: [https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) (if you don't have windows or would like to read more, you can do so here: [https://www.tensorflow.org/install/pip](https://www.tensorflow.org/install/pip)).

## Session Description

This lecture covers the fundamental aspects of neural networks. 

### Key Concepts

 - Artificial Neurons
 - Perceptrons
 - Network Structure
 - Activation Functions
 - Learning Rate
 - Loss Functions
 - Softmax Output

### Learning Objectives

- Explain what is meant by artificial neurons, and how these are linked to form artificial neural networks.
- Explain what a perceptron is, and how it transforms an input vector to an output, including the importance of weights and biases.
- Discuss how to structure a neural network.
- Discuss and summarize the method of (stochastic) gradient descent and how it is used to train a neural network, including how the learning rate influences results.
- Reflect upon the problems caused by using (a) perceptrons as artificial neurons and (b) the accuracy as the metric to optimize during model training, including how these problems can be solved using activation and loss functions, respectively.
- Sketch different activation functions, including the sigmoid, tanh and ReLU functions, and discuss why the softmax activation function is generally used in the output layer.
- Implement a neural network in python using the tensorflow.keras module.

## Video Lectures

[Playlist with all videos (Opens in Youtube) - 3Blue1Brown: Neural networks](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi)

### 9.1. Neural Networks - What is a neural network? (Part 1)
<iframe width="560" height="315" src="https://www.youtube.com/embed/aircAruvnKk?si=k_P1xbReKdeh6v9M" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### 9.2. Neural Networks - Gradient descent, how neural networks learn (Part 2)
<iframe width="560" height="315" src="https://www.youtube.com/embed/IHZwWFHWa-w?si=Yd4qweAf7L3cl3s7" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### 9.3. Neural Networks - Backpropagation (Part 3)
<iframe width="560" height="315" src="https://www.youtube.com/embed/Ilg3gGewQ5U?si=WF0H06Lx-NgxPp5t" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### 9.4. Neural Networks - Backpropagation calculus (Part 4)
<iframe width="560" height="315" src="https://www.youtube.com/embed/tIeHLnjs5U8?si=qTNoLk8xDWC9dTZ6" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### 9.5. Neural Networks - Large Language Models (Part 5)
<iframe width="560" height="315" src="https://www.youtube.com/embed/LPZh9BOjkQs?si=mbVSd1LUVc04Dflj" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### 9.6. Neural Networks - Transformers (Part 6)
<iframe width="560" height="315" src="https://www.youtube.com/embed/wjZofJX0v4M?si=coI9wXPv3qGfjc2c" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### 9.7. Neural Networks - Attention in transformers (Part 7)
<iframe width="560" height="315" src="https://www.youtube.com/embed/eMlx5fFNoYc?si=Z2NMLrtQUkK4P7Z6" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### 9.8. Neural Networks - How might LLMs store facts (Part 8)
<iframe width="560" height="315" src="https://www.youtube.com/embed/9-Jl0dxWQs8?si=dfKYPfmmOEYCXZnD" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>