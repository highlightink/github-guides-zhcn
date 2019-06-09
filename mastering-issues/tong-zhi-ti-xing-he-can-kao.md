# 通知，@提及 和引用

通过在问题中使用@提及 和引用，你可以通知其他 GitHub 用户和团队，并相互交叉关联问题。这些方法提供了一种灵活的方式，可以让合适的人员高效地解决问题，并且易于学习和使用。它们适用于 GitHub 上的所有文本字段 —— 它们是我们的文本格式化语法的一部分，称为 [GitHub 版 Markdown](https://help.github.com/articles/writing-on-github#name-and-team-mentions-autocomplete)。

![Markdown &#x4F8B;&#x5B50;](https://guides.github.com/features/issues/markdown-example.png)

如果你想了解更多信息，请查看 [**Mastering Markdown**](http://guides.github.com/features/mastering-markdown/)。

## 通知

[通知](https://github.com/notifications)是 GitHub 与你的 Issues 保持同步的方式。你可以使用它们来查找有关仓库的新 issues，或者只是知道某人何时需要你的输入才能继续处理 issue。

有两种方法可以接收通知：通过邮件和 web。你可以[在设置中](https://github.com/settings/notifications)配置接收通知的方式。如果你预计收到大量通知，我们建议你接收**所参与**项目的 web + 邮件通知，以及**所看过**项目的 web 通知。

![&#x901A;&#x77E5;&#x622A;&#x5C4F;](https://guides.github.com/features/issues/notifications.png)

通过这些设置，当人们特别提到你时，你会收到邮件，接着就可以访问基于 Web 的界面及时了解你感兴趣的仓库。

你可以通过[通知](https://github.com/notifications)界面访问你的所有通知。此界面非常适合一次浏览许多通知并将其标记为已读或静默该通知线程。尝试使用键盘快捷键来加速你的工作流 —— 在页面上按 `?` 查看可用的快捷键。

![&#x4E2A;&#x4EBA;&#x901A;&#x77E5;&#x622A;&#x5C4F;](https://guides.github.com/features/issues/notification.png)

被静默的通知线程在你再次特别提及之前，将不再显示为未读。这是一个静默你不感兴趣的（可能是你不熟悉的某个子系统）通知线程的一个很好的策略。如果你将问题标记为已读，则它将保持这种状态，直到有人再次对该通知线程发表评论为止。

GitHub 还同步邮件通知的已读/未读状态 —— 如果你在邮件客户端中读取通知，它将在基于 Web 的界面中（如果你喜欢此功能，请确保允许你的邮件客户端显示图片）标记为已读。

## @提及

@提及 是我们在 GitHub Issues 中引用其他 GitHub 用户的方式。在描述或 issue 的任何评论内，提及另一个 GitHub 用户的@用户名 以向他们发送通知。这与 Twitter 使用@提及 的方式非常相似。

我们喜欢使用 `/cc` 语法（ 抄送的缩写）来提及 issues 中的人：

> It looks like the new widget form is broken on Safari. When I try and create the widget, Safari crashes. This is reproducible on 10.8, but not 10.9. Maybe a browser bug?
>
> /cc @kneath @jresig

如果你知道要提及的特定用户，这种方法很有用，但很多时候我们在团队中工作但不知道谁可以帮助我们。@提及 也适用于 GitHub 组织内的团队。如果你在@acmeinc 组织下创建一个名为 _browser-bugs_ 的团队，你可以使用@提及 提醒该团队：

> /cc @acmeinc/browser-bugs

这将向 browser-bugs 团队的每个成员发送通知。

## 引用

通常情况下，issues 取决于其他 issues，或者至少与它们有关，并且你希望将这两个 issues 关联起来。你可以通过输入主题标签和问题编号来引用 issues。

> Hey @kneath, I think the problem started in \#42

当你这样做时，我们将在 issue \#42 中创建一个如下所示的事件：

![&#x521B;&#x5EFA;&#x5F15;&#x7528;&#x622A;&#x5C4F;](https://guides.github.com/features/issues/reference.png)

另一个仓库中的 issue 只需在名称之前包含仓库名即可：`kneath/example-project#42` 。

使用 GitHub Issues 的一个更有趣的方法是直接从提交中引用 issue。在提交消息中包含 issue 编号即可。

![&#x63D0;&#x4EA4;&#x4E2D;&#x5F15;&#x7528;&#x7684;&#x622A;&#x5C4F;](https://guides.github.com/features/issues/commit.png)

通过在提交合并到 `master` 分支时将提交信息前缀写为 “Fixes”，“Fixed”，“Fix”，“Closes”，“Closed”，或“Close”，它也会自动关闭该问题。

通过引用，可以将正在完成的工作与正在跟踪的错误进行深入关联，这是增加项目历史可读性的好方法。

