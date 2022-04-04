# Determine A Repo's status

Working with Git on the command line can be a little bit challenging because it's a little bit like a black box. I mean, how do you know when you should or shouldn't run certain Git commands? Is Git ready for me to run a command yet? What if I run a command but I think it didn't work...how can I find that out? The answer to all of these questions is the <code>git status</code> command!

```console
$ git status
```

The <code>git status</code> is our key to the mind of Git. It will tell us what Git is thinking and the state of our repository as Git sees it. When you're first starting out, **you should be using the git status command all of the time!** Seriously. You should get into the habit of running it after any other command. This will help you learn how Git works and it'll help you from making (possibly) incorrect assumptions about the state of your files/repository.

## Git Status Output

```console
(base) ludo /course-git-blog-project [master] $  git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
```

## Git Status Explanation

The output tells us two things:

- **On branch master** – this tells us that Git is on the master branch. You've got a description of a branch on your terms sheet so this is the "master" branch (which is the default branch). We'll be looking more at branches in lesson 5
- **Your branch is up-to-date with 'origin/master'**. – Because git clone was used to copy this repository from another computer, this is telling us if our project is in sync with the one we copied from. We won't be dealing with the project on the other computer, so this line can be ignored.
- **nothing to commit, working tree clean** – this is saying that there are no pending changes.

Think of this output as the "resting state" (that's not an official description - it's how I like to describe it!). This is the resting state because there are no new files, no changes have been made in files, nothing is in the staging area about to be committed...no change or action is pending, so that's why I like to call it the resting state.

So this is what it looks like when running git status in a repository that already has commits. Let's switch to the new-git-project project to see what the git status output will produce.

```console
(base) ludo /course-git-blog-project [master] $  cd ..
(base) ludo /udacity-git-course  $  ls
course-git-blog-project new-git-project
(base) ludo /udacity-git-course  $  cd new-git-project/
(base) ludo /new-git-project [master] $  git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
```

## Explanation Of Git Status In A New Repo
This is the output of running git status in the new-git-project project:

```console
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
```

To be completely clear, I haven't made any commits in my project yet. If you have made a commit, then your output should look exactly like that of the *course-git-blog-project project*.

If you compare this to the git status output from the course-git-blog-project project, then you'll see that they're pretty similar. The thing to note that's different is that this output includes the line *No commits yet*.

Wanna have a sneak peak of the next lesson and at the same time prove that there aren't any commits in this repo yet? Great, I knew you did! Try running the command <code>git log</code> and check out its response:

```console
(base) ludo /new-git-project [master] $  git log
fatal: your current branch 'master' does not have any commits yet
(base) ludo /new-git-project [master] $
```

Well, that's kind of scary looking. "Fatal"? Fortunately, it turns out that just means that the Git program is exiting because it can't find any work to do. Git tells us this as if it were an error, but it's really not a problem. We know we haven't put any commits into this repo yet.

It's pretty clear from the response that there aren't any commits!

We've just taken a very brief look at the <code>git status</code> command. Remember that the output of git status will change depending on if files have been *added/deleted/modified*, **what's on the staging index**, and the **state of the repository**. We'll be using the git status command throughout this entire course, so get comfortable running it!

## Git Status Recap
The git status command will display the current status of the repository.
```
$ git status
```
I can't stress enough how important it is to use this command all the time as you're first learning Git. This command will:

- tell us about new files that have been created in the Working Directory that Git hasn't started tracking, yet
- files that Git is tracking that have been modified
- a whole bunch of other things that we'll be learning about throughout the rest of the course ;-)

## Helpful links

- [Checking the status of your files](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository#Checking-the-Status-of-Your-Files)
- [git status docs](https://git-scm.com/docs/git-status)
- [git status tutorial](https://www.atlassian.com/git/tutorials/inspecting-a-repository)
