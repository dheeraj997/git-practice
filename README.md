What is Git?

Git is a distributed version control system.

It tracks changes in your code or files over time.

Helps teams collaborate, maintain history, and avoid conflicts.

Key idea: you can always rollback, branch, or merge safely.

Analogy:

Think of Git like a time machine for your project — you can go back, try new features, or collaborate without breaking the main project.


getting stated with git




echo "# git-practice" >> README.md


git init


git add README.md


git commit -m "first commit"


git branch -M main


git remote add origin https://github.com/dheeraj997/git-practice.


git push -u origin main
------------------------------------------------------------------------------
create and merge a new branch

git checkout -b branch name  or git branch branch name or git switch -c branch-name

merge conflicts must be done manually---

merge from main
git merge branch-name

deleting a branch
git branch -d branch name

delete in github
git push origin --delete dev
-------------------------------------------------------------------------------
revert to old time line

git log

git status

There are 4 main rollback methods in Git, each for a different purpose:

Undo last commit (keep changes) → git reset --soft

Undo last commit (discard commit but keep files) → git reset --mixed

Undo last commit and delete all changes → git reset --hard

Rollback by creating a new commit that reverses changes → git revert