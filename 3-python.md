
# Python Data Structures and Conditionals

### Agenda
* Homework Check
* Intro to Python
* Homework

### Intro to Python

##### Goals
Get acquainted with the Python language, that we'll use for data exploration and manipulation.
* [Software Carpentry Python Lesson](http://swcarpentry.github.io/python-novice-inflammation/index.html): Software Carpentry Lesson on Python basics for data manipulation
* [Python Basics Reference](https://pythonbasics.org/): Python basics simplified syntax for using Python basics

##### The Python Shell
1. Check what's the type of the following values in the python shell:
   * `1`
   * `3.14`
   * `"Big Data!"` and `'Big Data!'`
   * `True` and `False`
   * [1,2,"intruder",3]
2. Get some help on the value `True`
3. Write an equation that uses multiplication, subtraction and an addition that is equal to 42.5. Assign the result to the variable `result` and print it
4. Given the string `big data` give two commands that can print `d`.
5. Can you replace `big data` with `BIG DATA` in the list `['a',2,['b',4,5,'big data']]`

##### Writing a Python script
1. Write a script called `testing_scripts.py` with the following content below, run it using `python3 testing_scripts.py`:

```
#!/usr/bin/env python3

mynumber=1
myfloat=3.14
mystring="Hello World!"
myboolean=True
mylist=[1,2,3,4,5]

#Complete this script by 
#- printing each one of the variables above
#- printing the type of each of the variables above
```

2. Write another script called `hello_script.py`. It should take one number as input. If the number is equal to 42 print `Right answer to life the universe and everything`. If the number is not 42 print `wrong answer`. If the input is not a number print `Sorry, invalid input, expecting number`.
3. Add, commit and push these two scripts to the `class3-notebook` repository in GitHub!

##### Reading datasets with Python
1. Create a script called `my_csv_reader.py` that's able to read a file and that checks it's a valid file. If it is print `I have a file to process`, otherwise print `Boo, no file for me.`
2. Expand this script to read a csv dataset and print it to the screen line by line. Use any of the toys dataset for this!
3. Expand this script by printing each line as a list of values. Example:
   The line:
   ```
   abc,cde,efg,1,2,3
   ```
   in the source dataset should become:
   ```
   ['abc','cde','efg','1','2','3']
   ```
4. Add, commit and push this script to the `class3-notebook` repository in GitHub!

### Additional Exercises Material
* [Extra exercises](./3-python-exercises.md): Additional exercises to practice each Python topic

### Optional homework(no need to submit, preparation for next class)
* Read the `Part 1: Orientation` and `Part 2: Containers` from [Docker Getting Started](https://docs.docker.com/get-started/)
* Research what is a Python external `library` and what can you do with it.
* Research what are the `numpy` and `pandas` python libraries and what they're used for.

### Recommended Readings
* [Official Python3 Documentation](https://docs.python.org/3/): Python3 documentation page
* [Python3 Reference](https://docs.python.org/3/library/index.html):  Python3 reference pages containing all base types
* [Python3 for beginners tutorials](https://wiki.python.org/moin/BeginnersGuide/NonProgrammers): Several Python references for studying, all recommended for beginners
* [Python Coding Style Guidelines](https://www.python.org/dev/peps/pep-0008/): Coding style guidelines for Python if you want to make your code look good
