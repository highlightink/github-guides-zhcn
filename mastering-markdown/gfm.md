# GitHub Flavored Markdown

GitHub.com uses its own version of the Markdown syntax that provides an additional set of useful features, many of which make it easier to work with content on GitHub.com.

Note that some features of GitHub Flavored Markdown are only available in the descriptions and comments of Issues and Pull Requests. These include @mentions as well as references to SHA-1 hashes, Issues, and Pull Requests. Task Lists are also available in Gist comments and in Gist Markdown files.

#### Syntax highlighting

Here’s an example of how you can use syntax highlighting with [GitHub Flavored Markdown](https://help.github.com/articles/basic-writing-and-formatting-syntax/):

```text
```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```
```

You can also simply indent your code by four spaces:

```text
    function fancyAlert(arg) {
      if(arg) {
        $.facebox({div:'#foo'})
      }
    }
```

Here’s an example of Python code without syntax highlighting:

```text
def foo():
    if not bar:
        return True
```

#### Task Lists

```text
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
```

If you include a task list in the first comment of an Issue, you will get a handy progress indicator in your issue list. It also works in Pull Requests!

#### Tables

You can create tables by assembling a list of words and dividing them with hyphens `-` \(for the first row\), and then separating each column with a pipe `|`:

```text
First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column
```

Would become:

| First Header | Second Header |
| :--- | :--- |
| Content from cell 1 | Content from cell 2 |
| Content in the first column | Content in the second column |

#### SHA references

Any reference to a commit’s [SHA-1 hash](http://en.wikipedia.org/wiki/SHA-1) will be automatically converted into a link to that commit on GitHub.

```text
16c999e8c71134401a78d4d46435517b2271d6ac
mojombo@16c999e8c71134401a78d4d46435517b2271d6ac
mojombo/github-flavored-markdown@16c999e8c71134401a78d4d46435517b2271d6ac
```

#### Issue references within a repository

Any number that refers to an Issue or Pull Request will be automatically converted into a link.

```text
#1
mojombo#1
mojombo/github-flavored-markdown#1
```

#### Username @mentions

Typing an `@` symbol, followed by a username, will notify that person to come and view the comment. This is called an “@mention”, because you’re _mentioning_the individual. You can also @mention teams within an organization.

#### Automatic linking for URLs

Any URL \(like `http://www.github.com/`\) will be automatically converted into a clickable link.

#### Strikethrough

Any word wrapped with two tildes \(like `~~this~~`\) will appear crossed out.

#### Emoji

GitHub supports [emoji](https://help.github.com/articles/basic-writing-and-formatting-syntax/#using-emoji)!

To see a list of every image we support, check out the [Emoji Cheat Sheet](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md).

