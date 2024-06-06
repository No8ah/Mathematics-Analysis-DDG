1. 定义(  [[三角级数]]  )
	- $\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}(a_{n}\cos nx + b_{n}\sin nx)$
		- $\textcolor{orange}{\underline{\textbf{每一项}}}都以2\pi为\textcolor{orange}{\underline{\textbf{周期}}}$
# 一、三角级数与$Flourier$级数

1. 命题1(  $\forall \ \alpha \quad \Rightarrow \quad \int^{\alpha+T}_{\alpha}f(x)dx=\int^{T}_{0}f(x)dx$  )
	- **1个先决条件**
		1. $f(x)以T为\textcolor{orange}{\underline{\textbf{周期}}}$
	1. 定义(  [[三角函数系]]  )
3. 定理14.1(  $\forall \ \textcolor{orange}{\underline{\textbf{三角函数系}}}上的两个\textcolor{orange}{\underline{\textbf{不同函数}}}的\textcolor{pink}{\underline{\textbf{乘积}}} \quad \Rightarrow \quad 区间[-\pi, \pi]上的\textcolor{orange}{\underline{\textbf{积分}}}=0$  )
	1. $\int^{\pi}_{- \pi}\sin nxdx=0 \quad \int^{\pi}_{- \pi}\cos nx dx=0 \quad (\forall \ n \in \mathbb{N}_{+})$
	2. $\int^{\pi}_{- \pi}\sin mx \cos nx dx =0 \quad (\forall \ m,n \in \mathbb{N}_{+})$
	3. $\int^{\pi}_{- \pi}\sin mx \sin nx dx =0 \quad \int^{\pi}_{- \pi}\cos mx \cos nx=0 \quad (\forall \ m \neq n \in \mathbb{N}_{+})$
	- $\textcolor{pink}{\underline{\textbf{三角函数系}}}的\textcolor{orange}{\underline{\textbf{正交性}}}$
	- 三角级数的系数求解
	- 定义(  [[f(x)在闭区间上绝对可积]]  )
- 定义(  [[f(x)的Flourier系数]]  )
	- 定义(  [[f(x)的Flourier级数]]  )
# 二、$Flourier$级数的收敛性
# 三、任意区间上的$Flourier$级数

1. 定义(  [[周期为2l的函数f(x)的Flourier级数]]  )
	1. 定义(  [[偶延拓]]  )
	2. 定义(  [[奇延拓]]  )
# 四、$Flourier$级数的平均收敛性质

1. 定义(  [[平方可积]]  )
2. 断言(  $f在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{平方可积}}}\quad \Rightarrow \quad f在[-\pi,\pi]上\textcolor{red}{\underline{\textbf{绝对可积}}}$  )
	1. 断言(  $2个条件\quad \Rightarrow \quad f(x) \sim \frac{a_{0}}{2}+ \sum\limits_{n=1}^{\infty}(a_{n}\cos nx +b_{n} \sin nx)$  )
		- **2个条件**
			1. $f以2\pi为\textcolor{orange}{\underline{\textbf{周期}}}$
			2. $f在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{平方可积}}}$
1. 性质(  平方可积  )
	1. $f,g在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{平方可积}}}\quad \Rightarrow \quad fg在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{可积}}}+结论$
		- **结论**
			- $|\int^{\pi}_{- \pi}fgdx| \ \ \leq \ \  \int^{\pi}_{-\pi}|fg|dx \ \ \leq \ \  (\int^{\pi}_{-\pi}|f|^{2}dx)^{\frac{1}{2}}(\int^{\pi}_{-\pi}|g|^{2}dx)^{\frac{1}{2}}$
			- $Cauchy-Schwarz不等式$
	2. $f,g在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{平方可积}}}\quad \Rightarrow \quad f+g在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{平方可积}}}+结论$
		- **结论**
			- $(\int^{\pi}_{-\pi}|f+g|^{2}dx)^{\frac{1}{2}} \ \ \leq \ \ (\int^{\pi}_{-\pi}|f|^{2}dx)^{\frac{1}{2}} + (\int^{\pi}_{-\pi}|g|^{2})^{\frac{1}{2}}$
1. 定义(  [[n阶三角多项式]]  )
	- $T_{n}(x)=\frac{\alpha_{0}}{2}+\sum\limits_{k=1}^{n}(\alpha_{k}\cos kx + \beta_{k} \sin kx)$
		- $\alpha_{0}\ , \ \alpha_{k}\ , \ \beta_{k}(k=1\ , \ 2\ , \ \cdots \ , \ n)为\textcolor{pink}{\underline{\textbf{常数}}}$
1. 定理14.8
2. 定理14.9(  $Bessel不等式$  )
3. 引理1
4. 定理14.10
5. 定理14.11
	1. 推论1(  $Paseval等式$  )