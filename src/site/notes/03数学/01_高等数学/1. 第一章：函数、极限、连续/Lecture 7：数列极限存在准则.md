---
{"title":"Lecture 7：极限存在准则","tags":["数学"],"categories":null,"date":"2024-03-01","dg-publish":true,"permalink":"/03数学/01_高等数学/1. 第一章：函数、极限、连续/Lecture 7：数列极限存在准则/","dgPassFrontmatter":true}
---

---
---
# 极限存在准则基本概念
### 7.1.1 数列极限的存在准则
##### **定理**： #夹逼准则
> <font color="#8db3e2"><font color="#c6d9f0">描述：</font></font> $\text{若存在 }N,\text{当 }n>N\text{ 时, }x_n\leq y_n\leq z_n$，$\lim_{n\to\infty}x_n=\lim_{n\to\infty}z_n=a,\text{则}\lim_{n\to\infty}y_n=a$

**使用情况**：n 项和
+ 举例：$\lim_{n\to\infty}\left[\frac n{n^2+1}+\frac n{n^2+2}+\cdots+\frac n{n^2+n}\right]$
+ 放大：$\frac n{n^2+n}$
+ 缩小：$\frac n{n^2+1}$
+ 使用：$\frac{n^2}{n^2+n}\leq\left[\frac n{n^2+1}+\frac n{n^2+2}+\cdots+\frac n{n^2+n}\right]\leq\frac{n^2}{n^2+1}$
{ #hmcand}


**使用情况**：取整函数
+ 举例：$\lim_{x\to0^+}x[\frac1x]$
+ 大小：$\frac1x-1<[\frac1x]\leq\frac1x$

**常用数列极限**
![Pasted image 20250604201424.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250604201424.png)

**重要结论**
![Pasted image 20250604203038.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250604203038.png)
![Pasted image 20250604203146.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250604203146.png)




# 夹逼定理的重要结论
*需要把这个缩放思想运用起来*
![Pasted image 20250605210402.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250605210402.png)
![Pasted image 20250605210351.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250605210351.png) ![Pasted image 20250605211723.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250605211723.png) ![Pasted image 20250606144521.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250606144521.png)
![Pasted image 20250606144548.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250606144548.png) ![Pasted image 20250606144721.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250606144721.png)

![Pasted image 20250606144909.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250606144909.png)
![Pasted image 20250606144935.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250606144935.png)
![Pasted image 20250606145115.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250606145115.png)


# 数列的单调有界证明
##### **定理**： #数列的单调有界准则
> <font color="#8db3e2"><font color="#c6d9f0">描述：</font></font>单调有界数列必有极限；
> 1. 单调增、有上界的数列必有极限；
> 2. 单调减、有下界的数列必有极限；
> 3. ![Pasted image 20250606155957.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250606155957.png)
## 证明数列单调性的常用方法
![Pasted image 20250606155513.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250606155513.png)
*易错*
![Pasted image 20250606160510.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250606160510.png)

### 数学归纳法
第一类归纳法
![Pasted image 20251017172127.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020251017172127.png)
第二类归纳法
![Pasted image 20251017172144.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020251017172144.png)

例题
	![Pasted image 20251017173207.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020251017173207.png)
	
	![Pasted image 20250606160844.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250606160844.png)
# 数列收敛速度
![Pasted image 20250606164655.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250606164655.png)
![Pasted image 20250606164732.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250606164732.png)
![Pasted image 20250606164912.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250606164912.png)