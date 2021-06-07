# 一、标题 （Headings）
要创建标题，请在单词或短语前面添加井号（#）。井号的数量代表了标题的级别。例如，添加三个“#”即创建一个三级标题。例如：<br>
> ### 这是一个三级标题
## 可选语法
---
还可以在文本下方添加任意数量的“--”号来表示二级及以下标题。请参考本段标题。<br>
# 段落
## 创建段落
要创建段落，请使用空白行将一行或多行文本进行分隔。<br>
### 创建段落实践
除非在段落列表中，否则不要用空格（Spaces）或制表符（Tabs）缩进段落。<br>
## 换行
在一行的末尾添加两个或多个空格，然后按回车键（Return），即可创建一个换行（Line Break）。<br>
### 换行实践
相较于空格+Return的换行方法，使用HTML语法的\<br>标签换行更为直观和方便，也更方便后期的修改与文档维护。<br>
# 强调
## 粗体
要加粗文本，请在单词或短语的前后各添加两个星号（\*）。如需加粗一个单词或短语的中间部分用以强调的话，请在要加粗部分的两侧各添加两个星号。<br>
```markdown
> Love\**is**bold.
``` 
## 斜体
要用斜体显示文本，请在单词或短语前后添加一个星号。要斜体突出单词的中间部分，请在字母前后各添加一个星号，中间不要带空格。<br>
# 块引用（Blockquotes）
要创建块引用，请在段落前加一个\>符号。例如：<br>
> 这是一个块引用。
## 多个段落的块引用
块引用可以包含多个段落，为段落之间的空白行各添加一个\>符号。例如：<br>
``` markdown
> 第一行
>
> 第三行
```
渲染效果如下：<br>
> 第一行
>
> 第三行<br>
## 嵌套块引用（Nested Blockquotes）
块引用可以嵌套。在要嵌套的段落前添加一个“\>>”符号。例如：<br>
```markdown
> 第一行
>
>> 第二行
```
渲染效果如下：
> 第一行
>
>> 第二行 <br>
## 带有其他元素的块引用（Blockquotes with Other Elements）
块引用可以包含其他*Markdown*格式的元素。并非所有元素都可以使用，你需要进行实验以查看哪些元素有效。<br>
# 列表（Lists）
## 有序列表（Ordered Lists）
要创建有序列表，请在每个列表项前添加数字并紧跟一个英文句点。数字不必按数学顺序排列，但是列表应当以数字1起始。例如：
```markdown
1. First item.
2. Second item.
3. Third item.
5. Forth item.
```
1. First item.
2. Second item.
3. Third item.
5. Forth item.<br>
## 无序列表（Unordered Lists）
要创建无序列表，请在每个列表项前面添加破折号（-）、星号（*）或加号（+）。缩进一个或多个列表项可创建嵌套列表。例如：<br>
```markdown
- First item.
* Second item.
+ Third item.
```
- First item.
* Second item.
+ Third item.<br>
## 无序列表实践
要在保留列表连续性的同时在列表中添加另一种元素，请将该元素缩进四个空格或一个制表符，如下所示：<br>
### 段落
```markdown
* This is the first list item.
* Here's the second list item.
    I need to add another paragraph below the second list item.
* And here's the third list item.
```
* This is the first list item.
*   Here's the second list item.
    I need to add another paragraph below the second list item.
* And here's the third list item.<br>
### 引用块
```markdown
* This is the first list item.
* Here's the second list item.
    >I need to add another paragraph below the second list item.
* And here's the third list item.
```
* This is the first list item.
* Here's the second list item.
    >I need to add another paragraph below the second list item.
