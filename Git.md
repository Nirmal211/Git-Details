# Git Installation

- Global Set up for Git
  - git config --global user.name
  - git config --global user.email
  - git config --global core.editor "code --wait"
  - git config --global core.autocrlf

- If You want to Change / Edit something from this 
  - write command to change ( Edit ) Name , Email , Code Editor
  - git config --global -e  

- Stages :
 U - untracked - Git don't know about this file like file  exists or not 
 A - Added or Staged - Now we add our file or Staged our file so now Git knows and Aware of this file
 C - Committed - Now in committed Git will Track our all files and records about the file like is there any new Changes Available or not.

- Making a CheckPoint or Saved Point 
  - adding files
  - staging them
  - commiting them

- Commands you need to know 
  - git status -s => to know the current status of staged or unstaged files
  - git log --oneline => to know current status of saved points

- Going Back to Some Previous Saved Points
  - suppose you have made 4 checkpoints and you want to go back to previous checkpoint so for that you have to write this command -
  - git reset --hard HEAD~1 

- How to check status of a files
  - git status - this command will give you a lots of information about status but we don't need it. 
  - so we will write another command 
  - git status -s => it will only give you accurate info about your files

  - basically you can use anything form both of these commands it's totally up to you.

- Command => 
  - git init
  - git add <filename> , git add .
  - git commit -m <commit message>  
  - git status
  - git status -s
  - git log / git log --oneline

- Branch Related Commands :
  - git branch <nameOfTheBrach> => create branch
  - git branch => check all the branches
  - git switch <nameOfTheBrach> (in which you want to switch) => switch branch
  - git switch -C feature/Header => create and switch branch at the same time. -C means before switch create the branch.
  - git merge <nameOfTheBranch> => Merge the branch - for merging the branch you first have to come to your main branch using this command -
     - git switch main
    and then you can merge the new branch features in your main branch using this command - 
     - git merge <name of the branch which you want to merge>

- Merging Techniques :
  - fast forward merge
  - three way merge
  - we handled conflicts of three way merge technique

- Delete Branch 
  - git branch -d <nameOfTheBranch>

- Stashing in Git 
  - when we make some changes in our file and without adding or staging or commiting if  try to go to the another branch so git gives us error that you will have to commit all your changes otherwise i will delete it or we can say that i will not remember this changes that you did . so for that we do <Stashing> basically git save all the changes in the memeory and then we can go to another  branch and the when we came back to  main branch so that we can take those changes from the memory and apply them in our branch and after that we can commit all our changes.

  - git stash  // store changes in memory 
  - git stash apply // take those changes from memory to commit.
  - git stash clear // clear the  memory from stash

