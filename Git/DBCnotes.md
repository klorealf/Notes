DBC notes

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
| `git init` or `git clone` \<url\> | Initialize a new repository or clone an existing one from the internet | |
| `git status` | List all new or modified files | |
| `git diff` | Show file differences that haven't been staged | |
| `git add` \<name of file or folder\> | Stage those commit file | |
| `git commit -m` "Message decribing changes made" | commit changes with message about what you've fixed |**Commit early and often**
| `git diff` | Show file differences that haven't been staged | |
| `git diff` | Show file differences that haven't been staged | |