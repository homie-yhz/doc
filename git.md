# git 常用命令
|命令|说明|
|-|-|
|git init|初始化一个git文件夹|
|-|-|
|git log|查看所有的commit-id 列表|
|git show commit-id|显示某次提交的具体内容|
|git diff|比较工作区与暂存区|
|git diff --cached|比较暂存区与最新本地版本库|
|git diff HEAD|比较工作区与最新本地版本库|
|git diff commit-id|比较工作区与提交的某次id（git log）|
|git diff --cached [<commit-id>]|比较暂存区与提交的某次id|
|git diff [<commit-id>] [<commit-id>]|比较两次commit-id区别|
|||
|||

# 名词解释
|名词|解释|
|-|-|
|工作区|自己的编辑器编辑文件并保存后（ctrl+s）的文件|
|暂存区|add 后 会进入暂存区|
|本地库|commit 后进入本地库|
|commit-id|commit 后会有相应的提交 id|