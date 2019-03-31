
# *Intro 2 Linux & Version Control*

# Agenda
* Homework Check
* Intro to Shell
* Intro to Git
* Homework

# Intro to Shell

### Goals
* Establish the foundation for our data analysis by understanding how the Linux shell works:
  * Be able to Navigate through the file system
  * Work with Files and Directories
  * Use gnu core tools and compose them with pipes and filters
  * Write loops to iterate over lists
  * Create scripts to automate basic processes
  * Find files and directories accross the filesystem

### Exercises
* How do I customize my bash environment?
* Print your history file in reverse order!
* Can you explain the command ```du -a . | sort -n -r | head -n 20``` and why would you use it? 
* Print all the pid's of all python processes running.
* Write a script that allows the user to pick a food. Print and store it in the food.out file.
* [Introducing the Shell](http://swcarpentry.github.io/shell-novice/)

# Intro to Git

### Goals
* Learn the basics of a versioning control system to enable work organization and collaboration
  * Create a git repository and commit to it
  * Track changes and see the history of changes
  * Add remotes and push code to GitHub
  * Understand how licensing works

### Exercises
  - You accidentally committed with an ugly message, can you fix it?
  - How can you display all your latest commits? What about the topology?
  - How to remove a file you accidentally added to the staging area?
  - How can i see differences between local and remote?
  - How to see what I'm about to commit?
  * [Introducing Git](http://swcarpentry.github.io/git-novice/)

# Homework
* Don't forget to fill up the Weekly Journal! 

## Basic
1. Find a text editor you like! Any text editor should do. A few recommendations are: Visual Studio Code, Atom, Komodo and Vim. 
2. Install `git`/`bash` on your local machine at home, recommended steps here: [Shell Setup](http://swcarpentry.github.io/shell-novice/setup.html)
3. Install `python`, recommended steps here: [Git Setup](http://swcarpentry.github.io/python-novice-inflammation/setup/). For Windows, I’d recommend Option 3 (via Installing it through Anaconda) as it will make future steps much easier.
4. Complete the Software Carpentry Unix lesson send me:
```$ wc -l * | head -n 3 | sort -n``` ???

## Advanced
1. Complete Software Carpentry Git lesson as best as you can: [Git Novice](http://swcarpentry.github.io/git-novice/). We will plan to spend up to 1 hour in class next week going over `git`, depending on how successful the class is at the following reach challenge.
  
## Reach
1. Be a `git` master! That is, do the following *from scratch*:
  * create a new repository on Github, with a license and a readme
  * clone it locally
  * create a new text file that contains at least 1 line of text
  * add your file to the repository
  * commit your changes
  * edit the README file that came in the repo in some way
  * commit your changes
  * push your changes to Github
  * send me the url for your Github repository

# Optional homework
* What commands we learned are useful for data exploration and why?
* Can you complete these challenges from [cmdchallenge](https://cmdchallenge.com/)
* Learn what git does visually with [Git Branching](https://learngitbranching.js.org/)
* Python Basics!!!

# Recommended Readings
* [Git Documentation](https://git-scm.com/doc)
* [Gnu Core Utils](http://www.gnu.org/software/coreutils/manual/html_node/)
