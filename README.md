# MDD Portfolio Project

# Portfolio Site Deployment Plan
When creating and deploying updates to the live portfolio site please follow the steps below.

To minimize conflicts and confusion among team members, create a unique branch for your new code, develop code to completion, test new code, and then merge with master branch.

## Local Development

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

## Staging
After local development and testing is complete, push release to staging server for additional testing.

1. Push changes to the staging server and test
````
  git push staging master
````
2.   Input password when prompted
3. Go to staging site and test changes
4. Visit all conflicted files, resolve conflicts and commit
````
    git add -A
    git commit -m ‘Relevant commit message.’
````

## Production
After testing new release code on the staging server, push release to live production server

1. Push changes to the production server 
````
  git push production master
````
2.   Input password when prompted
3. Go to live site and verify 