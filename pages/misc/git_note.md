---
layout: default
---
### git command
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
git branch [branch-name]
git checkout [branch-name]
git merge [branch]
git branch -d [branch-name]
```
</details>
<details><summary markdown="span">Synchronize changes</summary>
```
git fetch  (Downloads all history from the remote tracking branches)
git merge  (Combines remote tracking branch into current local branch)
git push   (Uploads all local branch commits to GitHub)
git pull   (Updates your current local working branch with all new commits from the corresponding remote branch on GitHub. git pull is a combination of git fetch and git merge)
```
</details>
<details><summary markdown="span">Make changes</summary>
```
git log
```
Lists version history for the current branch
```
git log --follow [file]
```
Lists version history for a file, including renames
```
git diff [first-branch]...[second-branch]
```
Shows content differences between two branches
```
git show [commit]
```
git add [file]
git commit -m "[descriptive message]"
```
</details>
