# study-git
Using to study some git command

1.  先配置git的账号信息
```
git config --global user.name "用户名"
git config --global user.email zngyim@gmail.com
*并非必要*
```

2. git生成ssh公钥及私钥，github的ssh key配置
```
ssh-keygen -t rsa -C "zngyim@gmail.com"
**注意在主目录下执行，才会将.ssh文件防止在主目录下**
**连续敲击空格即可**

*公钥文件打开*
一般ubuntu并未配置可以直接打开的软件，于是使用命令
cat ~/.ssh/id_rsa.pub

另外.ssh文件一般处于隐藏状态，有两种方式可以看到
1. ls -a
2. 在交互界面使用ctrl+h

```
复制公钥后在github settings里添加即可
添加后使用一次`git clone`就可变为激活状态，此时`git clone`使用的是SSH key

3. `git status`查看git的目前状态
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

4. `git add .`可将所有文件添加到暂存区

5. `git add <file_name>`将所选文件添加到暂存区
```
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   README.md
 
**此时更改等待被commit**
```

6. `git commit -m"commit message"`commit提交

7. `git push`将commit推至github

8. `git branch <branch_name>`创建分支，`git switch <branch_name>`切换分支
9. `git checkout -b <branch_name>`合并上述两个命令

10. `git clone <SSH>`从远端克隆仓库

11. `git pull`把远端改动拉取到本地
	

