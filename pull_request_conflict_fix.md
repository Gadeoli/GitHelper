### Pull Request [conflict fix]
Option 1
Description: Fix conflict. By: https://community.atlassian.com/t5/Bitbucket-questions/How-can-I-solve-a-conflict-in-a-pull-request/qaq-p/577205
Option 1: 
1. $ git fetch && git checkout master && git pull [go to your destination branch]
2. $ git pull origin release/2 [then force a pull from the source branch]
3. Now fix the conflicts and make a new commit with the fixes

Option 2
Description: Fix the conflicts creating a new branch
1. $ git fetch && git checkout master && git pull [go to your destination branch]
2. $ git checkout -b resolve-conflicts-branch [create the new branch]
3. $ git pull origin release/2
4. fix the conflicts and commit
5. $ git push -u origin resolve-conflicts-branch
6. create a pull request