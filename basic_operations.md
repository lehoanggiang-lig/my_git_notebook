# Basic operations using git commands

## Register your remote repo to your local machine

To upload files to a remote repo, you first need to register that repo's URL
- Use ```$ git remote add remote_repo_name URL``` (for example ```$ git remote add origin https://___```)

```
Basic terms/actions in git
- add: to 'select' a file/files/changes, or to create new file
- commit: to 'record' a file/files/changes (prepare for push)
- push: to 'upload' a file/files/changes to remote repo
```

## Repo's status

To check whether there are files with new changes, files that were created (added) but not uploaded to remote repo (commit), 
- Use ```$ git status``` to check your repo's status

## Steps to commit to remote repo

1. To ```add``` = to create a new file **or** select a file to commit **or** select changes in a file to commit,
   -  Use ```$ git add file_name```
2. To ```commit``` = to record the files/changes that you previously selected and add a note when preparing to push to remote repo
   - Use ```$ git commit -m "your_note/message"``` (for example ```$ git commit -m "created index.html```)
3. To ```push``` = to upload files/changes to remote repo
   - Use ```$ git push remote_repo_name remote_repo_branch_name``` (for example ```$ git push origin master```)
