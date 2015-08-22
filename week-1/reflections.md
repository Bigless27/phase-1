#1.1 Think About Time Reflection
I tried to review each idea briefly, but I was ultimately most intrigued by the Fogg Method and mindfulness meditation. I liked these two topics because they were very different but they also seemed like they could be very effective together.
Timeboxing is the process of allocating a fixed period of time, or a time box, to each timed activity. It could be extremely effective in Phase 0 because Phase 0 is broken down into weekly schedules and that is broken down into a bunch of different assignments that each will take a short amount of time. It is the perfect scenario for time boxing.
Currently I use time boxing but I never had a name for it or how to improve my use of time boxing, for instance with the Pomodoro technique. My current strategy works but distractions have always been an issue, especially being on the computer all day. The Internet can be a big distraction and it is easy to procrastinate.
So I will employ a few new strategies. I will use the Pomodoro technique to work for a set 25 minute period with a timer, and actively block out distractions. I will also do a short 2 minute meditation session in the morning to clear my head, get rid of distractions and unhelpful thoughts and calm my brain.
I am hoping to start with tiny new habits and expand on them from there to change my behavior. Overall I plan to break each task down into smaller components and not get overwhelmed by the bigger picture so I can stay on track.
#1.2 The Command Line Reflection
The shell is a user interface that lets you interact with an operating system. An example of this is the Command Line which is a really efficient way to interact with the Unix Operating System. Bash is a free Unix Shell that gives you access to all the command line tools for interacting with the Unix operating system.
The toughest part for me when going through this was the pushd and popd commands, I didn't really get what they did when doing the examples in the crash course, but with some extra examples from a Google search it made more sense and it was pretty straight forward. Also I understood apropos but when I used it it was hard to find any useful information with it. For example, when I did "apropos search" I had a hard time finding "find" which is what I would be looking for.
I was able to successfully use all of the commands although sometimes when using "man" it was hard to figure out what do do. For example "man grep" gives you the manual for grep and there were all these options that I didn't understand completely what they did.  But I understood all the basics and to me the most important were the pipe command which would make doing multiple processes with one line of code very easy and makes the shell very powerful. Also with cd and ls, it makes moving around your computer very easier, much easier than using the GUI.
Here are my explanations for what these commands do:
-pwd: print working directory prints what directory you are currently in
-ls: This lists all the files and directories that are in your current directory
-mv: This moves a file from one location to another location that you specify.
-cd: This changes the curretn directory to the directory that you specify
-../ This means go up one level in your directory hierarchy.
-touch: touch will create a new file.
-mkdir: Create a new directory
-less: Less lets you move through a file and look at its contents
-rmdir: This lets you remove a directory that is empty.
-rm: This lets you remove a file
-help: This is the same as man for MacOS. It shows you the manual for a command.
#1.4 Forking and Cloning Reflection
First, I will explain how to create a new repository on Github. You need to have a Github account and you need to go to your profile. In the top right corner there is a plus sign. When you click on that, there are two options, the first is to create a new repository. Click on that and you are taken to another page where you can specify the name of the new repository, whether it is public or private (who can view), and whether or not to add a license. Click create and you are all done.
To fork a repository, you would go to an existing repository on someone's Github account and then in the upper right corner you would click Fork. This simple action would create a copy of that repository, same name and contents and all on your GitHub account.
To clone a repo, you would go to the repo's page on YOUR GitHub account and find the clone URL in the bottom right. Then you would go to your terminal and navigate to a folder where you would like to create the clone of the repository. Let's say it's a folder on your desktop called Phase 0. When you are in that folder you would type git clone [clone URL] with [clone URL] being the URL you copied from the repository page on GitHub. This creates a clone of the remote repository hosted on GitHub on your local computer.
I would fork a repository when I wanted to work off a open-source project or something that has already been started and I wanted to add to but didn't want to make changes to the original. I would create a new repository if I was starting a new project from scratch and wasn't using some open source code that was already available.
I didn't have many struggles with this assignment because I've used GitHub a little bit in the past but I was not aware of the forking feature so that was helpful to learn. I also had some trouble deleting a cloned repository with the command line. When I typed rm -r [repository directory] it would ask if I wanted to override, and I was not sure what it wanted me to do.
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