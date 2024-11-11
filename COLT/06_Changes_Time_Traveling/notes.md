## Checking Out Old Commits

git checkout <commit id> / git checkout <first 7 characters of commit id>

If we use git git checkout the Head will be detached. In Normal Head points to a specific branch reference not a commit.
The Branch reference is a pointer to the last commit made on this particualr branch.

Now if using git checkout <commit id> the Head directly will point to that commit reference.



## Re-Attaching Head To Current Branch

git switch <branch name>

git switch -  -> This will re-attach head to current branch


## Creating New Branch From Old Commit and switching to it

1. git checkout <commit id>

2. git switch -c <branch name>


## Git Checkout By Number

git checkout HEAD~<number>

~ -> This Symbol Means Previous. So ~1 -> Mean Last Commit


## Discarding Changes [Old Way / Old Command]

git chcheckout -- <file name>  -> This Will Discard Changes By Specific File

git checkout -- . / git checkout . -> This Will Discard All Changes


## Discarding Changes [New Way / New Command]

git restore <file name> / git restore .


## Discarding File By Commit

git restore --source HEAD~<number> <file name>


## Discarding File From Staging Area
If we want to discard file from staging area thet we add to staging area by mistake

git restore --staged <file name>


## Reset Commit

1. Soft Reset -> 

git reset <commit id> / git reset HEAD~<number>     -> This Will Revet Back the Commit, but keep the changes as unstaged area. If we want to keep changes we can switch the branch with the modified files. 

2. Hard Reset ->

git reset --hard <commit id> / git reset --hard HEAD~<number>    -> This Will Revet Back the Commit, and remove all the changes.


## Revert Commit

Revert Commit but did same things as Reser Commit but it create a new commit and undo all the changes in the new commit.
Basically it keep the record the commit which we want to undo 

git revert <commit id> / git revert HEAD~<number>  -> It will open editor to write the commit message to revert the commit

Bewware : It will create conflicts sometimes.