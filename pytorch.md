## Pytorch

### Common Questions - 

- Level of abstraction in Tensor - 

  - **Tensor:** Tensor is an imperative n-dimensional array which runs on GPU.
  - **Variable:** It is a node in the computational graph. This stores data and gradient.
  - **Module:** Neural network layer will store state the otherwise learnable weight.

- ### What is variable and autograd.variable? 

  - **Variable** is a package which is used to wrap a tensor. The **autograd.variable** is the central class for the package. The torch.autograd provides  classes and functions for implementing automatic differentiation of  arbitrary scalar-valued functions.

- ### What is the use of MSELoss, CTCLoss, and BCELoss function?

  - MSE stands for Mean Squared Error, which is used to create a criterion  the measures the mean squared error between each element in an input x  and target y. The CTCLoss stands for Connectionist Temporal  Classification Loss, which is used to calculate the loss between  continuous time series and target sequence. The BCELoss(Binary Cross  Entropy) is used to create a criterion to measures the Binary Cross  Entropy between the target and the output.

- ### Give any one difference between torch.nn and torch.nn.functional?

  - The torch.nn provide us many more classes and modules to implement and train the neural network. The **torch.nn.functional** contains some useful function like activation function and convolution  operation, which we can use. However, these are not full layers, so if  we want to define a layer of any kind, we have to use **torch.nn**.

- ###  What do you mean by Mean Squared Error?

  - The mean squared error tells us about how close a regression line to a  set of points. Mean squared error done this by taking the distance from  the points to the regression line and squaring them. Squaring is  required to remove any negative signs.

- ### Give any one difference between batch, stochastic, and mini-batch gradient descent?

  - **Stochastic Gradient Descent:** In SGD, we use only a single training example for calculation of gradient and parameters.
  - **Batch Gradient Descent:** In BGD, we calculate the gradient for the whole dataset and perform the updation at each iteration.
  - **Mini-batch Gradient Descent:** Mini-batch Gradient  Descent is a variant of Stochastic Gradient Descent. In this gradient  descent, we used mini-batch of samples instead of a single training  example.

- ### What is auto-encoder?

  - It is a self-government machine learning algorithm which uses the  backpropagation principle, where the target values are equal to the  inputs provided. Internally, it has a hidden layer which manages a code  used to represent the input.

- ### What is Autograd module in PyTorch?

  - The Autograd module is an automatic differentiation technique which is  used in PyTorch. It is more powerful when we are building a neural  network. There is a recorder which records each operation which we have  performed, and then it replays it backs to compute our gradient.

- ### What is the optim module in PyTorch?

  - Torch.optim is a module which implements various optimization algorithm  which is used for building neural networks. Below is the code of Adam  optimizer

- ### What is pooling layer.

  - Pooling layer plays a crucial role in pre-processing of an image.  Pooling layer reduces the number of parameters when the images are too  large. Pooling is **"downscaling"** of the image which is obtained from the previous layers.

- ### What is Max Pooling?

  - Max pooling is a **sample-based discrete process** whose  main objective is to reduce its dimensionality, downscale an input  representation. And allow for the assumption to be made about features  contained in the sub-region binned. 

- what is the difference between Type I and Type II error?

  - Type I error is the false positive value. And Type 1 error is a false negative value. Type I error represent something is happening when. Type II errors are describing that there nothing is wrong where something is not right.

- What is the role of weights and bias in a neural network?

  - This is where bias comes into the picture. Bias lets you assign some threshold which helps you activate a decision-point (or a neuron) only when that threshold is crossed.

- Why should we use Batch Normalization?

  - Batch Normalization is one of the techniques used for reducing the training time of our deep learning algorithm. Just like normalizing our input helps improve our logistic regression model, we can normalize the activations of the hidden layers in our deep learning model as well

- In a CNN, if the input size 5 X 5 and the filter size is 7 X 7, then what would be the size of the output?

  - Dimension of output will be (n+2p-f+1) X (n+2p-f+1) = 1 X 1

- What’s the difference between valid and same padding in a CNN?

  - Valid Padding: When we do not use any padding. The resultant matrix after convolution will have dimensions (n – f + 1) X (n – f + 1) Same padding: Adding padded elements all around the edges such that the output matrix will have the same dimensions as that of the input matrix

