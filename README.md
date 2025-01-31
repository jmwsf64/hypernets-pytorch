# Hyper Network Introduction

Hyper Networks are Neural Nets where one network (HyperNet) outputs the weights and biases of another network (TargetNet). [This](https://arxiv.org/abs/2306.06955) is a good introduction source/overview of HyperNetworks and their variations. There are methods to reduce the number of weights and biases required in the HyperNet, but this demonstration will use the simplest method of directly providing all weights and biases for the TargetNet.

# Project Overview

This project is intended as a demonstration on how to implement HyperNetworks using PyTorch. The example Hyper Network uses a Deep Neural Network as the HyperNet and a Long Short Term Memory (LSTM) network as the TargetNet. `gen_sin_data.ipynb` demonstrates one way of creating input data sets that relate the inputs to the HyperNet and TargetNet, and will create Sine Waves of varying amplitude and frequency. Amplitude and Frequency will be the inputs to the HyperNet DNN, and the sinusoidal series data will be the input to the TargetNet LSTM.

# Additional Links

If you are completely new to Neural Networks, this is probably not the tutorial for you. That being said, [this](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi) video series on YouTube is a great introduction to Neural Networks.

If you are unfamiliar with LSTMs:
* [This](https://colah.github.io/posts/2015-08-Understanding-LSTMs/) blog post is the defacto blog used as an explanation of LSTM Networks, how they work, and their variations.
* [This](https://www.youtube.com/watch?v=q_HS4s1L8UI) video is a good demonstration of how to prepare time sequenced data and then implementing/training LSTMs in PyTorch.
