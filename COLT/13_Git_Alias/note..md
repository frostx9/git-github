## Git Config File

Type :-
1. Local Config File
2. Global Config File
3. System Config File

## Write Alias For Git Commands

1. Go To The Config File -> touch ~/.gitconfig (Linux) / Home Directory (Windows)

2. Open The Config File 

3. Add Alias For Git Commands (Manually)

ex : 
[alias]
	s=status
  l=log

3.1 Add Alias For Git Commands (Comand Line)

ex:
git config --global alias.s status
git config --global alias.l 


4. Alias With Arguments

ex :
[alias]
  cm = commit -m


*List*
https://github.com/GitAlias/gitalias