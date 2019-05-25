# Python Data Visualization

### Agenda
* Homework Check
* What is Machine Learning
* Homework

### Python Data Visualization

##### Goals
Learn what is Machine Learning, and the different types of algorithms we can use to solve ML problems. By the end of this class you'll be able to:
* Explain what is Machine Learning
* Understand ML main concepts and glossary
* Identify different types of ML problems
* Understand which algorithms can be applied to each kind of ML problems
* Apply the algorithms and data preparation techniques to obtain a ML model
* Measure and compare the quality of extracted ML models
* Apply these techniques to your final project in order to find the best way to answer your originally formulated question

##### Machine Learning Concepts
* [Machine Learning](https://scikit-learn.org/stable/tutorial/basic/tutorial.html#machine-learning-the-problem-setting): Machine learning: the problem setting¶
* In groups of three, take ten minutes to research what is Machine Learning and the difference between Supervised and Unsupervised ML methods. Provide one sample of each.
* Supervised learning: regression (Show housing problem, with 1, 2 and 3 features, add chart and polynomials). Regression because wants to regress or minimize distance to the linear regression, giving wights to important vars
start with 2 dots, increase to hundreds(1 to many vars) (sums distance of all dots until reaches the optimum low for each feature)
* Supervised learning: classification (Show wine problem, with 1, 2 and 3 features, add chart and polynomials) give wights to important vars and reduces unimportant ones, targetting
* Add draw diagram on board <mix the diagrams you got over there in browser>
* We'll learn how to do these steps using scikit-learn

#####scikit-learn
* [sklearn tutorial](http://scipy-lectures.org/packages/scikit-learn/index.html#introduction-problem-settings): tutorial showing how to use python and sklearn to solve ML problems
The scikit-learn project started as scikits.learn, a Google Summer of Code project, now under active community development
* Pandas and sklearn
target, iris.target_names, data)
datashape target shape


##### Acquiring and loading data
* [Loading External Datasets](https://scikit-learn.org/stable/datasets/index.html#external-datasets): sklearn recommended ways to load datasets
* Generally, scikit-learn works on any numeric data stored as numpy arrays or scipy sparse matrices. Other types that are convertible to numeric arrays such as pandas DataFrame are also acceptable
* Using one of the many pandas read methods can be a great start: 'read_clipboard', 'read_csv', 'read_excel', 'read_feather', 'read_fwf', 'read_gbq', 'read_hdf', 'read_html', 'read_json', 'read_msgpack', 'read_parquet', 'read_pickle', 'read_sas', 'read_sql', 'read_sql_query', 'read_sql_table', 'read_stata', 'read_table'
* There are many libraries meant to load other types of data not covered here!
* For the class and project we'll now load our data straight from sklearn datasets that will provide it as a numpy matrix

##### Preparing the data
* All agorithms require a training dataset to create the ML model
* All agorithms require a validation dataset to validate the create ML model
* Supervised algorithms require both a X matrix (features) and a y array (labels)

* We'll use sklearn `train_test_split` method to separe the dataset for us, saving a set for a validation later. we'll use a validation dataset size between 30%-40% (common range for smaller sets)
* Initial cleaning of data should also be performed carefully not to strip the data of potentially valuable information. (Examples of cleaning data)
* Training: 60% Cross validation: 20% Testing: 20%

##### Training the model
* sklearn has a special type of processors called [estimators](https://scikit-learn.org/stable/tutorial/statistical_inference/settings.html), that are capable of creating ML models from data
* We'll be focusing on supervised methods that have the following interface:
`??? = model.fit(X,y)`
`??? = model.predict(X_to_predict)`
`??? = model.predict_proba(X_to_predict)` # classification only 0-1 how good
`??? = model.score` # classification only , score for each class first is predict
from sklearn.linear_model import LinearRegression or KNN
* Estimated Data

* regression and classification add some algorithms

lets look at the data new description, etc
sklearn Estimators (every alrogithm is an estimator): LinearRegression, 
Scikit-learn strives to have a uniform interface across all methods, and we’ll see examples of these below. Given a scikit-learn estimator object named model, the following methods are available:
http://scipy-lectures.org/packages/scikit-learn/index.html#a-recap-on-scikit-learn-s-estimator-interface
maybe run the code of a sample of each + chart (link to my exercise that we'll revisit later)
* The housing price example( get from andrew ng) - landsize, rooms vs price (embed above)
* Samples, features, target and label
* Dataset split: Train and Test
* Training/Fitting a model
* Checking model quality: error
* Using the model to predict new samples!

thinking on the plots from class 8, can we think of some specific variable sthat would make it easy to classify or regress my target variable? which ones were just noise?

* Let's look at some [examples](https://github.com/cce-bigdataintro-1160/spring2019/tree/master/class6-notebook) in order to learn how to:
  * Create plots
  * Create figures and subplots (axes)
  * Save figures to files
  * Decorate and customize plots
  * Explore datasets through plots
  * Add multiple plots to the same subplot(ax)

validating results:
http://scipy-lectures.org/packages/scikit-learn/index.html#gaussian-naive-bayes-classification

1. Using the dataset you chose for your project. Plot one chart of each type:
  - line `plot` passing one column(feature)
  - line `plot` passing two columns(features)
  - `scatter` plot passing two columns(features)
2. Make sure to add a `title`, `xlabel` and `ylabel` on each of the previous plots
3. Put the the 3 plots above on the same figure and save it on a single file
4. Play with the `color`, `linestyle`, `linewidth`, `marker`, `alpha` parameters of a `scatter` plot. You don't need to use multiple charts per figure anymore, just one is fine.
5. Use one more feature(column) to play with the `size` parameter of a `scatter` plot
6. Do a multifeature plot! Plot 3+ `scatter` plots on the same `ax` comparing one variable to other columns at the same time. Make sure to add a `legend` to make your multifeature chart easier to read. 
7. Modify the previous chart to use the `size` and `color` parameters. Tip, the `size` can be based on one of the features!
8. Explore your dataset by plotting scatter plots comparing all columns 2 at a time. Tip, use nested for-loops for this!

Using PCA to quickly have an overview on classification problems
http://scipy-lectures.org/packages/scikit-learn/index.html#visualizing-the-data-on-its-principal-components

* Optimizing our model
* Cleaning is also one of the most important steps at this stage: (some methods from pandas and sklearn to help), but we'll start 

##### Machine Learning in Big Data

##### About choosing the best algorithm to solve
* [Supervised Learning algorithms](https://scikit-learn.org/stable/supervised_learning.html): sklearn list of supervised learning algorithms
* [scikit-learn algorithm cheatsheet](https://scikit-learn.org/stable/tutorial/machine_learning_map/index.html): excellent starting point for deciding which algorithm to use when training models

##### Final Notes on Machine Learning
Supervised
Classification
* Self Driving Cars: Camera seeing what car, truck or person (maybe show video of robot identifyin things)
Regression


* Machine Learning in real life
  * Web search
  * Credit Scoring
  * Pricing recommendations
  * Cyber Security and intrusion detection
  * Advertisement and product recommendation
  * Suggestions, based on your watcher movies and ratings
  * Customer classification
  * Problems classification
  * Text recognition
  * Natural Language recognition
  * Computer vision
  * Finantial models
  * Email Spam Filtering
  * Evolution of call centers to ChatBots
  * Stocks algorithms
  * identify what's in a picture, a camera film, etc (a cat? a known criminal? a malign tumor?)  
  * cluster similar songs into automatically generated playlists (spotify)
  * show google api in action, maybe some other apis (aws for example)
  Fraud data
Unsupervised

cleaning up data
feature selection
pca for visualization and explanation
what happens when you use your ttrain set for validation?

cross validation http://scipy-lectures.org/packages/scikit-learn/index.html#cross-validation

### Optional homework(no need to submit)
* Read the machine learning introduction in: [this link](http://scipy-lectures.org/packages/scikit-learn/index.html#introduction-problem-settings), in particular, sections `3.6.1` to `3.6.5`. Don’t worry if this is a bit complex right now - it’ll really vary based on your math background.

### Recommended Readings
* [Visualization of Multi Dimensional data](https://towardsdatascience.com/the-art-of-effective-visualization-of-multi-dimensional-data-6c7202990c57): Excellent article about the challenges and solutions to visualize multi dimensional data


https://scikit-learn.org/stable/tutorial/index.html
https://scikit-learn.org/stable/tutorial/text_analytics/working_with_text_data.html
