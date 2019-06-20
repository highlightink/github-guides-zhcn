# GitHub

#### GitHub 是如何融入 Git 的

GitHub 是一个 Git 托管仓库，它为开发人员提供工具，通过命令行功能、issues（线程化的讨论流程）、拉取请求、代码审查或在 GitHub 集市中使用一系列免费和收费应用程序来造就更好的代码。通过 GitHub 工作流等协作方式，拥有 1500 万开发者的社区以及拥有数百个集成功能的生态系统，GitHub 改变了软件的构建方式。

#### GitHub 是如何工作的

GitHub 直接将协作构建到开发过程中。工作流程被组织到仓库中，开发者可以在其中概述需求或发展方向并为团队成员预设期望。然后，使用 GitHub 工作流，开发者只需创建一个分支来处理更新，提交更改并保存它们，发起拉取请求以提出并讨论更改，并在所有人达成共识时合并拉取请求。

**GitHub 工作流**

GitHub 工作流是一个基于分支的轻量级工作流，围绕世界各地团队（包括我们的团队）使用的核心 Git 命令构建。

GitHub 工作流有六个步骤，每个步骤在实施时都有显著的好处：

1. **创建分支：**从规范部署分支（通常是 `master` 分支）创建的主题分支允许团队为许多并行工作做出贡献。特别是短时间存在的主题分支，可以使团队专注工作并快速发展。
2. **添加提交：**分支上的开发快照在项目历史中创建了安全，可恢复的时间点。
3. **发起拉取请求：**拉取请求公开项目的持续进展，并为透明的开发过程定下基基调。
4. **讨论并审查代码：**团队通过评论，测试和审查开放的拉取请求来参与代码审查。代码审查是开放与参与文化的核心。
5. **合并：**单击合并后，GitHub 会自动执行与本地“git merge”等效的操作。GitHub 还在合并的拉取请求中保留整个分支开发历史记录。
6. **部署：**团队可以选择最佳的发布周期或加入持续集成工具，并确保部署分支上的代码通过了稳健的工作流程的考验。

**了解有关 GitHub 工作流更多信息**

开发者可以在下面提供的资源中找到有关 GitHub 工作流的更多信息。

* [指南](https://itechub.gitbook.io/github-guides-zhcn/github-flow/intro)
* [GitHub 工作流演示视频](https://www.youtube.com/watch?v=47E-jcuQz5c&index=1&list=PLg7s6cbtAD17Gw5u8644bgKhgRLiJXdX4)

#### GitHub 与命令行

对于刚接触命令行的开发者，GitHub 培训团队已经整理了一系列 Git 命令的 [教程](https://help.github.com/articles/git-and-github-learning-resources/) 来指导方向。有时候，一系列命令可以描绘出如何使用 Git 的景象：

**示例：为现有仓库做贡献**

```text
# 从 GitHub.com 把仓库下载到我们的设备上
git clone https://github.com/me/repo.git

# 切换到 `repo` 目录
cd repo

# 创建一个新分支以存储修改
git branch my-branch

# 切换到该分支（开发主题）
git checkout my-branch

# 做一些修改，例如使用文本编辑器编辑 `file1.md` 和 `file2.md`

# 暂存已修改的文件
git add file1.md file2.md

# 为暂存的文件（任何被添加入暂存区的文件）做一个快照
git commit -m "my snapshot"

# 将更改推送至 github
git push --set-upstream origin my-branch
```

**例子：新建一个仓库并发布到 GitHub**

首先，你需要在 GitHub 上创建一个新的仓库。你可以在我们的 [Hello World 指南](http://itechub.gitbook.io/github-guides-zhcn/hello-world/create-a-repository) 中学习如何创建新的仓库。**不要**使用 README、.gitignore 或 License 文件来初始化仓库。这个空的仓库就只等着你的代码。

```text
# 创建一个新目录，并使用 git 特定函数来初始化它
git init my-repo

# 切换到 `my-repo` 目录
cd my-repo

# 创建项目的第一个文件
touch README.md

# git 还没开始跟踪此文件，先暂存它
git add README.md

# 为暂存区拍一个快照
git commit -m "add README to initial commit"

# 为仓库设置 github 远程仓库地址
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git

# 将更改推送至 github
git push --set-upstream origin master
```

**例子：向 GitHub 上的现有分支贡献**

```text
# 假设：机器上已经存在一个名为 `repo` 的项目，并且自上次在本地进行更改后，有新的分支已被推送到 GitHub.com

# 切换到 `repo` 目录
cd repo

# 更新所有远程跟踪分支和当前所在的分支
git pull

# 切换到已有的 `feature-a` 分支
git checkout feature-a

# 做一些修改，例如：使用编辑器编辑 `file1.md` 文件

# 暂存修改的文件
git add file1.md

# 为暂存区做一次快照
git commit -m "edit file1"

# 将更改推送至 github
git push
```

#### 协作开发的模型

人们在 GitHub 上合作主要有两种方式：

1. 共享仓库
2. [分叉](https://help.github.com/en/articles/about-forks) 与 [拉取](https://help.github.com/en/articles/about-pull-requests)

使用_共享仓库_，个人和团队被明确指定为具有读取、写入或管理员访问权限的贡献者。这种简单的权限结构与受保护的分支和 Marketplace 等功能相结合，可以帮助团队在采用 GitHub 时快速进展。

对于开源项目或任何人都可以贡献的项目，管理个人权限可能具有挑战性，但是_分叉_与_拉取_模型允许任何可以查看项目的人做出贡献。分叉是开发者个人帐户下项目的副本。每个开发者都可以完全控制他们的分支，并可以自由地实现修复或新功能。在分叉中完成的工作要么保持独立，要么通过拉取请求合并回原始项目。在那里，维护人员可以在合并之前查看建议的更改。有关更多信息，请参阅 [分叉项目指南](http://itechub.gitbook.io/github-guides-zhcn/forking-projects/intro)。

#### 按自己的节奏学习

GitHub 团队创建了一个教育视频和指南库，以帮助用户继续充实他们的技能并构建更好的软件。

* [探索入门项目](https://github.com/showcases/great-for-new-contributors)
* [GitHub 指引视频](https://youtube.com/githubguides)
* [GitHub 按需学习](https://services.github.com/on-demand/)
* [GitHub 学习指南](https://guides.github.com/)
* [GitHub 学习资源](https://services.github.com/resources/)

