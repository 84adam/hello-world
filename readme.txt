<H2>Hello, GitWorld!</H2>

These are my notes from the Feb. 18, 2016 Galvanize Meetup: "GitHub & Git". This is the process I followed to create this "hello-world" repository locally on my Windows machine, and then add, commit, and push it to my GitHub account.

<hr />

<H3>The Setup</H3>

<ol><li>download git for windows http://git-scm.com/downloads</li>
<li>use all default settings when installing</li>
<li>create a GitHub account if you have not yet</li>
<li>get a text editor (Atom, Notepad++, etc.) if you don't have one yet</li>
<li>go to https://github.com/GalvanizeOpenSource/Learn-To-Code-GitHub-Git</li>
<li>read the instructions there</li>

<H3>Getting Started</H3>

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
...
Working Remotely
Now that you've got a taste of working locally, let's take it up a notch. 
First, we need to re-configure your Git to work with your GitHub.
...
Configure Git for GitHub
1) In Bash, enter in the command to sync your folder with your GitHub account:
    $ git config --global user.username "USeRnAMe" // this is case-sensitive and does not need "<" or ">"
2) Verify that the configuration was successful here:
    $ git-it verify
	NOTE: error - "command not found"
	

Pushing to GitHub

Pushing is another way to say that we're doing to upload code to GitHub from your local computer.

    Gut check: what's the difference between PUSHING and COMMITTING?

Exercise: Create a Remote Repository in GitHub

    Go to github.com, log in, and click the '+' in the top right to create a new repository.
    Give it a name that matches your local repository's name, 'hello-world', and a short description.
    Make it public.
    Don't initialize with a README because we already have a file, locally, named 'readme.txt'.
    Leave .gitignore and license on 'none'.
    Click create repository!

Connect the remote to your GitHub repo

In Bash, in the folder of your choosing:

$ git remote add origin <URLfromGitHub>

Bonus: you can also change the remote to another URL:

$ git remote set-url <RemoteName> <URL>

Time to push!

Here is the command to push from your original remote copy to the GitHub master:

$ git push origin master

