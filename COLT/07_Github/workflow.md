## Pull Request (PR)

Pull Request is not a native feature of git. It is a feature of github or bitbucket that allow developers to alert team
member to new works thhat neet to be reviewed and approved.



## How To Create Pull Request

1. Hit The Button *Comapre & Pull Request*

2. Add Title And Description what did you made

3. Click on *Create Pull Request* and wait for approval




## How To Approve Pull Request

1. Go To The Pull Request Section on the navbar and find the lists of pull requests that need to be approved

2. Click on any pull request title

3. Click The *Merge Pull Request* Button

4 Confirm Merge. Now All Changes From Feature Branch Will Merge With Main Branch and u can also delete the feature 




## Merge Pull Request With Conflicts 

Conflicts can be happened when in pull request. If Any Merge conflict happen it will show **Resolves Conflicts** button.

1. Conflicts can be resolved via browser, but best method is First fetch the origin and then resolve the conficts via *git switch <branch name>*. After
fetching switch the feature branch

2. Switch and Go To The main branch. Pull The Latest Changes. Then Merge the main branch with feature branch

3. Fix The Conflicts and save the file

4. Again Switch to the main branch

5. Merge the feature branch with main branch

5. Push The Code


## Branch Protection Rules

If u want to protect the branch so that no one can make any changes in that branch, then u can use branch protection rules.

1. Go To The *Settings Tab*

2. Click on *Add Clasics Branch Protection Rule*

3. Select the branch which you want to protect via branch name into *Branches Name Pattern*

4. Select the Options to Protect Marching Branch