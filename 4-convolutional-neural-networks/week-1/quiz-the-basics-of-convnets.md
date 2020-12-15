## Week 1 Quiz - The Basics of ConvNets

1. What do you think applying this filter to a grayscale image will do?

    |0 1 -1  0|
    |1 3 -3 -1|
    |1 3 -3 -1|
    |0 1 -1  0|

    - [x] Detect vertical edges.
    - [ ] Detect 45 degree edges.
    - [ ] Detect image contrast.
    - [ ] Detect horizontal edges.

2. Suppose your input is a 300 by 300 color (RGB) image, and you are not using a
convolutional network. If the first hidden layer has 100 neurons, each one fully
connected to the input, how many parameters does this hidden layer have
(including the bias parameters)?

    - [ ] 9,000,001.
    - [ ] 9,000,100.
    - [ ] 27,000,001.
    - [x] 27,000,100.

3. Suppose your input is a 300 by 300 color (RGB) image, and you use a
convolutional layer with 100 filters that are each 5x5. How many parameters does
this hidden layer have (including the bias parameters)?

    - [ ] 2501.
    - [ ] 2600.
    - [ ] 7500.
    - [x] 7600.

4. You have an input volume that is 63x63x16, and convolve it with 32 filters
that are each 7x7, using a stride of 2 and no padding. What is the output
volume?

    - [ ] 16x16x32.
    - [ ] 29x29x16.
    - [x] 29x29x32.
    - [ ] 16x16x16.

5. You have an input volume that is 15x15x8, and pad it using *pad = 2*. What is
the dimension of the resulting volume?

    - [x] 19x19x8.
    - [ ] 19x19x12.
    - [ ] 17x17x10.
    - [ ] 17x17x8.

6. You have an input volume that is 63x63x16, and convolve it with 32 filters
that are each 7x7, and stride of 1. You want to use a *same* convulution. What
is the padding?

    - [ ] 1.
    - [ ] 2.
    - [x] 3.
    - [ ] 7.

7. You have an input volume that is 32x32x16, and apply max pooling with a
stride of 2 and a filter size of 2. What is the output volume?

    - [ ] 32x32x8.
    - [x] 16x16x16.
    - [ ] 15x15x16.
    - [ ] 16x16x8.

8. Because pooling layers do not have parameters, they do not affect the
backpropagation calculation.

    - [ ] True.
    - [x] False.

9. In the lecture we talked about *parameter sharing* as a benefit of using
convolutional networks. Which of the following statements about parameter
sharing in ConvNets are true?

    - [ ] It allows gradient descent to set many of the parameters to zero, thu
      making the connections sparse.
    - [ ] It allows parameters learned for one task to be shared even for a
      different task (transfer learning).
    - [x] It allows a feature detector to be used in multiple locations
      throughout the whole input image.
    - [x] It reduces the total number of parameters, thus reducing overfitting.

10. In lecture we talked about *sparsity of connections* as a benefit of using
convolutional layers. What does this mean?

    - [x] Each activation in the next layer depends on only a small numer of
      activations from the previous layer.
    - [ ] Regularization causes gradient descent to set many of the
      parameters to zero.
    - [ ] Each layer in a convulutional network is connected only to two other
      layers.
    - [ ] Each filter is connected to every channel in the previous layer.

