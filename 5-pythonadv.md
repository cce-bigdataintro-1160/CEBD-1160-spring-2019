# Python Functions, Libraries & Numerical Analysis

### Agenda
* Homework Check
* Learning Python Functions
* Learning Python Numerical Analysis with Numpy and Pandas
* Homework

### Python Advanced Features

##### Goals
Understand some extra concepts of the Python language and start to manipulate data using libraries. By the end of this class you'll be able to:
* Plan ahead on before creating your scripts with the use of pseudocode, nothing more than expressing your objectives before you start coding
* Pass validated arguments to scripts using the argparse library
* 
Get to know a few Python Advanced language constructs that can make your code cleaner and better.
Get to know a the most important numerical analysis Python libs and how to apply them to process our datasets.

##### What is pseudocode
[Pseudocode in Wikipedia](https://en.wikipedia.org/wiki/Pseudocode): Article describing Pseudocode and what's it used for

##### Passing Arguments
[The argparse library](https://docs.python.org/3/library/argparse.html): Library that allows us to pass arguments in an organized way to scripts
1. Write a script that allows the user to pass in a filename as an argument. Using that filename, print the file contents.
2. Repeat exercise 1. using the argparse library.

##### Creating your own functions
1. Create a new script called `data-preparer.py`
2. Add a function that receive as row as a parameter and that returns that row in lower case.
3. Add a function that receive as row as a parameter and that checks each field of the row. In case the field is empty (or `""`), it should be replaced with the value `"empty"`. The method should return the updated row.
4. Finalize you script by writing the part that calls both functions:
* Your program should open a provided file as an argument
* Iterate over each row of the file
* Apply the first and second functions on each row
* Save the results of the `data-preparer.py` in a `clean-file.csv` output file

##### Importing and Using Libraries

##### Numerical Analysis with Numpy Arrays
[numpy Docs](https://www.numpy.org/devdocs/): numpy Documentation
[numpy Quick Start](https://www.numpy.org/devdocs/user/quickstart.html): A few quick recipes to using Numpy
1. Create your first array with the elements [1,22.4,5,35,4,6.7,3,8,40]. Experiment what the following functions do: ndim, shape, size, dtype, itemsize and data.
2. Create numpy array from 1 to 10 using the arange function.
3. Create a numpy array with five 0s, another with five 1s, and another with five 6s. Use the zeros and the ones function.
4. Create a random array of 20 x 20 dimensions, calculate the mean, min, max and std error for the matrix. Now do it for the first column.
5. Create an array with 9 values and reshape it to a 3 x 3 matrix.
add slicing

##### DataFrames with Pandas
[pandas Docs](http://pandas.pydata.org/pandas-docs/stable/): pandas Documentation
[pandas Quick Start](http://pandas.pydata.org/pandas-docs/stable/getting_started/10min.html): A few quick recipes to using DataFrames

7.load from csv, xls, html, sql
1. Create a pandas Series using the list [1,2,3]. Now add the index with ['a','b','c'].
2. Create a pandas DataFrame with 4 rows and 3 columns. Add indexes and columns to it. (add some theme here)
3. Still using the same data frame, select the two first column and provide the dataframe statistics for it.
4. Still using the same data frame, remove the third column.
5.dropna and fillna
6.unique value_counts, is_null, head
filtering and valuecounts
describe info

something closer to salaries exerc

add ilocloc slicing
##### Plotting Charts with MatPlotLib
[matplotLib Docs](https://matplotlib.org/contents.html): matplotlib Documentation
[matplotLib Galleries](https://matplotlib.org/gallery/index.html): matplotlib Gallery with many plots to use for reference
[matplotLib Tutorials](https://matplotlib.org/tutorials/index.html): matplotlib Tutorials for Beginners, Itermediate and Advanced users.
1. figure
2. axes
3. types of inputs arrays or df.values

get the min max std and mean from numpy array on given 
slicing numpy?

### Optional homework(no need to submit)

### Recommended Readings
https://docs.python.org/3/tutorial/index.html

https://docs.python.org/3/tutorial/index.html

### Advanced exercises material