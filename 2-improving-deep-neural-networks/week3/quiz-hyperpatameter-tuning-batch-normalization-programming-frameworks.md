## Week 3 Quiz - Hyperparameter Tuning, Batch Normalization, Programming
Frameworks

1. If searching among a large number of hyperparameters, ypu should try values
in a grid rather than random values, so that you can carry out the search more
systematically and not truly rely on chance.

    - [ ] True.
    - [x] False.

2. Every hyperparameter, if set poorly, can have a huge negative impact on
training, and so all hyperparameters are about equally important to tune well.

    - [ ] True.
    - [x] False.

3. During hyperparameter search, wether you try to babysit one model (*Panda*
strategy) or train a lot of models in parallel (*Caviar*) is largely determined
by:

    - [ ] Wether you use batch or mini-batch optimization.
    - [ ] The presence of local minima in your neural network.
    - [x] The amount of computational power you can access.
    - [ ] The number of hyperparameters you have to tune.

4. If you think *\beta* (hyperparameter for momentum) is between on 0.9 and
0.99, which of the following is the recommended way to sample a value for
*\beta*?

    ```python3
    r = np.random.rand()
    beta = 1 - 10 ** -(r + 1)
    ```

5. Finding good hyperparameter values is very time-consuming. So typically you
should do it once at the start of the project, and try to find very good
hyperhyperparameters so that you don't ever have to revisit tuning again.

    - [ ] True.
    - [x] False.

6. In batch normalization as presented in the videos, if you apply it on the
*l*th layer of your neural network, what are you normalizing?

    - *z^[l]*

7. In the normalization formula *z^(i)_norm = (z^(i) - \mu)/(\sqrt(\sigma^2 +
\epsilon))*, why do we use *\epsilon*?

    - [ ] To speed up convergence.
    - [x] To avoid division by zero.
    - [ ] In case *\mu* is to small.
    - [ ] To have more accurate information.

8. Which of these statements about *\gamma* and *\beta* in Batch Norm are true?

    - [ ] The optimal values are *\gamma = \sqrt(\sigma^2 + \epsilon)* and
      *\beta = \mu*.
    - [x] They set the mean and variance of the linear variable *z^[l]* of a
      given layer.
    - [ ] *\beta* and *\gamma* are hyperparameters of the algorithm, which we
      tune via random sampling.
    - [ ] There is one global variable *\gamma € R* and *\beta € R* for each
      layer, and applies to all the hidden units in that layer.
    - [x] They can be learned using Adam, gradient descent with momentum, or
      RMSprop, not just with gradient descent.

9. After training a neural network with Batch Norm, at test time, to evaluate
the neural network on a new example you should:

    - [ ] Use the most recent mini-batch's value of *\mu* and *\sigma* to perform
     the needed normalizations.
    - [ ] If you implemented Batch Norm on mini-batches of 256 examples, then to
      evaluate on one test sample, duplicate that example 256 times so that
      you're working with a mini-batch the same size as during training.
    - [ ] Skip the normalization step since a single test example cannot be
      normalized.
    - [x] Perform the needed normalizations, use *\mu* and *\sigma^2* estimated
      using an exponentially weighted average across mini-batches seen during
      training.

10. Which of these statements about deep learning programming frameworks are
true?

    - [x] A programming framework allows you to code up deep learning algorithms
      with typically fewer lines of code than a lower-level language such as
      Python.
    - [ ] Deep learning programming framework require cloud-based machines to
      run.
    - [x] Even if a project is currently open source, good governance of the
      project helps ensure that it remains open even in the long term, rather
      than become closed or modified to benefit only one company.

