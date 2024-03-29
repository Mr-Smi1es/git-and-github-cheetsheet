# Configure Tooling

Thanks to [GitHub](https://github.com/github/training-kit/blob/master/downloads/github-git-cheat-sheet.md).

---
## Coniguring

Configure user information for all local repositories

```bash
git config --global user.name "[name]"
```

Sets the name you want attached to your commit transactions

```bash
git config --global user.email "[email address]"
```

Sets the email you want attached to your commit transactions

```bash
git config --global color.ui auto
```

Enables helpful colorization of command line output

---
## Branches

Branches are an important part of working with Git. Any commits you make will be made on the branch you’re currently “checked out” to. Use git status to see which branch that is.

```bash
git branch [branch-name]
```

Creates a new branch

```bash
git checkout [branch-name]
```

Switches to the specified branch and updates the working directory

```bash
git merge [branch]
```

Combines the specified branch’s history into the current branch. This is usually done in pull requests, but is an important Git operation.

```bash
git branch -d [branch-name]
```

Deletes the specified branch

---
## Make changes

Browse and inspect the evolution of project files

```bash
git log
```

Lists version history for the current branch

```bash
git log --follow [file]
```

Lists version history for a file, including renames

```bash
git diff [first-branch]...[second-branch]
```

Shows content differences between two branches

```bash
git show [commit]
```

Outputs metadata and content changes of the specified commit

```bash
git add [file]
```

Snapshots the file in preparation for versioning

```bash
git commit -m"[descriptive message]"
```

Records file snapshots permanently in version history

---

## Redo commits

Erase mistakes and craft replacement history

```bash
git reset [commit]
```

Undoes all commits after [commit], preserving changes locally

```bash
git reset --hard [commit]
```

Discards all history and changes back to the specified commit

* **CAUTION!** Changing history can have nasty side effects. If you need to change commits that exist on GitHub (the remote), proceed with caution. If you need help, reach out at github.community or contact support.*

---

## Create repositories

When starting out with a new repository, you only need to do it once; either locally, then push to GitHub, or by cloning an existing repository.

```bash
git init
```

Turn an existing directory into a Git repository

```bash
git clone [url]
```

Clone (download) a repository that already exists on GitHub, including all of the files, branches, and commits

---

## The .gitignore file

Sometimes it may be a good idea to exclude files from being tracked with Git. This is typically done in a special file named .gitignore. You can find helpful templates for .gitignore files [here](github.com/github/gitignore).

---

## Synchronize changes

Synchronize your local repository with the remote repository on GitHub.com

```bash
git fetch
```

Downloads all history from the remote tracking branches

```bash
git merge
```

Combines remote tracking branches into current local branch

```bash
git push
```

Uploads all local branch commits to GitHub

```bash
git pull
```

*Updates your current local working branch with all new commits from the corresponding remote branch on GitHub. git pull is a combination of git fetch and git merge.*

---
