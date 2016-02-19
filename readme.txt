first readme text
testing git and github
galvanize meetup
February 18, 2016
...
set up:
1) download git for windows http://git-scm.com/downloads
2) use all default settings when installing
3) create a GitHub account if you have not yet
4) get a text editor (Atom, Notepad++, etc.) if you don't have one yet
5) go to https://github.com/GalvanizeOpenSource/Learn-To-Code-GitHub-Git
6) read the instructions there
...
starting up - try to do the following:
1) Navigate to the place you want to create your folder with Git (use: cd <dir name>)
2) See what’s in that folder (use: ls)
3) Create a new directory called “hello-world” (type: mkdir hello-world)
4) Navigate to that new folder (type: cd hello-world)
5) Initialize that folder for Git (type: git init)
...
Configure Your Git:
First step we need to do is configure your computer so that Git know who is making changes. 
1) Open up your Git Bash and enter in the following commands:
    $ git config --global user.name "<Your Name>"
2) Now set your email:
    $ git config --global user.email "<youremail@example.com>"
Your computer is now configured to you and your email address.
...
Exercise: Create a basic text file
1) Open up your text editor (download one from http://atom.io).
2) Write a few lines of text
3) Save the file as “readme.txt” to your folder, “hello-world”
...
...
Status, Add, Commit - saving changes in Git
    STATUS
    ADD
    COMMIT
...
Any time you want to save changes in Git, you must follow this 3-step command process.
* Step 1: Check the status
    $ git status // checks the changes you’ve made to this folder 
* Step 2: Add the changes for commitment
    $ git add <FILENAME> // add the files you’d like to commit (save) to change
* Step 3: Commit the changes with a message
    $ git commit -m “<your commit message>” // save your changes with a MANDATORY note
