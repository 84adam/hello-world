<html>
<body>

<h2>Learning to use GitHub</h2>

From the Feb. 18, 2016 Galvanize Meetup: "GitHub & Git". This is the process I followed to create this "hello-world" repository locally on my Windows machine, and then add, commit, and push it to my GitHub account.

<h3>The Setup</h3>
<ol>
<li>download git for windows http://git-scm.com/downloads</li>
<li>use all default settings when installing</li>
<li>create a GitHub account if you have not yet</li>
<li>get a text editor (Atom, Notepad++, etc.) if you don't have one yet</li>
<li>go to https://github.com/GalvanizeOpenSource/Learn-To-Code-GitHub-Git</li>
<li>read the instructions there</li></ol>

<h3>Getting Started</h3>
<ol>
<li>Navigate to the place you want to create your folder with Git (use: cd <dir name>)</li>
<li>See what’s in that folder (use: ls)</li>
<li>Create a new directory called “hello-world” (type: mkdir hello-world)</li>
<li>Navigate to that new folder (type: cd hello-world)</li>
<li>Initialize that folder for Git (type: git init)</li></ol>

<h3>Configuring the Git client:</h3>

<strong>Configure computer so that Git knows who is making changes:</strong>

1. Open up your Git Bash and enter in the following commands:
    $ git config --global user.name "<Your Name>"
2. Now set your email:
    $ git config --global user.email "<youremail@example.com>"

Your computer should now configured to you and your email address.

<hr />

<h3>Exercise: Create a basic text file</h3>

<ol><li>Open up your text editor (download one from http://atom.io).</li>
<li>Write a few lines of text</li>
<li>Save the file as “readme.txt” to your folder, “hello-world”</li></ol>

<h3>Learn This Pattern:</h3>

Status, Add, Commit: Save your changes in Git
   <ol><li>STATUS</li>
    <li>ADD</li>
    <li>COMMIT</li></ol>

<strong>Any time you want to save changes in Git, you must follow this 3-step command process:</strong>

* Step 1: Check the status
    $ git status // checks the changes you’ve made to this folder 
* Step 2: Add the changes for commitment
    $ git add <FILENAME> // add the files you’d like to commit (save) to change
* Step 3: Commit the changes with a message
    $ git commit -m “<your commit message>” // save your changes with a MANDATORY note

<hr />

<h3>Working Remotely</h3>

Now that you've got a taste of working locally, let's take it up a notch. First, we need to re-configure your Git to work with your GitHub.

<h3>Configure Git for GitHub</h3>

1. In Bash, enter in the command to sync your folder with your GitHub account:
    $ git config --global user.username "USeRnAMe" // this is case-sensitive and does not need "<" or ">"
2. Verify that the configuration was successful here:
    $ git-it verify
	NOTE: error - "command not found"
	
<h3>Pushing to GitHub</h3>

Push = upload code to GitHub from your local computer.

<h3>Exercise: Create a Remote Repository in GitHub</h3>

    1. Go to github.com, log in, and click the '+' in the top right to create a new repository.
    2. Give it a name that matches your local repository's name, 'hello-world', and a short description.
    3. Make it public.
    4. Don't initialize with a README because we already have a file, locally, named 'readme.txt'.
    5. Leave .gitignore and license on 'none'.
    6. Click create repository!

<h3>Connecting the remote to your GitHub repo</h3>

In Bash, in the folder of your choosing, perform the following:

    1. $ git remote add origin <URLfromGitHub>
	Bonus: you can also change the remote to another URL:
    2. $ git remote set-url <RemoteName> <URL>

<h3>Time to push changes!</h3>

Here is the command to push from your original remote copy to the GitHub master:

    $ git push origin master

</body>
</html>
