# Refactor code


1. Create a branch named `refactoring` on your local repository.

```console
$ git branch refactoring
```

2. Switch to the `refactoring` branch.

```console
$ git checkout refactoring
```

3. Similar to the process you used in making the documentation changes, make 2 or more changes in refactoring your code.

Edit the code in your python file.

  - For each change, stage and commit your work with a descriptive message of the changes made.
  - Push your commits to your remote repository branch.

```console
$ git add bikeshare.py
$ git commit -m “refactor: Remove unused function”
$ git push origin refactor
```

**second change**:

```console
$ git add bikeshare.py
$ git commit -m “refactor: Replace redundant code with function”
$ git push origin refactor
```

**Third change**:

```console
$ git add bikeshare.py
$ git commit -m “refactor: Delete redundant code”
$ git push origin master
```

4. Switch back to the master branch.

```console
$ git checkout master
```

5. Check the local repository log to see how all the branches have changed.

```console
$ git log --oneline --graph --all
```

Go to GitHub. Notice that you now have 3 branches. Notice how the files change as you move through the branches.
