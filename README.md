git init: initialise current folder as a git repo
git clone: brings the remote repo from URL to current folder
git status: tells us current repo and its state
git add <FILE>: adds a file to the staging area
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
