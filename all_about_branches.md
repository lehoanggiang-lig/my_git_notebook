# All about branch(es)

## How to see a list of branches in your repo
- Use ```$ git branch``` to see a list of branches in your local repo 
   ```
   le_hoang_giang@MBP20200826-09 my_git_notebook % git branch
   * draft
     main
   ```
-  Use ```$ git branch -a``` to see a list of all branches, both in your local repo and in your remote repo
    ```
    le_hoang_giang@MBP20200826-09 my_git_notebook % git branch -a
   * draft
      main
      remotes/origin/HEAD -> origin/main
      remotes/origin/draft
      remotes/origin/main
   ```
- Use ``` $ git branch --remote``` to see a list of branches in your remote repo
   ```
   le_hoang_giang@MBP20200826-09 my_git_notebook % git branch --remote
   origin/HEAD -> origin/main
   origin/draft
   origin/main
   ```

## How to check which branch you're on
- When using the command ```$ git branch``` or ```$ git branch -a```, you will see an asterisk mark ```*``` next to a branch name with the text colored in green. That's the branch you're currently on.

## How to see a list of files in a branch you're on
- The command ```$ ls``` will display name of all files in the branch you're on.
- The command ```$ ls -l``` will display name of all files and your access authority to those files.

## How to create a branch (and register it to remote repo)
- Move to the directory you want to create a branch in by using ``` $ cd directory_name```.
- See a list of all branches in that directory, as well as check which branch you're on, by using ```$ git branch``` or ```$ git branch -a```.
- Move to the branch you want to create a new branch in by using ```$ git checkout branch_name```.
- Create a new branch by using ```$git checkout -b new_branch-name```.
- Use ```$ git branch``` or ```$ git branch -a``` to check if the new branch was created.
- Register your newly created branch to your remote repo by using ```$ git push -u origin```.

## How to delete a branch
- See a list of all branches in that directory, as well as check which branch you're on, by using ```$ git branch``` or ```$ git branch -a```.
- Delete a branch **in your local repo** by using ```$ git branch --delete branch_name```.
- Delete a branch **in your remote repo** by using ```$ git push --delete origin branch_name```.
- If you still see that branch when using ```$ git branch``` or ```$ git branch -a``` even after deleting it (oftern seen as remote/origin/branch_name), that is the remote-tracking branch and you can remove it by using ```$ git branch -d -r origin/branch_name```.