# Git相关操作命令的集合


| 命令        | 介绍   |
| ------------| -----  | 
| git add. | 将工作区的变化提交到暂存区（.是必须要写的，而且add和.是连在一起的） | 
| git commit -m "提交说明"|将暂存区的文件提交到本地分支 | 
| git pull |从远程分支拉取最新的代码| 
| git push |将本地分支的代码推送远程服务器上，每次推送前必须先拉取代码git pull，保证本地代码为最新，才允许提交| 
| git branch -l |查看本地的分支，其中你正打开的分支名会高亮显示，而且前面会有一个*号 | 
| git branch -a|查看本地和远程分支 | 
| git branch gismaster |创建本地分支gismaster，可以将gismaster换成你想要创建的分支的名字| 
| git checkout gismaster|将代码切换到gismaster分支。如果本分支代码有更改，那么切换之前必须要将代码提交到暂存区，否则不允许你切换分支的 | 
| git push origin gismaster:gis |将本地分支gismaster推送到远程服务器上，并命名为gis | 
| git checkout -b gismaster origin/gis |将远程git仓库里的gis分支拉取到本地并命名为gismaster | 
| git branch -d gismaster|删除本地分支gismaster | 
| git push origin --delete gismaster|删除远程分支gismaster | 
| git merge gismaster |将gismaster分支合并到当前分支 | 
| git remote -v |显示远程仓库信息 | 
| git push origin master |推送远程分支 | 
| git remote set-url origin https***.git |修改远程仓库地址（在已经add了远程仓库地址，使用它进行修改地址） | 
| git remote add origin https***.git |关联远程库（添加远程仓库地址） | 

