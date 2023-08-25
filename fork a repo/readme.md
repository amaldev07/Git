If you want to create a copy of another one's respo
use fork
if you want to do opensource contribution
fork the repo , make changes and create pr to the original repo (this is a better approach than creating your branch in the original repo and make pr from your_branch to develop)
in some repos you wont be having access to create a branch
-------------------
To Fork a repo
Click on "For" in the repo
so a fork of that repo created under my repo
work on develop/master branch
commit changes to develop/master branch
then create pr from my forked repo
choose base as original/develop and compare as my "develop" branch
create pr
-------------------
to fetch or get the latest from original repo to my forked repo
git pull https://github.com/amaldev07/angular-lifecycle-hooks.git develop

here "https://github.com/amaldev07/angular-lifecycle-hooks.git" is a sample repo