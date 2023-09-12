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

> __N.B.!__ don't forget to use `cd` command to change directory of the repository folder

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
for better visualization use command `git log --graph`  

`git checkout`

Switch branches  

`git status`  

Show the working tree status

`cherry-pick`  
  
    
      
`reset`  
  
  

  
`revert`

# Remote repository

## Github
To create remote repository using Github follow the instruction below
1. Create Github account or sign in
2. Create local repository
3. Synchronize your local repositpry with remote one. Github has its own detailed instruction  
![monosnap screenshot just to show Markdown skills](https://monosnap.com/image/4oK79Og7dTGyzcca8DhVXP3XvkkxG8)
4. Use `push` command to add your local repository to your Github repository (for the first time you will need to authorize your account)  
5. After this you can `push` your changes into remote repository and `pull` changes remote repository to the local one

## Pull request
1. Make repository fork
2. Clone your repository version
3. Create new branch and make your edits
4. Commit changes
5. Push local repository to your Github repo
6. On Github push _pull request_ button
