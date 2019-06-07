# 创建一个分支

**分支**是同时在不同版本的仓库上工作的方式。

默认情况下，你的仓库有一个名为 `master` 的分支，它被认为是标准分支。在提交到 `master` 之前，我们使用其他分支进行试验和编辑。

当你从 `master` 创建分支时，相当于做了一个 `master` 的副本或快照，就像是位于和 `master` 同一个时间点一样。如果其他人更改了 `master` 分支，而此时你工作在自己的分支上，则可以拉取别人的更新。

该图显示了：

* `master` 分支
* 一个叫做 `feature`（因为我们在此分支上“开发功能”）的分支
* `feature` 在合并到 `master` 之前所经历的旅程

![&#x5206;&#x652F;&#x521B;&#x5EFA;&#x4E8E;&#x5408;&#x5E76;](https://guides.github.com/activities/hello-world/branching.png)

Have you ever saved different versions of a file? Something like:

你有没有保存过同一文件的不同版本？就像是：

* `story.txt`
* `story-joe-edit.txt`
* `story-joe-edit-reviewed.txt`

分支在 GitHub 仓库中实现了类似的目标。

在 GitHub，我们的开发者、作家和设计师使用分支来保持错误修复和功能开发与 `master`（生产）分支分开。当更改准备就绪时，他们才会将自己的分支合并到 `master`。

#### 创建一个新分支

1. 前往你的新仓库 `hello-world`。
2. 点击文件列表顶端显示了 **branch: master** 的下拉列表。
3. 往新建文本框里输入一个分支名，`readme-edits`。
4. 选择蓝色的 **Create branch** 块或按“Enter”键。

![&#x4ECE; master &#x521B;&#x5EFA;&#x4E00;&#x4E2A;&#x65B0;&#x5206;&#x652F;](https://guides.github.com/activities/hello-world/readme-edits.gif)

现在你有两个分支，`master`和`readme-edits`。它们看起来完全一样，但很快就是不是了！接下来，我们将更改添加到这个新分支。

