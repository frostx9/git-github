# 1. To Show All Branches
git branch

git branch -a (To Show All Branches Including Remote and Hidden Branches)

# 2. Create New Branch
git branch <branch name>

# 2.1. Create New Branch And Immediately Switch
git switch -c <branch name> [New Way]

git checkout -b <branch name> [Old Way]

# 3. Switch Branch
git switch <branch name> [New Way]

git checkout <branch name> [Old Way]

# 4. Delete Branch  
git branch -d <branch name>

** Remove from Another Branch

# 5. Rename Branch
git branch -m <old branch name> <new branch name>
