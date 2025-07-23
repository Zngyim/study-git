# study-git
Using to study some git command

1. `git status`查看git的目前状态
	修改文件后未添加到暂存区则会显示
```
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
```

2. `git add .`可将所有文件添加到暂存区

3. `git add <file_name>`将所选文件添加到暂存区
```
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   README.md
 
**此时更改等待被commit**
```

4. `git commit -m"commit message"`commit提交