- What do you mean by exploding and vanishing gradients? 

  - However, at times, the steps become too large and this results in larger updates to weights and bias terms – so much so as to cause an overflow (or a NaN) value in the weights. This leads to an unstable algorithm and is called an exploding gradient.
  - On the other hand, the steps are too small and this leads to minimal changes in the weights and bias terms – even negligible changes at times. We thus might end up training a deep learning model with almost the same weights and biases each time and never reach the minimum error function. This is called the vanishing gradient.

- How does LSTM solve the vanishing gradient challenge?

  - The LSTM model is considered a special case of RNNs. The problems of vanishing gradients and exploding gradients we saw earlier are a disadvantage while using the plain RNN model.
  - In LSTMs, we add a forget gate, which is basically a memory unit that retains information that is retained across timesteps and discards the other information that is not needed. This also necessitates the need for input and output gates to include the results of the forget gate as well.

- ###  List the supervised and unsupervised tasks in Deep Learning.

  - Now, this can be one tricky question. There might be a misconception  that deep learning can only solve unsupervised learning problems. This  is not the case. Some example of Supervised Learning and Deep learning  include:
  - Image classification
  - Text classification
  - Sequence tagging
  - On the other hand, there are some unsupervised deep learning techniques as well:
  - Word embeddings (like Skip-gram and Continuous Bag of Words): [Understanding Word Embeddings: From Word2Vec to Count Vectors](https://www.analyticsvidhya.com/blog/2017/06/word-embeddings-count-word2veec/?utm_source=blog&utm_medium=comprehensive-popular-deep-learning-interview-questions-answers)
  - Autoencoders: [Learn How to Enhance a Blurred Image using an Autoencoder!](https://www.analyticsvidhya.com/blog/2020/02/what-is-autoencoder-enhance-image-resolution/?utm_source=blog&utm_medium=comprehensive-popular-deep-learning-interview-questions-answers)

- ### What are the common data structures used in Deep Learning?

  - List, Matrix, Tensor, Data Frame, Computational Graph 

- ### Why should we use Batch Normalization?

  - Batch Normalization is one of the techniques used for reducing the  training time of our deep learning algorithm. Just like normalizing our  input helps improve our logistic regression model, we can normalize the  activations of the hidden layers in our deep learning model as well:

- ### What’s the difference between valid and same padding in a CNN?

  - Valid Padding: When we do not use any padding. The resultant matrix  after convolution will have dimensions (n – f + 1) X (n – f + 1)
  - Same padding: Adding padded elements all around the edges such that the  output matrix will have the same dimensions as that of the input matrix

- ### Why is GRU faster as compared to LSTM?

  - As you can see, the LSTM model can become quite complex. In order to  still retain the functionality of retaining information across time and  yet not make a too complex model, we need GRUs. Basically, in GRUs, instead of having an additional Forget gate, we  combine the input and Forget gates into a single Update Gate:
  - It is this reduction in the number of gates that makes GRU less complex  and faster than LSTM. You can learn about GRUs, LSTMs and other sequence models in detail here: [Must-Read Tutorial to Learn Sequence Modeling & Attention Models](https://www.analyticsvidhya.com/blog/2019/01/sequence-models-deeplearning/?utm_source=blog&utm_medium=comprehensive-popular-deep-learning-interview-questions-answers).

- **Why CNN is preferred over ANN for Image Classification tasks even though it is possible to solve image classification using ANN?**

  - ANN’s require concrete data points meaning if you are building a deep  learning model to distinguish between cats and dogs, the length of the  ears, the width of the nose, and other features should be provided as  data points while if using CNN for image classification spatial features are extracted from the input images. When there are thousands of  features to be extracted, CNN is a better choice because it gathers  features on its own, unlike ANN where each individual feature needs to  be measured.
  - Training a neural network model becomes computationally heavy (requiring additional storage and processing capability) as the number of layers  and parameters increases. Tuning the increased number of parameters can  be a tedious task with ANN, unlike CNN where the time for tuning  parameters is reduced making it an ideal choice for image classification problems.

- **Can you train a neural network model by initializing all biases as 0?**

  - Yes, there is a possibility that the neural network model will learn even if all the biases are initialized to 0.

- **Can you train a neural network model by initializing all the weights to 0?**

  - No, it is not possible to train a model by initializing all the weights  to 0 because the neural network will never learn to perform a given  task. Initializing all weights to zeros will cause the derivatives to  remain the same for every w in W [1] because of which neurons will learn the same features in every iteration. Not just 0, but any kind of  constant initialization of weights is likely to produce a poor result.

- **You want to train a deep learning model on a 10GB dataset but  your machine has 4GB RAM. How will you go about implementing a solution  to this deep learning problem?**

  - One of the possible ways to answer this question would be to say that a  neural network can be trained by loading the data into the NumPy array  and defining a small batch size.NumPy doesn’t load the complete dataset  into the memory but creates a complete mapping of the dataset. NumPy  offers several tools for compressing large datasets that can be  integrated with other NN packages like PyTorch, TensorFlow, or Keras.

- **How will you differentiate between a multi-class and multi-label classification problem?**

  - In a multi-class classification problem, the classification task has  more than two mutually exclusive classes whereas in a multi-label  problem each label has a different classification task, however, the  tasks are related somehow. For example, classifying a set of images of  animals which may be cats, dogs, or bears is a multi-class  classification problem that assumes that each sample has only one label  meaning an image can be classified as either a cat or a dog but not both at the same time. Now imagine that you want to process the below image. The image shown below needs to be classified as both cat and dog  because the image shows both the animals. In a multi-label  classification problem, a set of labels are assigned to each sample and  the classes are not mutually exclusive. So, a pattern can belong to one  or more classes in a multi-label classification problem.

- **What do you understand by Gradient Clipping?**

  - Gradient Clipping is used to deal with the exploding gradient problem  that occurs during the backpropagation. The gradient values are forced  element-wise to a particular minimum or maximum value if the gradient  has crossed the expected range. Gradient clipping provides numerical  stability while training a neural network but does not provide any  performance improvements.

- **Are convolutional neural networks translation-invariant?**

  -  Convolutional neural networks are translation invariant only to a  certain extent but pooling can make them translation invariant. Making a CNN completely translation-invariant might not be possible. However, by feeding the right kind of data this can be achieved although this might not be a feasible solution.

-  **What is the advantage of using small kernels like 3x3 than using a few large ones.**

  - Smaller kernels let you use more filters so you can use a greater number of activations functions and let the CNN learn a more discriminative  mapping function. Also, smaller kernels capture more spatial context and use fewer computations and parameters making them a better choice over  large ones.

- **How do you bring balance to the force when handling imbalanced datasets in deep learning?**

  - Weight Balancing 
  - Over and Under Sampling

- **What are the benefits of using batch normalization when training a neural network?**

  - Batch normalization optimizes the network training process making it easier to build and faster to train a deep neural network.
  - Batch normalization regulates the values going into each activation  function making activation functions more viable because non-linearities that don’t seem to work well become viable with the use of batch  normalization.
  - Batch normalization makes it easier to initialize weights and also  allows the use of higher learning rates ultimately increasing the speed  at which the network trains.

- **Can you name a few hyper parameters used for training a neural network.**

  - Initialization of weights
  - Setting the number of hidden layers
  - Learning Rate
  - Number of epochs
  - Activation Functions
  - Batch Size
  - Momentum

- **When is multi-task learning usually preferred?**

  - Multi-task learning with deep neural networks is a subfield wherein  several tasks are learned by a shared model. This reduces overfitting,  enhances data efficiency, and speeds up the learning process with the  use of auxiliary information. Multi-task learning is useful when there  is a small amount of data for any given task and we can benefit from  training a deep learning model on a large dataset.

- **Explain the Adam Optimizer in one minute.**

  - Adaptive momentum or Adam optimizer is an optimization algorithm  designed to deal with sparse gradients on noisy problems. Adam optimizer improves convergence through momentum that ensures that a model does  not get stuck in saddle point and also provides per-parameter updates  for faster convergence.

- **Which loss function is preferred for multi-category classification?**

  - Cross-Entropy loss function

- **To what kind of problems can the cross-entropy loss function be applied?**

  - Binary Classification Problems
  - Multi-Label Classification Problems
  - Multi-Category Classification Problems

- **What is the benefit of using max-pooling in classification convolutional neural networks?**

  - The feature maps become smaller after max-pooling in CNN and hence help  reduce the computation and also give more translation in-variance. Also, we don’t lose much semantic information because we’re taking the  maximum activation.

- **How will you implement Batch Normalization in RNN?**

  - It is not possible to use batch normalization in RNN because statistics  are computed per batch and thus batch normalization will not consider  the recurrent part of the neural network. An alternative to this could  be layer normalization in RNN or reparameterizing the LSTM layer that  allows the use of batch normalization.

- **Explain the difference between Gradient Descent and Stochastic Gradient Descent.**

  - To begin with, Gradient descent and stochastic gradient descent both are popular machine learning and deep learning optimization algorithms  which are used for updating a set of parameters in an iterative way in  order to minimize an error function. In gradient descent in order to  update parameters, the entire dataset set is to be considered for a  particular iteration while in stochastic gradient descent, computation  is carried over only one single training sample. For example, if a  dataset has 10000 datapoints, then GD, will train on all the 10000  datapoints and this will take a longer time, while on the other hand,  Stochastic GD, will be much faster as we will train on only a single  sample and update the parameters. This is because Stochastic gradient  descent usually converges faster than gradient descent on large  datasets, because updates are more frequent.

- **Differentiate between bias and variance with respect to deep learning models and how can you achieve a balance between the two?**

  - While understanding predictions, understanding the prediction errors is  most important. There are mainly two broad types of errors, reducible  and irreducible. In reducible errors we have two kinds, bias and  variance. Gaining a proper understanding of these errors helps one built an accurate model by avoiding overfitting and underfitting of the  model.

  - Bias – In the above diagram, the training error (blue dotted line) is  high in the initial stage (high bias) and then decreases sustainably  (low bias) High bias means, the data is under fitting, and hence the  data must have a low bias to achieve good results. In order to achieve  low bias:

  - Try increasing the number of iterations / epochs

  - Try a bigger network

    Variance – the variance in deep learning is nothing but the  difference between the validation error and the training error. In the  above figure, we can see that the gap between the training error and  validation error is high, i.e., the variance is high. This is the case  of overfitting. The model should have low variance and can be achieved  by: i. Increasing the training data ii. Using regularization iii. Using  different neural network architectures.

- **Can you train a neural network without using back-propagation? If yes, what technique will you use to accomplish this?**

  - Indeed, there are various optimization algorithms that does not require back-propagation to train the neural network.

    Among them are evolutionary optimization and Jeff Hinton’s capsule  routing. However, none of these methods exhibit a competitive  performance against back-propagation based algorithms. 

- ### **What is the difference between Entropy and Information Gain?**

  - Entropy is an indicator of how messy your data is. It decreases as you reach closer to the leaf node.
  - The Information Gain is based on the decrease in entropy after a dataset is split on an attribute. It keeps on increasing as you reach closer to  the leaf node.

- ### **Explain Ensemble learning technique in Machine Learning.**

  - Ensemble learning is a technique that is used to create multiple Machine Learning models, which are then combined to produce more accurate  results. A general Machine Learning model is built by using the entire  training data set. However, in Ensemble Learning the training data set  is split into multiple subsets, wherein each subset is used to build a  separate model. After the models are trained, they are then combined to  predict an outcome in such a way that the variance in the output is  reduced.

- ### **What is Cluster Sampling?**

  - It is a process of randomly selecting intact groups within a defined population, sharing similar characteristics.
  - Cluster Sample is a probability sample where each sampling unit is a collection or cluster of elements.
  - For example, if you’re clustering the total number of managers in a set of  companies, in that case, managers (samples) will represent elements and  companies will represent clusters.

  


### Links

```
https://www.glassdoor.com/Interview/machine-learning-developer-tensorflow-pytorch-interview-questions-SRCH_KO0,45.htm
https://www.analyticsvidhya.com/blog/2020/04/comprehensive-popular-deep-learning-interview-questions-answers/
https://www.edureka.co/blog/interview-questions/machine-learning-interview-questions/  (to do)
https://www.projectpro.io/article/100-deep-learning-interview-questions-and-answers-for-2021/419
https://www.analyticsvidhya.com/blog/2018/11/neural-networks-hyperparameter-tuning-regularization-deeplearning/?utm_source=blog&utm_medium=comprehensive-popular-deep-learning-interview-questions-answers (do this last)


```

