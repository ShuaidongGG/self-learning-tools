# Git
## 版本控制

为什么要版本控制？在交付一项任务时，提交的内容一次被老板接受的可能性几乎为0，所以需要不停的对内容进行增删改，直到有一版被老板认可或是经过对比还是选择了之前的一版。控制版本这个事情如果每次都由自己手动控制，那显然是不太方便而且不太现实的，尤其是在多人合作开发时，各人有各人的想法，每个人提出的都应该是一个独立的版本，那么采用自动化版本控制就显得非常有必要。

## 主流版本控制器
- Git
- SVN
- CVS
- VSS
- TFS
- Visual Studio Online

## 本地版本控制



## 集中式版本控制 SVN

单点故障

## 分布式版本控制 Git

每个人都拥有全部代码，在本地就可以查看历史版本

**Git是最先进的分布式版本控制**

## 文件状态

- Untracked
未跟踪，一个普通文件与git无关 git add 一个文件 该文件状态变为 `Staged`

- Unmodify
文件已入库，未修改。1.被修改，变为`Modified` 2. git rm 从库中移除 变为`Untracked`

- Modified
文件已修改。1. git add 再次提交 变为 `Staged` 2. git checkout 放弃修改 退回到 `Unmodify`

- Staged
暂存状态 通过git commit 将文件同步到库中 状态变为 `Unmodify`
执行 git reset HEAD 该文件 状态变为`Modified`

