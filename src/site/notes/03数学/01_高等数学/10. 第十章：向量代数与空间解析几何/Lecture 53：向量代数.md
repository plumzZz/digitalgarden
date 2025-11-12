---
{"tags":[],"dg-publish":true,"permalink":"/03数学/01_高等数学/10. 第十章：向量代数与空间解析几何/Lecture 53：向量代数/","dgPassFrontmatter":true}
---

---
---

![Pasted image 20250826162535.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250826162535.png)

## 53.1 数量积（点积、内积）
##### **定理**： #向量代数的数量积
> <font color="#8db3e2"><font color="#c6d9f0">描述：</font></font>
> $$1\text{)几何表示: }\mathbf{a}\cdot\mathbf{b}=\mid\mathbf{a}\mid\mid\mathbf{b}\mid\cos\alpha $$
> $$2\text{)代数表示:}\quad\mathbf{a}\cdot\mathbf{b}=\mathbf{a}_xb_x+\mathbf{a}_yb_y+\mathbf{a}_zb_z$$
> $$3\text{)运算规律:}\quad 交换律：\mathbf{a}\cdot\mathbf{b}=\mathbf{b}\cdot\mathbf{a} \quad \text{分配律: }\mathbf{a\cdot(b+c)=a\cdot b+a\cdot c}$$
> $$4\text{)几何应用:}\quad 求模：|\mathbf{a}|=\sqrt{\mathbf{a}\cdot\mathbf{a}}\text{求夹角: }\cos\alpha=\frac{\mathbf{a}\cdot\mathbf{b}}{|\mathbf{a}||\mathbf{b}|}\quad \text{判定两向量垂直:}\mathbf{a\perp b\Leftrightarrow a\cdot b=0}$$
> ![Pasted image 20250826163339.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250826163339.png)




## 53.2 向量积（外积、叉积，叉乘，乘积）
外积、叉积三维空间中二者等价，高维空间中外积是更广泛的概念，叉乘是三维特例外积的 “向量化” 结果。
##### **定理**： #向量代数的向量积
> <font color="#8db3e2"><font color="#c6d9f0">描述：</font></font>
> $1. \text{几何表示:}\quad\mathbf{a}\times\mathbf{b}\text{ 是一向量}.\quad\text{模}:\mid\mathbf{a}\times\mathbf{b}\mid=\mid\mathbf{a}\mid\mid\mathbf{b}\mid\sin\alpha$
> $2. \text{代数表示:}\quad{\mathbf{a}\times\mathbf{b}}=\begin{vmatrix}\mathbf{i}&\mathbf{j}&\mathbf{k}\\a_x&a_y&a_z\\b_x&b_y&b_z\end{vmatrix}$
> $3. i) a\times b= - ( b\times a) \quad ii)分配律：a\times(b+c)=a\times b+a\times c$
> $4. 运算规律：i)求同时垂直于 a 和 b 的向量: a×b\quad ii)求以 a 和 b 为邻边的平行四边形面积:S=|a×b|\quad iii)判断两向量平行：\mathbf{a//b}\Leftrightarrow\mathbf{a\times b}=0$![Pasted image 20250826164300.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250826164300.png)
> ![Pasted image 20250826164418.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250826164418.png)
c是平行四边形面积大小，复合右手法则
![Pasted image 20250826204413.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250826204413.png)

![Pasted image 20250826164705.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250826164705.png)


**解释**
+ 几何表示 `->` 右手法则 `->` 垂直于 $a,b$ 向量的一个直线；
+ 注意：
	+ 数量积满足交换律，向量积不满足交换律； 

## 53.3 混合积
##### **定理**： #向量代数的混合积
> <font color="#8db3e2"><font color="#c6d9f0">描述：</font></font> https://www.bilibili.com/video/BV18kNheVEWJ?t=164.9
> 基本表述：$\left[ abc \right] = (a \times b) \cdot c$先是
> 
> ![Pasted image 20250826164826.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250826164826.png)
> 
> 定义： $$\ a = a_xi + a_yj + a_zk \\ b = b_xi + b_yj + b_zk \\ c = c_xi + c_yj + c_zk$$
> 性质：
> 该性质是因为在算以a,b,c为棱的平行六面体的体积
>  $$轮换对称性：(abc)=(bca)=(cab)\quad $$
> $$(a\times b)\cdot c = a\cdot(b\times c) = b \cdot (c\times a)$$
>$$(\mathbf{abc})=-(\mathbf{acb})$$
>![Pasted image 20250827113452.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250827113452.png)
>
>




轮换对称性
![Pasted image 20250826212724.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250826212724.png)

> （2）$$\begin{aligned}(a\times b)\cdot c=-(b\times a)\cdot c\\(a\times b)\cdot c=-(c\times b)\cdot a\\(a\times b)\cdot c=-(a\times c)\cdot b\end{aligned}$$
> （3）$$a\text{、}b\text{、}c\text{三向量共面}\Leftrightarrow[abc]=0$$
> 几何意义：
> 1. 向量的混合积 $[abc]=(a\times b)\cdot c$ 的绝对值在数值上等于以向量 a、b、c 为棱的平行六面体的体积
> 2. $V_\text{平行六面体}=|\mathrm{(abc)}|$
# 53.4 方向角和方向余弦
![Pasted image 20250826165023.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250826165023.png)

