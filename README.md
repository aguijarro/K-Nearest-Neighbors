# KNN

This repository consists of the implementation of K-Nearest Neighbors algorithm to solve a Classification problem.

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






