## Rebase

1. It is an alternative to merge.

2. As A Clean Up Tools

Scenario: Suppose there are 5 developers working on a project. I create a new bugfix branch from main and continues working
on that branch. Suppose One developer push that code on main branch. So i have to marge my bugfix branch with main to get that
chages. Again another devloper push his code on main. Again I have to merge my bramch with main. This cycle is continue. 

Therefore branch will filles with extra merge commits. To avoid this problem we use rebase.

When we apply rebase on our branch it will placed on the tip of the main branch last commit, and create new history 
with new commits.

To Rebase go to the branch where you working and type the branch name which you want to rebase. 

git rebase <branch name>

ex : I working in feature branch. main branch is ahead by some commits, So in feature branch -> git rebase main

WARNING: Dont Reabase after pushing code to remote. Because if Someone pull the code, it is best to avoid rebase the branch.
Because Rebase will changes the commit history



## Reabase - Rewrite History

We can use rebase to rewrite commit history, combine commits together, delete commits, etc.

1. Rewrite History

git rebase -i HEAD~<number of past commits >

** -i -> interactive mode

ex: 
2029e20 my cat made this commit
655204d fix another navbar typo
2a45e71 fix navbar typos
4ff2290 add top navbar
6e39a76 whoops forgot to add bootstrap js script
240827f add bootstrap
519aab6 add basic HTML boilerplate
cbee26b I added project files  -> This is the I want to rename
0e19c7a initial commit

git rebase -i HEAD~9

it will open editor with following content

pick 24411d7 I add project files
pick 19e627c add basic HTML boilerplate
pick 40dad4f add bootstrap
pick ac62b54 whoops forgot to add bootstrap js script
pick b45543a add top navbar
pick 32470fd fix navbar typos
pick 0f07e83 fix another navbar typo
pick d8e203d my cat made this commit
pick 83c8701 Create README.md

** We use  <reword> to change the commit message. 
reword 24411d7 I add project files

** Save It. Then it another editor will open and there we chahnge the message


2. Combine Commits

git rebase -i HEAD~<number of past commits >

ex: 
2029e20 my cat made this commit
655204d fix another navbar typo
2a45e71 fix navbar typos
4ff2290 add top navbar
6e39a76 whoops forgot to add bootstrap js script
240827f add bootstrap
519aab6 add basic HTML boilerplate
cbee26b I added project files  -> This is the I want to rename
0e19c7a initial commit

git rebase -i HEAD~9

it will open editor with following content

pick 24411d7 I add project files
pick 19e627c add basic HTML boilerplate
pick 40dad4f add bootstrap
pick ac62b54 whoops forgot to add bootstrap js script
pick b45543a add top navbar
pick 32470fd fix navbar typos
pick 0f07e83 fix another navbar typo
pick d8e203d my cat made this commit
pick 83c8701 Create README.md

** We use  <fixup> to combine the commits with previous commit . 
fixup ac62b54 whoops forgot to add bootstrap js script

It combine with 40dad4f add bootstrap commit

3. Dropping Commit and its Changes

git rebase -i HEAD~<number of past commits >

ex: 
2029e20 my cat made this commit
655204d fix another navbar typo
2a45e71 fix navbar typos
4ff2290 add top navbar
6e39a76 whoops forgot to add bootstrap js script
240827f add bootstrap
519aab6 add basic HTML boilerplate
cbee26b I added project files  -> This is the I want to rename
0e19c7a initial commit

git rebase -i HEAD~2

it will open editor with following content

pick d8e203d my cat made this commit
pick 83c8701 Create README.md

** We use  <drop> to delete the commit and changes . 
drop d8e203d my cat made this commit