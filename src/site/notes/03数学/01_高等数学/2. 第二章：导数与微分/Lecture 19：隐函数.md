---
{"title":"Lecture 19：隐函数与参数方程","tags":["数学"],"categories":null,"date":"2023-12-21","dg-publish":true,"permalink":"/03数学/01_高等数学/2. 第二章：导数与微分/Lecture 19：隐函数/","dgPassFrontmatter":true}
---

---
	 ---
## 1.1 隐函数的导数
### 1.1.1 隐函数基本概念
**显函数**
y 可以用 x 一个解析式全部表达出来；
**隐函数**
+ 隐函数：$3y+x+1=0$
	+ 显函数化（显化）：$y=-\frac{x+1}3$
	+ 但并不是所有的隐函数都很好显化
+ 难显化的隐函数：$y-x-\varepsilon\sin y=0\quad(0<\varepsilon<1)$
 
**一般形式**
隐函数的一般形式（用二元函数表示）： $F(x,y)=0\Rightarrow y=f(x)$

**隐函数求导方法**
隐函数变成以下形式：
+ $F(x,f(x))\equiv0$ 
+ 两边对 x 进行求导，$y 看成 y（x）$ 复合函数，然后把导数部分提出来得到导数的等式；
推导过程（基于**复合函数求导法则**）：
若 $y = y(x)$ 是由 $F(x,y) = 0$ 确定的隐函数，将 $y$ 视为 $x$ 的函数，对 $F(x,y)$ 关于 $x$ 求全导数（复合函数求导）：
根据全导数公式，$\frac{dF}{dx} = F_x' + F_y' \cdot \frac{dy}{dx}$（其中 $F_x'$ 是 $F$ 对 $x$ 的偏导数，$F_y'$ 是 $F$ 对 $y$ 的偏导数）。

由于 $F(x,y) = 0$ 是恒等式，其对 $x$ 的导数也为 $0$，即 $\frac{dF}{dx} = 0$。因此：

$$
F_x' + F_y' \cdot \frac{dy}{dx} = 0
$$


若 $F_y' \neq 0$，将 $F_y' \cdot \frac{dy}{dx}$ 移到等式右边，再两边同时除以 $F_y'$，即可解出 $\frac{dy}{dx}$：

$$
\frac{dy}{dx} = -\frac{F_x'}{F_y'}
$$


简言之，这个公式是通过**复合函数求导法则**和**全导数概念**推导而来，核心是把隐函数 $y = y(x)$ 代入原方程后，对 $x$ 求导并解出 $y'$。


**易错点**：隐函数求导计算
+ 图示： 
	+ ![Pasted image 20240706152937.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020240706152937.png)

### 1.1.2 例题
**例题**：$\text{求由方程 }y^5+2y-x=0\text{ 确定的隐函数 }y=f(x)\text{ 的导数}$
+ 因为是加号，所以三项分别求导：$5y^4y^{\prime}+2y^{\prime}-1=0$
+ 然后提出导数的部分：$y^\prime=\frac1{5y^4+2}$
**例题**：$\text{设 }y=f(x)\text{ 由 }y=1+xe^y\text{ 所确定,求 }y^{\prime\prime}(0)$
先把 x = 0 带到原方程，求出 0 点时候的 y 的值，得到当时 y 等于 1；
然后对两边求导，得到一阶导数：
+ $y^{\prime}=\mathrm{e}^{y}+\mathrm{x}{e}^{y}{y}$
然后得知一阶导数在 y=1 时，其导数值为 e；
然后的二阶导数、再带入：$y^{\prime\prime}=e^{y}y^{\prime}+e^{y}y^{\prime}+x(e^{y}y^{\prime})^{\prime}$
最后得到结果：$y^{\prime\prime}(0)=e^{2}+e^{2}+0,\quad y^{\prime\prime}(0)=2e^{2}$

**例题**：$\text{设 }y=(1+x^2)^{\sin x}\text{ 求 }y^{\prime}$
+ 第一步：观测到是幂指类型函数，因此两边取 ln：
	+ $\ln y=\sin\ln(1+\mathrm{x}^2)$
+ 然后：$\frac{y^{\prime}}y=\left[\cos x ln(1+x^2)+\frac{2x\sin x}{1+x^2}\right]$
+ 得到结果：$y^{\prime}=(1+x^{2})^{4x}\left[4x\ln(1+x)+\frac{2x\sin x}{1+x^{2}}\right]$

**解题方法**：对数求导法
#对数求导法
+ 当观测到函数类型幂指类型的函数时，两边可以同时取对数；


