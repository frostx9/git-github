## Fast Forward Marging

When we create branch from main branch and we do some work on second branch. Then Some 
extra code will be added in second branch. Now if we want to merge this branch with main
branch then we will use fast forward marge. 

** Rember Fast Forward Marging will happened when no changes in Main Branch since work started
on Second Branch.

git merge <branch name>

## Marging With Recursive Strategy

when main branch is ahead of second branch and if we try to merge second branch with main, it
will us recursive marging. 

** Remember Recursive Marging will happen when main branch is ahead of second branch.
and it will use default editor to recursive marging.

git merge <branch name>


## Merge Conflicts
When we try to merge two branches and some changes are added in both branches in same file, then
it will show merge conflict. Because git can not decide which changes to keep and which changes to discard.

The contents from branch are trying to marge dispaly between 


<<<<<<<<< HEAD (Current Changes)

Content (From Current Branch) 

============

Content (From Branch Which we want to marge) 

>>>>>>>>>>>> (Branch Name) 




## Resolve Merge Conflicts

# 1. Edit Manually

# 2. Use Vs Code Editor 
1. Accept Current Changes -> It Means Keep Current Branch Changes
2. Accept Incoming Changes -> It Means Keep Incoming Branch Changes
3. Accept Both Changes -> It Means Keep Both Branch Changes