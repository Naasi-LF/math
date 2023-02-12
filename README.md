# math
高数的详细复习笔记
## 函数与极限

### 反函数

**定义**:关于`y=x`对称的函数

$y=f(x)$

$f^{-1}(y)=x$,**严格意义**上这个是原函数的反函数,x是函数,y是变量

$f^{-1}(x)=y$,人们习惯把x当作自变量

**本质**: 方法将函数中的`x`和`y`对调

**例**:$y=\sin x\\对调变量\\x=\sin y\\y=arcsinx为反函数(也可以写为x=arcsiny)$

###　无穷大与无穷小 

**无穷大**：趋于无穷

**无穷小**：趋于０

**几个未知**：

| 无穷大+无穷大 |
| ------------- |
| 无穷大-无穷大 |
| 无穷大*无穷小 |
| 无穷小/无穷小 |
| 无穷小/无穷小 |

**拓展**$无穷小*有界函数=无穷小$

### 无穷小的比较

**已知**:$\lim h(x)=0,\lim g(x)=0$

$$\lim \frac{h(x)}{g(x)} = \begin{cases}  
0 & h(x)是g(x)的高阶无穷小 \\
\infty & h(x)是g(x)的低阶无穷小\\C& h(x)是g(x)的同阶无穷小\\1&等价无穷小
\end{cases}$$

$\lim \frac{h(x)}{g(x)^k} =C$        $h(x)是g(x)的k阶无穷小$

### 等价无穷小(重点)

当 $x \rightarrow 0$ 时

|  $\sin x \backsim x$                                |
| ------------------------------------------------------- |
|  $\tan x \backsim x$                                |
|  $\arcsin x \backsim x$                             |
|  $\arctan x \backsim x$                             |
|  $\ln (1+x) \backsim x$                             |
|  $\mathrm{e}^{\mathrm{x}}-1 \backsim \mathrm{x}$    |
|  $1-\cos x \backsim \frac{1}{2} x^2$                |
|  $(1+x)^a-1 \backsim a x$                           |
|  $\mathrm{a}^{\mathrm{x}}-1 \sim x\ln   \mathrm{a}$ |
**几个复杂等价无穷小的证明**：

$1-\cos x=1-\cos^2\frac{x}{2}+\sin^2\frac{x}{2}=2\sin^2\frac{x}{2}=2*\frac{x^2}{4}=\frac{x^2}{2}$

得到$1-\cos x \backsim \frac{1}{2} x^2$

逆向求导：$\mathrm{x}-\sin \mathrm{x} \backsim \frac{1}{6} \mathrm{x}^3$

下图所示：$\mathrm{x}-\sin \mathrm{x}和\arcsin \mathrm{x}-x$等价

得到：$\arcsin \mathrm{x}-x\backsim\frac{1}{6} \mathrm{x}^3$

$tanx-sinx=tanx(1-cosx)=x\frac{1}{2}x^2=\frac{1}{2}x^3$

同理：$\arcsin \mathrm{x}-\arctan \mathrm{x} \sim \frac{1}{2} \mathrm{x}^3$

$\tan^2 x\sim x^2$

$\sec^2 x-1\sim x^2$

逆向求导:$\tan x-x\sim\frac{1}{3} \mathrm{x}^3$

对称性:$\mathrm{x}-\arctan \mathrm{x} \sim \frac{1}{3} \mathrm{x}^3$
<img src="https://raw.githubusercontent.com/Naasi-LF/image/master/2023-02-12-16-15-00.png" style="zoom:33%;" />
<img src="https://raw.githubusercontent.com/Naasi-LF/image/master/2023-02-12-16-19-04.png" style="zoom:33%;" />

### 极限存在准则

* 准则1：**夹逼定理**

* 准则2：单调有界必有**极限**

  两个条件：**单调**，**有界**

**例题**：$\lim_{n\rightarrow0}(\frac{1}{n^2+1}+\frac{1}{n^2+2}+\frac{1}{n^2+3}+\frac{1}{n^2+4}+...+\frac{1}{n^2+n})$

凑出两个**极限**，一个**小**，一个**大**

$\lim(\frac{1}{n^2+1}+\frac{1}{n^2+1}+...+\frac{1}{n^2+1})\leq\lim(\frac{1}{n^2+1}+\frac{1}{n^2+1}+...+\frac{1}{n^2+1})\leq\lim(\frac{1}{n^2+n}+\frac{1}{n^2+n}+...+\frac{1}{n^2+n})$

将左右**极限**求出，如果**相等**，中间也相等

### 两个重要极限

**定义一**
$$
  \lim _{x\rightarrow0}\frac{\sin x}{x}=1\\其中x可以被替换
$$

**定义二** 
$$
\lim _{x\rightarrow0}(1+x)^\frac{1}{x}=e\\\lim _{x\rightarrow\infty}(1+\frac{1}{x})^x=e\\凑出1^{\infty形式}
$$


### 连续性和间断点

**第一类**间断点

**可去间断点**
若 $\lim _{x \rightarrow x_0} f(x)=A \neq f\left(x_0\right)\left(f\left(x_0\right)\right.$ 甚至可以无定义 $)$
又称**可补**间断点
<img src="https://raw.githubusercontent.com/Naasi-LF/image/master/2023-02-12-21-03-34.png" style="zoom:33%;" />
**跳跃间断点**

左右极限**存在**但**不相等**
<img src="https://raw.githubusercontent.com/Naasi-LF/image/master/2023-02-12-21-04-15.png" style="zoom:33%;" />

***

