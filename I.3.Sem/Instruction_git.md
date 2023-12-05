# GIT Instruction

![git_logo](git_logo.jpeg)

_**Git** - it is system for monitoring file versions._ Program saves every change with comment. She saves difference. When you want to open file version, program loads source file and adds into the file change the version.

### Repository

*It is file versions (file changes) storage.*

Enter command to create new repository into the present folder:

    git init

Enter command to see status repository:

    git status

### Adding change to tracking

Enter command to index a change:

    git add <fale_name>

This means, you want add a change to next commit

## Commit change

Enter command to commit a chenge:

    git commit

*When text editor (installed by default) will open, enter comment to change and exit from text editor*

If you want to enter comment in terminal, enter command:

    git commit -m "you comment"

If you want to index all changes (execute command git add) and to commit the chenge, enter command:

    git commit -a

*When text editor (installed by default) will open, enter comment to change and exit from text editor*

If you want to index all changes (execute command git add), to commit the chenge and to enter comment in terminal, enter command:

    git commit -am "you comment"

## Log commits (changelog)

Enter command to show log commits present branch with full info (author, date, message):

    git log 

If you want see shortlog commits present branch, enter command:

    git log --oneline

If you want see log commits all branches with full info (author, date, message, enter command):

    git log --all

If you want see shortlog commits all branches, enter command:

    git log --oneline --all

## Moving through commits and branches

Enter command to move to commit with index "hash":

    git checkout <hash>

*After command you will see your file change with index "hash"*

Enter command for return:

    git checkout <name main branch>

Or enter command with index next commit, what you want see.

## Viewing the changes

Enter command to show changes between last commit and present file:

    git diff

If you want see changes between commits with index "hash1" and "hash2", enter command:

    git diff <hash1> <hash2>

### Ветвления

Ветвления в git нужны для ...

