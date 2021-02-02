## Week 2 Quiz - Natural Language Processing & Word Embeddings

1. Suppose you learn a word embedding for a vocabulary of 10,000 words. Then the
embedding vectors should be 10,000 dimensional, so as to capture the full range
of variation and meaning in those words.

    - [ ] True.
    - [x] False.

2. What is t-SNE?

    - [ ] A linear transformation that allows us to solve analogies on word
      vectors.
    - [x] A non-linear dimensionality reduction technique.
    - [ ] A supervised learning algorithm for learning word embeddings.
    - [ ] An open-source sequence modeling library.

3. Suppose you download a pre-trained word embedding which has been trained on a
huge corpus of text. You then use this word embedding to train a RNN for a
language task of recognizing if someone is happy from a short snippet of text,
using a small tranining set.

    | x (input text)               | y (happy?) |
    |------------------------------|------------|
    | I'm feeling wonderful today! | 1          |
    | I'm bummed my cat is ill.    | 0          |
    | Really enjoying this!        | 1          |

    Then even if the word "ecstatic" does not appear in your small tranining
    set, your RNN might reasonably be expected to recognize "I'm ecstatic" as
    deserving a label *y = 1*.

    - [x] True.
    - [ ] False.

4. Which of these equations do you think should hold for a good word embedding?

    - [x] *e_boy - e_girl /approx e_brother - e_sister*.
    - [ ] *e_boy - e_girl /approx e_sister - e_brother*.
    - [x] *e_boy - e_brother /approx e_girl - e_sister*.
    - [ ] *e_boy  - e_brother /approx e_sister - e_girl*.

5. Let *E* be an embedding matrix, and let *o_1234* be a one-hot vector
corresponding to word 1234. Then to get the embedding of word 1234, why don't we
call *E * o_1234* in Python?

    - [x] It is computationally wasteful.
    - [ ] The correct formula is *E^T * o_1234*.
    - [ ] This doesn't handle unknown words.
    - [ ] None of the above: calling the Python snippet as described above is
      fine.

6. When learning word embeddings, we create an artificial task of estimating
*P(target|content)*. It is okay if we do poorly on this artificial prediction
task; the more important by-product of this task is that we learn a useful set
of word embeddings.

    - [x] True.
    - [ ] False.

7. In the word2vec algorithm, you estimate *P(t|c)*, where *t* is the target
word and *c* is a context word. How are *t* and *c* chosen from the training
set?

    - [ ] *c* is the one word that comes immediately before *t*.
    - [x] *c* and *t* are chosen to be nearby words.
    - [ ] *c* is a sequence of several words immediately before *t*.
    - [ ] *c* is the sequence of all the words in the sentence before *t*.

8. Suppose you have a 10,000 word vocabulary, and are learning 500-dimensional
embeddings. The word2vec model uses the following softmax function:

    (word2vec softmax function)

    Which of these statements are correct?

    - [x] */theta_t* and *e_c* are both 500 dimensional vectors.
    - [ ] */theta_t* and *e_c* are both 10,000 dimensional vectors.
    - [x] */theta_t* and *e_c* are both trained with an optimization algorithm
      such as Adam or gradient descent.
    - [ ] After training, we should expect */theta_t* and *e_c* to be very close
      when *t* and *c* are the same word.

9. Suppose you have a 10,000 word vocabulary, and are learning 500-dimensional
word embeddings. The GloVe model minimizes this objective:
    
    (minimization objective)

    Which of these statements are correct?

    - [ ] */theta_i* and *e_j* should be initialized to 0 at the beggining of
      training.
    - [x] */theta_i* and *e_j* should be initialized randomly at the beggining
      of tranining.
    - [x] *Xij* is the number of times word *j* appears in the context of word
      *i*.
    - [x] The weighting function must satisfy *f(0) = 0*.

10. You have trained word embeddings using a text dataset of *m1* words. You are
considering using these word embeddings for a language task, for which you have
a separate labeled dataset of *m2* words. Keeping in mind that using word
embeddings is a form of transfer learning, under which of these cirscumtances
would you expect the word embeddings to be helpful?

    - [x] *m1 >> m2*.
    - [ ] *m1 << m2*.

