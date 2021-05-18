**1. What is Git ?**
- Git is a version control system.
- Git tracks the changes you make to the local files, so you have a record of what you have been done.
- Git also makes collaboration easier, allowing changes by multiple people to all be merged into one source file. 








git clone <remote_repo_url>  - get the hole remote project on a local


git fetch  <branch_name> - get the remote branch on a local


git pull- This command used to fetch changes from remote server to local


git reset - Reset all changes


git stash - Temporory store the changes

**2. Git Commands**


|Sr No.| Command |Description|
|----| ------ | ------ |
|1.  | git init | It is initialise the git repository in local. |
|2.  | git status | This Command lists all the files that have to be stage.(untracked,updated and deleted). |
|3.  | git add <file_name> | Add a single file to stage the comment. |
|4.  | git add . or * | Add all the files to stage the comment. |
|5.  | git commit -m |Comment the file It is used to save your changes to local repository. |
|6.  | git commit -a -m  | shorthand for add and commit at a time. |
|7.  | git remote origin <repo_url> | cell |
|8.  | git push origin master/main | It is used to upload local repository content to a remote repository master/main.|
|9.  | git push origin <branch_name> | It is used to upload local repository content to a remote repository branch.|
|10.  | git log  | It is used to list the version history commit and also show where the head is present for the current branch. |
|11.  | git diff  | It is gives the what are the changes made in the file .|
|12.  |git show <commit_id> | This command shows the content changes on the specified commit. |
|13.  | git branch <branch_name>  | This command create a new branch.|
|11.  | git checkout <branch_name> |It is used  to switch the branch (<branch_name>). It is used to revert the changes and recover|
|9.  | git checkout -b <branch_name> | This command used to create branch and switch on that branch at a time.|
|1   |git branch <branch_name> -D |This command using flag -D delete the branch|
|10.  | git merge branch_to_be Merged   |This command merge the specific history from one branch to current branch |
|11.  | git clone <remote_repo_url>  |This command upload/copy a repository that already exists on a remote. Including all file,commit and branches |
