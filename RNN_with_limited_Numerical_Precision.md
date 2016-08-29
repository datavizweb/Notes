# [Recurrent Neural Networks With Limited Numerical Precision](https://arxiv.org/pdf/1608.06902v1.pdf)

## Abstract

> Recurrent Neural Networks (RNNs) produce state-of-art performance on many machine learning
tasks but their demand on resources in terms of memory and computational power are often
high. Therefore, there is a great interest in optimizing the computations performed with these
models especially when considering development of specialized low-power hardware for deep
networks. One way of reducing the computational needs is to limit the numerical precision of
the network weights and biases. This has led to different proposed rounding methods which
have been applied so far to only Convolutional Neural Networks and Fully-Connected Networks.
This paper addresses the question of how to best reduce weight precision during training in the
case of RNNs. We present results from the use of different stochastic and deterministic reduced
precision training methods applied to three major RNN types which are then tested on several
datasets. The results show that the weight binarization methods do not work with the RNNs.
However, the stochastic and deterministic ternarization, and pow2-ternarization methods gave
rise to low-precision RNNs that produce similar and even higher accuracy on certain datasets
therefore providing a path towards training more efficient implementations of RNNs in specialized
hardware

##  Conclusion and Outlook
> This paper shows for the first time how low-precision quantization of weights can be performed effectively for
RNNs. We presented 3 existing methods and introduced 1 new method of limiting the numerical precision.
We used the different methods on 3 major RNN types and determined how the limited numerical precision
affects network performance across 4 datasets.
In the language modeling task, the low-precision model surpasses its full-precision baseline by a large
gap (0.133 BPC) on the PTB dataset. We also show that the model will work better if put in a slightly
8
overfitting setting, so that the regularization effect of stochastic quantization will begin to function. In the
speech recognition task, we show that it is not possible to binarize weights of GRUs while maintaining their
functionality. We conjecture that the better performance from ternarization is due to a reduced variance of
the weighted sums (when a near-zero real value is quantized to +1 or -1, this introduces substantial variance),
which could be more harmful in RNNs because the same weight matrices are used over and over again along
the temporal sequence. Furthermore, we show that weight and bias quantization methods using ternarization,
pow2-ternarization, and exponential quantization, can improve performance over the baseline on the TIDIGITs
dataset. The successful outcome of these experiments means that lower resource requirements are needed for
custom implementations of RNN models.
