
# Week 2 -- Logistic regression (8 Sep 2020)

## Lab #1 Assignment (to be completed before class on 8 Sep 2020)

* QUESTION #1: The multivariate random number generator uses a covariance that creates correlated features. You can see this in the scatterplot because the sample distribution is oriented from lower left to upper right.
    * Choose a covariance matrix that orients the scatterplot from upper left to lower right.
    * Choose a covariance matrix that makes the scatterplot uniform in all directions.

* QUESTION #2: The notebook computes sample mean two ways, a slow way using a Python `for` loop, and a fast way using numpy's vectorized `np.average` method. 
    * How big does `n` have to get before you notice the difference?

## Lab #2 Assignment (to be completed before class on 8 Sep 2020)

* QUESTION #1: The two features used to train the perceptron in the lab are linearly separable. Use two Iris features that are not linearly separable to demonstrate that the perceptron does not converge for non-separable classes. Make sure to investigate different values of the hyperparameters `eta` and `n_iter`.

## Reading for Week #2

* Rasckha & Mirjalili, Chapter 2: Training simple ML algorithms for classification
    * The entire chapter
* Rasckha & Mirjalili, Chapter 3: Tour of ML classifiers using scikit-learn
    * Section 1: Choosing a classification algorithm
    * Section 2: First steps with scikit-learn -- training a perceptron
    * Section 3: Modeling class probabilities via logistic regression

## Study guide for Week #2 quiz

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
