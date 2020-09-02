
# Week 1 -- Introduction to Machine Learning

## Related reading

* Rasckha & Mirjalili, 3rd Edition, Chapters 1 & 2

## Notebooks

* [week01_introduction.ipynb](https://github.com/umbcdata602/fall2020/blob/master/week01_introduction.ipynb)
    * Use the link at the top of the notebook to open it automatically in Google Colab.
    * Based on [Raschka ch01.ipynb](https://github.com/rasbt/python-machine-learning-book-3rd-edition/blob/master/code/ch01/ch01.ipynb) -- github notebook
    * Introductory material is based on the reading from Chapter 1 of Raschka & Mirjalili, 3rd Edition.
    * Supervised, unsupervised, reinforcement learning
    * Predicting class labels
    * Roadmap for building machine learning systems
    * Basic terminology for the Iris dataset
    * Some of this should be review from 601, but don't worry about it if you haven't seen it before
* [lab01_toolset.ipynb](https://github.com/umbcdata602/fall2020/blob/master/lab01_toolset.ipynb)
    * Use the link at the top of the notebook to open it automatically in Google Colab.
    * Review topics using Numpy, Pandas, Matplotlib -- demos using the classic Iris dataset
    * Random number generators and 2-D covariance
    * Supervised learning introductory concepts -- classification and regression
    * Introduction to object-oriented programming with Python
* [lab02_perceptron.ipynb](https://github.com/umbcdata602/fall2020/blob/master/lab02_perceptron.ipynb)
    * This is a stripped-down version parts of [Raschka ch02.ipynb](https://github.com/rasbt/python-machine-learning-book-2nd-edition/blob/master/code/ch01/ch01.ipynb) with a link that automatically opens in Colab.
    * Focus is on the perceptron (first few cells of ch02.ipynb)
    * Detailed explanations are in the book

## Lab #1 Homework

* QUESTION #1: The multivariate random number generator uses a covariance that creates correlated features. You can see this in the scatterplot because the sample distributions is oriented from lower left to upper right.
    * Choose a covariance matrix that orients the scatterplot from upper left to lower right.
    * Choose a covariance matrix that makes the scatterplot uniform in all directions.

* QUESTION #2: The notebook computes sample mean two ways, a slow way using a Python `for` loop, and a fast way using numpy's vectorized `np.average` method. 
    * How big does $n$ have to get before you notice the difference?

## Lab #2 Homework

* QUESTION #1: The two features used to train the perceptron in [Raschka ch02.ipynb](https://github.com/rasbt/python-machine-learning-book-2nd-edition/blob/master/code/ch01/ch01.ipynb) are linearly separable. Use two Iris features that are not linearly separable to demonstrate that the perceptron does not converge for non-separable classes. Make sure to investigate different values of the hyperparameters eta and n_iter.

## Reading for Week #2

* Rasckha & Mirjalili, Chapter 2: Training simple ML algorithms for classification
    * The entire chapter
* Rasckha & Mirjalili, Chapter 3: Tour of ML classifiers using scikit-learn
    * Section 1: Choosing a classification algorithm
    * Section 2: First steps with scikit-learn -- training a perceptron
    * Section 3: Modeling class probabilities via logistic regression

## Study guide for Week #2

* perceptron convergence
* decision region
* separating hyperplane
* difference between perceptron and adaline
* difference between adaline and logistic regression
* odds ratio
* logit
* sigmoid function
* activation function
* threshold function
* cost function
