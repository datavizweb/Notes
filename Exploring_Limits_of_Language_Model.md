# [Exploring the Limits of Language Modeling](https://arxiv.org/pdf/1602.02410v2.pdf)

# LSTM Training steps

* Dropout before and after every LSTM layer (Zaremba et al., 2014), (Srivastava, 2013)  
* Biases of LSTM forget gate were initialized to 1.0 (Jozefowicz et al., 2015) 
* LSTMs with a projection layer (i.e a bottleneck between hidden states (Sak et al., 2014)) 
* Trained with truncated BPTT (Williams & Peng, 1990) for 20 steps

# LSTM Training Process

* Trained until convergence with an AdaGrad optimizer using a learning rate of `0.2`
 * Fixed learning rate ? Doesn't AdaGrad require variable learning rate like Gradient Decent ? 
* In all the experiments the RNNs were unrolled for `20 steps` without ever resetting the LSTM states
 * LSTM states are not reset between the batches. Won't that learn different state representation all-together ?
 * Or is there any advantage to not reseting the LSTM states ? 
* Batch size of 128 used
* Gradients of the LSTM weights cliped such that their norm is bounded by 1.0 (Pascanu et al., 2012)
 * Why cliping the the norm to 1.0 why not to higher value ?
 * `Pascanu` doesn't say anything about clipping to 1.0.
 * TODO : Check how the gradient level (1.0 to 5.0) has impact on training.
* Model trained on 32 GPU workes with asynchronous gradient update

# Padding for data

* Maximum world length set to 50
* Special word begin and word end markers were added and padded when required
 * cat -> `$cat^  `


