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
1) is there a way i can find a commit in git is faked its date using  git commit --amend --date  command?

```If you suspect that a commit's date has been faked using the git commit --amend --date command, there are a few steps you can take to investigate and verify the authenticity of the commit's date:

Inspect Commit History: Use git log to view the commit history and identify the commit you suspect has a faked date. Pay attention to the commit's hash (SHA-1) and the dates associated with it.

View Commit Details: Use git show <commit_hash> to view the details of the commit you suspect. This will display information about the commit, including the author, committer, date, and commit message.

Check Reflogs: Git maintains a history of branch references in the reflog. You can use git reflog to see the history of branch movements and commits. This might help you track any changes or amendments to the commit in question.

Compare Dates: Compare the commit date with other commits in the repository. If you suspect a commit's date has been faked, check if the date stands out significantly from other commits. Keep in mind that there might be legitimate reasons for a commit to have a different date.

Analyze Commit History: Look at the context and the surrounding commits. If you see a commit with a suspicious date that doesn't fit the overall development timeline or seems out of place, it might warrant further investigation.

Check Remote Repositories: If your repository is connected to remote repositories, check the commit's history on those remotes as well. The commit's date should be consistent across all clones of the repository.

Use External Tools: There are third-party tools and scripts that can help analyze Git repositories for anomalies or inconsistencies. One such tool is "git-forensics," which can help you identify tampered commits. Keep in mind that using external tools should be done with caution, as they might have security and privacy implications.

Reach Out to Team Members: If you're working on a collaborative project, consider discussing your concerns with other team members who might have been involved in the commit in question. They might be able to provide additional context or insights.

Remember that while the git commit --amend --date command can be used to change the date of a commit, it's important to consider the overall context and reasons for such changes before jumping to conclusions. Mistakes can happen, and dates might be legitimately modified for various reasons, such as correcting historical inaccuracies or rebasing code.```

---------------------------------