**第二类**间断点
**无穷**间断点
若 $\lim _{x \rightarrow x_0} f(x)=\infty$, 的这类间断点
<img src="https://raw.githubusercontent.com/Naasi-LF/image/master/2023-02-12-21-05-32.png" style="zoom:33%;" />
**振荡**间断点
$例如：y=\sin \frac{1}{x}$
<img src="https://raw.githubusercontent.com/Naasi-LF/image/master/2023-02-12-21-11-11.png" style="zoom:33%;" />
**例题**:函数$y=\frac{x}{sinx}$有间断点$k\pi$,其中$x=0$为**可去**间断点,其他为**无穷**间断点

**连续性**
函数$f(x)=\left\{\begin{array}{ll}
x+1 & x \leq 0 \\
\frac{\sin x}{x} & x>0
\end{array} \quad \text { 在 } x=0\right.$

在 $\mathrm{x}=0$ 处的连续性?
$$
\begin{array}{ll}
f(0)=1 & \\
\lim _{x \rightarrow 0^{-}} f(x)=\lim _{x \rightarrow 0^{-}}(x+1)=1 & \lim _{x \rightarrow 0} f(x)=1 \\
\lim _{x \rightarrow 0^{+}} f(x)=\lim _{x \rightarrow 0^{+}} \frac{\sin x}{x}=1 & \lim _{x \rightarrow 0} f(x)=f(0)=1
\end{array}
$$
因此$f(x)在x=0处连续$

## 导数与微分

### 导数的概念

**实质**:变化率

**几何**:切线

**定义**:
$$
Def1:f'(x_0)=\lim_{{\Delta x}\rightarrow 0}\frac{f(x_0+\Delta x)-f(x_0)}{\Delta x}\\Def2:f'(x_0)=\lim_{{\Delta x}\rightarrow 0}\frac{\Delta y}{\Delta x}\\Def3:f'(x)=f'(x_0)=\lim_{{\Delta x}\rightarrow 0}\frac{f(x)-f(x_0)}{x-x_0}\\Def4:f'(x_0)=\frac{dy}{dx}|_{x=x_0}
$$

### **函数可导与函数连续**

可导**一定**连续,连续**不一定**可导

**例**:$y|x|$**连续**,但在$x=0$处**不可导**
<img src="https://raw.githubusercontent.com/Naasi-LF/image/master/2023-02-12-21-52-25.png" style="zoom:33%;" />
### 高阶函数求导

一阶:$\frac{dy}{dx}$

二阶:$\frac{d\frac{dy}{dx}}{dx}或\frac{d^2y}{dx^2}$

N阶:$\frac{d^ny}{dx^n}$

**方法**:
1. 归纳法

   $\begin{aligned} & y=\sin x \\ & y^{\prime}=\cos x=\sin \left(x+\frac{\pi}{2}\right) \\ & y^{\prime \prime}=-\sin x=\sin \left(x+2 * \frac{\pi}{2}\right) \\ & y^{\prime \prime \prime}=-\cos x=\sin \left(x+3 * \frac{\pi}{2}\right) \\ & y^{(4)}=\sin x=\sin \left(x+4 \cdot \frac{\pi}{2}\right) \\ & \cdots \cdots \\ &  y(n)=\sin \left(x+\frac{n \pi}{2}\right)\end{aligned}$

2. 莱布尼兹公式
   $$
   (u v)^{(n)}=\sum_{k=0}^n C_n^k u^{(n-k)} v^{(k)}
   $$
   **用法**：两个乘积的高阶导数
   **例题**：$\mathrm{y}=e^x \sin x$, 求 $y^{(n)}$
   解1: 
   
   $y^{\prime}=e^x \sin x+e^x \cos x=\sqrt{2} \sin \left(x+\frac{\pi}{4}\right)$
   $\begin{aligned}
   & y^{\prime \prime}=\sqrt{2}\left[e^x \sin \left(x+\frac{\pi}{4}\right)+e^x \cos \left(x+\frac{\pi}{4}\right)=(\sqrt{2})^2 e^x \sin \left(x+\frac{2 \pi}{4}\right)\right. \\
   & \ldots \\
   & y^{(n)}=(\sqrt{2})^n e^x \sin \left(x+\frac{\mathrm{n} \pi}{4}\right)
   \end{aligned}$
   解2:
   
   $y^{(n)}\\=\sum_{k=0}^n C_n^k {e^x}^{(n-k)} sinx^{(k)}\\=\sum_{k=0}^n C_n^k {e^x} \sin \left(x+\frac{n \pi}{2}\right)\\最后归纳得到y^{(n)}=(\sqrt{2})^n e^x \sin \left(x+\frac{\mathrm{n} \pi}{4}\right)$
   
3. 泰勒公式法

### 隐函数和参数方程的求导

**隐函数求导**

定义:将`y`和`x`放在一个式子里,例如$2x+y-9=0$
**例题1**
$e^x y^3-x^2+2 y=1 \text {, 求 } \frac{d y}{d x} 、 \frac{d^2 y}{d x^2}$
依题目知, $\mathrm{x}$ 为自变量, $\mathrm{y}$ 为关于 $\mathrm{x}$ 的函数
$\begin{aligned}
& e^x y^3-x^2+2 y=1 \\
& e^x y^3+e^x 3 y^2 \frac{d y}{d x}-2 x+2 \frac{d y}{d x}=0 \\
& \frac{d y}{d x}=\frac{2 x-e^x y^3}{e^x 3 y^2+2}
\end{aligned}$
**例题2**
$x^2+x y-x z+2 y^2-z^2=0 \text {, 求 } \frac{\partial z}{\partial x} 、 \frac{\partial \mathbf{z}}{\partial y}$
一个约束条件, 三个变量, 可以确定一个二元函数, 根据题目, $x, y$ 为自变量, $z$ 为关于 $x, y$ 的函数
**提示**:对x求导,y看成常数,对y求导,x看成常数
$\begin{aligned}
& 2 x+y-z-x \frac{\partial \mathbf{z}}{\partial x}-2 z \frac{\partial \mathbf{z}}{\partial x}=0 \\
& \frac{\partial \mathbf{z}}{\partial x}=\frac{2 x+y-z}{x+2 z} \\
& x-x \frac{\partial \mathbf{z}}{\partial y}+4 y-2 z \frac{\partial \mathbf{z}}{\partial y}=0 \\
& \frac{\partial \mathbf{z}}{\partial y}=\frac{x+4 y}{x+2 z}
\end{aligned}$

**反函数求导**

**定义**:反函数的导数等于原函数导数的倒数

**例题**:

$y=\arcsin x$换回原函数

$\sin y=x$两边求导

$\cos y*y'=1\\y'=\frac{1}{cosy}$

**对数求导**

**例题**:

$y=x^ {\sin x}求导$

$y=x^ {\sin x}=e^{\ln x^ {\sin x}}=e^{\ln x {\sin x}}$

这样便将求导**简化**

**参数方程求导**
参数方程是指一个函数, 自变量 $x$ 和 $y$不见面了, 找一个参数 $t$, 用关于 $t$ 的表达式来分别表示它们：
$$
\left\{\begin{array}{l}
y=\varphi(t) \\
x=\psi(t),
\end{array}\right.
$$
这个参数方程确定了 $y=y(x)$ 这样一个 函数关系, 这时 $y$ 对 $x$ 求导就等于：
$$
\frac{d y}{d x}=\frac{d y / d t}{d x / d t}=\frac{\varphi^{\prime}(t)}{\psi^{\prime}(t)} .
$$
二阶导数等于：
$$
\frac{d^2 y}{d x^2}=\frac{d\left(\frac{d y}{d x}\right)}{d x}=\frac{d\left(\frac{d y}{d x}\right) / d t}{d x / d t}=\frac{\left[\frac{\varphi^{\prime}(t)}{\psi^{\prime}(t)}\right]^{\prime}}{\psi^{\prime}(t)}
$$

### 微分

**定义**:

$\Delta y=f(x_0+\Delta x)-f(x_0)\\\Delta y=A\Delta x+O(\Delta x)\\dy=A\Delta x$

**性质**:可导**一定**可微,可微**一定**可导

**延申**:

$\lim_{\Delta x\rightarrow 0}\frac{\Delta y}{\Delta x}=f'(x_0)\\\frac{\Delta y}{\Delta x}=f'(x_0)+a,其中a\rightarrow 0\\\frac{dy}{dx}=f'(x_0)$

## 微分中值定理与导数的应用

定理1 (**罗尔**定理)
1) $f(x)$ 在 $[a, b]$ 上连续;
2) $f(x)$ 在 $(a, b)$ 内可导;
3) $f(a)=f(b)$
则 $\exists \xi \in(a, b)$, 使 $f^{\prime}(\xi)=0$
![](https://raw.githubusercontent.com/Naasi-LF/image/master/2023-02-13-00-12-28.png)
定理2 (**拉格朗日中值**定理)
1) $f(x)$ 在 $[a, b]$ 上连续;
2) $f(x)$ 在 $(a, b)$ 内可导; 则 $\exists \xi \in(a, b)$, 使
$$
\frac{f(b)-f(a)}{b-a}=f^{\prime}(\xi) 
$$
![](https://raw.githubusercontent.com/Naasi-LF/image/master/2023-02-13-00-12-40.png)
定理3 (**柯西中值**定理)
1) $f(x), F(x)$ 在 $[a, b]$ 上连续;
2) $f(x), F(x)$ 在 $(a, b)$ 内可导, 且 $F^{\prime}(x) \neq 0$; 则 $\exists \xi \in(a, b)$, 使
$$
\frac{f(b)-f(a)}{F(b)-F(a)}=\frac{f^{\prime}(\xi)}{F^{\prime}(\xi)}
$$
关系:

