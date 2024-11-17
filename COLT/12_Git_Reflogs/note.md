## Git Reflogs
Git Reflogs or Reference Logs. Git Keeps a record / Logs when the tips of branches and other other refereces
were updated in the repo

Logs will be found .git folder. Inside .git folder there is a folder called logs. In the logs folder all logs are stored in HEAD 
file. It is a Human Readable File

** It Only Keeps Local and old entries expire last 90 days. It can changed via config file

To Show Logs -> git reflog show HEAD / git reflog show <branch name>

*HEAD@{0}* -> This Indicate The Most Recent Log