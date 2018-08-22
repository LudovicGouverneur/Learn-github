
This is the change I made from gitbash editor, and pushed to github
## Description : 
Contains knowledge and ressources about git and github.

## What is it?
>The idea of git, is that when you are finished doing the changes on you computer, you want to put it where it could be accessed by anyone. Github is such a tool.

  * VCS : version control system
## Links

### youtube 
  * Series : [Git & GitHub Crash Course For Beginners](https://www.youtube.com/watch?v=SWYqp7iY_Tc)
  * Conference : [Linux Conference - 4 years old] https://www.youtube.com/watch?v=1ffBJ4sVUb4
  * Exercices : [LearnGitBranching.js.org](http://learngitbranching.js.org/)
### Elewa 
  * [pushing and merging](https://github.com/elewa-academy/pull-requesting-and-merging)
  * [Easy to do's](http://rogerdudler.github.io/git-guide/)
## Actions
### Merging
 * Desription : Combining the content of two branches

####  First method : `git merge`
create un special commit with two parents.
In other words : I want ot include the content of these two parents and all their own parens.

## Commands
### [init] Create a git repo

>In order to do VCS in a working directory, one must create a .git repository. This .git folder is nothing but an "empty folder structure". It contains all what is needed to work with git.
-
 * `git init` : create a .git repository

This folder is "hidden". To unhide it, follows [these steps]()

### Creating a file
 * 'git touch' : create a file
### Editing a file
 * 'git nano'  : edit a file in the "console"?
 * text editor : modify it in your text editor (ie Visual Studio, atom, ...)
### Adding a file to the staging area
 * The staging area is 
   * a place where you put all the files you want to put in the git tree. 
   * these files must be have been modified.
 * 'git add'   : file.ext 
 * 'git add .' : adds all the files to the staging area
### Commit  
 * 'git commit': wraps all the files in the staging area in a commit object. It attaches an ID and two labels to that object :
     * the branch where we last checked out 
     * the branch name.
 *  id : the 'id' is a unique number attached to any commit. It is the _checksum_ of
     * .author
     *  files in staging area'
     *  preceding ID
     *  ...
 *  'git ignore' or 'git .gitignore' : to specify the file/folder we don't want to include in the commit
    *  Examletouch .gitignore
         *  open the file
         *  type the name of the file/dir you want to ignore
         *  Will not be taken in consideration for commands like 'git add.'
### Branches 

When working with other developpers, you don't want the workflow and the files to be messy or even loose some documents in the process. You can create a branch to work on, which is different from the main project branch. You can add and commit to that branch, it will not affect the main branch (which is called Master branch), as other developpers are working on it.

Let's travel through the git tree : 
 * go in a folder, create/modify a file
 * 'git branch login' (login is the name of the new branch)
 * 'git checkout login' : which switches from "master branch" to "login branch"
 * Make the changes you want by _editing_ => _adding_ => _commiting_ ...
 * 'git checkout master' : go back in the master branch. You can see that changes you made on the "login branch" don't exist in master. Once you have done all the changes or added files to you working branch (login), you can merge both branches back.
 * 'git merge login' : from master branch, it merges the login branch to the master branch.
 * 'git remote add origin "https....."'
 * 'git push -u origin master'
 * 'git clone http....'
 * 'git pull'
     
### Useful commands
 *  git status : check what is in the staging area and compare it with the files created/modified
 *  clear : clear the terminal console
