# GitHub 风味 Markdown

GitHub.com 使用自己版本的 Markdown 语法，该语法提供了一组额外的有用功能，其中许多功能可以更轻松地使用 GitHub.com 上的内容。

注意，GitHub 风味 Markdown 的某些功能仅在 Issues 和拉取请求的说明和注释中提供。这些包括@提及以及对 SHA-1 哈希、Issues 和拉取请求的引用。任务列表也可以在 Gist 评论和 Gist Markdown 文件中使用。

#### 语法高亮

以下是如何使用 [GitHub 风味 Markdown](https://help.github.com/articles/basic-writing-and-formatting-syntax/) 进行语法高亮的示例：

```text
```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```
```

你还可以简单地将代码缩进四个空格：

```text
    function fancyAlert(arg) {
      if(arg) {
        $.facebox({div:'#foo'})
      }
    }
```

以下是没有语法高亮的 Python 代码示例：

```text
def foo():
    if not bar:
        return True
```

#### 任务列表

```text
- [x] 支持@提及、#引用、[链接]()、**格式化**、和 <del>标签</del>
- [x] 需要列表语法（支持任何无序或有序列表）
- [x] 这是一个已完成事项
- [ ] 这是一个未完成事项
```

如果你在 Issue 的第一条评论中包含任务列表，你将在问题列表中获得一个方便的进度指示器。 它也适用于拉取请求！

#### 表格

你可以通过组合单词列表并用连字符 `-` 分隔（第一行），然后用管道符 `|` 分隔每个列创建表格：

```text
标题一 | 标题二
------------ | -------------
第一格内容 | 第二格内容
第一列内容 | 第二列内容
```

会变成：

| 标题一 | 标题二 |
| :--- | :--- |
| 第一格内容 | 第二格内容 |
| 第一列内容 | 第二列内容 |

#### SHA 引用

对提交的 [SHA-1 哈希](http://en.wikipedia.org/wiki/SHA-1) 的任何引用都将自动转换为 GitHub 上对应提交的链接。

```text
16c999e8c71134401a78d4d46435517b2271d6ac
mojombo@16c999e8c71134401a78d4d46435517b2271d6ac
mojombo/github-flavored-markdown@16c999e8c71134401a78d4d46435517b2271d6ac
```

#### 仓库内引用 Issue

任何引用 Issue 或拉取请求的编号都将自动转换为链接。

```text
#1
mojombo#1
mojombo/github-flavored-markdown#1
```

#### 用户名 @提及

输入 `@` 符，后跟用户名，将通知该用户来查看评论。这被称为“@提及”，因为你_提及_了某个人。你还可以在组织内@提及团队。

#### 自动链接 URLs

任何 URL（如 `http://www.github.com/`）都将自动转换为可点击的链接。

#### 删除线

用两个波浪号包裹的任何单词（比如 `~~这个~~`）都会显示出删除线。

#### Emoji

GitHub 支持 [emoji](https://help.github.com/articles/basic-writing-and-formatting-syntax/#using-emoji)！

要查看我们支持的所有图片的列表，请查看 [Emoji 速查表](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)。

