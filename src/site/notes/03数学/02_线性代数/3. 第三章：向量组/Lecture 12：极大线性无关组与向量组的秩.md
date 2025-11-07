---
{"tags":[],"dg-publish":true,"permalink":"/03数学/02_线性代数/3. 第三章：向量组/Lecture 12：极大线性无关组与向量组的秩/","dgPassFrontmatter":true}
---

---

## 12.1 极大线性无关组
### 12.1.1 极大线性无关组基本概念
##### **定义**： #极大线性无关组
> <font color="#ccc1d9">描述：</font> $$\text{在向量组}a_1,a_2,\cdots,a_s\text{中,若存在部分组}a_{i_1},a_{i_2},\cdots,a_{i_r}\text{满足}:$$
> $$1.a_{i_1},a_{i_2},\cdots,a_{i_r}线性无关$$
> $$2. 向量组中任意向量 a_i 是原本向量组的极大线性无关组$$ 
> 则称：$$a_{i_1},a_{i_2},\cdots,a_{i_r}是原向量组的极大线性无关组$$

**解释**
+ 概念： 
	+ 向量组的极大线性无关组一般<font color="#ff0000">不唯一</font>；
	+ 只由一个零向量组成的向量组不存在极大线性无关组，一个线性无关向量组的极大线性无关组就是该向量组本身；
+ $a_{i_1},a_{i_2},\cdots,a_{i_r}$
	+ 来自原来的向量组；
	+ 从向量中挑出部分组：$i_r$ 个出来；
+ 注意： 
	+ 极大线性无关组是不唯一的；
	+ 零向量不研究；

### 12.1.2 等价向量组 
##### **定义**： #等价向量组
> <font color="#ccc1d9">描述：</font> $\text{设两个向量组:(I)}\alpha_1,\alpha_2,\cdots,\alpha_s,(II)\beta_1,\beta_2,\cdots,\beta_i.\text{若(I)中每个向量}\alpha_i(i=1,2,\cdots,s)\text{均可由}$ (Ⅱ)中向量线性表示,则称向量组 (1)可由向量组 (Ⅱ)线性表示; 若向量组 (I), (Ⅱ)可以相互线性表示,则称向量组 (I)与向量组 (I)是等价向量组，记作 (I)相似于(Ⅱ).

**解释**
+ 概念： 
	+ 表示**多个向量可以被多个向量表示**；
	+ 等价向量组不是极大线性无关组，其中可能会有“躺平”的向量组；
	+ 所以不是“相等”，而是叫**等价**；
+ 目的： 
	+ 本质上来说，其表示：**等价向量组所装成的空间是一致的**；
+ 解释： 
	+ A 和 B 等价 `<->` A 可以由 B 表示 + B 可以由 B 表示  `<->` `r(A)=r(B)=r(A|B)`


**补充**：充要条件 
+ $r(\alpha_{1}\alpha_2,\cdots,\alpha_s)=r(\beta_1,\beta_2,\cdots,\beta_i).$
+ 证明： 
	+ 不妨设：$r(\alpha_{1}\alpha_2,\cdots,\alpha_s,\beta_1,\beta_2,\cdots,\beta_i)=r(\beta_1,\beta_2,\cdots,\beta_i)=r(\alpha_{1}\alpha_2,\cdots,\alpha_s)$ 
	+ 则表示：$\alpha_{1}\alpha_2,\cdots,\alpha_s$ 可以由 $\beta_1,\beta_2,\cdots,\beta_i$ 表示；
	+ 还表示：$\beta_1,\beta_2,\cdots,\beta_i$ 也可以由 $\alpha_{1}\alpha_2,\cdots,\alpha_s$ 表示；
+ 等价向量组的充分条件 `<-` 三秩相同：
	+ $$r(\alpha_{1}\alpha_2,\cdots,\alpha_s,\beta_1,\beta_2,\cdots,\beta_i)=r(\beta_1,\beta_2,\cdots,\beta_i)=r(\alpha_{1}\alpha_2,\cdots,\alpha_s)$$
	+ 意义：将其转化为**求其秩是否相同的问题**；

**注意**：考生应注意等价矩阵和等价向量组概念的区别；
+ 矩阵等价要同型：`A,B` 等价 `->` `r(A)=r(B)`.
	+ 举例：$(\begin{matrix}1\\0\end{matrix})和(\begin{matrix}0\\1\end{matrix})$
+ 等价向量组的**充分**条件：$r(A|B)=r(B)=r(A)$

## 12.2 向量组的秩 
### 12.2.1 向量组的秩基本概念  
##### **定义**： #向量组的秩 
> <font color="#ccc1d9">描述：</font> $$r(\alpha_{1},\alpha_{2},\cdots,\alpha_{s})=r$$
> 等价向量组具有相等的秩，反之未必成立

