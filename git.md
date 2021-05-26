**1. What is Git ?**
- Git is a version control system.
- Git tracks the changes you make to the local files, so you have a record of what you have been done.
- Git also makes collaboration easier, allowing changes by multiple people to all be merged into one source file. 


**2. Git Commands**

|Sr No.| Command |Description|
|----| ------ | ------ |
|1.  | git init | It is initialise the git repository in local. |
|2.  | git status | This Command lists all the files that have to be stage.(untracked,updated and deleted). |
|3.  | git add <file_name> | Add a single file to stage the comment. |
|4.  | git add . or * | Add all the files to stage the comment. |
|5.  | git commit -m |Comment the file It is used to save your changes to local repository. |
|6.  | git commit -a -m  | shorthand for add and commit at a time. |
|7.  | git remote origin <repo_url> | This command used to set remote repository into local. |
|8.  | git push origin master/main | It is used to upload local repository content to a remote repository master/main.|
|9.  | git push origin <branch_name> | It is used to upload local repository content to a remote repository branch.|
|10.  | git log  | It is used to list the version history commit and also show where the head is present for the current branch. |
|11.  | git diff  | It is gives the what are the changes made in the file .|
|12.  |git show <commit_id> | This command shows the content changes on the specified commit. |
|13.  | git branch <branch_name>  | This command create a new branch.|
|14.  | git checkout <branch_name> / git switch <branch_name> |It is used  to switch the branch (<branch_name>). It is used to revert the changes and recover|
|15.  | git checkout -b <branch_name> | This command used to create branch and switch on that branch at a time.|
|16.   |git branch <branch_name> -D |This command using flag -D delete the branch.|
|17.  | git merge branch_to_be Merged   |This command merge the specific history from one branch to current branch.|
|18.  | git clone <remote_repo_url>  |This command upload/copy a repository that already exists on a remote. Including all file,commit and branches |
|19.   |git fetch|This command download commits, files, and branch from a remote repository into your local repository.|
|20.  | git pull origin <branch_name> |This command used to fetch changes from remote server to local.It is a combination of git fetch + git merge.|
|21.  | git stash  |This command used to store uncommited local changes into stash stack. |
|22.  |git stash pop|This command reverts the changes from stash stack.|
|23.  |git reset --hard|This command is very dangerous to use.If you don't know how this work this command don't use it.|
|24.  |git reset --soft|It is used to move the head to a stagging area.|
|25.  |git reset --mixed|It is used to move the head to a before stagging area.|
|26.  |git reset --mixed|It is used to move the head to a before stagging area.|
|27.  |git config --global user.name "sonali bankar"  and   git config --global user.email sona@gmail.com|This command set the git configuration values on a global or local project level.|
     
