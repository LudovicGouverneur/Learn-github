
This is the change I made from gitbash editor, and pushed to github
## Description : 
Contains knowledge and ressources about git and github.

## WHat is it?
  * VCS : version control system
## Links

### youtube 
  * [Git & GitHub Crash Course For Beginners](https://www.youtube.com/watch?v=SWYqp7iY_Tc)
  * [Elewa course video] https://www.youtube.com/watch?v=1ffBJ4sVUb4
  * [LearnGitBranching.js.org](http://learngitbranching.js.org/)

## Commands
### Creating a git repo

>In order to do VCS in a working directory, one must create a .git repository. This .git folder is nothing but an "empty folder structre". It contains all what is needed to work with git.

 * git init
 * git touch : create a file
git nano : edit a file in the "console"?
git add file.ext
git status : check what is in the staging area and compare it with the files created/modified
git add :
git add . : adds all the files to the staging area
git commit : wrap all the files in the staging area in a commit object. It attaches an ID and two labels to that object : the checkout and the branch name.
id : the id is the checksum of
author
files in staging area
preceding ID
...
git commit -m "comment about the commit"
clear : clear the terminal console
git ignore or .gitignore : to specify the file/folder we don't want to include
touch .gitignore
open the file
type the name of the file/dir you want to ignore
Will not be taken in consideration for commands like 'git add.'
Branches : when working with other developpers, you create a branch to work on which is different form the main project branch. So you can add and commit to that branch, it will not affect the main branch (which is called Master branch) other developpers are working on.
git branch login (login is the name of the new branch)
git checkout login : which switches from "master branch" to "login branch"
Make the changes you want by adding, commiting, etc
git checkout master : go back in the master branch. You can see that changes you made on the "login branch" don't exist in master. Once you have done all the changes or added files to you working branch (login), you can merge both branches back.
git merge login : from master branch, it merges the login branch to the master branch.
The idea of git, is that when you are finished doing the changes on you computer, you want to put it where it could be accessed by anyone. Github is such a tool.
git remote add origin "https....."
git push -u origin master
git clone http....
git pull
