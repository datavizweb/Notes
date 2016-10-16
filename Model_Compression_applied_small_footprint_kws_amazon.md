# Model compression applied to small-footprint keyword spotting

* DNN based keyword spotter
* Baseline is based on KWS by carolin prada, Google
* 
* RNN based is not tried
* Compressing the models
 * Tying weights with random hash functions
 * Quantizing blocks of weights with vector quantization
 * low-rank matrices
* Student-teacher model
 * Train small student model to mimic a large teacher model
 * soft-targets from large model is used
 * READ : Do deep nets really need to be deep ?
 * READ : Distilling the knowledge in a neural network
* Feature extraction, Classification, Posterior Smoothing
* Network Architecture
 * DNN with 4 hidden layer
 * 20 dimensional log-mel filter bank
 * 20 left context and 10 right context
 * 620 dimensional input
 * Frame wise cross entropy criterion
 * Performance based learning rate schedule
  * Halve the learning rate if performance on development set reduces
  * ADADelta, RMSProp
* Reducing the RANK has regularizing effect
 * Mean normalized stochastic gradient for large-scale deep learning
 * Fine tunining the initializatoin from SVD was necessary to achieve strong performance


# Multi-task learning and Weighted Cross-entroy for DNN based keyword spotting

* Improved Training techniques
 * Transfer learning, Multi-task learning, Knowledge Distillation
 * Multilingual Acocustic Models using distributed Deep Neural Networks
* Class weighted cross entropy
 * weight the frames from correct class

# Anchored Speech Detection

* 