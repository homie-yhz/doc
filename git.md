
# git 常用命令
|命令|说明|
|-|-|
|git init|初始化一个git文件夹|
|-|-|
|git log|查看所有的commit-id 列表|
|git log [-p] [-2] [file]|查看提交记录 [详情] [最近2次] [文件名称]|
|git show commit-id|显示某次提交的具体内容|
|-|-|
|git branch|查看本地已存在的分支，当前分支前面会有 * |
|git branch name|创建本地分支|
|git checkout branchname|切换本地分支|
|git checkout -b branchname|创建本地分支并切换本地分支|
|git branch -r|查看远程分支列表|
|git branch -a|查看远程和本地的所有的分支列表|
|git branch -d name|删除分支，如果在分支中有一些未merge的提交，那么会删除分支失败，此时可以使用 git branch -D name：强制删除dev分支，|
|git branch -vv|可以查看本地分支对应的远程分支|
|git remote add origin(远程库名字) 地址|增加远程库|
|git push origin master:master|在local repository中找到名字为master的branch，使用它去更新remote repository下名字为master的branch，如果remote repository下不存在名字是master的branch，那么新建一个|
|git push origin master|git push origin master:master 因为本地库的branch名字与远程库的branch一样，所以可以省略 :master|
|-|-|
|git checkout -- filename |撤销工作区的某个文件更改或者所有的文件更改|
|git reset HEAD filename |撤销暂存区的某个文件更改或者所有的文件更改|
|git diff|比较工作区与暂存区|
|git diff --cached|比较暂存区与最新本地版本库|
|git diff HEAD|比较工作区与最新本地版本库|
|git diff commit-id|比较工作区与提交的某次id（git log）|
|git diff --cached [<commit-id>]|比较暂存区与提交的某次id|
|git diff [<commit-id>] [<commit-id>]|比较两次commit-id区别|
|-|-|
|1|2|

# 名词解释
|名词|解释|
|-|-|
|工作区|自己的编辑器编辑文件并保存后（ctrl+s）的文件|
|暂存区|add 后 会进入暂存区|
|本地库|commit 后进入本地库|
|commit-id|commit 后会有相应的提交 id|