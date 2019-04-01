
# Intro 2 Linux & Version Control

### Agenda
* Homework Check
* Intro to Shell
* Intro to Git
* Homework

### Intro to Shell

##### Goals
Establish the foundation for our data analysis by understanding how the Linux shell works:
##### Be able to Navigate through the file system:

1. What is the `/` path? What does it contain?
2. Navigate to`/var/log` and list its files. What do we have here?
3. Type `cd ../../Users/<myusername>` Can you check your current dir? Can you list all the files in it recursively?
4. Type `cd` to move to your home. Now test both commands below and explain the difference:
    `cd Desktop`
    `cd /Desktop`
5. Assuming your current working directory is your Desktop, what `cd ~`, `cd .`, `cd ..` and `cd /` does?
6. List all the files that have been modified in the `/etc` folder, ordered by last modification date.

##### Work with Files and Directories

1. Create a `file foods.txt` using the `nano` editor containing your 3 favorite food.
2. Create a file `editor.fav` using the `vim` editor containing your favorite editor
3. Create a file `default-editor` using the `open` command. What editor does it bring? Save the name of the editor in the file.
4. Create a directory called `learning-shell` and move both your `editor.fav` and default-editor files is it.
5. Copy the directory to `/Users/<myusername>/Desktop` with all the files in it
6. Navigate to the directory where the files are and crete a new sub-directory called `nested-directory`. Move into it and check your current location.
7. Now copy everything under `/Users/<myusername>/Desktop/learning-shell` as `/Users/<myusername>/mybackup` 
8. Rename all files under `/Users/<myusername>/mybackup` adding the `bkp-` prefix to them.
9. Move your `foods.txt` into the backup folder, renamed to `bkp-foods.txt`
10. Delete your `/Users/<myusername>/Desktop/learning-shell` directory.

##### Use External Tools and Gnu Core Tools to enhance your shell skills. Compose them using pipes and filters.

1. Download the `titanic.zip` file from Slack and without using the UI, unzip it.
2. Can you provide the dimensions of this file `train.csv`?
3. List the first 5 rows of the file. Now list the last 5.
4. Print this file in your screen using `cat`, `less` and `more`.
5. Can you print only the names of all people in the file?
6. Print this file in reverse order and save it's output to train_reverse.txt.
7. Can you explain the command `du -a . | sort -n -r | head -n 20` and why would you use it? 
8. Print only the `cd` commands you did today.
9. Print all the `pid` of all `python` processes running.

##### Write loops to iterate over lists

1. Download the `ultratrail-du-montblanc.zip` file from Slack and without using the UI, unzip it to `/Users/<myusername>/ultratrail`
2. Write a loop that prints the name, dimensions and first 2 lines for each of the `.csv` files.
3. Write a loop that copies each of the `.csv` files with the prefix `bkp-` to a folder `/Users/<myusername>/ultratrail/backups`. 

##### Create scripts to automate basic processes

1. Write a script that allows the user to pick their favorite color, then save it to color.txt and print it to the console.
2. Write a script that backups up and cleans directories '/Users/<myusername>/veryimportant/*.csv' and '/Users/<myusername>/ultraimportant/*.xls'. How can we automate it's daily execution?

##### Finding files and contents in files

1. Download the `titanic.zip` file from Slack and without using the UI, unzip it.
2. Find the person called `Torborg` in the file `train.csv`
3. Count how many people were male and female in the file
4. Count how many people called `John` are in the file and how many of them are male or female
5. Find all csv files in your home directory

### Intro to Git

##### Goals
Learn the basics of a versioning control system to enable work organization and collaboration

##### Understanding the necessity for a versioning system
1. How do you currently collaborate in your work? What's the versioning system used there?

##### Creating a repository and doing your first commit.
1. Create a directory called `my-first-repo`. Navigate to it and initialize a `git` repository. Check it's status
2. Add a few files with a few lines of text each in the directory and check the status again.
3. Use `git add` to add one of those files to your staging area. Check the status
4. Use `git commit` to commit that file to git. Check the status
5. Use `git add` to add a second of those files to your staging area. Use `git commit` to commit that file to git. Check the status 
6. Use `git log` to see the history of your actions and `git diff` to see what are the changes in each commit
7. Add a few files to your staging area. Are you able to revert it?

##### Create a branch to split your development
1. Create a branch called `my-branch` and add a commit to it.
2. Checkout your `master` and create another branch. Add two commits to it.
3. Checkout your master again and merge both branches into it.
4. Visualize with `git log --graph --oneline --decorate --all` what happened.

##### Collaborate using git
1. Push all of your changes in your current repository to a remote git repository in GitHub.
2. Clone my existing repository into your local machine.

##### Ignore files that don't need versioning
1. Create a .gitignore file and test it with a file

##### Understand what licensing is

### Homework
* Don't forget to fill up the Weekly Journal! 

##### Basic
1. Find a text editor you like! Any text editor should do. A few recommendations are: Visual Studio Code, Atom, Komodo and Vim but feel free to explore!
2. Install `git`/`bash` on your local machine at home, recommended steps here: [Shell Setup](http://swcarpentry.github.io/shell-novice/setup.html)
3. Install `python`, recommended steps here: [Git Setup](http://swcarpentry.github.io/python-novice-inflammation/setup/). For Windows, I’d strongly recommend Option 3 (via Installing it through [Anaconda](https://www.anaconda.com/distribution/)) as it will make future steps much easier.
4. Complete the Software Carpentry Unix lesson send me what this command does: `$ wc -l * | head -n 3 | sort -n`

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

### Recommended Readings
* [Git Documentation](https://git-scm.com/doc)
* [Git CheatSheet](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet)
* [Gnu Core Utils](http://www.gnu.org/software/coreutils/manual/html_node/)

### Advanced exercises material
* Can you complete these challenges from [cmdchallenge](https://cmdchallenge.com/)
* Learn what git does visually with [Git Branching](https://learngitbranching.js.org/)