1. **罗尔**是**拉格朗日**的特殊形式,
2. **柯西**与**拉格朗日**本质相同

**渐近线**:
(1)**水平渐近线**:
$$
\lim _{x \rightarrow \infty} f(x)=a \Rightarrow y=a
$$
(2)**铅直渐近线**:
$$
\lim _{x \rightarrow x_0} f(x)=\infty \Rightarrow x=x_0
$$
举例:
求函数 $y=\frac{1}{x-1}$ 的水平渐近线和铅直渐近线 解:
$$
\lim _{x \rightarrow \infty} \frac{1}{x-1}=0 \Rightarrow y=0
$$
即水平渐近线为 $y=0$
$$
\lim _{x \rightarrow 1} \frac{1}{x-1}=\infty \Rightarrow x=1
$$
**洛必达**:

**条件**:$\frac{0}{0}或者\frac{\infty}{\infty}$
$$
\begin{aligned}
& f(x) \approx f\left(x_0\right)+f^{\prime}\left(x_0\right)\left(x-x_0\right)=f^{\prime}\left(x_0\right)\left(x-x_0\right) \\
& g(x) \approx g\left(x_0\right)+g^{\prime}\left(x_0\right)\left(x-x_0\right)=g^{\prime}\left(x_0\right)\left(x-x_0\right)
\end{aligned}
$$
思想:以直代曲
$$
\frac{f(x)}{g(x)} \approx \frac{f^{\prime}\left(x_0\right)\left(x-x_0\right)}{g^{\prime}\left(x_0\right)\left(x-x_0\right)}=\frac{f^{\prime}\left(x_0\right)}{g^{\prime}\left(x_0\right)}
$$
取极限, 两者相等
$$
\lim _{x \rightarrow x_0} \frac{f(x)}{g(x)}=\lim _{x \rightarrow x_0} \frac{f^{\prime}(x)}{g^{\prime}(x)}=a
$$
曲线的**凹凸性**和**拐点**:

