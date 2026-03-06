Handling Merge Conflicts
Merge conflicts happen when two people edit the same part of a file and Git can’t decide whose version to keep. They’re normal in group work and easy to fix once you know the steps.

What a merge conflict looks like
When you run git pull or git merge, Git may stop and show something like:
CONFLICT (content): Merge conflict in analysis.Rmd


Inside the file, you’ll see markers:

<<<<<<< HEAD

your version

=======

their version

>>>>>>> origin/main


You must choose which version to keep (or combine them).

 Steps to Fix a Merge Conflict
1. Open the conflicted file
Look for the conflict markers:

<<<<<<< HEAD

=======

>>>>>>> 


Decide what the final version should be.
2. Edit the file to remove the markers
Delete the conflict markers and keep the correct content.
The file should look clean—no <<<<<<<, =======, or >>>>>>>.

3. Stage the resolved file
git add filename.Rmd



4. Complete the merge with a commit
git commit


Git will auto‑generate a merge commit message.
Just save and close the editor if one opens.

5. Push your resolved version
git push



 If you want to cancel the merge instead
If you realize you pulled at the wrong time or want to restart:
git merge --abort


This resets your repo to the state before the merge attempt.

 Tips to Avoid Merge Conflicts
- Always run git pull before you start working.
- Communicate who is editing which file.
- Avoid editing the same section of the .Rmd at the same time.
- Commit and push frequently.
