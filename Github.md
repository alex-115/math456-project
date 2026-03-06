GitHub Workflow Commands
 Check your current status
These help you see what’s going on in your repo.
git status
git log --oneline



 Pull the latest changes (always do this first)
Before you start working each day:
git pull



 Stage files you changed
Add everything you modified:
git add .


Or add specific files:
git add filename.Rmd



 Commit your changes
Write a short message describing what you did:
git commit -m "Updated analysis section"



 Push your work to GitHub
Send your commits to the repo:
git push



 Create a new branch (optional but useful for group work)
If someone wants to work separately without touching main:
git checkout -b branch-name


Switch back to main:
git checkout main



 Merge your branch into main (only if needed)
From the main branch:
git merge branch-name



 Undo mistakes (safe versions)
Unstage a file:
git restore --staged filename


Discard local changes to a file:
git restore filename



 Typical daily workflow (3 commands)
Most days, your teammates will only need:
git pull
git add .
git commit -m "message"
git push




