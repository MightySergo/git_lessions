# Table of content
* What is git?
* Repositories and Branches
* Main commands

## What is git?
Git is a distributed version control system that tracks changes in any set of computer files. Git was created by Linus Torvalds during the Linux develpment. Git saves only the difference between files and not the entire files allowing git to save a considerable amount of memory.

## Repository
To start a new git repository follow the instruction below
1. Create a directory to contain the project
2. Go into the new directory
3. Open console
4. Type **git init** and execute the command (this will also create _master_ branch)

## Branches
Use the **git branch** command with the branch name to create a new branch in your project.   
Alternatively, use the **git checkout** command with the __-b__ option and specify the branch name as well as the commit to create your branch from.  
To switch between branches use **git checkout** command with the branch name.

### Common Options with branch
`git branch`   
 List all of the branches in your repository. This is synonymous with git branch --list.  
  
`git branch <name>` 
  
  Create a new branch called ＜name＞. This does not check out the new branch  

`git branch -d <branch>`    
   
   Delete the specified branch. This is a “safe” option to delete branch with unmerged content  

`git checkout <name>`  

 Switches to the branch with name that follows __checkout__  

`git merge <name>`  

 This command will merge the current branch into the master branch  

 **N.B.!** If the two branches you're trying to merge both changed the same part of the same file, Git won't be able to figure out which version to use. When such a situation occurs, it stops right before the merge commit so that you can resolve the conflicts manually
 