凹凸性的**本质**:二阶导

几何意义:切线的**变化率**

拐点:$f''(x)=0$

性质:$f^2(x)>0,k单调递增,凹\\f^2(x)<0,k单调递减,凸$

# 一.不定积分

## 1.不定积分的简单介绍

>**引入**：
>$$
>{(sin x)'=cos x}，其中sin x是cos x的一个原函数, cos x是sin x的导函数
>$$
>
>**思考**：还有哪些表达式为$cos x$的原函数？
>　　　$sin x,$  $sin x+1,$  $sin x+2......$
>　　　因此，原函数可以表示为$\bf{sin x+C}$
>**注意**：求积分时不要忘记把C丢掉
>　　　$\bf sin x+C$就是$cos x$的**全体原函数**，或者叫**不定积分**
>
>

***
## 2.不定积分的表达式

$$
{\int{f(x)}{d}x}
$$


可以理解为f(x)求导的**逆运算**

>**分析**:积分和微分有什么联系
>$$
> df(x)/dx=f'(x)\\{df(x)=f'(x)*dx}\\{\int{f(x)}dx=f(x)}\\{d\int{f'(x)dx=f'(x)*dx}}
>$$
>由此可见，$\int$和$d$可以抵消，$\int$和$d$是**互逆的**
>*这个也很好理解，微分的本质是求导，而积分的本质是求导的逆运算*

***
## 3.微积分公式的变形

> **简单的微分变形**：$dkx=kdx$
>
> 道理很简单，$d(kx)/dx=(kx)'$

由此得到通式：
$$
{d}f(x)=f'(x){\rm d}x
$$
**积分变形**：$\int{[f(x)+g(x)]}dx$=$\int{f(x)}dx$+$\int{g(x)}dx$
　　　　　$\int{kf(x)}dx$=$k\int{f(x)}dx$
　　　　　(两者都可以举例轻松论证，不做推导)

***
## 4.基本的求积分法

>高中没有涉及到的三角函数  
>$$
>csc x=\frac{1}{sin x}\\
>cot x=\frac{1}{tan x}\\
>sec x=\frac{1}{cos x}
>$$

**原函数导函数表格**(牢记)

|原函数|导数|
|-|-|
|$\frac{x^{u+1}}{u+1}$|$x^u$|
|$\ln\vert x \vert$|$\frac{1}{x}$|
|$arc tan x$|$\frac{1}{1+x^2}$|
|$arc sin x$|$\frac{1}{\sqrt{1-x^2}}$|
|$sin x$|$cos x$|
|$tan x$|$sec^2 x$|
|$cot x$|$-csc^2 x$|
|$sec x$|$tan x*sec x$|
|$e^x$|$e^x$|
|$\frac{1}{2}\ln[\frac{1-cosx}{1+cosx}]$|$csc x$|
|$-\ln|\cos x|$|$tan x$|
| $\ln \left|\sin \left(x\right)\right|$|$\cot x$|
|$=\ln \left|\tan \left(x\right)+\sec \left(x\right)\right|$|$\sec x$|
**分式拆分法**: 

1. 为**假分式**时

> - 可以直接化成真分式
> - 长除法：$\frac{x^4}{x^2+1}$为例
> 将他当成整数的除法运算去处理，可以很快的将他拆分成$x^4/x^2+1=x^2-1......1$
> 也就是$\frac{x^4}{x^2+1}=x^2-1+\frac{1}{x^2+1}$  

2. 为**真分式**时

> - 分母为多分式乘积：
> $\frac{1}{(1+2x)(1+x^2)}=\frac{A}{1+2x}+\frac{Bx+C}{1+x^2}$
> - 看看能不能因式分解：
> 高中没学的公式:
> $x^3+1=(x+1)*(x^2-x+1)$
> $x^3-1=(x-1)*(x^2+x+1)$

**积化和差**：

$$
\cos a*cos b=\frac{1}{2}[cos(a+b)+cos(a-b)]
$$

***
## 5.换元积分法和分布积分法

**本质**：这两种方法的本质都是为了**尽可能化简为基本积分**

### **换元积分法**

#### **第一类换元积分法**

$$
\int f(g(x)){d}g(x)\\
\int f(u){d}u
$$

其中，$\bf u=g(x)$,此时的式子满足基本积分法
**例题**：

>- $ \int 2x e^{x^2} {\rm d}x$
>
>   此时希望将他变成$\bf{\int e^u du}$的形式
>   让$u=x^2$
>   有$du=dx^2=2xdx$
>   写到这里，题目其实已经分析出来了
>   完整过程为：
>   $\int 2x e^{x^2} {\rm d}x
>   =\int e^{x^2}(x^2)'dx=\int e^{x^2}dx^2$
>   令u=x^2
>
>   $\int e^udu=e^u+C$
>   最后再换回x,原式为$e^{x^2}+C$
>

