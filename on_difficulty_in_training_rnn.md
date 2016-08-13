# [On the difficulty of training Recurrent Neural Networks](https://arxiv.org/pdf/1211.5063v2.pdf)

> Abstract
There are two widely known issues with properly
training Recurrent Neural Networks, the
vanishing and the exploding gradient problems
detailed in Bengio et al. (1994). In
this paper we attempt to improve the understanding
of the underlying issues by exploring
these problems from an analytical, a geometric
and a dynamical systems perspective.
Our analysis is used to justify a simple yet effective
solution. We propose a gradient norm
clipping strategy to deal with exploding gradients
and a soft constraint for the vanishing
gradients problem. We validate empirically
our hypothesis and proposed solutions in the
experimental section.

## Major issues with training RNN
* Exploding gradients
 * To deal with the exploding gradients problem, we propose a solution that involves clipping the norm of the 
   exploded gradients when it is too large. The algorithm is motivated by the assumption that when gradients 
   explode, the curvature and higher order derivatives explode as well, and we are faced with a specific pattern 
   in the error surface, namely a valley with a single steep wall.
* Vanishing Gradients
 * In order to deal with the vanishing gradient problem we use a regularization term that forces the error 
   signal not to vanish as it travels back in time. This regularization term forces the Jacobian matrices 
   ∂xi / ∂xi−1 to preserve norm only in relevant directions. In practice we show that these solutions improve 
   performance on both the pathological synthetic datasets considered as well as on polyphonic music prediction 
   and language modelling.
