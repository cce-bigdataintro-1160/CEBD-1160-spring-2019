# Python Functions, Libraries & Numerical Analysis

### Agenda
* Homework Check
* What is pseudocode
* Creating your own functions
* Importing and Using Libraries
* Numerical Analysis with Numpy Arrays
* DataFrames with Pandas
* Plotting Charts with MatPlotLib
* Homework

### Python Advanced Features

##### Goals
Understand some extra concepts of the Python language and start to manipulate datasets using libraries. By the end of this class you'll be able to:
* Plan ahead on before creating your scripts with the use of pseudocode
* Create your own functions to apply repeatable code across your scripts
* Use the Numpy library to manipulate n-dimensional arrays
* Use the Pandas library to organize data in DataFrames and extract insights from it
* Use the Matplotlib library to generate simple plots from Datasets
* After leaning all of those utilities, we'll put this in practice by starting the creation of our final project using the chosen dataset

##### What is pseudocode
* [Pseudocode in Wikipedia](https://en.wikipedia.org/wiki/Pseudocode): Article describing Pseudocode and what's it used for
* it's nothing more than expressing your objectives in a speech-like language before you start coding, omiting complex details that would otherwise clutter your line of thought
* helps to focus on initial objectives when you lose track due to technical dificulties
* can be written in a way that it resembles the programming language, to facilitate implementation
* helps us identify simple challenges that can be hard to foresee

1. Write pseudocode for a program that reads the titanic file and saves two other files one for the male passengers and another for the female passengers

##### Creating your own functions
* [Function Definition](https://docs.python.org/3/tutorial/controlflow.html#defining-functions): Overview of how to define a function
* A function is a block of reusable code that can be written once and executed later (or never)
* The advantage of using functions is that you can write it once but call it multiple times, saving time and code
* Functions can receive values (aka parameters) and can return a result to the function `caller`
* We already know a few `built-in functions` like `len`, `help`, `open` and `enumerate`, they come from the [python standard library](https://docs.python.org/3/library/index.html)

1. We'll be using the titanic `train.csv` file for this exercise, and we'll categorize the gender of the passengers as `0` for male and `1` for female
2. In order to do that create a function called `categorize_gender` that receives a list of strings as a parameter and returns `0` if the passenger is man or `1` if is a woman
```
def categorize_gender(row):
   ???
   return row + [0 or 1]
```

3. Iterate over each row of the file applying your function
4. Add the result of your function call to each row of the dataset, producing a new list
5. Print your new list with an extra field

##### Importing and Using Libraries
* [Importing Libraries](https://docs.python.org/3/tutorial/modules.html#importing-from-a-package): How to import python existing libraries
* Libraries are packages of classes and functions with existing code
* In order to import packages in Python they either have to be part of the standard library or be installed manually using pip or the os package manager
* After the installation using libraries is as simples as using import statements like `import sys` or `import numpy as np`
* Some other libs that can contain useful functions are `time`, `random`, `os` and etc you can check the available methods in each lib by using the function `dir`
* Code for the libraries is also available through your IDE or through open repositories like GitHub

1. Write a python script that makes tests one functionality of each of the following imported libs: `argparse`, `sys`
2. Write a python script that makes tests one functionality of each of the following imported libs: `time`, `random`, `os`

##### Numerical Analysis with Numpy Arrays
[numpy Docs](https://www.numpy.org/devdocs/): numpy Documentation
[numpy Quick Start](https://www.numpy.org/devdocs/user/quickstart.html): A few quick recipes to use Numpy
* Numpy is a Linear Algebra Library for Python, and it's very fast because of it's native bindings
* The most important concept in Numpy are Array and Matrix and they'll initially look a lot like lists
* Many Data Science libs like pandas, sklearn and matplotlib rely on Numpy as base, and consequently take Numpy Arrays as inputs and outputs to it's methods
* We're going to learn the most important things we can do with Numpy arrays: how to create, slice, filter, reshape and aggregate Numpy vectors
* Numpy is also capable of loading files and parsing csvs

1. Create your first array with the elements `[1,22.4,5,35,4,6.7,3,8,40]`. Experiment what the following functions do: `ndim`, `shape`, `size`, `dtype`, `itemsize` and `data`.
2. Create your first matrix with the elements `[[1, 1],[2, 2],[3, 3]]`. Experiment what the following functions do: `ndim`, `shape`, `size`, `dtype`, `itemsize` and `data`.
3. Create numpy 1 dimension array using each of the functions `arange`, `zeros`, `ones`, `eye`, `linspace` and `rand`
4. Create numpy 2 dimensions matrix using each of the functions `arange`, `zeros`, `ones`, `eye` and `rand`
5. Create an array containing 20 times the value `7`. Reshape it to a 4 x 5 Matrix
6. Create a matrix of 6 x 6 containing random values between 0 and 0.999... print:
* only the first element on it
* only the first 2 rows for it
* only the last 2 rows for it
* only the mid 2 rows for it
* only the last column for it
* only the two mid columns and 2 mid rows for it
* only the lines containing XXX > 0.5
7. load the data from `insurance.csv` using numpy, then print: 
* the sum, average, max and min values for each feature(column)
* the sum, average, max and min values for each sample(row)


##### DataFrames with Pandas
[Pandas Docs](http://pandas.pydata.org/pandas-docs/stable/): main pandas documentation page
[pandas Quick Start](http://pandas.pydata.org/pandas-docs/stable/getting_started/10min.html): A few quick recipes to using DataFrames
* Library meant to help with data analysis using two new data structures: Series and DataFrames
* At first it will resemble a lot like numpy Arrays, but the big difference is that we can assign labels to our n dimensional, making it possible to create DataFrames, a table structure that can be used very similarly to Excel or SQL tables
* Has many productivity functions to facilitate data visualization, manipulation and cleaning
* Has many data loaders making it capable of integrating with many sources like csvs, xlsx, sql and html pages

1. Create a pandas Series using the list [1,2,3] and index ['a','b','c']. Explore the dataset using functions like `to_string()`, `index`, `dtypes`, `shape` and `describe()`
2. Create a pandas DataFrame to resemble this structure:
```
    Age   Name   Gender 
1    18   John   Male
2    17   Sandra Female
3    20   Mike   Male
```

Explore the dataset using functions like `to_string()`, `columns`, `index`, `dtypes`, `shape`, `info()` and `describe()`
3. Load the `insurance.csv` in a DataFrame using pandas. Explore the dataset using functions like `to_string()`, `columns`, `index`, `dtypes`, `shape`, `info()` and `describe()`. Use this DataFrame for the following exercises.
Print only the column `age`
Print only the columns `age`,`children` and `charges`
Print only the first 5 lines and only the columns `age`,`children` and `charges`
4. What is the average, minimum and maximum `charges` ?
5. What is the average, minimum and maximum `age` ?
6. What is the `age` and `sex` of the person that paid `10797.3362`. Was he a smooker?
7. What is the `age` of the person who paid the maximum charge?
8. How many insured people do we have for each `region`?
9. What is the average `bmi` in the `southwest` and `southeast` regions?
10. How many insured people are children?
11. Can you identify if there are any smokers among the children's dataset?
12. What do you expect to be the correlation between `charges` and the other fields? 
13. Using the method `corr()`, check if your assumptions were correct.


##### Plotting Charts with MatPlotLib
[matplotLib Docs](https://matplotlib.org/contents.html): Matplotlib Documentation
[matplotLib Galleries](https://matplotlib.org/gallery/index.html): matplotlib Gallery with many plots to use for reference
[matplotLib Tutorials](https://matplotlib.org/tutorials/index.html): matplotlib Tutorials for Beginners, Itermediate and Advanced users.

* one of the main libraries for scientifical data exploration, allows for quick prototyping and has all basic functionalities
* was built with the MATLAB interface as a reference
* compatible with Jupyter notebooks, facilitating it's usage on interactive python clients
* has a very rich gallery page with tons of examples that can be copied and modified
* allows users to save figures in high resolution for printing and supports many different formats

1. Still using the same DataFrame from the previous exercise `insurance.csv` plot the chart for `charges` and save it as `charges_plot.png`
2. plot the histogram for `bmi` and save it as `bmi_hist.png`
3. plot the scatterplot for `age` vs `charge` and save it as `age_charge_scatter.png`
4. Re-do the previous items, adding the title, x label and y label for each item.

##### Final Notes on Python Libraries
* These utilities are widely used in the industry and represent some of the most essential building blocks for data analysis
* Many worksplaces have unexplored datasets that can produce interesting insights, looks around for excel, csv, databases or html you can play with
* There are many other more specialized libraries and tools like: pyspark, tensorflow, plotly, but all of them require the basic understanding and assimilation of the concepts we learned

### Additional Exercises Material
* [Extra exercises](./4-docker-exercises.md): Additional exercises to practice each Docker topic

### Optional homework(no need to submit)
* Reserch the following matplotlib types of plots: `bar` and `pie`
* Research the library `seaborn`, another plotting library based on `matplotlib`
* Research the library `plotly`, another plotting library widely used for data analysis

### Recommended Readings
[Loading csv files in pandas](https://towardsdatascience.com/pandas-dataframe-playing-with-csv-files-944225d19ff): Tutorial explaining how to load CSV files in pandas DataFrames
[Loading excel files in pandas](https://datatofish.com/read_excel/): Tutorial explaining how to load excel files in pandas DataFrames
[Loading sql tables in pandas](https://stackoverflow.com/questions/10065051/python-pandas-and-databases-like-mysql): page explaining how to load sql tables in pandas DataFrames
[Loading html tables in pandas](https://beenje.github.io/blog/posts/parsing-html-tables-in-python-with-pandas/): page explaining how to load html tables in pandas DataFrames
