# MDD Portfolio Project

## Portfolio Site Deployment Plan
When creating and deploying updates to the live portfolio site please follow the steps below.

To minimize conflicts and confusion among team members, create a unique branch for your new code, develop code to completion, test new code, and then merge with master branch.

### 1. Create Local Development Branch

  a. Switch to the local master branch
````
  git checkout master
````
  b. Make sure local master branch is current by pulling from the remote master branch
````
  git pull github master
````
  c. Create unique branch for new code development
````
  git branch newCodeBranch
  git checkout newCodeBranch
````

### 2. Develop new code to completion

a. After completing new code and testing locally commit changes
````
  git add -A
  git commit -m 'Relevant commit message.'
````
### 3. Merge development branch with master branch
````
  git checkout master
  git merge newCodeBranch
````

  1. Visit all conflicted files and resolve conflicts and commit
````
    git add -A
    git commit -m ‘Relevant commit message.’
````

### 4. Push updates to remote servers
````
  git push github master
  git push production master
````