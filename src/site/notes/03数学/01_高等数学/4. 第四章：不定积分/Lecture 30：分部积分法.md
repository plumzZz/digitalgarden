---
{"title":"Lecture 30：分部积分法","tags":[],"categories":null,"date":"2024-01-19","dg-publish":true,"permalink":"/03数学/01_高等数学/4. 第四章：不定积分/Lecture 30：分部积分法/","dgPassFrontmatter":true}
---

---
---
## 1.1 分部积分法
<font color="#ff0000">time2</font>
### 1.1.1 基本概念
##### **定义**： #分布积分法
> <font color="#ccc1d9">描述：</font>设 $u(x),\nu(x)$ 有连续一阶导数，则 $\int udv=uv-\int vdu$

**解释**
+ 其中：有时候是 $udv$ 简单，有时候是 $vdu$ 简单
+ v、u 的选取是其核心点；

### 1.1.2 例题
**例题**：$\int xe^xdx$
+ 分析
	+ 由于 $ex$ 的积分比较好求，所以需要考虑如何把 ex 放到 vdu 的位置上；
	+ 但也可以考虑把 x 放到 vdu 的位置上，但是要更难做一些；
+ 解析
	+ $\int xe^xdx=\int x\operatorname{de}^x=xe^x-\int e^x\operatorname{dx}$
	+ $\int\mathrm{e}^{\mathrm{x}}\mathrm{d}\mathrm{x}=\times\mathrm{e}^{\mathrm{x}}-\mathrm{e}^{\mathrm{x}}+\mathrm{d}$
+ 题型： #分部积分法

**例题**：$\int x sin xdx$
+ 分析
+ 解析
	+ 原式的等于： $-\int xdcosx=-\left[x\cos x-\int\cos dx\right]$
+ 题型： #分布积分法 

**例题**：$\int sec^3 xdx$
+ 分析
	+ 
+ 解析
	+ 原式： $\int\sec^{3}xdx=\int\sec xd\tan x=\sec xdx-\int\tan^{2}x\sin xdx$ $=\sec x\tan x-\int\sec^3xdx+\int\sec xdx$
	+ 此时，由于原式的右边也出现了一个 sec 3 xdx 的负，所以可以将其放到右边去
	+ $\int sec^3x\mathrm{~d}x=\frac12\left[secxtanx+\ln|\sec x+\ln x|\right]+\mathrm{C}$
		+ 其中的 1\2 是因为右边的 sec 移到左边去了；
+ 题型： #分部积分法 

## 1.2 分部积分法总结
**总结**
+ 概念：把之前求导时候的乘法公式过程，倒转过来，形成分布积分法；
+ 令其为 u 的口诀为，<font color="#ff0000">反对幂指三</font>

**何时用**
+ 适用于**两类不同函数相乘**；
+ 1. $\int xe^{x}dx$
+ 2. $\int x\sin xdx$
+ 3. $\int e^{x}\sin xdx$
  
**如何用**
+ 八类典型分部积分规律；
+ 多项函数 × 指数|三角：
	+ 1. $\int p_n(x)e^{ax}\operatorname{d}x$
		+ 凑指数
	+ 2. $\int p_n(x)\sin ax\operatorname{d}x$
		+ 凑三角
	+ 3. $\int p_n(x)\cos axdx$
		+ 凑三角
+ 多项函数 × 对数|反三角：
	+ 4. $\int P_n(x)\ln xdx$
		+ 凑多项式
	+ 5. $\int P_n(x)\arctan xdx$
		+ 凑多项式
	+ 6. $\int P_n(x)\arcsin xdx$
		+ 凑多项式
+ 指数 × 三角
	+ 7. $\int e^{\alpha x}\sin\beta xdx$
		+ 凑谁都行
	+ 8. $\int e^{\alpha x}\cos\beta xdx$
		+ 凑谁都行


# 分部积分法表格法拓展公式： <font color="#ff0000">time1</font>
![Pasted image 20250723165943.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250723165943.png)

分布积分的特殊情况
![Pasted image 20250723171929.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250723171929.png)



![Pasted image 20250808152023.png](/img/user/01%E9%99%84%E4%BB%B6/Pasted%20image%2020250808152023.png)
图中类似行列式的计算是**分部积分法的“表格速算形式”** ，是简化分部积分（尤其含多次分部时）的技巧，核心逻辑和步骤如下：
### 1. 原理基础
本质是 **分部积分公式** $\boldsymbol{\int u\mathrm{d}v = uv - \int v\mathrm{d}u}$ 的“可视化简化”，通过“函数列 + 符号列 + 导数/积分列” 快速对应分部积分的 $u$、$v$ 与 $\int v\mathrm{d}u$ 。

### 2. 表格构造（以 $\boldsymbol{\int e^{-2x}\cos 2x \mathrm{d}x}$ 这类多次分部为例 ）
- **左列（函数列）**：选其中一个函数不断求导，另一个不断积分。比如算 $\int e^{-2x}\cos 2x \mathrm{d}x$，可设 $\boldsymbol{u = \cos 2x}$（求导列），$\boldsymbol{\mathrm{d}v = e^{-2x}\mathrm{d}x}$（积分列 ），则左列依次为：  
  $\cos 2x \quad \downarrow$ 求导 $\quad -2\sin 2x \quad \downarrow$ 求导 $\quad -4\cos 2x \quad \dots$  
- **中间列（符号列）**：首行符号为 $\boldsymbol{+}$，交替变号（$+,-,+,\dots$ ），对应分部积分的 $uv$ 符号和后续积分的符号。  
- **右列（积分/导数列）**：与左列对应，对另一函数积分（或求导）。比如 $\boldsymbol{\mathrm{d}v = e^{-2x}\mathrm{d}x}$ 积分得 $\boldsymbol{-\frac{1}{2}e^{-2x}}$，再积分得 $\boldsymbol{\frac{1}{4}e^{-2x}}$  ，即：  
  $\boldsymbol{e^{-2x}}$ （原 $\mathrm{d}v$ 对应的 $v$ 需积分，这里简化为“积分方向” ） $\quad \downarrow$ 积分 $\quad -\frac{1}{2}e^{-2x} \quad \downarrow$ 积分 $\quad \frac{1}{4}e^{-2x} \quad \dots$  
### 3. 计算逻辑
- **一次分部**：取表格首行乘积（左列首行×右列首行），对应分部积分的 $\boldsymbol{uv}$ 项；  
- **符号与后续积分**：中间列符号×下一行 “左列导数×右列积分”，对应 $\boldsymbol{-\int v\mathrm{d}u}$ 。若需多次分部（如函数复杂、多次求导后简化），就继续按 “符号×行列乘积” 累加，直到导数为 $0$（或满足停止条件）。  

### 4. 简化作用
- 避免反复写 “$\int u\mathrm{d}v = uv - \int v\mathrm{d}u$” 的文字过程，尤其多次分部时（如 2 次、3 次分部），表格能快速对应 “$uv$ 项” 和 “剩余积分项”，减少书写与符号错误。  

简单说，这是 **把分部积分的 “$u$ 求导、$v$ 积分、符号交替” 规律，用表格直观呈现的速算技巧** ，适合含指数、三角乘积的积分（如 $\boldsymbol{\int e^{ax}\sin bx\mathrm{d}x}$ 、$\boldsymbol{\int e^{ax}\cos bx\mathrm{d}x}$ ），能大幅简化多次分部的计算流程~

