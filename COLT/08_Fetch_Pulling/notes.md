## Remote Tracking Branch

git branch -r

It Will Show all remote branches


## To Checkout Origin Branch Pointer

git checkout origin/<branch name>


## Working With Remote Branches
When We Clone a project by default local main / master branch tracking the remote main / master branch

if we want to work another remote branch we using same comand to change branch 

git switch <remote branch name> [New Way]

git checkout --track <remote name>/<branch name>

It will automatically create a local branch and connect with remote branches


## Git Fetch
Fetching allow us to download changes from remote repository but it will not automatically merge with our local working files
It lests to see what other have been working on with out marge those changes into our local repo. To See The Changes we have to 
checkout the branches by using   git checkout <branch name>

git fetch <remote name> / git fetch

if remote name specified, by defaults from origin

Specified Branch

git fetch <remote name> <branch name>

** It also download new branch to local repo


## Git Pull
Pulling does the opposite of fetching. It will merge the changes from the remote repository into your local repository

git pull <remote name> <branch name>  / git pull