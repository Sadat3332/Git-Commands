# Git-Commands

---
## *Basic Git Commands*


### Setting up Your Git Identity
| Command           | Description                               |  Example(s)                                            |
| ----------------- | ----------------------------------------- |  ----------------------------------------------------- |
| `git config --global user.name`        | Setup your name in Git   | `git config --global user.name Your-Name`                                 |
| `git config --global user.email`        | Setup your mail in Git   | `git config --global user.email Your-mail@example.com`  |

---

### Getting started with Git
| Command           | Description                                 | Example(s)                                            |
| ------------------------ | -----------------------------------------  |----------------------------------------------------- |
| `git init`        | Initialize empty Git repository    | `git init new-project`                                 |
| `git clone`        | Clone a repository from remote server      |  `git clone https://github.com/user/repo.git`                                 |

---

### Commiting Changes
| Command                 | Description                               | Example(s)                                            |
| ------------------------ | ----------------------------------------- |----------------------------------------------------- |
| `git status` | Show the status of Working Directory|  -|
| `git add`| Add files to staging Area|  `git add file1.txt file2.txt`|
| `git add -A`| Add all new and changed files to staging area     | -|
| `git commit`| Commit staged changes|  `git commit -m "latest bug fix"`|
---

### Branching
| Command                 | Description                               | Example(s)                                            |
| ------------------------ | ----------------------------------------- |----------------------------------------------------- |
| `git branch` | List branches|  -|
| `git branch <branch-name>`| Create a new branch|  `git branch feature-branch`|
| `git branch -d <branch-name>`| Delete a merged branch    | `git branch -d feature-branch`|
| `git branch -D <branch-name>`| Delete a branch (Merged or not)|  `git branch -D test-branch`|
| `git branch -m <old-branch-name> <new-branch-name> `| Rename a branch | `git branch -m  feature-branch-v1.0  feature-branch-v2.0`|
| `git push origin --delete <branch-name>`| Delete a remote branch|  `git push origin --delete feature-branch`|
| `git checkout <branch-name>`| switch to a branch |  `git checkout feature-branch`|
| `git checkout -b <branch-name>`| create a new branch and switch to it |  `git checkout -b feature-branch`|
| `git checkout -- <file-name>`| Discard changes to a file | `git checkout -- test.txt`|
| `git checkout . `| Discard all changes in your working directory and  revert the files to the last committed state. | -|

---
### Merging

| Command                                        | Description                        | Example(s)                                          |
| ---------------------------------------------- | ---------------------------------- | --------------------------------------------------- |
| `git merge <branch-name>`       | Merge a branch          | `git merge feature-branch`               |
| `git merge <source-branch> <target-branch>`              |Merge a branch into target branch | `git merge feature-V1 feature-V0`               |
---

### Reviewing

| Command                                        | Description                        | Example(s)                                          |
| ---------------------------------------------- | ---------------------------------- | --------------------------------------------------- |
| `git status`       | Displays the current status of your working directory and staged changes   | -               |
| `git log`              | Displays a detailed commit history of the current branch | -          |
| `git log --oneline`              |Displays a simplified commit history of the current branch in a compact format | -          |
| `git diff`              | Shows the differences between your working directory and the most recent commit | -          |
| `git diff <commit1> <commit2>`              | Compares two commits and displays the differences between themt | `git diff abc123 xyz987`        |

---
### Stashing

| Command                                        | Description                        | Example(s)                                          |
| ---------------------------------------------- | ---------------------------------- | --------------------------------------------------- |
| `git stash`       |store modified and staged changes         | -              |
| `git stash save "comment"`              |stash the modified changes with description| `git stash save "Work in Progress - Feature 1"`               |
| `git stash list`              |List all stashes| -               |
| `git stash apply`              |Applies the most recent stash entry to your working directory, without deleting the stash entry| -               |
| `git stash pop`              |Applies the most recent stash entry to your working directory and deletes it| -               |
| `git stash show`              |Show the difference summary of recent stash entry| -               |
| `git stash drop`              |Delete the recent stash entry without applying it| -               |
| `git stash clear`              |Delete all stash entries| -               |




---
### Git commands related to remote repositories

| Command                                        | Description                        | Example(s)                                          |
| ---------------------------------------------- | ---------------------------------- | --------------------------------------------------- |
| `git push`       |Push changes to remote repository       | -              |
| `git pull`       |Fetch the latest update from remote repository and merge with local one      | -              |
| `git push origin <branch-name>`       |Push a branch to the remote repository      | `git push origin feature-branch`              |
| `git push origin --delete <branch-name>`       |Delete a remote branch    | `git push origin --delete feature-branch`           |
| `git fetch origin`       |Fetch the changes from remote repository without merging   | -|
| `git fetch origin <branch-name>`       |fetch changes from a remote branch without merging  | `git fetch origin main`           |
| `git remote`       |view all remote connections        | -              |
| `git remote remove <connection-name>`              |Remove a connection| -               |
| `git remote rename <old-name> <new-name>`              |Rename a connection| -            |
| `git pull --rebase origin`              |Rebase local changes on top of new changes from remote repository| -               |



---
### Common Configuration

| Command                                        | Description                        | Example(s)                                          |
| ---------------------------------------------- | ---------------------------------- | --------------------------------------------------- |
| `git config --global alias.<alias-name> <git command>`       | Configure Git aliases              | `git config --global alias.co checkout`               |
| `git config --global core.editor`              | Configure default text editor      | `git config --global core.editor "code"`               |
| `git config --global --edit`                   | Edit Git configuration in an editor | -                                               |

---
