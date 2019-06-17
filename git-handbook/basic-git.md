# Git 基础

#### Git 基础命令

要使用 Git，开发者用特定命令来复制、创建、更改和组合代码。这些命令可以直接从命令行执行，也可以使用 [GitHub 桌面版](https://desktop.github.com/) 或 Git Kraken 等应用程序执行。以下是一些使用 Git 的常用命令：

* `git init` 初始化一个全新的 Git 仓库并开始跟踪相应目录。它在现有目录中添加了一个隐藏的子目录，其中包含版本控制所需的内部数据结构。
* `git clone` 创建已存在远端的项目的本地副本。克隆将会包括所有的项目文件、历史记录和分支。
* `git add` 暂存修改。Git 跟踪开发者对代码库的更改，但是有必要先暂存并拍摄更改的快照以将其包含在项目的历史记录中。此命令执行暂存功能，这是两步过程的第一部分。任何已暂存的更改都将成为下一个快照的一部分，并成为项目历史的一部分。分别执行暂存和提交可使开发者完全控制其项目的历史记录，而无需更改其编码和工作习惯。
* `git commit` 将快照保存到项目历史记录中并完成更改跟踪过程。简而言之，提交功能就像拍照一样。任何使用 `git add` 暂存的内容都将成为 `git commit` 快照的一部分。
* `git status` 显示更改的跟踪状态，有未跟踪、已修改和已暂存三种。
* `git branch` 显示在本地工作的分支。
* `git merge` 将各个开发分支合并在一起。此命令通常用于将两个不同分支上的更改合并起来。例如，当开发者想要把来自功能分支的更改合并到主分支以进行部署时，他们就可以使用 `git merge`。
* `git pull` 使用远程对应的内容更新本地仓库。如果队友已经对远程分支提交了更新，开发者便可以使用此命令，并且他们希望在本地环境中反映这些更改。
* `git push` 使用本地提交到分支的更改来更新远程仓库。

从 [Git 命令完整参考指南](https://git-scm.com/docs) 中了解更多信息。

**探索更多 Git 命令**

有关 Git 实践的详细介绍，下面的视频展示了如何充分利用 Git 命令。

* [在本地设备工作](https://www.youtube.com/watch?v=rBbbOouhI-s&index=2&list=PLg7s6cbtAD17Gw5u8644bgKhgRLiJXdX4)
* [`git status`](https://www.youtube.com/watch?v=SxmveNrZb5k&list=PLg7s6cbtAD17Gw5u8644bgKhgRLiJXdX4&index=3)
* [两步提交](https://www.youtube.com/watch?v=Vb0Ghkkc2hk&index=4&list=PLg7s6cbtAD17Gw5u8644bgKhgRLiJXdX4)
* [`git pull` 与 `git push`](https://www.youtube.com/watch?v=-uQHV9GOA0w&index=5&list=PLg7s6cbtAD17Gw5u8644bgKhgRLiJXdX4)

