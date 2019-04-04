
# Python Data Structures and Conditionals

### Agenda
* Homework Check
* Intro to Python Data Structures
* Flow Control with conditionals
* Homework

### Intro to Python Data Structures

##### Goals
Get acquainted with the Python language, that we'll use for data exploration and manipulation.

##### The environment
1. Check what's the type of the following values in the python shell:
   * `1`
   * `3.14`
   * `"Big Data!"` and `'Big Data!'`
   * `True` and `False`
   * [1,2,"intruder",3]
2. Get some help on the value `True`

##### Numbers
1. Write an equation that uses division, multiplication, an exponent, subtraction and an addition that is equal to 42.5. Assign the result to the variable `result`
2. Find out if 45234 is divisible by 4

##### Strings
1. Given the string `big data` give two commands that can print `d`.
2. Given the string `big data` give two commands that can print `g da`
3. Reverse the string `big data` in two different ways
4. Given the strings `big` and `data`, produce the string `big data`

##### Booleans
1. Can you write an expression that evaluates if a string is a palyndrome? i.e. `'abba'` should be True and `'rock'` should be False.

##### Lists, Tuples and Sets
1. Can you replace `big data` with `BIG DATA` in the list `['a',2,['b',4,5,'big data']]`
2. What's the difference between `[1,2,3] + [4]` and `[1,2,3].append(4)`
3. Find the unique elements in the list `[3,333,333,3,3,3333,3,3333,333,3,333333,3]`
4. Return all between(non-inclusive) 4 and 8 on the list `[1,2,3,4,5,6,7,8,9]`
5. Return the element `nested` in the list `[1,2,'a','b',[0,0,'nested'],5,'c']`
6. Count the occurrences of `token` on the list  `['rat','dog','cat','token','elephant','token','token']`

##### Dictionaries
1. Retrieve the value cat from `{'simple_key':'cat'}`
2. Retrieve the value dog from `{'k1':{'k2':'dog'}}`
3. Retrieve the value bird from `{'k1':[{'nested':['not_me',['bird']]}]}`

###### Using Scripts
1. Write a script called `hello_script.py`. It should take one number as input. If the number is equal to 42 print `right answer to life the universe and everything`. If the number is not 42 print `wrong answer`. If the input is not a number print `Sorry, invalid input, expecting number`.

##### Flow Control with Conditionals
1. A script that returns the lesser of two numbers if both numbers are odd, but returns the greater one if one or both numbers are even!
2. A script that receives two parameters and returns True if the sum of both is 50 or if one of the integers is 20. If not, return False

##### Loops
1. A script that prints the integers from 1 to 100. For multiples of three print "Fizz" instead , and for the multiples of five print "Buzz". For numbers which are multiples of both print "FizzBuzz"
2. Can you find the maximum or minimum integer value in a list.
3. If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23.
Find the sum of all the multiples of 3 or 5 below 1000.

##### Error
1. Write a script that can convert a string into an int and print its value and type on the console. If the value can't be converted print: `bad string {} couldn't be cast to int`
2. ???

##### Files
1. Open and print the titanic train.csv file. Prefix the line by `Male: ` and `Female: ` according to the gender of the person. Output the prefixed text and output the final count for each.
2. Open and print the [boston.housing](https://archive.ics.uci.edu/ml/machine-learning-databases/housing/housing.data). Can you print it value by value?

### Homework
* Don't forget to fill up the Weekly Journal! 

##### Basic
1. Complete the "homework" section of the "our_csv_parser.py" file in this repository, and upload it to your own Github repo (use either the Boston data or another from the ski-kit learn toy datasets): https://github.com/cce-bigdataintro-1160/class3-hwk
*important* point for the Python homework: do not import any libraries for this. There are many that can help, but the point of doing it the hard way first is to gain experience, understanding, and appreciation of what they do :)
2. Learn the Difference between Docker (https://docker.com) and Singularity (https://www.sylabs.io/docs/), and write 3-4 sentences of your own words when you’d use one or the other, and upload this to the same Github repo  as part 1.
3. Install Docker community edition on your personal computers

##### Advanced
1. Complete [Introduction to Python Software Carpentry](http://swcarpentry.github.io/python-novice-inflammation/). You'll need to import the library numpy to do this! ()
  
##### Reach
1. From your list of python values completed in 1, create a new list for each of the columns in the dataset (i.e. if there are 10 columns/features, extract each feature into its own list, and print them)

### Optional homework
* What commands we learned are useful for data exploration and why?
* Do a quick research explaining what are the main pros and cons of the Python language.

### Recommended Readings
* [Official Python3 Documentation](https://docs.python.org/3/)
* [Python3 Reference](https://docs.python.org/3/library/index.html)
* [Python3 Tutorial](https://docs.python.org/3/tutorial/index.html)
* [Python Coding Style Guidelines](Python Coding Style (https://www.python.org/dev/peps/pep-0008/))


### Advanced exercises material
* Can you complete these challenges from [cmdchallenge](https://cmdchallenge.com/)
* Learn what git does visually with [Git Branching](https://learngitbranching.js.org/)
