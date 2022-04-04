# Set Up Your Repository

The following are the steps you will take to work on the `README` markdown file, your BikeShare python `file` (project completed in the previous Python Lesson), and post the files to your GitHub profile.

- Step 1. Create a GitHub profile (if you don’t already have one).
- Step 2. Complete the tasks outlined below and add in the Required Responses in the Git Commands Documentation.

1. **Fork** the following GitHub repo [https://github.com/udacity/pdsnd_github](https://github.com/udacity/pdsnd_github)

2. After forking you will have a remote repo in your GitHub account.

The only file is the **README.md**, message of the commit `create README.md`.

```
### Date created
Include the date you created this project and README file.

### Project Title
Replace the Project Title

### Description
Describe what your project is about and what it does

### Files used
Include the files used

### Credits
It's important to give proper credit. Add links to any repo that inspired you or blogposts you consulted.
```

**Clone** the remote repository to your local machine.

```console
$ git clone https://github.com/lpinzari/pdsnd_github.git
```

3. Move your `bikeshare.py` and data files into your local machine.

4. Create a `.gitignore` file containing your data file, `.csv` files. We don't want to push our data to GitHub, as they are large files.

```console
$ touch .gitignore
```

**.gitignore**
```
# bikeshare data files
chicago.csv
new_york_city.csv
washington.csv
```

**Note**: Remember to push changes ONLY to your own repo in your GitHub account. You can verify the remote using `git remote -v` command.

5. Check the `status` of your files to make sure that your data files are not being track.

```console
$ git status
```

6. Stage your changes

```console
$ git add .gitignore
$ git add bikeshare.py
```

7. Commit your changes with a descriptive message:

```console
$ git commit -m "chore: Add .gitignore file"
$ git commit -m "feat: Add bikeshare.py script"
```

8. Push your commit to your remote repository

```console
$ git push origin master
```

9. Go to GitHub. Ensure that the files you wanted to push to your remote repo match your local, and that the files you did not want to add are not available.
