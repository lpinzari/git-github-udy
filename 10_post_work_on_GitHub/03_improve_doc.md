# Improve Documentation

In this section, you will be improving the documentation associated with your project.

For this part, you will want to be a little familiar with markdown. For the most part, you can use regular text within a markdown file, but there are some easy ways to make the file more aesthetically appealing (bold, italic, headers, lists).

Now you will be working in your local repository, on the BikeShare python file and the README.md file. You should repeat steps `C` through `E` three times to make at least three commits as you work on your documentation improvements.

A. Create a branch named documentation on your local repository.

```console
$ git branch documentation
```

B. Switch to the documentation branch.

```console
$ git checkout documentation
```

C. Update your README.md file.

D. Stage your changes.

```console
$ git add README.md
```

E. Commit your work with a descriptive message.

```console
$ git commit -m "docs: initial commit"
```

F. Push your commit to your remote repository branch.

```console
$ git push origin documentation
```

G. Switch back to the master branch.

```console
$ git checkout master
```

## Additional changes to documentation

A. Switch back to the documentation branch

```console
$ git checkout documentation
```

B. Make at least 2 additional changes to the documentation - this might be additional changes to the README or changes to the document strings and line comments of the bikeshare file.

After each change, stage and commit your changes. When you commit your work, you should use a descriptive message of the changes made. Your changes should be small and aligned with your commit message.

Push your changes to the remote repository branch.

```console
$ git add README.md
$ git commit -m “Add Credits content”
$ git push origin documentation
$ git add README.md
$ git commit -m “docs: Add Acknowledgement content”
$ git push origin documentation
```

C. Switch back to the master branch.

```console
$ git checkout master
```

D. Check the local repository log to see how all the branches have changed.

```console
$ git log --oneline --graph --all
```

Go to Github. Notice that you now have two branches available for your project, and when you change branches the README changes.