* And here's the third list item.<br>
### 代码块（Code Blocks）
```markdown
* This is the first list item.
* Here's the second list item.
    ```python
    print("Hello World!)
    ```
* And here's the third list item.
```
* This is the first list item.
* Here's the second list item.
    ```python
    print("Hello World!)
    ```
* And here's the third list item.<br>
# 代码（Codes）
 要将单词或短语表示为代码，请将其包裹在反引号“`”中。例如：<br>
 ```markdown
`print("Hello World.")`
 ```
`print("Hello World.")`
# 分割线（Horizontals Rules）
要创建分隔线，请再单独一行上使用三个或多个星号（***）、破折号（---）或下划线（___），并且不能包含其他内容。为了兼容性，请在分隔线的前后均添加空白行。例如：<br>
```markdown
***

---

_________
```
***

---

_________ 
# 链接（Links）
要创建链接，请将链接文本括在中括号中，后面紧跟着括在圆括号中的URL。例如：<br>
```markdown
我最喜欢的搜索引擎是[谷歌](https://google.com)
```
我最喜欢的搜索引擎是[谷歌](https://google.com)。
## 添加标题
你可以选择为链接添加标题（即title属性）。当用户将鼠标悬停在链接上时，将显示一个提示。要添加标题，请将其放在URL后面（注意留出空格）。例如：<br>
```markdown
我最喜欢的搜索引擎是[谷歌](https://google.com"The best search engine ever.")
```
我最喜欢的搜索引擎是[谷歌](https://google.com "The best search engine ever").
## 网址和电子邮件地址
要将URL或电子邮件地址快速转换为链接，请将其括在尖括号中。例如：<br>
```markdown
<https://www.markdownguide.org>
<username@example.com>
```
<https://www.markdownguide.org>
<username@example.com>
## 格式化链接
如需强调某个链接，请在方括号前及圆括号后添加星号。
要将链接表示为代码，请在方括号内添加反引号。
```markdown
This is the *[Markdown Guide](https://www.markdownguide.org)*.
This is the **[Markdown Guide](https://www.markdownguide.org)**.
查阅有关[`代码（Codes）`](#代码（Codes）)的表述。
```
This is the *[Markdown Guide](https://www.markdownguide.org)*.<br>
This is the **[Markdown Guide](https://www.markdownguide.org)**.<br>
查阅有关[`代码（Codes）`](#代码（Codes）)的表述。

# 引用式链接
引用式（Reference-Style）链接是一种特殊类型的链接，它使得URL在Markdown中更易于显示和阅读。引用式链接由两部分组成：一部分被放置于正文文本中；另一部分被放置在文档中的其他地方，以便于阅读。<br>
## 引用式链接第一部分的格式
引用式链接的第一部分的格式由两组方括号组成。第一组方括号内放的是显示为链接的文本，第二组方括号内放的是一个标签，该标签用于指向您存放在文档中其它位置的链接。<br>
尽管不是必须的，但你可以在第一组和第二组方括号之间添加一个空格。第二组方括号中的标签不区分大小写，并且可以包含字母、数字、空格或标点符号。<br>
以下示例中，链接的第一部分是等效的：<br>
```markdown
+ [hobbit-hole][1]
+ [hobbit-hole] [1]
```
## 引用式链接第二部分的格式
引用式链接的第二部分可以包含以下属性：
1. 放在方括号内的标签，以及紧跟在方括号后面的一个冒号和至少一个空格（例如 [label]: ）。
2. 链接的 URL，可以选择将其括在尖括号内。
3. 链接的标题（可有可无），可以将其括在双引号、单引号或括号内。<br>
以下示例中，链接的第二部分是等效的：<br>
```markdown
· [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle
· [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"
· [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'
· [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)
· [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
· [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'
· [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles)
```
可以将链接的第二部分放在 Markdown 文档中的任何位置。有些人将它们放在被引用的段落的后面，有些人将它们放在文档的末尾（类似尾注或脚注）。<br>
## 将两部分组合在一起使用的示例
假设你将一个 URL 作为一个 [`标准 URL 链接`](#链接（Links) 添加到段落中，在 Markdown 中如下所示：<br>
```markdown
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
eat: it was a [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"), and that means comfort.
```
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
eat: it was a [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"), and that means comfort.
```markdown
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
eat: it was a [hobbit-hole][1], and that means comfort.

[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
```
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
eat: it was a [hobbit-hole][1], and that means comfort.

[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
## 实践
不同的Markdown应用程序在处理URL中间的空格方面是不一样的。为了兼容起见，请尽量使用\%20（空格的编码形式）来代替空格。<br>
- [X] 请这样做
```markdown
[link](https:\\www.example.com/my%20great%20page)
```
# 图片
要添加图片，首先请添加感叹号（!），然后紧跟着是方括号，方括号中可添加替代文本（alt text,即图片显示失败后显示此文本），最后跟着圆括号，圆括号中添加图片资源的路径或 URL。你可以选择在圆括号中的 URL 之后添加标题（即 title 属性）。
```markdown
![Not Found 404!](‪https://pro2-bar-s3-cdn-cf1.myportfolio.com/f3aecbdb-cf87-40aa-bdb0-5247ff2ccecc/ced5be84-0a20-495b-8e83-ea3f22248b52_rw_1200.jpg?h=32357ff6adcca602768bf11ef5a63717 "SunSet in Rochester")
```
![Not Found 404!](https://pro2-bar-s3-cdn-cf1.myportfolio.com/f3aecbdb-cf87-40aa-bdb0-5247ff2ccecc/ced5be84-0a20-495b-8e83-ea3f22248b52_rw_1200.jpg?h=32357ff6adcca602768bf11ef5a63717 "SunSet in Rochester")

## 带链接的图片
要为图片添加链接，请先为图片的 Markdown 标记添加一个方括号，然后紧跟着一个圆括号，并在圆括号中添加链接地址。
```markdown
[![Not Found 404!](https://pro2-bar-s3-cdn-cf1.myportfolio.com/f3aecbdb-cf87-40aa-bdb0-5247ff2ccecc/ced5be84-0a20-495b-8e83-ea3f22248b52_rw_1200.jpg?h=32357ff6adcca602768bf11ef5a63717 "SunSet in Rochester")](https://tommyhe.myportfolio.com)
```
[![Not Found 404!](https://pro2-bar-s3-cdn-cf1.myportfolio.com/f3aecbdb-cf87-40aa-bdb0-5247ff2ccecc/ced5be84-0a20-495b-8e83-ea3f22248b52_rw_1200.jpg?h=32357ff6adcca602768bf11ef5a63717 "SunSet in Rochester")](https://tommyhe.myportfolio.com)