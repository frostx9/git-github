## Github
Github is a hosting platform for git repositories. It a service taht hosts git repositories over the cloud.


## To Check Git Remote

git remote -v

It will show you the url of the remote repository


## To add a remote repository

git remote add <any remote name> <url>


## Rename Remote Repository

git remote rename <old remote name> <new remote name>
ex : git remote rename master main


## Delete Remote Repository

git remote remove <remote name>
ex : git remote remove master 


## Push to Remote Repository

git push  <remote name> <branch name> 

ex : git push origin master 
In Behind it will create a new branch called master in github if it does not exist or first time


## Git Push from Local to Remote By Differen Name

git push <remote name> <local branch name>:<remote branch name>

ex: git push origin master:main


## Up Stream -> -u

git push -u origin master

It Create a link between local branch and remote branch. Next time we can push directly to remote branch just by typing git push