>- $\int\frac{1}{2x+3}dx$
>
>   凑出$\int\frac{1}{u}du$
>   $ u=2x+3$
>   $du=d(2x+3)=2dx$
>   再凑个$2dx$
>   过程为：
>   $\int \frac{1}{2} \frac{1}{2x+3}2dx\\=\frac{1}{2} \int\frac{1}{2x+3}d(2x+3)$
>

>- $\int \frac{1}{\sqrt{x}(1+x)}dx$
>
>   要熟悉上面的表格
>   具体做法：
>   $\int \frac{1}{1+x}\frac{1}{\sqrt{x}}dx$=$2\int \frac{1}{1+\sqrt{x}^2}d \sqrt{x}$=$2 arc tan\sqrt{x}+C$
>

***
#### **第二类换元积分法**
**方法**：用**三角函数**替换变量

$$1-sin^2x=cos^2x$$
$$1+tan^2x=sec^2x$$

**意义**：这种换元方法往往比前者更容易想到

**例题**

>* $\int \frac{dx}{x^2\sqrt{1+x^2}}$
> 
>根据第二个公式，$x=tan t$
> 可以将公式化简为
> $\int \frac{1}{tan^2t*sec t}d tan t$
>
>=$\int\frac{sec^2t}{tan^2t*sec t}dt$
>
> =$\int\frac{cost}{sin^2t}dt$
> 
> =$\int\frac{1}{sin^2t}d sin t$
> 
>  最后结果是：$\frac{-1}{sin t}$
> 
> 再化为x,利用$tan x$,$sin x$的关系得到结果为：$-\frac{\sqrt{1+x^2}}{x}$
> 
> 注意：**需要写t的范围**（保证函数连续可导并且拆开方时不用加绝对值）

***
### **分部积分法**

>**证明**：
>$(uv)'=uv'+u'v$
>$\int (uv)'dx=\int uv'dx+\int u'v dx$
>进一步化简：
>$uv=\int udv+\int v du$
$$
 \int udv=uv-\int v du
$$

**意义**：$\int udv$计算复杂，而$\int v du$计算简单

**口诀**：反对幂三指

**题目**：

>- $\int x sin xdx =-\int x d cos x$
>  根据口诀，**幂函数**在**三角函数**前面。**幂函数**不动，把**三角函数**放后面
>  然后进一步化简：$-x cos x+\int cos x dx$
>  后面求起来就方便多了

>- $\int e^x xdx=\int xde^x=xe^x-\int e^xdx$
>  同样，因为口诀里**幂函数**在**指数函数**前面

>- $\int lnx dx=lnx x-\int x d lnx$
>  **对数函数**在**幂函数**前面

>- ${\int e^x sin xdx}\\=e^x sin x-\int e^x cos xdx\\=e^x sin x-e^x cos x+\int e^xd cos x\\=e^x sin x-e^x cos x-{\int e^x sin xdx}$
>   形成了一个递归，最后通过方程求解
>  第一次拆分时，**指数函数**没有动
>  第二次拆分时，**三角函数**没有动
>  这样便可以形成一个**递归**，从而求解
>  也因此说明，**指数函数**和**三角函数**属于同等地位
>  所以口诀也可以写成：**反对幂指三**

***
# 二.定积分

## 1.定积分的基本概念

### **引入**
>
>   存在一个函数 $y=f(x)$ , 求$(a,b)$所包含的函数的面积 。
>
>   设 $\varepsilon_i \in (x_{i-1},x_i)$,总面积为$A$
>
>   $\Delta x_i=x_i-x_{i-1}$
>
>   则有$\Delta A_i \approx f(\varepsilon_i)\Delta x_i$ 
>
>   所以$A=\sum _{i=1}^{n} \Delta A_i\approx\sum _{i=1}^{n}f(\varepsilon_i)\Delta x_i$
>
>   当$\Delta x_i$无限逼近零时，所得到的值会越来越接近
>
>   **本质**：区间长度(越小越好)$*$函数值在$(a,b)$的无限求和

***

* 此时，我们可以用定积分表示这个函数的面积;

$$
\int_a^b f(x)dx=\lim_{\Delta x_i\rightarrow0}\sum _{i=1}^{n}f(\varepsilon_i)\Delta x_i
$$

* 注意点  

  1. $a$是积分上限。$b$是积分下限

  2. 这里x和一般函数中的$x$不同，并不是变量

  3. **含义**：$f(x)$在$(a,b)$所包含的面积，影响值的是a和b，而不是x

  4. $\int_a^b f(x)dx=\int_a^b f(u)du=\int_a^b f(t)dt$

  5. 可导必连续，连续必可积

***

> * **拓展**
>
>   将上述公式进行改写，可以获得一种求积分的办法：
>   $$
>   \int_a^b f(x)dx=\lim_{\Delta n\rightarrow\infty}\sum _{i=1}^{n}f(a+\frac{b-a}{n}*i)\frac{b-a}{n}
>   $$
>   令$a=0,b=1$
>   $$
>   \int_0^1 f(x)dx=\lim_{\Delta n\rightarrow\infty}\sum _{i=1}^{n}f(\frac{i}{n})\frac{1}{n}
>   $$
>
> ​           求极限时，注意能不能写成$\sum _{i=1}^{n}f(\frac{i}{n})\frac{1}{n}$的形式

***

* **二级结论**
$$
\int_a^b f(x)dx=-\int_b^a f(x)dx
$$

