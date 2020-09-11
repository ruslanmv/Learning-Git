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
##... push an existing respository from the command line
In our  local console we use
git remote add origin https://github.com/......
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
