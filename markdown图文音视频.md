# markdown 图文音视频

[toc]

***



图片、音乐、视频、链接等

## 一、链接




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



***



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