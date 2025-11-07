---
{"title":"Lecture 17：导数求导法则","tags":["数学"],"categories":null,"date":"2023-12-17","dg-publish":true,"permalink":"/03数学/01_高等数学/2. 第二章：导数与微分/Lecture 17：导数求导法则/","dgPassFrontmatter":true}
---

---
---
## 1.1 和差积商求导法则
**有理运算法则**
设 $u(x),\nu(x)$ 都可导，则
+ $(u\pm v)^{\prime}=u^{\prime}\pm v^{\prime}$
+ $(uv)^{\prime}=u^{\prime}v+uv^{\prime}$
+ $(\frac\mu\nu)^{\prime}=\frac{\mu^{\prime}\nu-\nu^{\prime}\mu}{\nu^2}\quad(\nu\neq0)$
+ ![Pasted image 20250607173910.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250607173910.png)

## 1.2 反函数的求导法则
**定理 2：**
设区间 $I$ 上严格单调且连续的函数 $x=f(y)$ 在 $y$ 处可导，且 $f^{\prime}(y)\neq0$,则它的反函数 $y=f^{-1}(x)$ 在对应点可导。
+ 则：$(f^{-1})^{\prime}(x)=\frac1{f^{\prime}(y)}\quad\frac{dy}{dx}=\frac1{dx}$
+ 含义
	+ 函数和反函数是两个函数，但是是同一条曲线；
	+ 因此**当函数连续且单调时，可以知其反函数也同样可导**；

**例题：**$\text{求}\quad y=\arcsin\quad x\quad(x\in[-1,1])\text{ 导数}$
反函数：$x=\sin y\quad y\in\left[-\frac\pi2,\frac\pi2\right]$
函数的导数：$\frac{dy}{dx}=(\arctan x)^{\prime}=\frac{1}{\log}=\frac{1}{\sqrt{1-\sin^{2}y}}=\frac{1}{\sqrt{1-x^{2}}}$
####  反函数的二阶导
![Pasted image 20250607194831.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250607194831.png)
![Pasted image 20250607194916.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250607194916.png)
## 1.3 复合函数求导法则
**定理 3：链式法则**
设 $u=g(x)$ 在 $x$ 可导，$y=f(u)$ 在对应 $u$ 处可导，则 $y=f[g(x)]$ 在 x 处可导。
+ 则： $\frac{dy}{dx}=f^{\prime}(u)g^{\prime}(x)$
+ 其他形式：
	+ $\frac{dy}{dx}=\frac{dy}{du}\cdot\frac{du}{dx}$
![Pasted image 20250607192706.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250607192706.png)
![Pasted image 20250607193031.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250607193031.png)
**例题：**$y=2\cos^2\frac1x$
使用链式法则： $y=2u^{2},u=\cos v,v=\frac{1}{-x^2}$
+ $\begin{aligned}\frac{dy}{dx}&=4u\cdot(-\sin v)(-\frac1{x^2})\\&=4\end{aligned}$

**注意：求函数值时，是从里到外；但求导数时，是从外到里，一直求到对 x 求导；**

**结论**：奇函数、偶函数求导之后，导函数的奇偶性发生反转；
+ 奇函数的导函数：偶函数；
+ 偶函数的导函数：奇函数；

## 1.4 求导结论
**基本初等函数**
+ 基本
	+ $\begin{aligned}&\quad(C)^{\prime}=0\quad&\quad(x^\alpha)^{\prime}=\alpha x^{\alpha-1}\\&\quad(a^x)^{\prime}=a^x\ln a\quad&\quad(e^x)^{\prime}=e^x\\&\quad(\log_ax)^{\prime}=\frac1{x\ln a}\quad&\quad(\ln|x|)^{\prime}=\frac1x\end{aligned}$
+ 三角函数
	+ $(\sin x)^{\prime}=\cos x\quad\quad\quad\quad\quad(\sin x)^{\prime}=-\cos x$
	+ $\begin{aligned}(\tan x)^{\prime}&=\sec^2x&(\cot x)^{\prime}&=-\csc^2x\\\\(\sec x)^{\prime}&=\sec x\tan x&(\csc x)^{\prime}&=-\csc x\cot x\end{aligned}$
+ 反函数导数
	+ $\begin{aligned}&(\arcsin x)^{\prime}=\frac1{\sqrt{1-x^2}}&&(\arccos x)^{\prime}=-\frac1{\sqrt{1-x^2}}\\&(\arctan x)^{\prime}=\frac1{1+x^2}&&(arcot x)^{\prime}=-\frac1{1+x^2}\end{aligned}$
	+ ![Pasted image 20250826115919.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250826115919.png)
	+ 注意此时的定义域
	+ 
	+ ![Pasted image 20250607173810.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250607173810.png)

## 1.5 对数求导法 
**例题引入**
+ $\text{设}y=\left(1+\sin x\right)^{x},\text{则}\mathrm{d}y|_{x=\pi}=$ __
+ 幂指函数；
+ 对数求导法：
	+ 先取对数：$\ln y=x\ln(1+\sin x)$
	+ 两边同时求导：$\frac{y^{\prime}}{y}=\ln(s+\sin x)+\frac{xCosx}{1+\sin x}$
	+ 提出 $y^{\prime}$，得到导函数
	+ 带入 x=Π；

**一个重要结论**
+ $(\ln|x|)^{\prime}=\frac{1}{x}$
+ $In$ 的加绝对值后的导数依然是 1/x；

**对数求导法使用场合**
+ 1. 幂指型函数；
+ 2. 连乘、连除、乘法、开方；

## 1.5 幂指函数求导法 
![Pasted image 20250608164632.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250608164632.png)
重要结论
![Pasted image 20250608182849.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250608182849.png)
### 函数 $y = x^x$ ($x > 0$) 的导数求解

#### 求解步骤：
1. **函数变形**（利用指数对数恒等式）：  
   $y = x^x = e^{\ln(x^x)} = e^{x \ln x}$

2. **链式法则求导**：  
   令 $u = x \ln x$，则 $y = e^u$。  
   - 求 $u$ 的导数（乘积法则）：  
     $u' = \frac{d}{dx}(x) \cdot \ln x + x \cdot \frac{d}{dx}(\ln x) = \ln x + x \cdot \frac{1}{x} = \ln x + 1$
   - 代入链式法则：  
     $y' = e^u \cdot u' = e^{x \ln x} \cdot (\ln x + 1)$

3. **还原原函数形式**：  
   $y' = x^x (\ln x + 1)$

---

#### 最终结果：
$\boxed{y' = x^x (\ln x + 1)}$

---

### 扩展：$x^{nx}$ 型函数的导数通式
对一般形式 $y = x^{nx}$ ($n$ 为常数)：  
1. 变形：$y = e^{\ln(x^{nx})} = e^{nx \ln x}$  
2. 求导：$y' = e^{nx \ln x} \cdot \frac{d}{dx}(nx \ln x) = x^{nx} \cdot n(\ln x + 1)$  
3. 特例：  
   - $n=1$ 时：$y' = x^x (\ln x + 1)$  
   - $n=2$ 时：$y' = x^{2x} \cdot 2(\ln x + 1)$  
   - $n=3$ 时：$y' = x^{3x} \cdot 3(\ln x + 1)$



![Pasted image 20250608191552.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250608191552.png)