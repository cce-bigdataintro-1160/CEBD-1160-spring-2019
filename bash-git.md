# Intro 2 Linux & Version Control

### Agenda
* Homework Check
* Intro to Shell
* Intro to Git
* Homework

### A brief introduction to Linux
* [The Linux Ancestry](https://en.wikipedia.org/wiki/Unix#/media/File:Unix_history-simple.svg)
* [Linux list of distributions](https://en.wikipedia.org/wiki/List_of_Linux_distributions)

### Intro to Shell
* [The shell](./shell.png)
* [Bash, the Unix Shell](https://en.wikipedia.org/wiki/Bash_(Unix_shell))

##### Goals
Establish the foundation for our data analysis by understanding how the Linux shell works:
* [Gnu Core Utils](http://www.gnu.org/software/coreutils/manual/html_node/)
* [The man command - manual](http://www.linfo.org/man.html)
* [Software Carpentry Unix](https://swcarpentry.github.io/shell-novice/)

##### Be able to Navigate through the file system:
* [Filesystem Hierarchy Standard - Linux Standard Directories](https://en.wikipedia.org/wiki/Filesystem_Hierarchy_Standard)

1. Find out what's your username. Find your home folder and list its contents.
2. Navigate to `/` and list the contents of this directory. Why is this a special directory?
3. Navigate to `/var/log` and list its files. What do we have here?
4. From the previous dir `/var/log` type `cd ../../Users/<myusername>`, why is the new current directory special?
5. Test the following commands: `cd .`, `cd ..`, `cd /` and  `cd ~`. Can you explain what each of those symbols mean?
6. From your home directory test both commands below and explain the difference:
    `cd Desktop`
    `cd /Desktop`
7. What command can give you the most recently modified file in your home directory?
8. Download the file titanic.zip from Slack and locate it through the Terminal by listing it

##### Work with Files and Directories

1. Create a directory called `learning-shell` in your home directory.
2. Create a file (using vi or nano) called `a_dataset.csv` in your home directory, write a few csv lines in it and save it.
3. Print the contents of your file on the console/terminal screen.
4. Move the `a_dataset.csv` file in the `learning-shell` directory.
5. Print the contents of your file without navigating into the `learning-shell` directory. This means you have to print it from your home folder!
6. Copy the directory `learning-shell` to your `~/Desktop`.
7. Navigate to the copied `learning-shell` folder on your `~/Desktop` and create another directory inside it, called `nested-folder`. Navigate into it and check your current location, it should be `/Users/<myusername>/Desktop/learning-shell/nested-folder`
8. Inside your `nested-folder` directory, create a file called `precious-dataset.csv` (using vi or nano). Add a few precious lines in it.
9. Copy everything under `/Users/<myusername>/Desktop/learning-shell` to `/Users/<myusername>/Desktop/mybackup`
10. Rename all files under `/Users/<myusername>/Desktop/mybackup` adding the `bkp-` prefix to their names.
11. Check all of your changes using the MacOS UI
12. Delete your `/Users/<myusername>/Desktop/learning-shell` directory.

##### Use External Tools and Gnu Core Tools to enhance your shell skills. Compose them using pipes and filters.

1. Unzip (using the terminal) our `titanic.zip` file to `titanic`, 
2. Provide the shape/dimensions of the file `train.csv`?
3. List the first 5 rows of the file. Now list the last 5.
4. Print this file in your screen using `cat` now use the `less` command.
5. Can you print only the names of all people in the file?
6. Print this file in reverse order and save the output to train_reverse.txt.
7. Print only the lines 3 to 5 of the file?
8. Can you explain the command `du -a . | sort -n -r | head -n 20` and why would you use it? 
9. Print only the `cd` commands you did today.
10. Split the train.csv file in multiple files with 20 lines each. 

##### Write loops to iterate over lists

1. Download the `ultratrail-du-montblanc.zip` file from Slack and unzip it to `/Users/<myusername>/ultratrail`
2. Write a loop that prints the name, dimension and first 2 lines for each of the `.csv` files.
3. Write a loop that copies each of the `.csv` files with the prefix `bkp-` to a folder `/Users/<myusername>/ultratrail/backups`. 

##### Create scripts to automate basic processes

1. Write a script that suggests 5 data formats: csv, xlsx, pdf, doc and txt. It should allow the user to pick their desired extension then create a file named `selected.<extension selected>`. Use the read command to read the user input!
2. Write a script that removes the N number of lines of all files in '/Users/<myusername>/files_with_headers/*.csv'. If other people depend on this being done daily, wow can we automate it's daily execution at 8:00AM? N should be an argument passed before starting the script!

##### Finding files and contents in files

1. Find the person called `Torborg` in the file `train.csv`
2. Count how many people were male and female in the file
3. Count how many people called `John` are in the file and how many of them are male or female
4. Find all csv files in your home directory. Play with the -maxdepth flag to see the difference.

### Intro to Git
* [Official Pro Git Book](https://git-scm.com/book/en/v2)
* [Git Reference](https://git-scm.com/docs)

##### Goals
Learn the basics of a versioning control system to enable work organization and collaboration

##### Understanding the necessity for a versioning system
1. How do you currently collaborate in your work? What's the versioning system used there?

##### Creating a repository and doing your first commit.
1. Create a directory called `my-first-repo`. Navigate to it and initialize a `git` repository. Check it's status
2. Add a few files with a few lines of text each in the directory and check the status again.
3. Add one of those files to your staging area. Check the status
4. Commit that file to git. Check the status
5. Add a second of those files to your staging area. Commit that file to git. Check the status 
6. See the history of your actions and see what are the changes in each commit
7. Add a few files to your staging area. Are you able to revert it?

##### Undoing things
1. Undo a non-staged change
2. Undo a staged change
3. Undo a commited change
4. Reset your master branch to an older commit

##### Create a branch to split your development
1. Create a branch called `my-branch` and add a commit to it.
2. Checkout your `master` and create another branch. Add two commits to it.
3. Checkout your master again and merge both branches into it.
4. Visualize with `git log --graph --oneline --decorate --all` what happened.

##### Collaborate using git
1. Create a repository in GitHub, clone it and commit a file into it.

##### Ignore files that don't need versioning
1. Create a .gitignore file and test it with a file

##### Understand what licensing is
* [Licensing a Repository](https://help.github.com/en/articles/licensing-a-repository)
* [Choose a license](https://choosealicense.com/)

### Homework
* Don't forget to fill up the Weekly Journal! 

##### Basic
1. Make sure you have your `bash installed`, and then choose a text editor you like to use at home! Any text editor should do. A few recommendations are: Visual Studio Code, Atom, Komodo and Vim but feel free to explore!
2. Install `python`, recommended steps here: [Python Setup](http://swcarpentry.github.io/python-novice-inflammation/setup/). For Windows, I’d strongly recommend Option 3 (via Installing it through [Anaconda](https://www.anaconda.com/distribution/)) as it will make future steps much easier.
3. Complete the [Software Carpentry Unix](https://swcarpentry.github.io/shell-novice/) lesson send me what this command does: 
   `$ wc -l * | head -n 3 | sort -n`

##### Advanced
1. Complete Software Carpentry Git lesson as best as you can: [Git Novice](http://swcarpentry.github.io/git-novice/). We will plan to spend up to 1 hour in class next week going over `git`, depending on how successful the class is at the following reach challenge.
  
##### Reach
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

### Optional homework
* What commands we learned are useful for data exploration and why?
* Do a quick research explaining what are the main pros and cons of the Python language.

### Recommended References
* [Git Documentation](https://git-scm.com/doc)
* [Most popular Open Source licenses](https://opensource.org/licenses)
* [Interactive](https://explainshell.com/)

### Advanced exercises material
* Can you complete these challenges from [cmdchallenge](https://cmdchallenge.com/)
* Learn what git does visually with [Git Branching](https://learngitbranching.js.org/)
* Extension to use the shell like a boss: [Oh My Zsh](https://ohmyz.sh/)

