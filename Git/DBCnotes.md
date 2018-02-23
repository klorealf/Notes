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
| `git checkout`\<branch name\> | Bring up branch created | |
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