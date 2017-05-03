# KNN

This repository consists of the implementation of K-Nearest Neighbors algorithm to solve a Classification problem.You can also view this repository through [Gitpages.](https://satishjasthi.github.io/K-Nearest-Neighbors/)


### Install

This project requires **Python 3.5** or above and the following Python libraries are installed:

- [Numpy](http://www.numpy.org)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](http://continuum.io/downloads)
distribution of Python, which already has the above packages and more included. Make sure that you select the Python 3.4
or above and not the Python 2.x installer

### Getting started
### About KNN:

In pattern recognition, the k-nearest neighbors algorithm (k-NN) is a non-parametric method used for classification and regression.In both cases, the input consists of the k closest training examples in the feature space. The output depends on whether k-NN is used for classification or regression:

- In k-NN classification, the output is a class membership. An object is classified by a majority vote of its neighbors, with the object being assigned to the class most common among its k nearest neighbors (k is a positive integer, typically small). If k = 1, then the object is simply assigned to the class of that single nearest neighbor.

- In k-NN regression, the output is the property value for the object. This value is the average of the values of its k nearest neighbors.

k-NN is a type of instance-based learning, or lazy learning, where the function is only approximated locally and all computation is deferred until classification. The k-NN algorithm is among the simplest of all machine learning algorithms.

Both for classification and regression, it can be useful to assign weight to the contributions of the neighbors, so that the nearer neighbors contribute more to the average than the more distant ones. For example, a common weighting scheme consists in giving each neighbor a weight of 1/d, where d is the distance to the neighbor.

The neighbors are taken from a set of objects for which the class (for k-NN classification) or the object property value (for k-NN regression) is known. This can be thought of as the training set for the algorithm, though no explicit training step is required.

A shortcoming of the k-NN algorithm is that it is sensitive to the local structure of the data.[citation needed] The algorithm is not to be confused with k-means, another popular machine learning technique.

**To know more about KNN you can go through these tutorials:**

* [K-Nearest Neighbors for Machine Learning](http://machinelearningmastery.com/k-nearest-neighbors-for-machine-learning/)
* [Implement k-Nearest Neighbors in Python From Scratch](http://machinelearningmastery.com/tutorial-to-implement-k-nearest-neighbors-in-python-from-scratch/)
* [A Complete Guide to K-Nearest-Neighbors with Applications in Python and R](https://kevinzakka.github.io/2016/07/13/k-nearest-neighbor/)


#### Dataset

This data was extracted from the [1994 Census bureau](http://www.census.gov/en.html) database by Ronny Kohavi and 
Barry Becker (Data Mining and Visualization, Silicon Graphics). A set of reasonably clean records was extracted using the
following conditions: ((AAGE>16) && (AGI>100) && (AFNLWGT>1) && (HRSWK>0)). The prediction task is to determine whether a 
person makes over $50K a year.

**Description of fnlwgt (final weight):**

The weights on the Current Population Survey (CPS) files are controlled to independent estimates of the civilian noninstitutional 
population of the US. These are prepared monthly for us by Population Division here at the 
Census Bureau. We use 3 sets of controls. These are:

* A single cell estimate of the population 16+ for each state.
* Controls for Hispanic Origin by age and sex.
* Controls by Race, age and sex.

We use all three sets of controls in our weighting program and "rake" through them 6 times so that by the end we 
come back to all the controls we used. The term estimate refers to population totals derived from CPS by creating 
"weighted tallies" of any specified socio-economic characteristics of the population. People with similar 
demographic characteristics should have similar weights. There is one important caveat to remember about this 
statement. That is that since the CPS sample is actually a collection of 51 state samples, each with its own 
probability of selection, the statement only applies within state.

**Relevant papers:**

Ron Kohavi, ["Scaling Up the Accuracy of Naive-Bayes Classifiers: a Decision-Tree Hybrid"](http://robotics.stanford.edu/~ronnyk/nbtree.pdf), Proceedings of the 
Second International Conference on Knowledge Discovery and Data Mining, 1996. (PDF)

**Description of dataset:**

**Attributes:**

income: >50K, <=50K

age: continuous

workclass: Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked

fnlwgt: continuous

education: Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool

education-num: continuous

marital-status: Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse

occupation: Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces

relationship: Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried

race: White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black

sex: Female, Male

capital-gain: continuous

capital-loss: continuous

hours-per-week: continuous

native-country: United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, 
Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, 
Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, 
Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands

### Run

In a terminal or command window, navigate to top-level project directory `KNN/` (that contains
this README) and run one of the following commands:

```bash
ipython notebook Source.ipynb
```
or 
```bash
jupyter notebook Source.ipynb
```
This will open the Jupyter Notebook software and project file in your browser.

If you are unable to run 'Source.ipynb` using any of the above methods, follow these steps:

* In a terminal or command window, navigate to top-level project directory `KNN/` (that contains
this README)

* now run 

``` export PATH=~/anaconda3/bin:$PATH
 jupyter-notebook
```
Jupyter Notebook creates an instance in your browser with home directory as `KNN/`, you can run `Source.ipynb`
by double clicking on it.





