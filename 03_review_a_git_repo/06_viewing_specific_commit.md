# Viewing a specific commit

Wouldn't it be super handy if you could just display a specific commit's details without worrying about all of the others in the repo? **Too much scrolling**

There are actually two ways to do this!

1. providing the SHA of the commit you want to see to <code>git log</code>
2. use a new command <code>git show</code>

They're both pretty simple, but let's look at the <code>git log</code> way and then we'll look at <code>git show</code>.

You already know how to "log" information with:

- <code>git log</code>
- <code>git log --oneline</code>
- <code>git log --stat</code>
- <code>git log -p</code>

But did you know, you can supply the SHA of a commit as the final argument for all of these commands? For example:

```
$ git log -p fdf5493
```

By supplying a SHA, the git log -p command **will start at that commit!** No need to scroll through everything! Keep in mind that **it will also show all of the commits that were made prior to the supplied SHA**.

## New Command: git show
The other command that shows a specific commit is git show:

```
$ git show
```

Running it like the example above will only display the most recent commit. Typically, a SHA is provided as a final argument:

```
$ git show fdf5493
```

### What does git show do?

The git show command will **show only one commit**. So don't get alarmed when you can't find any other commits - it only shows one. The output of the <code>git show</code> command is exactly the same as the <code>git log -p</code> command. So by default, git show displays:

- the **commit**
- the **author**
- the **date**
- the **commit message**
- the **patch information**

However, git show can be combined with most of the other flags we've looked at:

- <code>--stat</code> - to show the how many files were changed and the number of lines that were added/removed
- <code>-p</code> or <code>--patch</code> - this the **default**, but if <code>--stat</code> is used, the patch won't display, so pass <code>-p</code> to add it again <code>git show fdf5493 --stat -p</code>
- <code>-w</code> - to ignore changes to whitespace
