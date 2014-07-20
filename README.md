# Portfolio
=========

## MDD Portfolio Project

# Portfolio Site Deployment Plan
To deploy updates to the live portfolio site please follow the steps below.

## 1. Merge Development Branch with Master
After completing development of new site code and testing it in your local development environment, merge your development branch with the master branch.

1. Switch to the local master branch:

  * `git checkout master`

2. Make sure local master branch is current by pulling from the remote master branch:

  * `git pull github master`

  1. Visit all conflicted files and resolve conflicts... then commit and pull from remote master:
    * `git add -A`
    * `git commit -a -m ‘Relevant commit message.’`
    * `git pull github master`

3. Merge Development Branch with Master Branch
  * `git merge 'newCode'`

  1. Visit all conflicted files and resolve conflicts... then commit and pull from remote master:
    * `git add -A`
    * `git commit -a -m ‘Relevant commit message.’`
    * `git pull github master`

## Communicate changes to your team
Let your team know that you have updated the site with some new code.
