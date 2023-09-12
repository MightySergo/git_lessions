# Table of content
* What is git?
* Repositories and Branches
* Main commands
* Remote repository

## What is git?
Git is a distributed version control system that tracks changes in any set of computer files. Git was created by Linus Torvalds during the Linux develpment. Git saves only the difference between files and not the entire files allowing git to save a considerable amount of memory.

## Repository
To start a new local git repository follow the instruction below
1. Create a directory to contain the project
2. Go into the new directory
3. Open console
4. Type **git init** and execute the command (this will also create _master_ branch)

### Createating repository by cloning  
You can create a new local repository by cloning already existing one from the remote server.  
Please note, that git supports several URL syntaxes. For more information visit official git manual on [https://git-scm.com/docs/git-clone](https://git-scm.com/docs/git-clone)

To copy repository from remote sever  
1. Run console
2. Use `git clone {URL}` and then execute the command

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
 
## Main commands
`git init`  

Create an empty Git repository or reinitialize an existing one

`git add` 

This command updates the index using the current content found in the working tree, to prepare the content staged for the next commit

`git commit`  

Create a new commit containing the current contents of the index and the given log message describing the changes  

`git commit -m <comment>`  
Use _-m_ to add message or comment to commit for better understanding of log


`git diff`

Show changes between commits, commit and working tree  

`git log`  

Show commit logs  

`git checkout`

Switch branches  

`git status`  

Show the working tree status

`cherry-pick`  
  
    
      
`reset`  
  
  

  
`revert`

