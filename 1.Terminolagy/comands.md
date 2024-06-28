# 1. Check Git Version (To Check Git Version on Current System)

git --version


# 2. To Show Git Conig List

git config --list


# 3. Set User Name And User Email For Git  Global Config

git config --global user.emal "<email>"
git config --global user.name "<name>"


# 4. Git Intailze

git init


# 5. Staging Area

git add . 

. -> This Mean Select All Files

// We Can Choose Also File

git add file1.js file2.js 


# 6. Commit

git commit -m "Git Hub"

-m -> This Mean Passing A Message


# 7. Log

git log 

This Command Show Commit History

Ex : 
commit 4ac66c9bf9ab9bbafb83fb5bfe7ccee6553caa32
Author: Saumya Som <saumyasom92@gmail.com>
Date:   Fri Jun 28 16:13:13 2024 +0530

git log --oneline

This Command Show Commit History In Single Line