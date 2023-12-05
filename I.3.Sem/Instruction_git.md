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

### Branching

*Branching uses for collaborate on the file or changes on the file while another users use this file.*

Enter command to viewing branches:

    git branch

Enter command to create new branc:

    git branch <branch_name>

If you want delete branch, enter command with option:

    git branch -d <branch_name>

### Merging branches

*Merging branches used when you want joining information from two branches into one. Information will adding into branch where are you.* 

For merging enter comman:

    git merge <branch_name>

#### Merging conflicts

*Error in merge process it is conflict between current local branch and branch with which do merging. It is conflict with code another programmer. Git do all for merging but some conflicts need correct by yourself.*

For resolve conflict merging do:

1. Open file in text redactor
* Text between lines "<<<<<<< HEAD" and  "=======" it is text current branch.
* Text from line "=======" to line ">>>>>>> new_branch_to_merge_later" it is branch text with which do merging
2. Correct file and delete lines  "<<<<<<< HEAD",  "=======", ">>>>>>> new_branch_to_merge_later"
3. Save and close text redactor.
4. Add and commit changed in repository in terminal

If you work in VSC you can chose one of several resolve conflict:

* Accept current change
* Accept incoming change
* Accept both change
* Compare changes

Or resolve conflict  on redactor