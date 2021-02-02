# git_intro

Hi,

The file you're looking at is a markdown (.md file). Here's a [link](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) to learn some markdown syntax. Github is a website built on a program called git, which does version control.

# Start with Github

1. Make an account on [Github](https://github.com).
2. Download/Install git from [here](https://git-scm.com/downloads).
3. You're ready to begin.

# Repositories

1. Make a repo under our [organization](https://github.com/FHBiostat-Postdocs)
2. Click on the green "New" button and name your repo.
3. Once created on Github, on your local machine/computer, clone the repo from Github. 

  For Windows users, open the Git Bash program (a Windows linux terminal shell), navigate to the folder you want to save the repo. On Github on your repo's page, click on the green "Code" button, copy the https link. In the Git Bash program, type `git clone <copied_https_link>`.

For Mac / Linux(cluster) users, the git program is just a command accessible from the command line within the terminal. Like Windows users, navigate to where you would like to place the repo and type `git clone <copied_https_link>`. 

Congrats, your repo (from Github) is now copied onto your local computer.

# Saving progress

While a project is worked on, files are created, edited, saved, or deleted. Any files created under your repo directory are all by default being tracked with version control.

Try creating a simple text or script file with a few lines of text. Save it like you normally would on your local machine. 

Type `git status` to see which files are being tracked and have been updated relative to the current repo directory on Github. When in doubt about the status of a repo, type `git status` to gain some insights. 

In git, the word "save" is not commnly used. Instead, there are three general steps called **add**, **commit**, and **push**. 

1. Git add is used to specify which of the files listed in the `git status` output you want to eventually save to Github. To syntax is 

```
git add <file1> <file2> ... <fileN>
```

You can type multiple things to save files. `git add *.R` will add all files ending in .R that appeared from `git status`. `git add *` will add all files from `git status`.

2. Next, we `commit` our changes from `git add` and we can include a handy note/message informing ourselves or others what was changed. This is useful because we could be looking at a long list of commits to track the changes to a file over time. The syntax and example is 

```
git commit -m "fix bug, add slides"
```

3. Finally, we `push` our commits to Github with

```
git push
```

By doing these steps, we can see our updated repo on Github after refreshing the webpage. Also, once updates are pushed to Github, everyone that can access your repo will see exactly what was updated. The best part is you can edit your repo on local computer 1 by (1) cloning the repo onto that computer, (2) git add/commit/push your changes, (3) go to your local computer 2 and continue where you left off after git cloning.

We only need to run the `git clone ...` command once for each repo to copy the current version of the repo from Github. If the repo already exists on your local computer, to get the next updated repo, type (from within the repo directory on your computer)

```
git pull
```

The list of changes within a repo can be found on Github under the green Code button where you will see "# commits".

# Other topics to maybe include in this repo

* Multiple people editing a repo
* .gitignore This is useful to instruct git to, by default, not save certain files ending in certain extensions.

# Other repo ideas

* Navigating linux/bash
* installing R locally vs using R module
* Running interactive R vs batch R
* Submitting customized linux job
* Scripting everything I just wrote

# Some References



