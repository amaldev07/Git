# GitCommands

to see the user name/ email
---------------------------------
$ git config user.name
Amaldev
---------------------------------
$ git config user.email
amaldev.psn@gmail.com
---------------------------------
Git Commit with a Past Date
git commit --amend --date "2021-06-14 20:12:20"
youtube reference : https://www.youtube.com/watch?v=cSwgkUHk_Qo
---
this wont work so
make changes
git add
git commit -m "test commit msg"
git commit --amend --date "2022-08-05 20:12:20"
git push origin master

if some error occurs u have to rebase 
Solution ois below
```
        Run the following commands in the feature branch
        
        git pull origin featureBranch --rebase
        If you have any conflicts, after resolving conflicts:
        
        git rebase --continue
        Enter commit messages -> press ESC -> enter “:wq!” and enter
        git push origin featureBranch
```


https://stackoverflow.com/questions/39399804/updates-were-rejected-because-the-tip-of-your-current-branch-is-behind-its-remot
---------------------------------
