
# Week 3 -- Dimensionality reduction (23 Sep 2020)

## Assignment

Complete the following 2 exercises before class #3 on 23 Sep.

1. KNN and overfitting
    * Open [lab_knn.ipynb](https://github.com/umbcdata602/fall2020/blob/master/lab_knn.ipynb) in Colab
    * Use the following code to create a dataset with `make_blobs`
    ```
    from sklearn.datasets import make_blobs
    from matplotlib.colors import ListedColormap

    plt.rcParams.update({'font.size': 16})
    colors = ('red', 'blue')
    cmap = ListedColormap(colors)

    std_true = 5.0    # original: 1.5
    n_samples = 150   # original: 100

    X, y = make_blobs(n_samples, 2, centers=2, random_state=2, cluster_std=std_true)

    plt.scatter(X[:, 0], X[:, 1], c=y, s=50, cmap=cmap, alpha=.7);
    ```
    * Use the `train_test_split` method in scikit-learn to split the data with `test_size=0.3`
    * Use the `StandardScaler` in scikit-learn to scale the data
    * Use the `KNeighborsClassifier` class in scikit-learn to create and train a classifier. 
    * Plot the decision region and investigate different values of K.
    * Use the confusion_matrix method in scikit-learn to demonstrate that the model overfits with K=1.
2. Curse of dimensionality
    * Open [lab_curse_of_dimensionality.ipynb](https://github.com/umbcdata602/fall2020/blob/master/lab_curse_of_dimensionality.ipynb) in Colab
    * Use the `NearestNeighbor` class in scikit-learn for the following 1-D and 2-D calculations.
    * In 1-D, find the sample in the 1-D dataset `samples[:,0]` that is nearest to the origin `x1=0`
    * Plot the result as follows:
        * Create a copy of the plot provided in the notebook, 
        * Add a line extending from the nearest sample in 1-D to the 1-D origin: `x1=0`.
        * Note: For this 1-D example, your solution should be independent of the 2nd coordinate, `x2`.
    * In 2-D, find the element in `samples` that is closes to the 2-D origin: `[x1, x2]=[0,0]`.
    * Plot the result as follows:
        * Add a line to the plot you just created.
        * This line should extend from the nearest sample in 2-D to the 2-D origin.
    * Explain how this exercise illustrates the problem that adding dimensions leads to sparse sampling.

## Reading

Make sure to look at associated Jupyter notebooks in github, and try running them in Google Colab.

* Rasckha & Mirjalili, Chapter 4: Building good training datasets
* Rasckha & Mirjalili, Chapter 5: Compressing data via dimensionality reduction

## Study guide for Week #3

* Curse of dimensionality
* Regularization -- L1 vs L2
* Scaling -- min/max vs zero mean/unit variance
* Feature selection -- greedy vs exhaustive algorithms
* High variance models -- the options
* Feature selection -- objectives
* Feature scaling -- min/max vs mean/variance
* Regularization -- L1 vs L2
* Sequential feature selection algorithms -- pros and cons
* Feature importance with random forest -- pros and cons
* PCA -- role of covariance matrix
* Feature transformation and principal components
* LDA vs PCA
* Kernel PCA and the kernel trick