**解释**
+ 极大无关组的空间的维数；

### 12.2.2 有关秩的重要定理和公式
##### **定理**： #三秩相等 
> <font color="#8db3e2"><font color="#c6d9f0">描述：</font></font> `r(A)(矩阵的秩)=A的行秩(A的行向量组的秩)=A的列秩(A的列向量组的秩)`

**解释**
+ 竖着看和横着看的向量组它们的秩都是一样的；

##### **定理**： #A到B的初等行变换 
> <font color="#8db3e2"><font color="#c6d9f0">描述：</font></font>若 `A` 到 `B` 进行初等行变换，则：
> 1. `A` 的行向量组和 `B` 的行向量组是等价向量组；
> 2. `A` 和 `B` 的任何相应的部分列向量组具有相同的线性相关性；

**解释**
+ 1. `A` 的行向量组和 `B` 的行向量组是等价向量组 `<-` $r(A|B)=r(B)=r(A)$
+ 2. `A` 和 `B` 的任何相应的部分列向量组具有相同的线性相关性； 
	+ 不仅是性质相同，最后得到的解也是相同的；

##### **定理**： #向量组的线性表示 
> <font color="#8db3e2"><font color="#c6d9f0">描述：</font></font>若向量组 `A` 可以被 `B` 表示，则 $r(A)<=r(B)$

### 12.2.3 解题：求极大线性无关组 
**方法**：求极大线性无关组的步骤 
+ 1. 将列向量们组成矩阵作初等**行**变换，化为行阶梯形矩阵，并确定 `r(A)`；
+ 2. 按列找出一个秩为 `r(A)` 的子矩阵，即为一个极大线性无关组；
![Pasted image 20250728132653.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250728132653.png)
![Pasted image 20250728133240.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250728133240.png)
由此延申的考点求矩阵$A^n$ ，求其分解形式
### 12.2.4 结论
**结论一**：`r(AB)≤min{r(A),r(B)` 

**结论二**：`r(A+B)≤r([A, B]≤r(A)+r(B)`

**结论三**：设 A 是 `n (n≥2)` 阶方阵，$A^*$ 是 $A$ 的伴随矩阵，则：

+ $$r\left(A^{*}\right)=\begin{cases}n,&r\left(A\right)=n,\\1,&r\left(A\right)=n-1,\\0,&r\left(A\right)<n-1.\end{cases}$$
+ ![Pasted image 20250728153040.png|800](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250728153040.png)
	![Pasted image 20250728142626.png|800](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250728142626.png)

	![Pasted image 20250728142546.png|700](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250728142546.png)

解空间（也叫解空间、零空间）的严格定义是：**齐次线性方程组$(\boldsymbol{A}\boldsymbol{x} = \boldsymbol{0})$的所有解向量构成的集合
$(\boldsymbol{A}\boldsymbol{x} = \boldsymbol{0})$.若平面方程是**齐次线性方程（$如(ax + by + cz = 0$) ，则它是齐次方程组$(\begin{pmatrix} a & b & c \end{pmatrix}\begin{pmatrix} x \\ y \\ z \end{pmatrix} = 0)$的解空间。 此时系数矩阵$\boldsymbol{A}$是$(1 \times 3)$矩阵，秩$(r(\boldsymbol{A}) = 1)$（若(a,b,c)不全为 0 ）。
- 根据解空间维数公式$(\dim V = n - r(\boldsymbol{A}))$（(n=3\)是未知数个数 ），得$(\dim V = 3 - 1 = 2)。$
- 几何意义：过原点的平面是二维线性子空间，维数为 2，符合 “解空间维数” 的定义。

- 这里的 “秩为 1”，本质是**方程组只有 1 个独立的约束条件**（比如 “\(x + y + z = 0\)” 只约束了\(x,y,z\)的和，没有其他独立约束）。

你提到的 “n阶” 容易混淆，这里的**关键不是 “方阵的阶数”**，而是**未知数的个数 = 矩阵的列数**（记为n）。
在平面方程的例子中：
- $矩阵(\boldsymbol{A})是(1 \times 3)矩阵（1 行 3 列），列数(n = 3)（对应未知数(x,y,z)的个数）。$
- $解空间维数公式(\dim V = n - r(\boldsymbol{A}))中，n是未知数个数（矩阵列数），而非 方阵的阶数。$
只有当矩阵是方阵（行数 = 列数 =n）时，才会说 “n阶矩阵”，但解空间维数公式的n始终是**未知数个数（列数）**，与行数无关。




![Pasted image 20250728161730.png|800](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250728161730.png)