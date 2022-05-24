# git-demo
git常用命令
一.基本命令：
1.设置用户签名：
git config --global user.name 用户名
git config --global user.email 邮箱
2.初始化本地库：
git init
3.查看本地库状态：
git status
4.添加到暂存区：
git add 文件名
5.提交到本地库：
git commit -m "说明信息" 文件名
6.查看历史记录：
git reflog
git log
7.版本穿梭：
git reset --hard 版本号

二.分支操作：
1.查看分支：
git branch -v
2.创建分支：
git branch 分支名
3.切换分支：
git checkout 分支名
4.合并分支(把指定分支合并到当前分支)
git merge 分支名
5.解决分支冲突：
    编辑有冲突的文件，删除特殊符号，决定要使用的内容
    添加到暂存区
    执行提交（注意：此时使用 git commit 命令时不能带文件名）
6.更改分支名
git branch -m 旧分支名 新分支名

三.远程仓库：
1.查看远程仓库别名：
git remote -v
2.创建远程仓库别名：
git remote add 别名 远程地址
3.推送本地分支上的内容到远程仓库
git push 别名 分支名
4.将远程仓库的内容克隆到本地
git clone 远程地址
5.将远程仓库对于分支最新内容拉下来后与当前本地分支直接合并
git pull 远程仓库别名 远程分支名
