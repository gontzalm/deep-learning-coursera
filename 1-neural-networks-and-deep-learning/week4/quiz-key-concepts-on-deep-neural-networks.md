## Week 4 Quiz - Key Concepts on Deep Neural Networks

1. What is the "cache" used for in our implementation of forward propagation and
backward propagation?

    - [ ] It is used to cache the intermediate values of the cost function
      during training.
    - [ ] We use it to pass variables computed during backward propagation to
      the corresponding forward propagation step. It contains useful values for
      forward propagation to compute activations.
    - [ ] It is used to keep track of the hyperparameters that we are searching
      over, to speed up computation.
    - [x] We use it to pass variables computed during forward propagation to the
      corresponding backward propagation step. It contains useful values for
      backward propagation to compute derivatives.

2. Among the following, which ones are "hyperparameters"?

    - [x] Learning rate $\alpha$.
    - [x] Size of the hidden layers.
