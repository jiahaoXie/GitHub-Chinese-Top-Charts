# Git 仓库在 Fork 后同步源仓库
1. 列出当前为 Fork 配置的远程仓库
2. 指定将与 Fork 同步的新远程上游（upstream）仓库
  $ git remote add upstream https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git
3. git remote -v 验证新上游仓库
4. 抓取原仓库的更新 git fetch upstream
5. 将来自 upstream/master 的更改合并到本地 master 分支中。这就实现了与上游仓库的同步，而不会丢失本地的更改
    git merge upstream/master
6. git push 推送到远程，git push不成功则使用git push origin master

参考资料：
https://www.jianshu.com/p/b3506494ad98
https://github.com/selfteaching/the-craft-of-selfteaching/issues/67

# 备注
* 数据结构和算法可学习：
krahets/hello-algo

* Java 知识可学习：
doocs/advanced-java