$$
\int_a^a f(x)dx=0
$$

$$
\int_a^b f(x)dx=\int_a^c f(x)dx+\int_c^b f(x)dx(c可以是以外的点)
$$

$$
\int_a^b dx=b-a
$$

***

### **积分不等式**

  已知$m\leq f(x)\leq M$， $f(a)=m,f(b)=M$

  由图可知:
$$
  m(b-a)\leq \int_a^b f(x)dx\leq M(b-a)
$$
  **用途**：估计，比大小


***

### **积分中值定理**（重点）

  $f(x)在(a,b)上连续，则至少存在一点\varepsilon\in(a,b),使得$
$$
  \int_a^bf(x)dx=f(\varepsilon)*(b-a)
$$
  **意义**：将**积分**转换为了**函数**

  > **证明**：用**拉格朗日中值定理**,**上限函数的求导**
  >
  > $\int_a^bf(x)d(x)\\=\int_a^bf(x)d(x)-\int_a^af(x)d(x)\\=\phi(b)-\phi(a)\\=\frac{\phi(b)-\phi(a)}{b-a}(b-a)\\=\phi\prime(\varepsilon)(b-a)\\=f(\varepsilon)(b-a)$
  >
  > 由此可见，**拉格朗日中值定理**和**积分中值定理**是同一个点
***

### **上限函数**

将**常量**换成**变量**，就是上限函数
$$
Def:设 f(x)在[a,b]有定义，\forall x \in[a,b],则上限函数为：\varphi (x)=\int _a^x f(u) du
$$
**本质**： $f(x)$在$(0,x)$的面积的映射,$\varphi(x)$表达一种面积的变化

**注意**：1. 为了避免混淆，`x`换成`u`

​           2.$x \in (a,b),u \in [a,x]$

***

### **上限函数的求导**

$$
\varphi \prime(x)=(\int _a^x f(u) du)\prime=f(x)
$$
>**证明**：用**导函数的定义**,**积分二级结论**，**积分中值定理**,其中$\theta\in(0,1)$
>
>$\varphi\prime(x)\\=\lim_{\Delta x\rightarrow0} \frac{\varphi(x+ \Delta x)-\varphi(x)}{\Delta x}\\=\lim_{\Delta x\rightarrow0}(\int_a^{x+\Delta x}f(u)d(u)-\int_a^{x}f(u)d(u))/\Delta x\\=\lim_{\Delta x\rightarrow0}(\int_x^{x+\Delta x}f(u)d(u))/\Delta x\\=\lim_{\Delta x\rightarrow0}f(x+\theta \Delta x)*(\Delta x)/\Delta x\\=\lim_{\Delta x\rightarrow0}f(x+\theta \Delta x)\\=f(x)$

  **推广公式**
$$
  (\int _a^{\varphi{(x)} }f(u) du)\prime=(f(\varphi{(x)})\prime=f(\varphi{(x)})\varphi\prime{(x)}
$$
***
### **牛顿莱布尼兹公式**(也称作**积分基本公式**)

$$
\int_a^bf(x)dx=F(b)-F(a),其中F\prime(x)=f(x),x\in(a,b)\\也可以记为：\int_a^bf(x)dx=F(x)\mid_a^b
$$
***

## 2.定积分的换元法

**本质**：**换元积分**法+**范围**

***例题***：$\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}} \sqrt{\cos x-\cos ^2 x}dx$

$=\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}} \sqrt{\cos x*(1-\cos ^2 x)}dx\\=\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}} \sqrt{\cos x}*|\sin x|dx\\=\int_{-\frac{\pi}{2}}^{0} \sqrt{\cos x}*(-\sin x)dx+\int_{0}^{\frac{\pi}{2}} \sqrt{\cos x}*\sin xdx$*

**注意:**绝对值的拆分

**二级结论**: 

**偶倍 ** **奇零**
$$
\int _{-1}^1\frac{x^2\cdot \:tanx}{1+x^2}\:dx\\\mathrm{如果\:f\left(x\right)\:是奇函数，并且在区间:}\:\left[-a,\:\:a\right]\:\mathrm{范围内连续，则}\:\int _{-a}^af\left(x\right)dx=0
$$

$\int _{-1}^1\sqrt{1-x^2}\:dx\\=2\int _{0}^{\frac{\pi }{2}}\cos ^2\left(u\right)du\\=2\int _{0}^{\frac{\pi }{2}}\frac{1+\cos \left(2u\right)}{2}du\\=\int _{0}^{\frac{\pi }{2}}1+\cos \left(2u\right)du\\=\int _{0}^{\frac{\pi }{2}}1du+\int _{0}^{\frac{\pi }{2}}\cos \left(2u\right)du\\=\frac{\pi }{2}+\frac{1}{2}\int _{0}^{\frac{\pi }{2}}\cos \left(2u\right)d2u\\=\frac{\pi }{2}+\frac{1}{2}\sin 2u|_0^\frac{\pi }{2}\\=\frac{\pi }{2}$

$$
\mathrm{如果\:f\left(x\right)\:是偶函数，并且在区间:}\:\left[-a,\:\:a\right]\:\mathrm{范围内连续，则}\:\int _{-a}^af\left(x\right)dx=2\int _{0}^af\left(x\right)dx
$$

$含有f(\sin x)的式子$
$$
Def:\int_0^{\pi}xf(\sin x)dx=\frac{\pi}{2}\int_0^{\pi}f(\sin x)dx
$$


## 3.定积分的分部法

**本质**:**分部积分**法+**范围**

