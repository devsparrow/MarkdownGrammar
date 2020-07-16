# markdown 输入指南



markdown 的设计初衷是为了书写、阅读 简约方便，但适用的场景越多难免会有复杂的情况。

这里做一份总结，基于 macOS 系统，typora 的引擎，其他需要测试。

- [markdown 文本处理](README.md)
- [markdown 图文音视频](markdown图文音视频.md)
- [markdown 图表](markdown图表.md)
- [markdown 数学](markdown数学.md)
- [LATEX Mathematical Symbols.pdf](LATEXMathematicalSymbols.pdf)



***

本篇参考自：

- https://www.zybuluo.com/codeep/note/163962

- [Keaton2020](https://www.jianshu.com/u/5f550fe15c01)： [【集锦】Markdown 语法快速上手](https://www.jianshu.com/c/65c0f5f216cc)

  https://www.jianshu.com/c/65c0f5f216cc

- https://www.zybuluo.com/static/editor/md-help.markdown

- 



本页面直接展示常用操作

***

[TOC]

***

## 一、常见操作及快捷键

快捷键和每个编辑器的设置关系比较大，typora 应用内无法设置快捷键，需要去偏好设置中添加，这里贴上它的官方说明：

<https://support.typora.io/Shortcut-Keys/>。此文中快捷键还涉及到应用的整体操作，如新建关闭文档，这里只截取 markdown 编辑相关快捷键：



### 1、Paragraph 段落

| Function                            | Hotkey (Windows/Linux) | Hotkey (macOS)            |
| :---------------------------------- | :--------------------- | ------------------------- |
| Heading 1 to 6                      | Ctrl + 1/2/3/4/5/6     | Command + 1/2/3/4/5/6     |
| Paragraph                           | Ctrl + 0               | Command + 0               |
| Increase Heading Level 提高标题层级 | Ctrl + =               | Command + =               |
| Decrease Heading Level 降低标题层级 | Ctrl + -               | Command + -               |
| Table                               | Ctrl + T               | Command + Option + T      |
| Code Fences                         | Ctrl + Shift + K       | Command + Option + C      |
| Math Block                          | Ctrl + Shift + M       | Command + Option + B      |
| Quote                               | Ctrl + Shift + Q       | Command + Option + Q      |
| Ordered List                        | Ctrl + Shift + [       | Command + Option + O      |
| Unordered List                      | Ctrl + Shift + ]       | Command + Option + U      |
| Indent                              | Ctrl + [ / Tab         | Command + [ / Tab         |
| Outdent                             | Ctrl + ] / Shift + Tab | Command + ] / Shift + Tab |



***

### 2、Format 格式

| Function         | Hotkey (macOS)      | md 公式                | 效果                 |
| :--------------- | ------------------- | :--------------------- | -------------------- |
| Strong 加粗      | Command + B         | `**我是粗体字**`       | **我是粗体字**       |
| Emphasis         | Command + I         | `*我是斜体字*`         | *我是斜体字*         |
| Underline 下划线 | Command + U         | `<u>UnderLine</u>`     | <u>UnderLine</u>     |
| Code 代码        | Command + Shift + ` | ``我是代码``           | `我是代码`           |
| Strike           | Control + Shift + ` | `~~这是被删除的内容~~` | ~~这是被删除的内容~~ |



### 3、View 视图

| Function                        | Hotkey (Windows/Linux) | Hotkey (macOS)        |
| :------------------------------ | :--------------------- | --------------------- |
| Toggle Sidebar                  | Ctrl + Shift + L       | Command + Shift + L   |
| Outline                         | Ctrl + Shift + 1       | Command + Control + 1 |
| Articles                        | Ctrl + Shift + 2       | Command + Control + 2 |
| File Tree                       | Ctrl + Shift + 3       | Command + Control + 3 |
| Source Code Mode                | Ctrl + /               | Command + /           |
| Focus Mode                      | F8                     | F8                    |
| Typewriter Mode                 | F9                     | F9                    |
| Toggler Fullscreen              | F11                    | Command + Option + F  |
| Actual Size                     | Ctrl + Shift + 0       | *(Not Supported)*     |
| Zoom In                         | Ctrl + Shift + =       | *(Not Supported)*     |
| Zoom Out                        | Ctrl + Shift + -       | *(Not Supported)*     |
| Switch Between Opened Documnets | Ctrl + Tab             | Command + `           |
| Toggle DevTools                 | Ctrl + Shift + I       | -                     |






| 功能         | 效果               | markdown公式         | 快捷键              |
| ------------ | ------------------ | -------------------- | ------------------- |
| 下划线       | <u>UnderLine</u>   | `<u>UnderLine</u>`   | `⌘` + `U`           |
| 粗体         | **我是粗体字**     | `**我是粗体字**`     | `⌘` + `B`           |
| 斜体         |                    |                      | `⌘` + `I`           |
| 删除线       | ~~这是删除的内容~~ | `~~这是删除的内容~~` | `⌘` + `S`           |
| 分隔线       |                    | `***`                | `⌘` + `L`           |
| 编号列表     |                    |                      | `⌘` + `Shift` + `O` |
| 项目符号列表 |                    |                      | `⌘` + `Shift` + `U` |
| 插入待办事项 |                    |                      | `⌘` + `Shift` + `T` |
| 代码块       |                    |                      | `⌘` + `Shift` + `P` |
| 撤销         |                    |                      | `⌘` + `Z`           |
| 在笔记内搜索 |                    |                      | `⌘` + `F`           |
| 短文字       | `第一点`           | ` `第一点` `         | `⌘` + `             |
|              |                    |                      |                     |
|              |                    |                      |                     |
|              |                    |                      |                     |
|              |                    |                      |                     |
|              |                    |                      |                     |

##常见文本操作

### 标题

Markdown 支持两种标题的语法，类 [Atx](https://links.jianshu.com/go?to=http%3A%2F%2Fwww.aaronsw.com%2F2002%2Fatx%2F) 和类 [Setext](https://links.jianshu.com/go?to=http%3A%2F%2Fdocutils.sourceforge.net%2Fmirror%2Fsetext.html) 形式。

**类 Atx 形式是使用 `#` 数量表示标题的阶数**

在行首插入 1 到 6 个 `#` ，对应到标题 1 到 6 阶，例如：



```markdown
# 这是 H1        # typora 快捷键 Ctrl + 1
## 这是 H2       # typora 快捷键 Ctrl + 2
### 这是 H3      # typora 快捷键 Ctrl + 3
#### 这是 H4     # typora 快捷键 Ctrl + 4
##### 这是 H5    # typora 快捷键 Ctrl + 5
###### 这是 H6   # typora 快捷键 Ctrl + 6
```



**类 Setext 形式则是用底线的形式**（不常用，了解即可）

利用 `=` （最高阶标题）和 `-` （第二阶标题），例如：



```markdown
This is an H1
=============

This is an H2
-------------
```

任何数量的 `=` 和 `-` 都可以有效果。

 

------





作者：Keaton2020
链接：https://www.jianshu.com/p/b2401aecc304
来源：简书
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。



***

### 复选框 



格式：

>**- [ ] content** 
>**-空格[空格]空格content** 
>解释：[ ]括号里面的空格可以换成[x]，代表选中对话框




效果：

- [ ] 001

- [x] 002

- 003
  - [ ] 0031



代码：

```md
- [ ] 001

- [x] 002

- 003
  - [ ] 0031

```





***

### 引用

> 引用一段话

`>注释一段话`



***

### 代码



```
​```

​```
```



***

#### 代码高亮

在第一个 ` ```  ` 后指定代码语言，c 也可以替换为 python, objective-c

```c
​```c

​```
```



***

## 参考



1. [Markdown 标题](https://www.jianshu.com/p/b2401aecc304)
2. [Markdown 引用](https://www.jianshu.com/p/d87d7d2dcea9)
3. [Markdown 强调: 倾斜加粗删除下划线](https://www.jianshu.com/p/8fbcde18906d)
4. [Markdown 插入链接](https://www.jianshu.com/p/ab539e9a7955)
5. [Markdown 插入图片](https://www.jianshu.com/p/835d72b837bf)
6. [Markdown 列表](https://www.jianshu.com/p/525001212ec5)
7. Markdown 任务列表（简书不支持，可[参阅](https://links.jianshu.com/go?to=https%3A%2F%2Fclaop.github.io%2Fcourses%2Fmarkdown%2Fmarkdown-%E4%BB%BB%E5%8A%A1%E5%88%97%E8%A1%A8%2F)）
8. [Markdown 代码块与语法高亮](https://www.jianshu.com/p/65ab196bef04)
9. [Markdown 换行与段首缩进](https://www.jianshu.com/p/8d2d4283bf08)
10. [Markdown 插入表格](https://www.jianshu.com/p/c1c6e8bb3a49)
11. [Markdown 生成内容目录](https://www.jianshu.com/p/7986ee08792d)
12. [Markdown 插入分割线](https://www.jianshu.com/p/68431b350139)
13. [Markdown 添加注脚](https://www.jianshu.com/p/6cbdd103461a)
14. Markdown 插入音乐（[参阅](https://links.jianshu.com/go?to=https%3A%2F%2Fclaop.github.io%2Fcourses%2Fmarkdown%2Fmarkdown-%E6%8F%92%E5%85%A5%E9%9F%B3%E4%B9%90%2F)）
15. Markdown 插入视频（[参阅](https://links.jianshu.com/go?to=https%3A%2F%2Fclaop.github.io%2Fcourses%2Fmarkdown%2Fmarkdown-%E6%8F%92%E5%85%A5%E8%A7%86%E9%A2%91%2F)）
16. Markdown 嵌入地图（[参阅](https://links.jianshu.com/go?to=https%3A%2F%2Fclaop.github.io%2Fcourses%2Fmarkdown%2Fmarkdown-%E5%B5%8C%E5%85%A5%E5%9C%B0%E5%9B%BE%2F)）
17. Markdown 设置字体、字号与颜色（[参阅](https://links.jianshu.com/go?to=https%3A%2F%2Fclaop.github.io%2Fcourses%2Fmarkdown%2Fmarkdown-%E8%AE%BE%E7%BD%AE%E5%AD%97%E4%BD%93%E5%AD%97%E5%8F%B7%E4%B8%8E%E9%A2%9C%E8%89%B2%2F)）
18. Markdown 添加背景色（[参阅](https://links.jianshu.com/go?to=https%3A%2F%2Fclaop.github.io%2Fcourses%2Fmarkdown%2Fmarkdown-%E6%B7%BB%E5%8A%A0%E8%83%8C%E6%99%AF%E8%89%B2%2F)）
19. Markdown 插入数学公式（[参阅](https://links.jianshu.com/go?to=https%3A%2F%2Fclaop.github.io%2Fcourses%2Fmarkdown%2Fmarkdown-%E6%8F%92%E5%85%A5%E6%95%B0%E5%AD%A6%E5%85%AC%E5%BC%8F%2F)）
20. Markdown 插入流程图（[参阅](https://links.jianshu.com/go?to=https%3A%2F%2Fclaop.github.io%2Fcourses%2Fmarkdown%2Fmarkdown-%E6%8F%92%E5%85%A5%E6%B5%81%E7%A8%8B%E5%9B%BE%2F)）

光懂语法还不能写出排版优秀的文章，我们还需要学习 **Markdown 编写规范**，让我们的文章看起来很专业。已经有好人写了文章：

- [Markdown 编写规范](https://www.jianshu.com/p/84481d344a3f)
- [技术文档写作规范（Markdown）](https://www.jianshu.com/p/3b638180e42c)

 