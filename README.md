git init: initialise current folder as a git repo
git clone: brings the remote repo from URL to current folder
git status: tells us current repo and its state
git add <FILE>: adds a file to the staging area
    git add . :adds files and folders in the current folder
git commit: open text editor to add a commit message
    git commit -m "<message>": commit with a message
    git commit -a -m "<message>": add and commit with message
git restore <FILE>: discard any changes that have been made to the file
git log: view chamge history
    git log --oneline: view change history summary
git diff: compare changes in unstaged files
    git diff --staged: compare changes in staged files
    git diff HEAD~<n>: compare HEAD commit with previous n commit, eg git diff HEAD~2
    git diff <commit hash>: compare HEAD with given commit hash (use git log --oneline to see the commit hashes)
git restore --source <HASH OR HEAD~n> <FILE>: restore file to given commit
    git checkout <HASH OR HEAD~n> <FILE>: restore file to given commit (older command)
        git checkout <HASH OR HEAD~n>: no file given, detached HEAD state
        undo using 
            git switch -
        or
            git checkout <branch>

.gitignore file - held in the top level directory, can be overrideen using .gitignore files in lower folders

git remote -v: list the remotes you have
git push <WHERE> <WHAT>: pushes (sync) the WHAT branch to WHERE, eg git push origin master
git pull <WHERE> <WHAT>: pulls (sync) the WHAT branch in WHERE to local computer, eg git pull origin master
