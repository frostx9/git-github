## Rebase

It is alternative to merge.

Scenario: Suppose there are 5 developers working on a project. I create a new bugfix branch from main and continues working
on that branch. Suppose One developer push that code on main branch. So i have to marge my bugfix branch with main to get that
chages. Again another devloper push his code on main. Again I have to merge my bramch with main. This cycle is continue. 

Therefore branch will filles with extra merge commits. To avoid this problem we use rebase.

When we apply rebase on our branch it will placed on the tip of the main branch last commit, and create new history 
with new commits.

To Rebase go to the branch where you working and type

git rebase <branch name>

ex : I working in feature branch. main branch is ahead by some commits, So in feature branch -> git rebase main