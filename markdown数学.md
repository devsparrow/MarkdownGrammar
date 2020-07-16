# markdown 数学

[toc]

***



## 零、关于 LaTex 和 Markdown Math

LaTeX（LATEX，音译“拉泰赫”）是一种基于ΤΕΧ的排版系统

主页：https://www.latex-project.org

Markdown Math也就是LaTex语法输出数学公式的基本用法



***

Typora 内置 latex 解释器，github 不带；所以github 上使用 html 中的数学表达式比较合适。



***

用法

行间公式的形式为

```latex
$$ 此处插入公式 $$
```



***

而行内公式的形式为

```latex
\\( 此处插入公式 \\)
```



***

***

##  

## 一、数学符号

数学符号非常多，可参考莱斯大学的 [LATEX Mathematical Symbols](https://www.caam.rice.edu/~heinken/latex/symbols.pdf)

本站也保存了一份：[LATEX Mathematical Symbols](LATEX Mathematical Symbols.pdf)

这里介绍一些常用的：

***

### 希腊字母

|||||||
|-|-|-|-|-|-|
|`$\alpha$`|$\alpha$|`$\beta$`|$\beta$|`$\delta$`|$\delta$|
|``$\Delta$``|$\Delta$|``$$``||`$$`||
|``$\pi$``|$\pi$|``$sigma$``|$sigma$|`$theta$`|$theta$|
|``$$``||``$$``||`$$`||
|``$$``||``$$``||`$$`||

***

### 三角运算符

三角函数、对数、指数的写法以及其他符号的语法和字母是一样的，也是使用`$LaTex符号$`，也就是将LaTex的希腊字母语法用两个美元符号围住即可，我们来看下面的案例：  

| 名称 |数学表达式 |markdown公式| 名称 |数学表达式 |markdown公式|
|-|-|-|-|-|-|
|正弦|$\sin$|`$\sin$`|余弦|$\cos$|`$\cos$`|
|正切|$\tan$|`$\tan$`|余切|$\tan$|`$\tan$`|
||$\arcsin$|`$\arcsin$`||$\arctan$`$\arctan$`|
|垂直|$\bot$	|`$\bot$`| 角|	 	$\angle $| `$\angle $`|





***

### **运算符**

运算符的写法也是如此，不过要注意的是加号、减号、等于号、大于、小于的写法有点不同，是直接用符号即可，这个要注意一下。



| 名称 |数学表达式 |markdown公式| 名称 |数学表达式 |markdown公式|
|-|-|-|-|-|-|
|加|$+$|`$+$`|减|$-$|`$-$`|
|乘|$\times$|`$\times$`|除|$\div$|`$\div$`|
|大于|$>$|`$>$`|小于|$<$|`$<$`|
|大于等于|$\geq$ | `$\geq$`|小于等于|$\leq$|`$\leq$`|
|等于|$=$|`$=$`|不等于|$\neq$|`$\neq$ ` |





***

### **集合符号**

|markdown公式| 数学表达式 | markdown公式 | 数学表达式 | markdown公式 | 数学表达式 | markdown公式 | 数学表达式 |
|-|-|-|-|-|-|-|-|
|| $\cup$  | `$\cup$`   |  | $\cap$   | `$\cap$`          |||
| | $\in$    | `$\in$`     |  | $\notin$    | `$\notin$`     |||
|  | $\ni$  | `$\ni$`         |               |             |             |||
|  | $\subset$ | `$\subset$`  |   | $\subseteq$| `$\subseteq$`  |||
|  | $\supset$ |`$\supset$` |  |$\supseteq$ | `$\supseteq$`|||
| |||               |             |             |||



***

## 对数运算符

| 名称 | 数学表达式 | markdown公式   |
| ---- | ---------- | -------------- |
| 对数 | log        | `$\log$`       |
| 对数 | log218     | `$\log_2{18}$` |
| 对数 | ln         | `$\ln$`        |



***

### 其它

| 名称   | 数学表达式 | markdown公式 | 名称   | 数学表达式 | markdown公式 |
| ------ | ---------- | ------------ | ------ | ---------- | ------------ |
| 正无穷 |  $+\infty$          | `$+\infty$`    |负无穷|$-\infty$|`$-\infty$`|
| 无穷 | $\infty$ | `$\infty$` ||||
|最小|$\min$|`$\min$`|最大|$\max$|`$\max$`|
||$\exp$|`$\exp$`|        |            |              |
|对数| $\log$     | `$\log$`     ||$\ln$|`$\ln$`|

***

## 二、数学公式

### 内联 & 块

内联：`$数学公式$`，可以把数学符号嵌入到文字段落里面

```latex
函数式：$f(x)=\frac{P(x)}{Q(x)}$    ，我们可以看到这段公式在文字段落里面。
```

函数式：$f(x)=\frac{P(x)}{Q(x)}$    ，我们可以看到这段公式在文字段落里面。



***

块：`$$数学公式$$`，凸出并独立显示公式

如果我们需要输出的数学公式比较复杂，或者我们需要，这个时候我们就需要使用到公式的块状输出，块状输出的语法使用4个美元符号，我们来看案例。

```latex
$$f(x)=\frac{P(x)}{Q(x)}$$ 
```

使用块状输出，函数会居中显示，值得一提的是我们在使用块状输出数学公式时，在Markdown里需要换行来写公式。

$$f(x)=\frac{P(x)}{Q(x)}$$ 



***

### 简单的四则运算

我们先来看简单的四则运算怎么用Markdown Math编写，

```latex
$2x - 5y =  8$  
$3x + 9y =  -12$
$7x \times 2y \neq 3z$
```

注意这里的`\times`是乘号，`\neq`是不等于，输出的效果如下：

$2x - 5y =  8$  
$3x + 9y =  -12$
$7x \times 2y \neq 3z$

***

### 上下标

| 名称 | 数学表达式 | markdown公式 |
| ---- | ---------- | ------------ |
| 上标 | ab         | `ab`         |
| 下标 | ab         | `ab`         |

`H2O CO2` H2O CO2 `爆米TM` 爆米TM

注意：使用 `$a^b$` 和 `$a_b$` 时，如果b只要一位，可以实现。如果b有两位，则实现失败。



***

Markdown Math的指数运算符是`^`，这个在Python里位运算符，Python的指数运算符是`**`，这个注意区别即可。

```latex
$x^3+x^9$  
$x^y$  
```

输出的结果为：
$x^3+x^9$  
$x^y$  



***

### 开方 $\sqrt{2}$

 `\sqrt{}`是开平方，注意数值使用大括号{}围住，而开n次方的语法是`\sqrt[n]{}`，n次方的n用中括号[]围住，我们来看下面的案例：

```latex
$\sqrt{3x-1} + \sqrt[5]{2y^5-4}$
```

输出的结果是：
$\sqrt{3x-1}+\sqrt[5]{2y^5-4}$



***

### 三角公式

三角公式通常括号、字母、符号、运算符混杂的比较厉害，所以书写的时候要特别注意，我们来看下面的例子：

```latex
$$\cos (2\theta) = \cos^2 \theta - \sin^2 \theta$$
```

输出的结果如下：

 $$\cos (2\theta) = \cos^2 \theta - \sin^2 \theta$$



***

### 输出分数

输出带有分子分母的分数的语法为`\frac{分子}{分母}`，使用大括号把分子、分母都围住。

```latex
$$\frac{x}{2y} +\frac{x-y}{x+y} $$
```

输出的结果如下：

$$\frac{x}{2y} +\frac{x-y}{x+y} $$



***

### 累加  $$\sum$$

求和公式比较复杂，会涉及到上标和下标，在输出指数`^`时我们可以把它看成是上标，使用`_`来输出下标，我们来看具体案例：

```latex
$$\sum_{n=1}^\infty k$$
```

输出的结果如下：

$$\sum_{n=1}^\infty k$$



***

### 累乘 $\prod$

- \prod_{ }^{ }
- 累加号的上标下标的前后顺序可以互换。

| 名称       | 数学表达式            | markdown公式          |
| ---------- | --------------------- | --------------------- |
| 求和号     | $\prod{3x^n}$         | $\prod{3x^n}$         |
| 带范围求乘 | $\prod_{n=1}^N{3x^n}$ | $\prod_{n=1}^N{3x^n}$ |



***

### 极限的输出

在我们了解了上下标的概念之后，输出极限就会使用到下标，

```latex
$$\lim\limits_{x \to \infty} \exp(-x) = 0$$
```

输出的结果：

![\lim\limits_{x \to \infty} \exp(markdown%20%E6%95%B0%E5%AD%A6.assets/equation-20200716145737179) = 0](https://juejin.im/equation?tex=%5Clim%5Climits_%7Bx%20%5Cto%20%5Cinfty%7D%20%5Cexp(-x)%20%3D%200)



***

### 阶乘的输出

```latex
$$\frac{n!}{k!(n-k)!} = \binom{n}{k}$$
```

输出的结果如下：

 $$\frac{n!}{k!(n-k)!} = \binom{n}{k}$$



***

### 矩阵

使用`\begin{matrix}`和`\end{matrix}`围住即可输出矩阵，矩阵之间用`$`来空格，用`\\`来换行。

```latex
$$
  \begin{matrix}
   1 & 2 & 3 \\
   4 & 5 & 6 \\
   7 & 8 & 9
  \end{matrix} 
$$ 
```



输出的结果是：
$$
\begin{matrix}
   1 & 2 & 3 \\
   4 & 5 & 6 \\
   7 & 8 & 9
  \end{matrix}
$$



***

#### 带分割符号的矩阵

详见"[数组使用参考](https://www.zybuluo.com/codeep/note/163962#五数组与表格使用参考)"。

- 例子：

```latex
$$
\left[    
	\begin{array}{cc|c}      
		1&2&3\\      
		4&5&6    
	\end{array}
\right]
$$
```

$$
\left[ 
	\begin{array}{cc|c}      
		1&2&3\\      
		4&5&6    
	\end{array}
\right]
$$




***

#### 行中矩阵

若想在一行内显示矩阵， 
使用 `\bigl(\begin{smallmatrix} ... \end{smallmatrix}\bigr)`。



例子: 这是一个行中矩阵的示例 $\bigl( \begin{smallmatrix} a & b \\ c & d \end{smallmatrix} \bigr)$ 。显示：这是一个行中矩阵的示例 。



***

## 积分 $\int$

- \int_{ }^{ }

| 名称     | 数学表达式                   | markdown公式                 |
| -------- | ---------------------------- | ---------------------------- |
| 积分     | $\int^5_1{f(x)}{\rm d}x$     | `$\int^5_1{f(x)}{\rm d}x$`   |
| 二重积分 | $\iint^5_1{f(x)}{\rm d}x$    | `$\iint^5_1{f(x)}{\rm d}x$`  |
| 三重积分 | `$\iiint^5_1{f(x)}{\rm d}x$` | `$\iiint^5_1{f(x)}{\rm d}x$` |



***

## 三、复杂数学公式

### **分段函数的编写** 

分段函数是非常复杂的，这时候会用到LaTex的cases语法，用`\begin{cases}`和`\end{cases}`围住即可，中间则用`\\`来分段，具体我们来看下面的例子。

```latex
$$
X(m,n)=
\begin{cases}
x(n),\\
x(n-1)\\
x(n-1)
\end{cases}
$$
```

分段函数输出的结果如下：
$$
X(m,n)=
\begin{cases}
x(n),\\
x(n-1)\\
x(n-1)
\end{cases}
$$

***

 



***

参考

- 李东bbsky：使用Markdown输出LaTex数学公式
 https://juejin.im/post/5c8c5da36fb9a049d236f47c


- magicly：在markdown里如何写数学公式
	https://magicly.me/markdown-math/
	
- 墨氲：markdown math 数学公式语法
	https://blog.csdn.net/dss_dssssd/article/details/82692894