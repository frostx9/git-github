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


## Discarding Changes

git chcheckout -- <file name>  -> This Will Discard Changes By Specific File

git checkout -- . / git checkout . -> This Will Discard All Changes