**定义**
$$
\int_a^budv=(uv)|_a^b-\int_a^bvdu
$$
**二级结论**:**点火**公式
$$
\int_0^{\frac{\pi}{2}}\sin ^n xdx=\int_0^{\frac{\pi}{2}}\cos ^n xdx\\=\begin{cases}
\frac{(n-1)!!}{n!!} *\frac{\pi}{2} &{n为偶数}\\
\frac{(n-1)!!}{n!!}&n为奇数
\end{cases}
$$



## 4.反常积分

**本质**:非同寻常,需要求**极限**

**定义**:
$$
\int_a^{+\infty}f(x)dx=F(x)|_a^{+\infty}=\lim_{x\rightarrow\infty}F(x)-F(a)
$$
***例题***

* $
  \int_0^{+\infty} e-xdx\\=-e^{-x}|_0^{+\infty}\\=(0-1)\\=1
  $
  
* $
  \int ^{+\infty }_1\frac{1}{x^p}dx
  $

  $=\frac{x^1-p}{1-p}|_1^{+\infty}\\=F(+\infty)-F(1)\\=\lim _{x\to +\infty }\frac{x^{1-p}}{1-p}-\frac{1}{1-p}\\令1-p=t\\=\lim _{x\to +\infty }(\frac{x^t}{t})-\frac{1}{t}$

  | t>0  | 无穷 |
  | ---- | ---- |
  | t<o  | 0    |
  | t=0  | 无穷 |

  **综上所述**：$t\ge 0时\int ^{+\infty }_1\frac{1}{x^p}dx发散，及p\le 1时发散$

## 5.定积分的几何意义

### 1.面积法(画图)

<img src="https://raw.githubusercontent.com/Naasi-LF/image/master/2023-02-08-22-03-25.png" style="zoom:50%;" />


$$
\int _{-1}^1\sqrt{1-x^2}\:dx为以上y=\sqrt{1-x^2},x=1,x=-1所围成的面积
$$
### 2.极坐标

<img src="https://raw.githubusercontent.com/Naasi-LF/image/master/2023-02-08-22-05-14.png" style="zoom:50%;" />
**介绍**:点O叫**极点**，射线Ox叫做**极轴**，对于平面内任何一点M，用**ρ**表示线段**OM的长度**，**θ**表示从Ox到OM的**角度**，那么，**点M**就可以用有序数对 **(ρ,θ)**来表示，该有序数对就叫点M的**极坐标**，其中，ρ叫做点M的**极径**，θ叫做点M的**极角**。

**例**:$\rho =2\alpha \cos \left(\theta \right),坐标(\rho,\theta)$

如下图所示:
<img src="https://raw.githubusercontent.com/Naasi-LF/image/master/2023-02-08-22-07-37.png" style="zoom:33%;" />

$其中,OA=2a,\angle POA=\theta,OP=p$

**本质:**极坐标其实就是以极角$\theta$为参数的曲线弧的参数方程

### 3.旋转体的体积

$Def$:设连续曲线 $y=f(x)$ 、直线 $x=a, x=b$ 及 $x$ 轴所围成的曲边梯形绕 $x$ 轴旋转一周所围成的旋转体的体积，体积微元是 $d V=$ $\pi[f(x)]^2 d x$ ，体积是 $V=\int_a^b \pi[f(x)]^2 d x$
例6: 连接坐标原点 $O$ 及点 $P(h, r)$ 的直线、直线 $x=h$ 及 $x$ 轴围成一个直角三角形，将它绕 $x$ 轴旋转一周构成一个底面半径为 $r$ 、高为 $h$ 的 圆锥体，计算该圆锥体的体积
$$
\begin{aligned}
& d V=\pi y^2(x) d x=\pi\left(\frac{r}{h} x\right)^2 d x \\
& V=\pi\left(\frac{r}{h}\right)^2 \int_0^h x^2 d x=\frac{\pi r^2 h}{3}
\end{aligned}
$$

### 4.弧长

<img src="https://raw.githubusercontent.com/Naasi-LF/image/master/2023-02-08-22-17-28.png" style="zoom:50%;" />
如图,弧长可以分成**无数个小线段**,最后**累加**

设平面曲线 $C=\tilde{A B}$. 如图 $10-14$ 所示, 在 $C$ 上从 $A$ 到 $B$ 依次取分点:
$$
A=P_0, P_1, P_2, \cdots, P_{n-1}, P_n=B,
$$
它们成为对曲线 $C$ 的一个分割, 记为 $T$. 然后用线 段联结 $T$ 中每相邻两点,得到 $C$ 的 $n$ 条弦 $\overline{P_{i-1} P_i}$ $(i=1,2, \cdots, n)$, 这 $n$ 条弦又成为 $C$ 的一条内接折线
$$
\|T\|=\max _{1 \leqslant i \leqslant n}\left|P_{i-1} P_i\right|, s_T=\sum_{i=1}^n\left|P_{i-1} P_i\right|,
$$
分别表示最长弦的长度和折线的总长度

**公式**:$\int _a^b\sqrt{d^2x+d^2y}$,先**微**后**积**

