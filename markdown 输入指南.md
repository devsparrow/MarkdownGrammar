# markdown 输入指南

[TOC]

***

markdown 的设计初衷是为了书写、阅读 简约方便，但适用的场景越多难免会有复杂的情况。

这里做一份总结，基于 macOS 系统，typora 的引擎，其他需要测试。



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

| Function             | Hotkey (macOS)        |md 公式| 效果|
| :-------------------  | --------------------- | :--------------------- | --------------------- |
| Strong 加粗            |Command + B     | `**我是粗体字**`|**我是粗体字**|
| Emphasis                        | Command + I           |`*我是斜体字*`|*我是斜体字*|
| Underline 下划线             | Command + U       | `<u>UnderLine</u>`    |<u>UnderLine</u> |
| Code 代码            | Command + Shift + `   |``我是代码``|`我是代码`|
| Strike                   | Control + Shift + `   |`~~这是被删除的内容~~`|~~这是被删除的内容~~|


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






|功能|效果|markdown公式|快捷键|
|-|-|-|-|
|下划线|<u>UnderLine</u>| `<u>UnderLine</u>` |`⌘` + `U`|
|粗体|**我是粗体字**|`**我是粗体字**`|`⌘` + `B` |
|斜体|||`⌘` + `I`|
| 删除线   |~~这是删除的内容~~| `~~这是删除的内容~~` | `⌘` + `S`      |
| 分隔线   || `***` | `⌘` + `L` |
| 编号列表  ||         | `⌘` + `Shift` + `O` |
| 项目符号列表 ||      | `⌘` + `Shift` + `U` |
| 插入待办事项 ||      | `⌘` + `Shift` + `T` |
| 代码块   ||          | `⌘` + `Shift` + `P` |
| 撤销    ||           | `⌘` + `Z`      |
| 在笔记内搜索  ||     | `⌘` + `F`      |
| 短文字 |`第一点`| ` `第一点` ` | `⌘` + `       |
|   ||     | `⌘` + `       |
|   ||     | `⌘` + `       |
|   ||     | `⌘` + `       |
|   ||     | `⌘` + `       |
|   ||     | `⌘` + `       |





##二、常见文本操作





***

### 2、复选框 



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

## 二、图片、音乐、视频、链接等

### 1、链接




Markdown 支持两种形式的链接语法： **行内链接**和 **参考链接**。

### 行内形式：

链接文字都是用 [方括号] 来标记，使用 (圆括号) 来把文字转成链接。还可以为链接文字配个Title，当然 Title 属性是可选项，加不加看心情咯。

```
[链接文字](链接网址 "标题")
This is an [example link](http://example.com/ "With a Title"). 
```

