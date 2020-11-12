## Week 1 Quiz - Practical Aspects of Deep Learning

1. If you have 10,000,000 examples, how would you split the *train/dev/test*
set?

    - [ ] 33% train, 33% dev, 33% test.
    - [ ] 60% train, 20% dev, 20% test.
    - [x] 98% train, 1% dev, 1% test.

2. The *dev* and *test* sets should:

    - [x] Come from the same distribution.
    - [ ] Come from different distributions.
    - [ ] Be identical to each other.
    - [ ] Have the same number of examples.

3. If your neural network model seems to have high variance, what of the
following would be promising things to try?

    - [ ] Make the neural network deeper.
    - [x] Get more training data.
    - [ ] Increase the number of units in each hidden layer.
    - [ ] Get more test data.
    - [x] Add regularization.

4. You are working on an automated check-out kiosk for a supermarket, and are
builging a classifier for apples, bananas and oranges. Suppose your
classifier obtains a training set error of 0.5%, and a dev set error of 7%.
Which of the following are promising things to try to improve your
classifier?

    - [x] Increase the regularization parameter *lambda*.
    - [ ] Decrease the regularization parameter *lambda*.
    - [x] Get more training data.
    - [ ] Use a bigger neural network.

5. What is *weight decay*?

    - A regularization technique (such as *L2 regularization*) that results in
      gradient descent shrinking the weights on every iteration.

6. What happens when you increase the regularization hyperparameter *lambda*?

    - Weights are pushed toward becoming smaller.

7. With the *inverted dropout* technique, at test time:

    - You do not apply *dropout* and do not keep the *1/keep_prob* factor in the
      calculations used in training.

8. Increasing the parameter *keep_prob* from (say) 0.5 to 0.6 will likely cause
the following:

    - [x] Increasing the regularization effect.
    - [ ] Reducing the regularization effect.
    - [x] Causing the neural network to end up with a higher training set error.
    - [ ] Causing the neural network to end up with a lower training set error.

9. Which of these techniques are useful for reducing variance?

    - [ ] Exploding gradient.
    - [x] Dropout.
    - [x] Data augmentation.
    - [x] L2 regularization.
    - [ ] Xavier initialization.
    - [ ] Vanishing gradient.
    - [ ] Gradient checking.

10. Why do we normalize the imputs *x*?

    - It makes the cost function faster to optimize.
