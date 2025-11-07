---
{"title":"Lecture 4：极限基础","tags":["数学","极限"],"categories":null,"date":"2024-02-28","dg-publish":true,"permalink":"/03数学/01_高等数学/1. 第一章：函数、极限、连续/Lecture 4：数列极限的概念/","dgPassFrontmatter":true}
---

---
---
## 4.1 极限的基本概念
+ 主要是两种
	+ 1. 数列极限；
	+ 2. 函数极限；

### 4.1.1 数列极限 
##### **定义**： #数列极限
> <font color="#ccc1d9">描述：</font>对 $\lim_{n\to\infty}x_n=a$ 而言：$\forall\varepsilon>0,\exists N>0,\text{ 当 }n>N\text{ 时, 恒有 }|x_n-a|<\varepsilon$

**解释**
+ $\varepsilon>0$ ：函数的接近程度；
+ 几何意义：$x_n$ 在 $\varepsilon$ 前后的小领域内；
+ N：大 N 项之后的所有数字，都落在了 $|x_n-a|<\varepsilon$ 的范围内，而 N 是一个无穷多的项，N 之前的数字是一个有限项；
	+ 有限项总是有界的；  
	+ 数列 $\left\{x_n\right\}$ 的极限**和前有限项无关**；
	![Pasted image 20250604201849.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250604201849.png)
	

**概念**：结论 1
+ $$\lim_{n\to\infty}x_n=a\Leftrightarrow\lim_{k\to\infty}x_{2k-1}\overset{\color{red}{}}{\operatorname*{=}}\lim_{k\to\infty}x_{2k}=a.$$
+ 如果**一个数列以 a 为极限，则其子数列都以 a 为极限**；

**概念**：结论 2
+ 1. $$\text{若 }\lim_{n\to\infty}x_n=a,\text{则}\lim_{n\to\infty}\lvert x_n\rvert=\lvert a\rvert,\text{ 但反之不成立}$$
+ 2. $$\lim_{n\to\infty}x_n=0\text{ 的充分必要条件是 }\lim_{n\to\infty}|x_n|=\mathbf{0}$$

**概念**：结论 3
+ 一个数列的子数列如果满足以下两个条件，则可以推出完整数列的值：
	+ 1. 子数列的值全部都相等；
	+ 2. 几个子数列取遍了原数列的所有情况；

### 数列的收敛与发散

#### 1. **收敛数列**
- **定义**：若存在有限实数 $L$，使得对任意 $\varepsilon > 0$，都存在正整数 $N$，当 $n > N$ 时满足  $|a_n - L| < \varepsilon$ $则称数列 $\{a_n\}$ 收敛于极限 $L$，记为：
  $$
  \lim_{n \to \infty} a_n = L
  $$
- **直观理解**：当 $n$ 充分大时，$a_n$ 无限接近某个固定值 $L$。
- **例子**：
  - $a_n = \frac{1}{n}$ 收敛于 $0$（因为 $\lim_{n \to \infty} \frac{1}{n} = 0$）。
  - $a_n = 2 - \frac{1}{n^2}$ 收敛于 $2$。

#### 2. **发散数列**
- **定义**：若不存在满足上述条件的有限极限 $L$，则数列 $\{a_n\}$ 发散。
- **常见类型**：
  - **振荡型发散**：数列在多个值间振荡，如 $a_n = (-1)^n$（取值 $-1, 1, -1, 1, \ldots$）。
  - **无穷发散**：数列趋向无穷大，如 $a_n = n^2$（$\lim_{n \to \infty} n^2 = +\infty$）。
  - **无界但不趋向无穷**：如 $a_n = n \cdot \sin(n)$（无界但振荡）。
- **例子**：
  - $a_n = 2^n$ 发散到 $+\infty$。
  - $a_n = \sin(n\pi/2)$ 振荡（取值 $0, 1, 0, -1, \ldots$）。

#### 3. **关键判别法**
- **收敛的必要条件**：若收敛，则 $\{a_n\}$ 必有界（反之不成立，如振荡数列有界但发散）。
- **极限唯一性**：若数列收敛，其极限唯一。
- **运算性质**：若 $\lim a_n = A$，$\lim b_n = B$，则：
  $$
  \lim (a_n \pm b_n) = A \pm B, \quad \lim (a_n \cdot b_n) = A \cdot B, \quad \lim \frac{a_n}{b_n} = \frac{A}{B} \ (B \neq 0).
  $$


#### 4. **经典反例**
- **调和级数**：$a_n = \sum_{k=1}^n \frac{1}{k}$ 发散（虽趋向无穷，但速度极慢）。
- **交替调和数列**：$a_n = (-1)^n \frac{1}{n}$ 收敛于 $0$（振荡但幅度衰减）。



# 海涅定理
联系函数于数列的纽带
![Pasted image 20250605181652.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250605181652.png)
![Pasted image 20250605183105.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250605183105.png)

# 对于连续定义的补充 
*用迪利克雷函数的有界性或者夹逼定理*

**思路**
![Pasted image 20250605204239.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250605204239.png)
**步骤**
![Pasted image 20250605202830.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250605202830.png)

## 这里的问题意思是 $x_0$ 处连续，并不意味着 $x_0$ 附近的所有的点都连续

![Pasted image 20250605203310.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250605203310.png)
![Pasted image 20250605203215.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250605203215.png)
![Pasted image 20250605203053.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250605203053.png)
![Pasted image 20250605202621.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250605202621.png)

应用归结原则
![Pasted image 20250605204109.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250605204109.png)