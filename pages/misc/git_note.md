---
layout: default
---
### git command (expand)
#### References:
* [Book](https://git-scm.com/book/en/v2)


{::options parse_block_html="true" /}
<details><summary markdown="span">Create repositories</summary>
```
git init
git clone [url]
```
</details>
<details><summary markdown="span">Configuration tools</summary>
```
git config --list
git config --global user.name "[name]"
git config --global user.email "[email address]"
git config --global color.ui auto
```
</details>
<details><summary markdown="span">The .gitignore file</summary>
```
step:1 create a text file name .gitignore
step:2 include the files you want not to git
```
</details>
<details><summary markdown="span">Git Branches</summary>
```
git branch [branch-name]      (Creates a new branch)
git checkout [branch-name]    (Switches to the specified branch
                               and updates the working directory)
git merge [branch]            (Combines the specified branch’s history into the
                               current branch. This is usually done in pull
                               requests, but is an important Git operation.
git branch -d [branch-name]   (Deletes the specified branch)
```
</details>
<details><summary markdown="span">Synchronize changes (Synchronize local repo with the remote repo)</summary>
```
git fetch  (Downloads all history from the remote tracking branches)
git merge  (Combines remote tracking branch into current local branch)
git push   (Uploads all local branch commits to GitHub)
git pull   (Updates your current local working branch with all new commits from the corresponding remote branch on GitHub. git pull is a combination of git fetch and git merge)
```
</details>
<details><summary markdown="span">Make changes (Browse and inspect the evolution of project files)</summary>
```
git log                           (Lists version history for the current branch)
git log --follow [file]           (Lists version history for a file, including
                                   renames)
git diff [first-branch]...[second-branch]  (Shows content differences between
                                            two branches)
git show [commit]                 (Outputs metadata and content changes of the
                                   specified commit)
git add [file]                    (Snapshots the file in preparation for versioning)
git commit -m "[descriptive message]"  (Records file snapshots permanently in version history)
```
</details>
<details><summary markdown="span">Redo commits (Erase mistakes and craft replacement history)</summary>
```
git reset [commit]   (Undoes all commits after [commit], preserving changes locally)
git reset --hard [commit]   (Discards all history and changes back to the specified commit)
```
</details>
