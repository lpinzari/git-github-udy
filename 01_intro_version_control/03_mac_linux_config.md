# Mac/Linux Set up

We are going to install Git on our machine.

## Installing Git

Git is actually installed on MacOS, but we'll be reinstalling it so that we'll have the newest version:

1. go to [https://git-scm.com/downloads](https://git-scm.com/downloads)
2. download the software for Mac
3. install Git choosing all of the default options

Once everything is installed, you should be able to run git on the command line. If it displays the usage information, then you're good to go!

## First Time Git Configuration

Before you can start using Git, you need to configure it. Run each of the following lines on the command line to make sure everything is set up.

```console
# sets up Git with your name
$ git config --global user.name "<Your-Full-Name>"

# sets up Git with your email
$ git config --global user.email "<your-email-address>"

# makes sure that Git output is colored
$ git config --global color.ui auto

# displays the original state in a conflict
$ git config --global merge.conflictstyle diff3

$ git config --list
```

## Git & Code Editor
The last step of configuration is to get Git working with your code editor. Below are three of the most popular code editors. If you use a different editor, then do a quick search on Google for "associate X text editor with Git" (replace the X with the name of your code editor).

**Atom Editor Set up**

<code>git config --global core.editor "atom --wait"</code>

**Sublime Text Set up**

<code>git config --global core.editor "'/Applications/Sublime Text 2.app/Contents/SharedSupport/bin/subl' -n -w"</code>

**VS Code setup**

<code>git config --global core.editor "code --wait"</code>
