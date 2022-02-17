# # Clone Repository 

``` git clone [url]```

---
# See information about branch 

```git status```


- - - -
# create branch

```git branch new_branch```


Create branch and switch to it 

```git checkout -b new_branch```

This is shorthand for:

```
git branch new_branch
git checkout new_branch
```
- - - -
# change branch

```git checkout <branch>```



---
# see branches

```git show-branch```


- - - -
# see difference in working directory:

```git diff```

use arrow up/down to scroll, and press q to quit.

see difference in file:

```git diff <file>```



- - - -
# pull changes

```git pull```



---
# push changes

```git push```

or

```git push <repository> <branch>```



---
# add a file to staged files:

```git add <file>```

add all files to staged files in current directory (notice the "."):

```git add . ```

Untage file 

```git restore --staged <file>...```

unstage all files 

```restore --staged ```


---
# discard changes in file:

```git checkout -- <file>```

Discard all changes in all files 

```git checkout -- .```


---
# remove file from staging area:

```git reset HEAD -- <file>```

Remove directory from staging area

```git reset HEAD -- <directoryName>```



---
# commit with message

```git commit -m "changed some things"```




- - - -
# stop detecting changes in file:

```git update-index --assume-unchanged [path]```


---
# see history of commits

```git log```

- - - -
# Revert commit

If you wish to undo/revert the last commit you can do the following, using the commit hash that you get from the git log command:

```git revert <commit hash>```

---
# Remove Last Commits

To remove the last commit from git, you can simply run ```git reset --hard HEAD^``` If you are removing multiple commits from the top, you can run ```git reset --hard HEAD~2``` to remove the last two commits. You can increase the number to remove even more commits

Then, force a push (```git push --force origin``` or ```git push --force origin master``` should be enough)

---
# list settings of git

```git config --list``` will list the settings. There you should also find user.name and user.email.

- - - -
# save git password

```git config --global credential.helper store```

then do

```git pull```

- - - -
# Merge

run ```git checkout master``` to change the active branch back to master. 

run ```git pull```

run  ```git merge new-branch``` to merge the new feature into the master branch. 

Note that git merge merges the specified branch into the currently active branch. So we need to be on the branch that we are merging into.

run ```git push```


If there are, conflicts use GIT GUI like Smartgit or VS Code


- - - -
# Delete Branch

Use Smartgit GUI just to be safe :
```mouse right click branch -> delete```


### bash (don't use this)

delete locally :

The -d option stands for --delete, which would delete the local branch, only if you have already pushed and merged it with your remote branches.

The -D option stands for --delete --force, which deletes the branch regardless of its push and merge status, so be careful using this one!

```
git branch -d branch_name
git branch -D branch_name
```

delete remote:

```
git push <remote_name> --delete <branch_name>
```

- - - -