$Def 1$
设曲线 $C$ 由参数方程 (1) 给出. 若 $C$ 为一光滑曲线 $\Phi$, 则 $C$ 是 可求长的, 且弧长为
$$
s=\int_\alpha^\beta \sqrt{x^{\prime 2}(t)+y^{\prime 2}(t)} \mathrm{d} t .
$$
***
$Def2$
若曲线 $C$ 由直角坐标方程
$$
y=f(x), x \in[a, b]
$$
表示, 把它看作参数方程时, 即为
$$
x=x, y=f(x), x \in[a, b] .
$$
所以当 $f(x)$ 在 $[a, b]$ 上连续可微时, 此曲线即为一光滑曲线. 这时弧长公式为
$$
s=\int_a^b \sqrt{1+f^{\prime 2}(x)} \mathrm{d} x .
$$
***
$Def3$
又若曲线 $C$ 由极坐标方程
$$
r=r(\theta), \theta \in[\alpha, \beta]
$$
表示, 把它化为参数方程, 则为
$$
\begin{gathered}
x=r(\theta) \cos \theta, y=r(\theta) \sin \theta, \theta \in[\alpha, \beta] . \\
x^{\prime}(\theta)=r^{\prime}(\theta) \cos \theta-r(\theta) \sin \theta, \\
y^{\prime}(\theta)=r^{\prime}(\theta) \sin \theta+r(\theta) \cos \theta, \\
x^{\prime 2}(\theta)+y^{\prime 2}(\theta)=r^2(\theta)+r^{\prime 2}(\theta),
\end{gathered}
$$
因此当 $r^{\prime}(\theta)$ 在 $[\alpha, \beta]$ 上连续, 且 $r(\theta)$ 与 $r^{\prime}(\theta)$ 不同时为零时, 此极坐标曲线为 一光滑曲线. 这时弧长公式为
$$
s=\int_a^\beta \sqrt{r^2(\theta)+r^{\prime 2}(\theta)} \mathrm{d} \theta .
$$

# 三.总结

## 1.图解

 ```mermaid
graph LR
a(求解积分)-->b(分式)
a-->c(一般式)
b-->d(假分式)-->e(真分式)
b-->e
e-->g(分母因式分解)-->f(多个真分式)

e-->h(分子单独拿出)-->f
b-->i(分母为a^2+1,1-a^2,a^2-1)-->j(第二类换元法)
b-->k(有复合函数)
c-->k-->l(第一类换元法)
c-->m(函数*函数的形式)-->n(分部积分法)
 ```
## 2.错题
$$
\text { (1) 设 } \varphi(x)=\mathrm{e}^x-\int_0^x(x-u) \cdot \varphi(u) \mathrm{d} u \text {, 其中 } \varphi(x) \text { 是连续可微函数, 求 } \varphi^{\prime \prime}(x) \text {. }
$$

**分析**：$\int_0^x(x-u) \cdot \varphi(u) \mathrm{d} u 为积分上限函数\\是对函数(x-u) \cdot \varphi(u) 在(0,x)的面积的映射\\因此可以做以下化简:\\=\int_0^xx \cdot \varphi(u) \mathrm{d} u-\int_0^xu \cdot \varphi(u) \mathrm{d} u\\=x\int_0^x \cdot \varphi(u) \mathrm{d} u-\int_0^xu \cdot \varphi(u) \mathrm{d} u$
$$
(2)\lim _{x \rightarrow 0} \frac{\int_{\cos x}^1 \mathrm{e}^{-t^2} d t}{\sin ^2 x}
$$
**分析**:
$
=\lim \:_{x\:\rightarrow \:0}\:\frac{-\int _1^{cos\:x}\:\:\mathrm{e}^{-t^2}\:d\:t}{\sin \:^2\:x}\\=\frac{\frac{1}{e^{cos^2x}}\sin x}{2sin\:x\cos\:x}\:\\=\frac{\frac{1}{e^{cos^2x}}}{2cos\:x}\:\\=\frac{1}{2e^{cos^2x}\cos x}\\=\frac{1}{2e}
$
$$
(3) 求由对数螺线 \rho=a \mathrm{e}^{\theta}(-\pi \leqslant \theta \leqslant \pi)及射线 \theta=-\pi, \theta=\pi 所围成的图形的面积.
$$

<img src="https://raw.githubusercontent.com/Naasi-LF/image/master/2023-02-08-23-16-29.png" style="zoom: 50%;" />

**分析**：$\frac{1}{2}\int _{-\pi}^{\pi}\rho^2d\theta代入$

**方法**：看成一个个**小扇形**的**累加**

(4). 设由挞物线 $y^2=2 p x(p>0)$ 与直线 $x+y=\frac{3}{2} p$ 所围成的平面图形为 $D$. 

求: (1) $D$ 的面积 $S$; (2) 将 $D$ 绕 $y$ 轴旋转一周所得的旋转体的体积 $V$.

(1) $S=\int_{-3 p}^p\left(\frac{3}{2} p-y-\frac{y^2}{2 p}\right) \mathrm{d} y=\frac{16}{3} p^2$
或 $S=\int_0^{\frac{p}{2}}(\sqrt{2 p x}+\sqrt{2 p x}) \mathrm{d} x+\int_{\frac{p}{2}}^{\frac{p}{2}}\left(\frac{3}{2} p-x+\sqrt{2 p x}\right) \mathrm{d} x=\frac{16}{3} p^2$
(2) $V=\int_{-3 p}^p \pi\left(\frac{3}{2} p-y\right)^2 \mathrm{~d} y-\int_{-3 p}^p \pi\left(\frac{y^2}{2 p}\right)^2 \mathrm{~d} y=\frac{272}{15} \pi p^3$.

***

(5). 计算曲线 $y=\frac{\sqrt{x}}{3}(3-x)$ 上对应于 $1 \leqslant x \leqslant 3$ 的一段弧的长度.
$\frac{4}{3} \sqrt{3}$.









