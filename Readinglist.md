# Image Processing

* [DENSELY CONNECTED CONVOLUTIONAL NETWORKS](http://arxiv.org/pdf/1608.06993v1.pdf)


# Reading

* [ICML 2016 Videos](http://techtalks.tv/icml/2016/tutorials/?utm_campaign=Revue%20newsletter&utm_medium=Newsletter&utm_source=revue)
* [Deep Learing Summer School 2016, Montreal](http://videolectures.net/deeplearning2016_montreal/?utm_campaign=Revue%20newsletter&utm_medium=Newsletter&utm_source=revue)


# Variational Auto Encoders

* [Unreasonable confusion of Variational AutoEncoders](https://jaan.io/unreasonable-confusion/)


# Graphical Model

* [Bishop Graphical Model 1](http://mlss.tuebingen.mpg.de/2013/bishop_slides.pdf)
* [Bishop Graphical Model 2](http://www.cs.ucf.edu/~mtappen/cap6412/lecs/graphical_models.pdf)
* [Machine Learning Summer School 2013](http://webdav.tuebingen.mpg.de/mlss2013/2013/speakers.html)


# Deep Learning School Day

* [Deep Learning School Day 1](https://www.youtube.com/watch?v=eyovmAtoUx0&feature=youtu.be)
* [Deep Learning School Day 2](https://www.youtube.com/watch?v=9dXiAecyJrY&feature=youtu.be)

* Back Propagation Derivation

* [Derviation of back propagation](http://briandolhansky.com/blog/2013/9/27/artificial-neural-networks-backpropagation-part-4)
* [Derivation of back propagation](http://briandolhansky.com/blog/2014/10/30/artificial-neural-networks-matrix-form-part-5)

# Reddit Pages
* [Machine Learning](https://www.reddit.com/r/MachineLearning/)
* [Deep Learning](https://www.reddit.com/r/deeplearning/)
* [Reddit Machine Learning Q&A Thread](https://www.reddit.com/user/feedtheaimbot)
* [ML Questions](https://www.reddit.com/r/MLQuestions/)

# [Visualize tSNE](http://distill.pub/2016/misread-tsne/)

# [ICASSP 2016](http://www.icassp2016.org/Papers/RegularProgram_MS.asp)

* EXPLORING MULTIDIMENSIONAL LSTMS FOR LARGE VOCABULARY ASR
* END-TO-END ATTENTION-BASED LARGE VOCABULARY SPEECH RECOGNITION
* DEEP CONVOLUTIONAL ACOUSTIC WORD EMBEDDINGS USING WORD-PAIR SIDE INFORMATION
* VERY DEEP MULTILINGUAL CONVOLUTIONAL NEURAL NETWORKS FOR LVCSR
* LISTEN, ATTEND AND SPELL: A NEURAL NETWORK FOR LARGE VOCABULARY CONVERSATIONAL SPEECH RECOGNITION

## [Adaptation](http://www.icassp2016.org/Papers/PublicSessionIndex3_MS.asp?Sessionid=1159)

* CONTEXT ADAPTIVE DEEP NEURAL NETWORKS FOR FAST ACOUSTIC MODEL ADAPTATION IN NOISY CONDITIONS
* ON COMBINING I-VECTORS AND DISCRIMINATIVE ADAPTATION METHODS FOR UNSUPERVISED SPEAKER NORMALIZATION IN DNN ACOUSTIC MODELS
* NON-NEGATIVE INTERMEDIATE-LAYER DNN ADAPTATION FOR A 10-KB SPEAKER ADAPTATION PROFILE
* SPEAKER CLUSTER-BASED SPEAKER ADAPTIVE TRAINING FOR DEEP NEURAL NETWORK ACOUSTIC MODELING
* EFFICIENT NON-LINEAR FEATURE ADAPTATION USING MAXOUT NETWORKS
* SEQUENCE SUMMARIZING NEURAL NETWORK FOR SPEAKER ADAPTATION

## Decoders

* PARALLELIZING WFST SPEECH DECODERS
* ACCELERATING MULTI-USER LARGE VOCABULARY CONTINUOUS SPEECH RECOGNITION ON HETEROGENEOUS CPU-GPU PLATFORMS

## [Neural Networks in Speech](http://www.icassp2016.org/Papers/PublicSessionIndex3_MS.asp?Sessionid=1160)

* FLAT START TRAINING OF CD-CTC-SMBR LSTM RNN ACOUSTIC MODELS
* PREDICTION-ADAPTATION-CORRECTION RECURRENT NEURAL NETWORKS FOR LOW-RESOURCE LANGUAGE SPEECH RECOGNITION
* A STUDY OF RANK-CONSTRAINED MULTILINGUAL DNNS FOR LOW-RESOURCE ASR
* MULTILINGUAL REGION-DEPENDENT TRANSFORMS
* EXPLOITING LSTM STRUCTURE IN DEEP NEURAL NETWORKS FOR SPEECH RECOGNITION
* SELF-STABILIZED DEEP NEURAL NETWORK


## [Language Models](http://www.icassp2016.org/Papers/PublicSessionIndex3_MS.asp?Sessionid=1165)

## [Robust Speech Recognition](http://www.icassp2016.org/Papers/PublicSessionIndex3_MS.asp?Sessionid=1158)

## RNN LM
* [Building an Efficient Neural langauge model](https://research.facebook.com/blog/building-an-efficient-neural-language-model-over-a-billion-words/)
* [n-gram interpolation with RNN LM](http://mi.eng.cam.ac.uk/~xc257/papers/ASRU2015-Interpolation.pdf)
> Methods to combine multiple language models had been studied and
compared in [27, 13, 28]. Most of these techniques are investigated
on n-gram LMs and their derivations, such as topic based n-gram
LM and cached based n-gram LM. RNNLMs are inherently different
from n-gram LMs in terms of their generalisation patterns. For this
reason, RNNLMs are usually linearly interpolated with n-gram LMs
to obtain both a good context coverage and strong generalisation [1,
3, 17, 18, 19, 20]. The interpolated LM probability is given by
P(wi|h
i−1
1
) = λPNG(wi|h
i−1
1
) + (1 − λ)PRN(wi|h
i−1
1
) (5)
λ is the global weight of the n-gram LM distribution PNG(·), which
can be optimized using the EM algorithm on a held-out set.
