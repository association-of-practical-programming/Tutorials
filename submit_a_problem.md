# Submit a problem to GitHub
So you just finished the problem, now you need to submit your problem to GitHub. How do you do that?
Well first you want to make sure that you have git installed on your computer. If you do not, consult the
`clone_a_repo` tutorial.

We use git as a version control system. It makes it easier to store all of our code on GitHub (note: **git** and **GitHub** are not the same thing. git
is version control software and GitHub is a service that uses git to store files. There are many alternatives to GitHub like GitLab and BinBucket)

Once you pull the repository and you are done coding you are going to want to create a new branch. A **branch** in git is a different version of the code. It takes all of the same code and allows you to edit it without affecting the main version of the code. To make a new branch navigate to the directory containing the files that you changed and run `git checkout -b <branch name>` where you replace "\<branch name\>" with the name of the branch you want to create.

Now that we are on a new branch, we want to tell git about files so it can track them. To do this we need to **add** the files to git. Type `git add <filename>` where you replace "\<filename\>" with the name of the file. This is adding a certain file to git's list of files to track. If you just want to add all of your files in the current directory you can run the command `git add .`.

Now that the files are added to git's tracking, we need to take a snapshot of the code. This is called a **commit** in git. We have to commit our code to group all of our changes into one snapshot. To commit, type `git commit -m "<your message>"` Where you replace "\<your message\>" with a small blurb of information about these file changes. For example, you could write this `git commit -m "Fixed bug with game"`.

Now that we have a commit on our branch, we want to **push** that to GitHub. To do this we want to type `git push`. If this is the first time pushing to that branch, you'll have to set the upstream so git knows where to push the code, the command for that is `git push --set-upstream origin <branch name>`.

Now you should be able to see your code on GitHub if you go to the repository and search for your branch by clicking the dropdown. Then you need to create a Pull Request. A pull request is a way of merging your files on your branch into the main branch. To make a PR, click the Pull Request button on your branch. Then give your PR a good name and description and press the green button that says "Create Pull Request". Then you are done, I will review your code and make sure everything is in order then I will approve your code and then merge it into master.

If you want anymore resources on git and making pull requests here are some more resources that you can read.
- [git tutorial](https://www.tutorialspoint.com/git/)
- [another git tutorial](https://www.atlassian.com/git/tutorials)
- [Youtube series about git](https://www.youtube.com/watch?v=BCQHnlnPusY&list=PLRqwX-V7Uu6ZF9C0YMKuns9sLDzK6zoiV)
- [Create a PR](https://help.github.com/desktop/guides/contributing-to-projects/creating-a-pull-request/)

