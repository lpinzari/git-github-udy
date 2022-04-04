# Merge Branches

Now that you have completed your work, your coworkers have meticulously reviewed the work on your branches, and you are ready to move forward with the changes, we have a few steps to take!

1. Switch to the master branch.

```console
$ git checkout master
```

2. Pull the changes you and your coworkers might have made in the passing days (in this case, you won't have any updates, but **pulling changes is often the first thing you do each day**).

```console
$ git pull origin master
```

3. Since your changes are all ready to go, merge all the branches into the master. Address any merge conflicts. If you split up your work among your branches correctly, you should have no merge conflicts.

```console
$ git merge documentation -m “Merge branch documentation”
$ git merge refactoring -m “Merge branch refactoring”
```

4. You should see a message that shows the changes to the files, insertions, and deletions.

5. Push the repository to your remote repository.

```console
$ git push origin master
```

Go to GitHub. Notice that your master branch has all of the changes.
