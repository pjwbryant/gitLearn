- 在要上传的文件夹下使用git bash打开

- git init
  在当前目录下创建一个 `.git` 子目录，包含 Git 仓库所需的所有元数据和对象存储结构，用于版本控制。

- git add *
  将当前目录下所有改动的文件添加到 Git 的暂存区，准备好文件以便在下一次提交中记录到仓库中

- 配置用户名、和github关联的邮箱：

  - git config --global user.name "pjwbryant"

  - git config --global user.email "pjwbryant@outlook.com"

-  git commit -m "first commit"
  提交暂存区的更改到本地仓库，`-m` 标志允许添加提交信息（这里是 "first commit"），描述本次更改的内容。提交会创建一个快照，永久记录当前暂存区的状态。将更改保存到本地 Git 仓库的历史中，生成一个唯一的提交 ID。

-  git remote add origin https://github.com/pjwbryant/Instant-Messaging-project.git
  添加一个远程仓库并命名为 `origin`，此命令将本地仓库与远程仓库（这里是 GitHub 上的 `https://github.com/pjwbryant/Instant-Messaging-project.git`）关联起来，`origin` 是远程仓库的默认别名。建立本地与远程仓库的连接，允许后续推送或拉取操作

- git push -u origin master
  将本地仓库的提交推送至远程仓库的指定分支，`origin` 是远程仓库的别名。`master` 是本地分支名，推送至远程的同名分支。`-u`（或 `--set-upstream`）设置上游关系，关联本地 `master` 分支与远程 `origin/master`，以后可直接用 `git push` 或 `git pull`。



查看所有分支：
git branch

切换分支：
git switch xxx

创建分支
git branch xxx

查看git配置的github的邮箱、用户名：
git config --global user.name
git config --global user.email

查看所有的配置
git config --global -l

配置代理：
git config --global http.proxy "http://192.168.101.47:7890"
git config --global https.proxy "http://192.168.101.47:7890"

查看代理：
git config --global --get http.proxy 
git config --global --get https.proxy

取消代理：
git config --global --unset http.proxy



![image-20250603203859182](C:\Users\lenovo\AppData\Roaming\Typora\typora-user-images\image-20250603203859182.png)