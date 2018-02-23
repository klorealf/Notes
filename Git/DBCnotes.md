# DBC notes

## Command Line
| Command | Description | Example |
| --- | --- | -- |
|  Command line = Terminal = Bash = Shell | Programmer's tool for working with files and running code.| |
| `mkdir` \<name of folder\> | Create folder | |
| `cd ..` \<name of folder\> | Change directory to a sub directory or a parent path | |
| `pwd` | Print the current directory | |
| `ls` | List files and folders in current directory | |
| `touch` \<name of file\>  | Create a new file | |
| `mv` \<name of file\>  \<name of folder\>  | Move a file to a folder | mv solution.md coding |
| `mv` \<name of file\>  \<name of file\>  | rename a file | mv solution.md new-solution.md |
| `cp` \<original file\>  \<target file\>  | Copy a file | cp new-solution.md algorithm.md|
| `open` \<name of file\> | Open a file with default application | open algorithm.md |
| `rm` \<name of file\> | Remove a file | |
| `rmdir` \<name of file\> | Remove a directory. | rmdir coding |
  | `rm -rf` \<name of folder\> | Remove a directory and everything inside it. BE CAREFUL! You can accidentally delete a lot of files this way. | |
| `clear` | clear commands from terminal | |
| `find` \<name of folder\> -name \<name of file\> | Search a directory (and all its subdirectories) for a file | find . -name practice.html |
| `find` \<name of folder\> -name \*<name of file\>` | You can also use the * wildcard to search for all files of a given type (like .jpg) | find . -name '*.jpg' |
| `grep` \"string"\> \<name of file\> | Search for a string in a file | grep "hello" myfile.md |
| `grep -r` \"string"\> | Search recursively through a directory for all occurrences of a string. (Recursive: method where the solution to a problem depends on solutions to smaller instances of the same problem (as opposed to iteration) | grep -r "hello"  |
| `cd~` | userfolder/home | |
| `git init` | Initialize a new repository | |
| `git clone` \<url\> | Clone an existing repository from the internet | |
| `git status` | List all new or modified files | |
| `git diff` | Show file differences that haven't been staged | |
| `git add` \<name of file or folder\> | Stage those commit file | |
| `git commit -m` "Message decribing changes made" | commit changes with message about what you've fixed |**Commit early and often** |

## Branching Git
| Command | Description | Example |
| --- | --- | -- |
| git branch | Shows master branch | Created whenever you create a Git repository. When you work on software don't work on master but create your own branch, do your work, and then merge back into master.
This perseves the working condition of master.
Keep master clean so that it always works |
| `git branch` | Shows master branch | |
| `git branch`\<branch name\> | Creates branch but doesn't switch to branch | |
| `git checkout`\<branch name\> or `git checkout -b`\<branch name\> | Creates new branch and switches to it | |
| `git checkout`\<branch name\> or `git co -b`| Bring up branch created | |
| `git branch -d`\<branch name\> | Delete branch | |
| `subl .` | brings up sublime | |
| `git checkout master` | Brings up original branch | |
| `git branch -d`\<branch name\> | Creates branch but doesn't switch to branch. to move to it | |
| `git checkout master` --> `git merge`\<branch name\>  | Creates branch but doesn't switch to branch. to move to it | |

## GitHub
| Command | Description | Example |
| --- | --- | -- |
| `git push` | sends local (on your cpu) changes to GitHub | |
| `git pull` | will download the changes made to the version others are working on | |
| Create of local repo on your computer first before sending it to github
>1. Start with a folder on computer with files in it(from the command line on the computer)
>2. run: git init inside that folder.
>3. git will create a repo and you can run an initial commit on that repo to store the files you already have in the folder.
>4. Then, use github web interface to create an empty repo that you can copy your local repo into.
>5. On the command line on the computer use: git remote add origin \<url of the repo on git hub\> to connect the two
>6. Then run `git push` to upload the code on github then the two repo files will be the same code and code base. easier (best) is to clone the repo and bringing it to the command line. | | |

| Command | Description | Example |
| --- | --- | -- |
| forking | another way to copy repo | |
| Fork an exsiting repository to our own githup organization:
> 1. navigate to the "Devbootcamp/phase-0-tracks" repository
> 2. click fork in the upper right hand corner of the screen. This creates a copy of this repository to our own github organization.

| `ls -la` | verify that the folder you are creating is not already a git repo  | |
click the button next to that "compare and pull request" . this will push your branch to the master branch. the settings for the pull
base for: your organization (not devbootcamp)
base = master
head fork = your repo
compare = name of branch

1. update the title and description and then click "create pull request"
2. After this step you would normally stop and wait for someone to merge pull request, but in phase 0 you'll be doing this (submitting pull request into your own repo)
3. check the "commits" and "files merged" tabs before you merge to make sure everything is correct
go back to your repo, and you should see the master branch will contain all of the changes made on the feture branch.
4. go to branches to delete old braches that have already been merged to master you don't need to keep the rpo clean and easy to follow.

## 2nd way to create a repo is if you already have existing code
1. go to terminal and create a new folder and file: mkdir <new folder name>, cd <folder name just created>, touch <new file name.file type>.
2. type "ls" to make sure the file is in the folder you created. Now this local file can be pushed locally  to github
3. to push: go to github, your organization (profile), choose new repository, enter name of the folder you created in terminal in the empty field, select public or private, don't select README because you already have existing code. Select "create the repository" you will now see directions/commands instructing you how to set up the inital repo locally.

## to set up the inital repo locally:
1. go to terminal and type "git init" (make sure you are in the new folder you created). "git init" will change that folder into a repository.
2. add files that were in the local folder: "git add <name of file already created.file type>
3. commit the change of adding the file to a git folder: "git commit -m "initial commit".
4. type "git status " to make sure everything is commited (nothing to commit) before pushing and working is clean
5. link local repo to repo on github: "git remote add origin <http repo web address>
6. type "git remote -v" to see that you have the remote file  linked to the github file so that it can be pushed
7. push changes by: "git push -u origin <branch that you want to push/master (most likely master branch because that's where the initial commit was)"
it wil ask for username and password
8. go to github, go to repo and click refresh and you can see that changes have been pushed up. Now the github repository is link to the local repository.
