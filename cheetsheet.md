# Git Cheetsheet

## Github Flow

The 6 Step GitHub flow:

1. Create a branch: Topic branches created from the canonical deployment branch (usually master) allow teams to contribute to many parallel efforts. Short-lived topic branches, in particular, keep teams focused and results in quick ships.

2. Add commits: Snapshots of development efforts within a branch create safe, revertible points in the project’s history.
3. Open a pull request: Pull requests publicize a project’s ongoing efforts and set the tone for a transparent development process.
4. Discuss and review code: Teams participate in code reviews by commenting, testing, and reviewing open pull requests. Code review is at the core of an open and participatory culture.
5. Merge: Upon clicking merge, GitHub automatically performs the equivalent of a local ‘git merge’ operation. GitHub also keeps the entire branch development history on the merged pull request.
6. Deploy: Teams can choose the best release cycles or incorporate continuous integration tools and operate with the assurance that code on the deployment branch has gone through a robust workflow.

---

## Configure Tooling

Configure user information for all local repositories

```$ git config --global user.name "[name]"```

Sets the name you want attached to your commit transactions

```$ git config --global user.email "[email address]"```

Sets the email you want attached to your commit transactions

```$ git config --global color.ui auto```

Enables helpful colorization of command line output

---

Branches
Branches are an important part of working with Git. Any commits you make will be made on the branch you’re currently “checked out” to. Use git status to see which branch that is.

```$ git branch [branch-name]```

Creates a new branch

```$ git checkout [branch-name]```

Switches to the specified branch and updates the working directory

```$ git merge [branch]```

Combines the specified branch’s history into the current branch. This is usually done in pull requests, but is an important Git operation.

```$ git branch -d [branch-name]```

Deletes the specified branch

---

## Make changes

Browse and inspect the evolution of project files

```$ git log```

Lists version history for the current branch

```$ git log --follow [file]```

Lists version history for a file, including renames

```$ git diff [first-branch]...[second-branch]```

Shows content differences between two branches

```$ git show [commit]```

Outputs metadata and content changes of the specified commit

```$ git add [file]```

Snapshots the file in preparation for versioning

```$ git commit -m"[descriptive message]"```

Records file snapshots permanently in version history

---

## Redo commits

Erase mistakes and craft replacement history

```$ git reset [commit]```

Undoes all commits after [commit], preserving changes locally

```$ git reset --hard [commit]```

Discards all history and changes back to the specified commit

* **CAUTION!** Changing history can have nasty side effects. If you need to change commits that exist on GitHub (the remote), proceed with caution. If you need help, reach out at github.community or contact support.*

---

## Create repositories

When starting out with a new repository, you only need to do it once; either locally, then push to GitHub, or by cloning an existing repository.

```$ git init```

Turn an existing directory into a Git repository

```$ git clone [url]```

Clone (download) a repository that already exists on GitHub, including all of the files, branches, and commits

---

## The .gitignore file

Sometimes it may be a good idea to exclude files from being tracked with Git. This is typically done in a special file named .gitignore. You can find helpful templates for .gitignore files [here](github.com/github/gitignore).

---

## Synchronize changes

Synchronize your local repository with the remote repository on GitHub.com

```$ git fetch```

Downloads all history from the remote tracking branches

```$ git merge```

Combines remote tracking branches into current local branch

```$ git push```

Uploads all local branch commits to GitHub

```$ git pull```

*Updates your current local working branch with all new commits from the corresponding remote branch on GitHub. git pull is a combination of git fetch and git merge.*