This is an [example link](https://links.jianshu.com/go?to=http%3A%2F%2Fexample.com%2F).



***

#### 参考形式：

为参考形式的链接定一个 `[名称]`方便我们在文章中多次引用（链接名称可以用字母、数字和空格，但是不分大小写）。

```
[链接文字][name]

[name]: link "Title"
当我知道 [搜狗][2] 可以搜索微信和知乎时，我毫不犹豫地选择使用 [搜狗][2]。学术搜索还是用 [Google][1] 靠谱，因为安全是第一位的，被墙我只能说「自作孽不可活」。偶尔也会用一下 [Bing][4] 和 [某度][3]。
在这里“祝贺” [某度搜索][3] 的竞价排名遗臭万年，但是就像现实生活中一样，请保护自己，别傻了吧唧被人骗。因为骗子固然最可恨，被骗难道不正说明了自己的脆弱无知？

[1]: https://www.google.com/ "Google"
[2]: https://www.sogou.com/ "Sogou"
[3]: https://www.baidu.com/ "Baidu Search"
[4]: https://cn.bing.com/ "Bing Search"
```



当我知道 [搜狗](https://links.jianshu.com/go?to=https%3A%2F%2Fwww.sogou.com%2F)可以搜索微信和知乎时，我毫不犹豫地选择使用 [搜狗](https://links.jianshu.com/go?to=https%3A%2F%2Fwww.sogou.com%2F)。学术搜索还是用 [Google](https://links.jianshu.com/go?to=https%3A%2F%2Fwww.google.com%2F)靠谱，因为安全是第一位的，被墙我只能说「自作孽不可活」。偶尔也会用一下 [Bing](https://links.jianshu.com/go?to=https%3A%2F%2Fcn.bing.com%2F)和 [某度](https://links.jianshu.com/go?to=https%3A%2F%2Fwww.baidu.com%2F)。
在这里“祝贺” [某度搜索](https://links.jianshu.com/go?to=https%3A%2F%2Fwww.baidu.com%2F)的竞价排名遗臭万年，但是就像现实生活中一样，请保护自己，别傻了吧唧被人骗。因为骗子固然最可恨，被骗难道不正说明了自己的脆弱无知？

```
早饭后，我打开 [每日英语听力][TING] 学习英语。遇到不懂的英语单词，我借助 [欧路在线词典][zxB] 
查看释义并加入生词本，方便使用 [客户端][khd] 随时记忆单词。

[ting]: https://dict.eudic.net/ting "每日英语听力 - 欧路词典"
[zxb]: https://dict.eudic.net/ "《欧路词典》在线版"
[khd]: https://www.eudic.net/v4/en/app/eudic "《欧路词典》英语翻译软件官方主页"
```

早饭后，我打开 [每日英语听力](https://links.jianshu.com/go?to=https%3A%2F%2Fdict.eudic.net%2Fting)学习英语。遇到不懂的英语单词，我借助 [欧路在线词典](https://links.jianshu.com/go?to=https%3A%2F%2Fdict.eudic.net%2F)查看释义并加入生词本，方便使用 [客户端](https://links.jianshu.com/go?to=https%3A%2F%2Fwww.eudic.net%2Fv4%2Fen%2Fapp%2Feudic)随时记忆单词。



***

#### 自动链接：

Markdown 支持以比较简短的自动链接形式来处理网址和电子邮件信箱，只要是用 < > 包起来，Markdown 就会自动把它转成链接。一般网址的链接文字就和链接地址一样，邮址的自动链接也很类似，例如：

```
<http://example.com/>
<address@example.com>
```

[http://example.com/](https://links.jianshu.com/go?to=http%3A%2F%2Fexample.com%2F)
[address@example.com](https://links.jianshu.com/go?to=mailto%3Aaddress%40example.com)



#### 添加锚点,跳到本页 指定位置 



在预览状态下跳转，跳转时按住ctrl/cmd点击

<a href="#表格">点击跳转</a>



***

`<a href="#表格">点击跳转</a>`

比如 ## header1 的header1，放到`<a href="">`的引号里面 : `<a href="#header1">header1</a>`，



***

#### 跳转到其他文件





***

### 2、图片

#### 关于markdown图片相对路径

这几天在使用markdown的时候遇到的问题，没有看到对应的解决方案。在此记录总结一下
相对路径通常在表示图片、网页等位置时需要用到，相比于绝对路径更不容易出错。 
如果图片与.md文件在同一目录下，那么相对路径这样表示

`![avatar](buildWebsites.jpg) `
其中avatar表示图片未正常加载时所显示的内容，buildWebsites.jpg为文件名

其子路径这样表示 
`![avatar](1/buildWebsites.jpg) `
其中1为文件夹名称

其父路径用“..”表示，例如 
`![avatar](../buildWebsites.jpg)`





***

#### 使用 base64 插入图片

图片转base64 http://imgbase64.duoshitong.com

在文档中插入编码：

![image][data:image/png;base64, ......]

***

当然 base64 编码一般很长，直接将编码放入段落内部会影响正常编辑。通常的做法是将base64编码定义到一个中间变量中，将编码本体放到文档末：

![image][tmp]
your document here ...

[tmp]:data:image/png;base64, ......



***

### 3、音频


方法一，进入**网易云音乐**歌曲界面，点击光碟下方的生成外链播放器：

```
<iframe
    frameborder="no"
    border="0"
    marginwidth="0"
    marginheight="0"
    width=330
    height=86
    src="//music.163.com/outchain/player?type=2&id=393697&auto=1&height=66">
</iframe>
```

***

方法二，到 http://www.333ttt.com/up/ 获得外链，**嵌入音乐：**

```
<audio id="audio" controls="" preload="none">
<source id="mp3" src="http://sc1.111ttt.cn:8282/2018/1/03m/13/396131229550.m4a?tflag=1546606800&pin=97bb2268ae26c20fe093fd5b0f04be80#.mp3">
</audio>
```





<audio id="audio" controls="" preload="none">
<source id="mp3" src="http://music.163.com/song?id=40257852&userid=18946869">
</audio>






***

### 4、视频



***



```
1. 插入视频
<video src="http://structr.learn-anything.cn/video/道理/陈铭：像我这种老好人，根本没什么真朋友！不jue亲戚的人，根本没什么真亲戚！.mp4" width="320" height="180"
controls="controls"></video> 

2. 插入图片
![图片](http://structr.learn-anything.cn/[Neo4jArticle]with%E7%94%A8%E6%B3%95.png)
```





***

## 四、图表

### 1、表格

>语法格式如下：
>```
>|  表头   | 表头  |
>|  ----  | ----  |
>| 单元格  | 单元格 |
>| 单元格  | 单元格 |
>
>```
>使用 | 来分隔不同的单元格，使用 - 来分隔表头和其他行。
>
>
>
>**表格的对齐方式：**
>
>- `-:` 设置内容和标题栏居右对齐。
>- `:-` 设置内容和标题栏居左对齐。
>- `:-:` 设置内容和标题栏居中对齐。




显示效果：

| 表头   | 表头   |
| ------ | ------ |
| 单元格 | 单元格 |
| 单元格 | 单元格 |



### 2、组织结构图 mermaid

>语法结构

>>```
>	​```mermaid
>	graph 方向
>	节点以及节点连线（定义和连线步骤可以分开）
>	（样式调整）
>\```  
>	```
>```
>
>
>```




https://www.jianshu.com/p/789f02d745ec?open_source=weibo_search

http://blog.yahui.wang/2019/04/09/talkabout-markdown-mermaid/

https://blog.csdn.net/suoxd123/article/details/84992282

***



***

#### 节点类型

   节点本身的展现形式，是通过不同括号来代表各自不同的形状，默认为矩形。

- 默认节点： A
- 矩形节点： B[矩形]
- 圆角矩形节点： C(圆角矩形)
- 圆形节点： D((圆形))
- 非对称节点： E>非对称]
- 菱形节点： F{菱形}



***

#### 显示方向

- TB/TD（ top bottom/top down）表示从上到下
- BT（bottom top）表示从下到上
- RL（right left）表示从右到左
- LR（left right）表示从左到右



***

节点连线

   线条本身的形式有多种，通过常规的英文格式的格式来标识，具体如下：

箭头连接 `A1-->B1`
开放连接 `A2---B2`
虚线箭头连接 `A3.->B3` 或者 `A3-.->B3`
虚线连接`A4.-B4` 或者 `A4-.-B4`
粗线箭头连接 `A5==>B5`
粗线开放连接 `A6===B6`
标签虚线箭头连接 `A7-.text.->B7`
标签开放连接 `A8--text---B8`



***

```mermaid
graph TB
A1-->B1
A2---B2
A3.->B3
A31-.->B31
A4.-B4
A41-.-B41
A5==>B5
A6===B6
A7-.text.->B7
A8--text---B8
```



***



***
```
​```mermaid
	graph TB
	A[Apple]-->B{Boy}
	A---C(Cat)
	B.->D((Dog))
	C==喵==>D
	style A fill:#2ff,fill-opacity:0.1,stroke:#faa,stroke-width:4px
	style D stroke:#000,stroke-width:8px;
```


```


​```mermaid
	graph TB
	A[Apple]-->B{Boy}
	A---C(Cat)
	B.->D((Dog))
	C==喵==>D
	style A fill:#2ff,fill-opacity:0.1,stroke:#faa,stroke-width:4px
	style D stroke:#000,stroke-width:8px;
```







***

~~~go
```mermaid
graph TD
A[总经理] -->|A1| B(XX副总)
B --> C[XX部]
B --> D[XX部]
B --> E[XX部]
C--> G[模块4]
C--> H[模块5]
C--> J[模块6]
D--> K[模块K]
E--> L[模块1]
E--> Z[模块2]
E--> X[模块3]
~~~




```mermaid
graph TD
A[总经理] -->|A1| B(XX副总)
B --> C[XX部]
B --> D[XX部]
B --> E[XX部]
C--> G[模块4]
C--> H[模块5]
C--> J[模块6]
D--> K[模块K]
E--> L[模块1]
E--> Z[模块2]
E--> X[模块3]
```



***





***

#  



写法



***

## 1、上下标

- 上标 ^
- 下标 _

| 名称 | 数学表达式 | markdown公式 |
| ---- | ---------- | ------------ |
|  上标| a<sup>b</sup>         | `a<sup>b</sup>`        |
| 下标 | a<sub>b</sub>         | `a<sub>b</sub>`      |

`H<sub>2</sub>O  CO<sub>2</sub>`  H<sub>2</sub>O  CO<sub>2</sub>
`爆米<sup>TM</sup>`  爆米<sup>TM</sup>



注意：使用 `$a^b$` 和 `$a_b$` 时，如果b只要一位，可以实现。如果b有两位，则实现失败。 

***
## 2、分数

- \frac{ }{ }
- 第一个{ }写分子，第二个{ }写分母。

| 名称 | 数学表达式 | markdown公式        |
| ---- | ---------- | ------------------- |
| 分数 | 3+8a5b+6   | `$\frac{3+8a}{5b+6}$` |

***
## 3、累加

- \sum_{ }^{ }
- 累加号的上标下标的前后顺序可以互换。



| 名称 | 数学表达式 | markdown公式        |
| ---- | ---------- | ------------------- |
|求和号|	∑3xn| `$\sum{3x^n}$`|
|带范围求和	|∑Nn=13xn | `$\sum_{n=1}^N{3x^n}`|



***
## 4、累乘

- \prod_{ }^{ }
- 累加号的上标下标的前后顺序可以互换。

| 名称 | 数学表达式 | markdown公式        |
| ---- | ---------- | ------------------- |
|求和号|	∏3xn | $\prod{3x^n}$|
|带范围求乘|	∏Nn=13xn|$\prod_{n=1}^N{3x^n}$|



***
## 5、开方

- \sqrt[ ]{ }
- [ ]中写的是开几次方，{ }中写的是需要开方的数值。


| 名称 | 数学表达式 | markdown公式 |
| ---- | ---------- | ------------ |
| 开方号	| 100−−−√5 | `$\sqrt[5]{100}$`|



***
## 6、积分

- \int_{ }^{ }

| 名称 | 数学表达式 | markdown公式 |
| ---- | ---------- | ------------ |
| 积分| 	∫51f(x)dx| `$\int^5_1{f(x)}{\rm d}x$`|
| 二重积分| 	∬51f(x)dx| `$\iint^5_1{f(x)}{\rm d}x$`|
| 三重积分| 	∭51f(x)dx| `$\iiint^5_1{f(x)}{\rm d}x$`|



***
## 7、正无穷、负无穷

- \infty

| 名称 | 数学表达式 | markdown公式 |
| ---- | ---------- | ------------ |
| 正无穷| 	+∞| $+\infty$|
| 负无穷| 	−∞| $-\infty$|



***
## 8、极限


| 名称 | 数学表达式 | markdown公式 |
| ---- | ---------- | ------------ |
| 左箭头	| limn→+∞n| `$\lim_{n\rightarrow+\infty} n$`|

***

***
## 9、关系运算符


| 名称 | 数学表达式 | markdown公式 |
| ---- | ---------- | ------------ |
|大于等于	|≥|`$\geq$`|
|小于等于|	≤|`$\leq$`|
|包含于	|⊂|`$\subset$`|
|包含|	⊃|`$\supset$`|
|属于	|∈|`$\in$`|



***
## 10、二元运算符


| 名称 | 数学表达式 | markdown公式 |
| ---- | ---------- | ------------ |
|加减|	±| `$\pm$`|
|点乘	|⋅|`$\cdot$`|
|乘	|×|`$\times$`|
|除|	÷|`$\div$`|





***
## 11、否定关系运算符


| 名称 | 数学表达式 | markdown公式 |
| ---- | ---------- | ------------ |
|不等于|	≠|`$\not=$`|
|不小于	|≮|`$\not<$`|
|不包含|	⊅ |`$\not\supset$`|

***
## 12、对数运算符


| 名称 | 数学表达式 | markdown公式 |
| ---- | ---------- | ------------ |
|对数|	log | `$\log$` |
|对数|	log218|`$\log_2{18}$`|
|对数|	ln | `$\ln$`|



***
## 13、三角运算符


| 名称 | 数学表达式 | markdown公式 |
| ---- | ---------- | ------------ |
|垂直	|⊥ |`$\bot$`|
|角|	∠|`$\angle $`|
|30度角|	30∘|`$30^\circ$`|
|正弦|	sin|`$\sin$`|
|余弦 | cos| `$\cos$`|
|正切|	tan| `$\tan$`|



***

## 14、箭头

| 名称 | 数学表达式 | markdown公式 |
| ---- | ---------- | ------------ |
| 左箭头| 	←| `$\leftarrow$`|
| 右箭头	→| `$\rightarrow$`|
| 长箭头| 	⟶|  `$\longrightarrow$`|
| 上箭头| 	↑|  `$\uparrow$`|
| 下箭头| 	↓| `$\downarrow$`|





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

[少数派](https://links.jianshu.com/go?to=https%3A%2F%2Fsspai.com%2F)的文章排版比较规范，大家可以多逛逛。

```

```