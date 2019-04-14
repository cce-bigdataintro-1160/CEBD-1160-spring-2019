# Python Advanced Features

### Agenda
* Homework Check
* Learning Python Advanced features
* Homework

### Python Advanced Features

##### Goals
Get to know a few Python Advanced language constructs that can make your code cleaner and better.

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

### Optional homework(no need to submit)

### Recommended Readings
https://docs.python.org/3/tutorial/index.html

### Advanced exercises material

