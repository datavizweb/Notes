# [Deep Networks with Stochastic Depth](https://arxiv.org/pdf/1603.09382v3.pdf)

> Abstract. Very deep convolutional networks with hundreds of layers
have led to significant reductions in error on competitive benchmarks.
Although the unmatched expressiveness of the many layers can be highly
desirable at test time, training very deep networks comes with its own
set of challenges. The gradients can vanish, the forward flow often diminishes,
and the training time can be painfully slow. To address these
problems, we propose stochastic depth, a training procedure that enables
the seemingly contradictory setup to train short networks and use deep
networks at test time. We start with very deep networks but during training,
for each mini-batch, randomly drop a subset of layers and bypass
them with the identity function. This simple approach complements the
recent success of residual networks. It reduces training time substantially
and improves the test error significantly on almost all data sets that we
used for evaluation. With stochastic depth we can increase the depth
of residual networks even beyond 1200 layers and still yield meaningful
improvements in test error (4.91% on CIFAR-10).


* Training a deep network is a challenge
* Training Stochastic Depth Network
 * Train short network and use deep network at test time
* Training
 * Train very deep neural network for each mini-batch
 * Drop subset of layers bypass them with identity function
  * What we achieving by bypassing ?
  * What is the role of identity function ?
 * What is a residual network ?
* Advantage
 > Reduces the training time   
   Reduces the test set error
   
* ResNet had 152 layers
* Model expressiveness and network depth


* Deep networks with stochastic depth
  * deep network during testing but a short network during training. 
  * Training
   * Deep Residual Network architectures (with hundreds or even thousands of layers) with sufficient modeling
capacity
   * shorten the network significantly by randomly removing a substantial fraction of layers independently for each sample or
mini-batch. 
    * Unlike dropout make network shorter than thinner
   * The effect is a network with a small expected depth during training, but a large depth during testing.

* Observation : 
 * training with stochastic depth substantially reduces training time and test error
 * The reduction in training time can be attributed to the shorter forward and backward
propagation, so the training time no longer scales with the full depth, but the
shorter expected depth of the network. 
 * Reduction in test error is could be due to 
  * shortening the (expected) depth during training reduces the chain of forward propagation steps and gradient computations, which strengthens
the gradients especially in earlier layers during backward propagation
  * networks trained with stochastic depth can be interpreted as an implicit ensemble
of networks of different depths, mimicking the record breaking ensemble of depth varying ResNets trained by He et al
  * Similar to Dropout training with stochastic depth acts as a regularizer, even in the presence of Batch Normalization. 
  * On CIFAR-10, depth of a ResNet beyond 1000 layers obtain significant improvements in test error.
 

* Dropout
 * Reduces co-adaptation
 * Collaborates in group instead of indepdendently learning features
 * Anagolous to training ensemble of exponentially many small networks
 * Dropout loses effectiveness with Batch Normalization
 * Acts as regularization
  * DropConnect
  * MaxOut
  * DropIn