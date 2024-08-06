---
title: Git常用指令
date: 2024-03-10
categories: 关于产品文档
top: 150
---

-  git init ：在当前目录下初始化一个新的 Git 仓库。
-  git clone \<repository-url> ：克隆远程仓库到本地计算机。
-  git add \<file(s)> ：将文件添加到暂存区，准备提交到版本库。
-  git commit -m "commit message" ：提交暂存区的文件到版本库，并附上提交说明。
-  git status ：显示工作目录和暂存区的状态，查看哪些文件被修改或是已经准备好被提交。
-  git diff ：显示工作目录中当前文件与暂存区文件的差异。
-  git log ：显示提交日志，列出当前分支的所有提交记录。
-  git pull ：从远程仓库拉取最新内容并合并到本地分支。
-  git push ：将本地分支的更新推送到远程仓库。
-  git branch ：列出本地分支，显示当前分支以及其他分支的信息。
-  git branch \<branch-name> ：创建一个新的分支。
-  git branch -d \<branch-name> ：删除指定的本地分支。
-  git branch -D \<branch-name> ：强制删除指定的本地分支，即使该分支还未合并。
-  git push origin --delete \<branch-name> ：删除远程仓库中的指定分支。
-  git checkout \<branch-name> ：切换到指定分支。
-  git merge \<branch-name> ：将指定分支合并到当前分支。
-  git reset \<file(s)> ：从暂存区中移除指定文件，但保留工作目录中的修改。
-  git stash ：将当前的工作目录状态保存到堆栈中，稍后可以恢复。
-  git tag \<tag-name> ：打标签，用于标记重要的提交或版本。
