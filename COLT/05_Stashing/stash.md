## Git Statsh
When we do some work on one branch and try to switch to another branch without commiting any changes
git wont let switch to another branch without commiting changes.

error: Your local changes to the following files would be overwritten by checkout:
COLT/05_Stashing/stash.md
Please commit your changes or stash them before you switch branches.
Aborting

In this condition we use stash.

## How use
git stash  - To Stash Changes
git stash pop - To Pop Stashed Changes. Back The Stashed Changes

## Stashing Multiaple

We Can Stash Multiple Changes. It work like as a stack.

## To See Stash List 
git stash list

## To Pop Specific Stash From List
git stash apply stash@{<id>}

## To Drop Specific Stash From List
git stash drop stash@{<id>}

## To Drop All Stash / Clear
git stash clear