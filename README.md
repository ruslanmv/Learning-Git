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


## Synchronize your local git repo to github

We open our account in www.github.com
Create a new repository
A repository contains all project files
We select Public if we want to share our project
##... push an existing respository from the command line
In our  local console we use
git remote add origin https://github.com/......
git push -u origin master
