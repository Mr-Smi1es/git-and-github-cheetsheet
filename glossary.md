# Glossary

---

## What is **git**

Git is an open source, distributed version-control system

## What is [**GitHub**](https://github.com)

[**GitHub**](https://github.com) is a platform for hosting and collaborating on Git repositories

## What is **HEAD**

A **HEAD** representing your current working directory, the HEAD pointer can be moved to diff.

---

```git init``` initializes a brand new Git repository and begins tracking an existing directory. It adds a hidden subfolder within the existing directory that houses the internal data structure required for version control.

```git clone``` creates a local copy of a project that already exists remotely. The clone includes all the project’s files, history, and branches.

```git add``` stages a change. Git tracks changes to a developer’s codebase, but it’s necessary to stage and take a snapshot of the changes to include them in the project’s history. This command performs staging, the first part of that two-step process. Any changes that are staged will become a part of the next snapshot and a part of the project’s history. Staging and committing separately gives developers complete control over the history of their project without changing how they code and work.

```git commit``` saves the snapshot to the project history and completes the change-tracking process. In short, a commit functions like taking a photo. Anything that’s been staged with git add will become a part of the snapshot with git commit.

```git status``` shows the status of changes as untracked, modified, or staged.

```git branch``` shows the branches being worked on locally.

```git merge``` merges lines of development together. This command is typically used to combine changes made on two distinct branches. For example, a developer would merge when they want to combine changes from a feature branch into the master branch for deployment.

```git pull``` updates the local line of development with updates from its remote counterpart. Developers use this command if a teammate has made commits to a branch on a remote, and they would like to reflect those changes in their local environment.

```git push``` updates the remote repository with any commits made locally to a branch.

```git pull``` requests a place to compare and discuss the differences introduced on a branch with reviews, commentsintegrated tests, and more.

```fork``` a copy of a repository on GitHub owned by a different user.

```git remote``` a common repository on GitHub that all team members use to exchange their changes

```git revert``` Create new commit that undoes all of the changes made in **commit**, then apply it to the current branch.

```git reset``` Remove **file** from the staging area, but leave the working directory unchanged. This unstages a file without overwriting any changes.

```git reflog`` Show a log of changes to the local repository’s HEAD. Add **relative-date** flag to show date info or --all to show all refs.

```git branch``` List all of the branches in your repo. Add a **branch** argument tocreate a new branch with the name **branch**.

```git status``` List which files are staged, unstaged, and untracked.

```git checkout -b``` Create and check out a new branch named **branch**. Drop the -b flag to checkout an existing branch.

```git log``` Display the entire commit history using the default format. For customization see additional options.

```git merge **branch**``` Merge **branch** into the current branch.

```git diff``` Show unstaged changes between your index and working directory.

```git remote add``` Create new commit that undoes all of the changes made in **commit**, then apply it to the current branch.

```git clean -n``` Shows which files would be removed from working directory. Use the -f flag in place of the -n flag to execute the clean.

```git diff HEAD``` Show difference between working directory and last commit.

```git diff --cached``` Show difference between staged changes and last commit

```git reset``` Reset staging area to match most recent commit, but leave the working directory unchanged.

```git config --system core.editor **editor**``` Set text editor used by commands for all users on the machine. **editor** arg should be the command that launches the desired editor (e.g., vi).

```git reset --hard``` Reset staging area and working directory to match most recent commit and overwrites all changes in the working directory.

```git config``` Open the global configuration file in a text editor for manual editing.

```git reset **commit**```Move the current branch tip backward to **commit**, reset the staging area to match, but leave the working directory alone.

```git reset --hard``` Same as previous, but resets both the staging area & working directory to match. Deletes uncommitted changes, and all commits after **commit**.

```--global --edit git log **commit** git log -**limit**``` Limit number of commits by **limit**. E.g. git commits.

```git log --oneline``` Condense each commit to a single line.

```git log -p``` Display the full diff of each commit.

```git log --stat``` Include which files were altered and the relative number of lines that were added or deleted from each of them.

```git log --author=``` Search for commits by a particular author.

```git log``` Search for commits with a commit message that matches **pattern**.

```git log **since**..**until**``` Show commits that occur between **since** and **until**. Args can be a commit ID, branch name, HEAD, or any other kind of revision reference.

```git push **remote** --force``` Forces the git push even if it results in a non-fast-forward merge. Do not use the --force flag unless you’re absolutely sure you know what you’re doing.

```git log -- **file**``` Only display commits that have the specified file.

```git log --graph``` --graph flag draws a text based graph of commits on left side of commit
