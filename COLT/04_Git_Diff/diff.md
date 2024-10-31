## Git Diff
We Use git diff to check difference between two commits, files, or working directory and many more
 
## 1. To View Git Diff in Unstaged Changes
git diff

## 2. How To Read Git Diff
diff --git a/COLT/04_Git_Diff/rainbow.txt b/COLT/04_Git_Diff/rainbow.txt

Explaintion: This Line Indicate Which Files we are comparing


--- a/COLT/04_Git_Diff/rainbow.txt
+++ b/COLT/04_Git_Diff/rainbow.txt

Explaintion: This Line Indicate Which Files we are comparing

@@ -2,5 +2,5 @@ red  

Explaintion: -2,5 this means from file a 5 line extracted from line 2
Explaintion: +2,5 this means from file b 7 line added from line 2

 orange
 yellow
 green
-blue
-purple
+indigo
+violet

Explaintion: ' - 'this symbol means deleted line from file a 
Explaintion: ' + ' this symbol means added line from file b

## 3. Show All Chages From Last Commit
git diff HEAD .\rainbow.txt 

## 4. Show All Chages Between TWo Branches
git diff <branch1>..<branch2>

## 5. Show All Chages Between TWo Commits
git diff <commit1 hash>..<commit2 hash>