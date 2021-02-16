# Practice repository to start learning Git

## Commands used
 mkdir -p ~/code/git-practice
 cd ~/code/git-practice/
 git init
 atom .

 # We create the README.md
 # We create two directories dir1 and dir2 with fileA and file B
 git status  
 git add README.md dir1/ dir2/
In vim press i
Write the changes of the code
Esc -> :wq-> enter
 git status

- git init: Create a repository
- git status: Compare working directory, staging area,  and
current branch  
- git add: Add changes from working directory to staging area
- git commit: Commit changes from staging area to current branch
- git config: Set or get configuration
- git log: Show history of project commits
## Commit messages

Default editor is vim( this cab be changed)
- 'i' to enter *insert* mode
- Type commit message
- 'Esc'-> ':wq' -> 'Enter' to write message and quit
Or use 'git commit -m' " <Message>"
- First line should be clear, acccurate and concise
- Use proper spelling, grammar, and punctuation
- Don't end with a '.'

For more advice, see: https://chris.beams.io/posts/git-commit/
                      https://www.youtube.com/watch?v=USjZcfj8yxE


## Synchronize your local git repo to github

We open our account in www.github.com
Create a new repository
A repository contains all project files
We select Public if we want to share our project
Commit the files that you've staged in your local repository.
$ git commit -m "First commit"
# Commits the tracked changes and prepares them to be pushed to a remote repository. 
At the top of your GitHub repository's Quick Setup page, click  to copy the remote repository URL.
Copy remote repository URL field
In the Command prompt, add the URL for the remote repository where your local repository will be pushed.
$ git remote add origin  <REMOTE_URL> 
# Sets the new remote
$ git remote -v
# Verifies the new remote URL

Push the changes in your local repository to GitHub.
$ git push origin main
# Pushes the changes in your local repository up to the remote repository you specified as the or








##... push an existing respository from the command line
In our  local console we use
git remote add origin <REMOTE_URL> 
git push -u origin master









### Add new branch on github

create new file called extra.txt

git add extra.txt

git commit -m " adding an extra.txt file"

git push -u origin extra


For more advice, see: https://www.youtube.com/watch?v=nhNq2kIvi9s



## Adding an existing project to GitHub using the command line

Create a new repository on GitHub. To avoid errors, do not initialize the new repository with README, license, or gitignore files. You can add these files after your project has been pushed to GitHub.

Create New Repository drop-down

Open Terminal.

Change the current working directory to your local project.

Initialize the local directory as a Git repository.

$ git init

Add the files in your new local repository. This stages them for the first commit.

$ git add .

 Adds the files in the local repository and stages them for commit. To unstage a file, use 'git reset HEAD YOUR-FILE'.
Commit the files that you've staged in your local repository.

$ git commit -m "First commit"

 Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this commit and modify the file, use 'git reset --soft HEAD~1' and commit and add the file again.
 
At the top of your GitHub repository's Quick Setup page, click  to copy the remote repository URL.
Copy remote repository URL field
In Terminal, add the URL for the remote repository where your local repository will be pushed.

$ git remote add origin remote repository URL

 Sets the new remote
 
$ git remote -v

Verifies the new remote URL

Push the changes in your local repository to GitHub.

$ git push -u origin master

 Pushes the changes in your local repository up to the remote repository you specified as the origin
 
 
 
 
 You can clone a repository from GitHub to your local computer to make it easier to fix merge conflicts, add or remove files, and push larger commits. When you clone a repository, you copy the repository from GitHub to your local machine.

Cloning a repository pulls down a full copy of all the repository data that GitHub has at that point in time, including all versions of every file and folder for the project. You can push your changes to the remote repository on GitHub, or pull other people's changes from GitHub. For more information, see "Using common Git commands".

You can clone your existing repository or clone another person's existing repository to contribute to a project.

Tip: You can also clone a repository using the GitHub CLI. For more information, see "gh repo clone" in the GitHub CLI documentation.

Cloning a repository using the command line
On GitHub, navigate to the main page of the repository.

Above the list of files, click  Code.

"Code" button
To clone the repository using HTTPS, under "Clone with HTTPS", click . To clone the repository using an SSH key, including a certificate issued by your organization's SSH certificate authority, click Use SSH, then click . To clone a repository using GitHub CLI, click Use GitHub CLI, then click .

The clipboard icon for copying the URL to clone a repository
The clipboard icon for copying the URL to clone a repository with GitHub CLI
Open Git Bash.

Change the current working directory to the location where you want the cloned directory.

Type git clone, and then paste the URL you copied earlier.

$ git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY
Press Enter to create your local clone.

$ git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY
> Cloning into `Spoon-Knife`...
> remote: Counting objects: 10, done.
> remote: Compressing objects: 100% (8/8), done.
> remove: Total 10 (delta 1), reused 10 (delta 1)
> Unpacking objects: 100% (10/10), done.


GitHub: Permission denied (publickey). fatal: The remote end hung up unexpectedly

I have followed these instructions below to upload a project.

Global setup:

 Download and install Git
  git config --global user.name "Your Name"
  git config --global user.email tirenga@gmail.com
  Add your public key


Next steps:

  mkdir tirengarfio
  cd tirengarfio
  git init
  touch README
  git add README
  git commit -m 'first commit'
  git remote add origin git@github.com:tirenga/tirenga.git
  git push origin master


Let us say 'yourWebApp' is the folder you have your local web app. Change it to the directory

cd 'yourWebApp'
Init git in the folder

git init
Now add your github url as a remote

git remote add origin git://github.com/somename/Web-App.git
Here origin is the short name for your url

Now pull the read me file from the github repo

 git pull origin master
Now push your web app to the github repository

git push origin master
