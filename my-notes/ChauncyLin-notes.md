# 学习这本书的目标
- 学会自学，掌握自学的技巧
- 掌握**进化** 方法

# 自学能力的重要性
- 缓解甚至消除个人焦虑
- 做到持续学习、持续成长
- 不因学习以及学习过程焦虑

# 手艺的定义
- 无需天分
- 由熟练程序决定

# 为什么说99%的人没掌握自学能力？
99%的人在别人教、有人带、被人逼的情况下被动学习那些没真学明白的基础知识，这些知识的用处只是为了通过考试，考完就遗弃了。
在以后的生活中，能意识到自己应该学些什么，但因为没人教、没人带基本以无奈结束。

# 如何成为前百分之二十的少数人？
- 把买来的书真切的认真读过
- 不要只屯书，买了要读

# Git入门指南
以下示意图中仅包含最基本的 Git 命令 —— 并且基本上都是独自使用 Git 时的常用命令。

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/git-command-relationships.png?raw=true)

```
Between:upstrem repository & upstrem repository
upstrem repository 上游仓库
origin/master
fork
pull request
git init
>新建一个Git管理项目

Between:upstream repository & working directory
git clone
>从目标服务器得到整个用Git管理项目的拷贝
git pull
>类似与SVN中的update动作，如果你N久前clone得到某项目的一份拷贝，用pull可以更新到最新版本

Between:upstrem repository & local repository
local repository
HEAD
master
commit
git fetch
git push
>把当前的这份拷贝push到服务器


Between: local repository & branches
branches 两个子版本，当前版本出现了两个不同分支
git merge
>如果我正在编辑一个新版本a，有人在编辑新版本b，我们想把两个版本合成一个，就可以用merge。当然，合的过程中，有时候会检出有哪些地方不一样，询问到底要保留哪一个，需要手动处理不同的地方。事实上，这更像一个审查的过程。
git branch

Between: local repository & staging area
staging area
Index
git reset
>如果你正在编辑的文件乱了，可以选择从前面的commit点(假设是a点）重新开始编辑，通常是选择恢复到上一个编辑点。
git commit 
>告诉Git你想要记录现在的操作，Git会保留一个当前修改过文件的快照。
git diff
>找出两个文档或目录的不同
git revert
>回卷到指定的commit
Between:staging area & working directory
git add 
>添加新的文件（文件夹）到Git项目中，如果添加文件夹，该文件夹下所有文件将被包含。同时可以使用rm，mv从git项目中删除或是重命名文件（文件夹）。
git rm



```