Git is a distributed version control system.
Git is free software distributed under the GPL.
Git has a mutable index called stage.



初始化一个Git仓库，使用git init命令。

添加文件到Git仓库，分两步：
使用命令git add <file>，注意，可反复多次使用，添加多个文件；
使用命令git commit -m <message>，完成。


现在，运行git status命令看看结果：

已经记不清上次怎么修改的readme.txt，所以，需要用git diff这个命令看看：


提交修改和提交新文件是一样的两步，第一步是git add：

$ git add readme.txt
同样没有任何输出。在执行第二步git commit之前，我们再运行git status看看当前仓库的状态：

$ git commit -m "add distributed"

保存一个快照

HEAD指向的版本就是当前版本，因此，Git允许我们在版本的历史之间穿梭，使用命令git reset --hard commit_id。

穿梭前，用git log可以查看提交历史，以便确定要回退到哪个版本。

要重返未来，用git reflog查看命令历史，以便确定要回到未来的哪个版本。


