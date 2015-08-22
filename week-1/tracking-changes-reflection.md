## Tracking Changes Reflection

- How does tracking and adding changes make developers' lives easier?
- What is a commit?
- What are the best practices for commit messages?
- What does the HEAD^ argument mean?
- What are the 3 stages of a git change and how do you move a file from one stage to the other?
- Write a handy cheatsheet of the commands you need to commit your changes?
- What is a pull request and how do you create and merge one?
- Why are pull requests preferred when working with teams?

Tracking and adding changes makes developers' lives easier because they can see every single thing that was done on a project and can easily roll back if there was a change made that is creating issues.
A commit is basically a snapshot of the project. You are saving your work.
Commit messages should be in the imperative form, present tense. Instead of saying "Added this and that to the project" you would say "Add this and that to the project" They should be one line 50 characters or less and then if they need to be longer do paragraphs or bullet points underneath.
The HEAD^ argument is the last commit that was made on the current branch. So if you just made a commit on the master branch and were still checked out to the master branch and wanted to roll back one commit you would use HEAD^.
The 3 stages of a git change are untracked, staged and committed. When you first create a file, it is not initially being tracked by git so you can't save the changes. To get a file to be staged, you would use the command "git add ." with the period meaning the current file you are on. You could also use the file's name. Once you do that, the file is being tracked and it is also staged, which means that the files is ready to be committed. If you then went and modified the new file, the file would be modified but those changes are not staged. You would have to use git add command again. To commit them, which is the last stage of git change, you would use "git commit -m "message"". This would commit those staged changes and your local directory would be saved.
Cheat Sheet
git commit -m "message here" - This is what you do to commit a change
git add filename - This is what you write to start tracking a new file or stage some changes
git push origin branch-name - This is what you use to push changes up to Github
git pull origin branch-name - This is what you do to pull changes from Github down to your local machine
git checkout branch-name - This is how you switch branches
git checkout -b branch-name - This is how you make a new branch with the name branch-name
git status - This is how you check the status of what's being tracked and committed
git log - This is how you check the history of all the commits you've made.
A pull request is a request for a change you have made to project on GitHub. Once you have pushed your branch and changes up to GitHub, you create a pull request by selecting "New Pull Request" on your Github account. At this point you can review the changes you've made to the Master branch and then you would select merge and merge your branch with the master branch. You can then delete your branch and go to your local machine and pull down the new master branch.
Pull requests are preferred when working with a team because it allows a lot of people to work at once on the same project but allow all the changes you are making to not affect the master branch of the project until changes are approved. Then they can be merged.