# Basic operations using git commands (add, commit, push, pull)

## Register your remote repo to your local machine

To upload files to a remote repo, you first need to register that repo's URL
- Use ```$ git remote add remote_repo_name URL``` (for example ```$ git remote add origin https://___```)

```
Basic terms/actions in git

- add: to 'select' a file/files/changes, or to create new file

- commit: to 'record' a file/files/changes (prepare for push)

- push: to 'upload' a file/files/changes to remote repo

- fetch: to get the latest version from remote to local, without automatic merge

- merge: to integrate your current directory with the selected directory

- pull: to 'fetch' the latest version of the project from remote repo then 'merge' to your local repo
```

## Firstly, pull, always

Whenever you reopen a project, you want to have the latest version of that project on your local machine. With that being said, before making any changes, remember to first ```$ git pull```.

## Repo's status

To check whether there are files with new changes, files that were created (added) but not uploaded to remote repo (commit), 
- Use ```$ git status``` to check your repo's status

## To commit to remote repo

1. To ```add``` = to create a new file **or** select a file to commit **or** select changes in a file to commit,
   -  Use ```$ git add file_name```
2. To ```commit``` = to record the files/changes that you previously selected and add a note when preparing to push to remote repo
   - Use ```$ git commit -m "your_note/message"``` (for example ```$ git commit -m "created index.html```)
3. To ```push``` = to upload files/changes to remote repo
   - Use ```$ git push remote_repo_name remote_repo_branch_name``` (for example ```$ git push origin master```)

## To revert (undo) a commit

To ```revert``` a commit = to undo/delete a commit you made
- Use ```$ git revert commit_id``` to revert a commit
- Use ```$ git status``` to check if the revert content is executed in your local repo
- Use ```$ git commit -m "commit_message"``` to commit the revert to local repo
- Use ```$ git push branch_name``` to push the commit to remote repo