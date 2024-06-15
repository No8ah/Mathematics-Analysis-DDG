1. 定义(  [[三角级数]]  )
	- $\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}(a_{n}\cos nx + b_{n}\sin nx)$
		- $\textcolor{orange}{\underline{\textbf{每一项}}}都以2\pi为\textcolor{orange}{\underline{\textbf{周期}}}$
		- $用\textcolor{pink}{\underline{\textbf{上式}}}表示\textcolor{orange}{\underline{\textbf{所有}}}以2\pi为\textcolor{pink}{\underline{\textbf{周期}}}的函数 \quad (并不必然)$
# 一、三角级数与$Flourier$级数

1. 命题1(  $\forall \ \alpha \quad \Rightarrow \quad \int^{\alpha+T}_{\alpha}f(x)dx=\int^{T}_{0}f(x)dx$  ) #数分下/第十四章/重要求解方法 
	- **1个先决条件**
		1. $f(x)以T为\textcolor{orange}{\underline{\textbf{周期}}}$
	1. 定义(  [[三角函数系]]  )
		- $\{1\ , \ \cos x \ , \ \sin x \ , \  \cos 2x \ , \ \sin 2x \ , \ \cdots \ , \ \cos nx \ , \ \sin nx \ , \  \cdots\}$
1. 定理14.1(  $\forall \ \textcolor{orange}{\underline{\textbf{三角函数系}}}上的两个\textcolor{orange}{\underline{\textbf{不同函数}}}的\textcolor{pink}{\underline{\textbf{乘积}}} \quad \Rightarrow \quad 区间[-\pi, \pi]上的\textcolor{orange}{\underline{\textbf{积分}}}=0$  )
	1. $\int^{\pi}_{- \pi}\sin nxdx=0 \quad \int^{\pi}_{- \pi}\cos nx dx=0 \quad (\forall \ n \in \mathbb{N}_{+})$
	2. $\int^{\pi}_{- \pi}\sin mx \cos nx dx =0 \quad (\forall \ m,n \in \mathbb{N}_{+})$
	3. $\int^{\pi}_{- \pi}\sin mx \sin nx dx =0 \quad \int^{\pi}_{- \pi}\cos mx \cos nx=0 \quad (\forall \ m \neq n \in \mathbb{N}_{+})$
		- $\textcolor{pink}{\underline{\textbf{三角函数系}}}的\textcolor{orange}{\underline{\textbf{正交性}}}$
		- $可改为\textcolor{orange}{\underline{\textbf{任意区间长度}}}为2\pi的\textcolor{pink}{\underline{\textbf{区间}}}$
- 三角函数系的$\textcolor{orange}{\underline{\textbf{系数}}}$
	- $a_{n}=\frac{1}{\pi} \int^{\pi}_{-\pi}f(x) \cos nx dx \quad n=0\ , \ 1\ , \ 2\ , \ \cdots$ #数分下/第十四章/重要求解方法
	- $b_{n}=\frac{1}{\pi} \int^{\pi}_{-\pi}f(x)\sin nx dx \quad n=1\ , \ 2\ , \ \cdots$ #数分下/第十四章/重要求解方法 
- 定义(  [[f(x)在闭区间上绝对可积]]  )
	- $\int^{\pi}_{-\pi}|f(x)|dx <+ \infty$
- 定义(  [[f(x)的Flourier系数]]  )(  $周期为2\pi$  )
	- $a_{n}=\frac{1}{\pi} \int^{\pi}_{-\pi}f(x) \cos nx dx \quad n=0\ , \ 1\ , \ 2\ , \ \cdots$
	- $b_{n}=\frac{1}{\pi} \int^{\pi}_{-\pi}f(x) \sin nx dx \quad n=1\ , \ 2\ , \ \cdots$
	- 定义(  [[f(x)的Flourier级数]]  )(  $周期为2\pi$  ) #数分下/第十四章/重要定义 
		- $f(x) \ \ \sim \ \ \frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}(a_{n}\cos nx + b_{n} \sin nx)$
# 二、$Flourier$级数的收敛性
# 三、任意区间上的$Flourier$级数

1. 定义(  [[周期为2l的函数f(x)的Flourier级数]]  )
	- $f(x) \ \ \sim \ \ \frac{a_{0}}{2}+ \sum\limits_{n=1}^{\infty}(a_{n}\cos \frac{n \pi}{l}x+b_{n}\sin \frac{n \pi}{l}x)$  #数分下/第十四章/重要定义 
	- $\varphi(t) \ \ \sim \ \ \frac{a_{0}}{2} + \sum\limits_{n=1}^{\infty}(a_{n} \cos nt + b_{n} \sin nt)$
		- $a_{n}=\frac{1}{l}\int^{l}_{-l}f(x) \cos \frac{n \pi}{l} xdx \quad n=0\ , \ 1\ , \ 2\ , \ \cdots$ #数分下/第十四章/重要求解方法 
		- $a_{n}= \frac{1}{\pi}\int^{\pi}_{- \pi}f(\frac{l}{\pi}t)\cos ntdt \quad n=0\ , \ 1\ , \ 2\ , \ \cdots$
		- $b_{n}=\frac{1}{l}\int^{l}_{-l}f(x) \sin \frac{n \pi}{l}xdx \quad n=1\ , \ 2\ , \ 3\ , \ \cdots$ #数分下/第十四章/重要求解方法 
		- $b_{n}=\frac{1}{\pi}\int^{\pi}_{- \pi}f(\frac{l}{\pi}t)\sin nt dt \quad n=1\ , \ 2\ , \ 3\ , \ \cdots$
		- $\textbf{Key}$
			- $x=\frac{l}{\pi}t$
			- $\varphi(t)=f(\frac{l}{\pi}t)$
			- $f(x)以\textcolor{orange}{\underline{\textbf{2l}}}为周期$
	1. 定义(  [[偶延拓]]  ) #数分下/第十四章/重要定义
		- $F_{e}(x) \ \ \sim \ \ \frac{a_{0}}{2}+ \sum\limits_{n=1}^{\infty}a_{n} \cos \frac{n\pi}{l}x$
			- $\textcolor{orange}{\underline{\textbf{特别地}}}\ , \ 如果f在[0,l]上\textcolor{orange}{\underline{\textbf{逐段可微}}}\quad \Rightarrow \quad F_{e}(x)=\frac{a_{0}}{2}+ \sum\limits_{n=1}^{\infty}a_{n} \cos \frac{n\pi}{l}x$ #数分下/第十四章/注意点
			- $a_{n}=\frac{1}{l}\int^{l}_{-l}f(x) \cos \frac{n \pi}{l} xdx \quad n=0\ , \ 1\ , \ 2\ , \ \cdots$ #数分下/第十四章/注意点 
				- $\frac{1}{\pi} \rightarrow \frac{1}{l}$
				- $\int^{\pi}_{-\pi} \rightarrow \int^{l}_{-l}$
				- $\cos nx \rightarrow cos \frac{n \pi}{l}x$
	1. 定义(  [[奇延拓]]  ) #数分下/第十四章/重要定义 
		- $F_{e}(x) \ \ \sim \ \ \sum\limits_{n=1}^{\infty}b_{n}  \sin \frac{n\pi}{l}x$
			- $\textcolor{orange}{\underline{\textbf{特别地}}}\ , \ 如果f在[0,l]上\textcolor{orange}{\underline{\textbf{逐段可微}}}\quad \Rightarrow \quad F_{e}(x)=\sum\limits_{n=1}^{\infty}b_{n}cos \frac{n\pi}{l}x$ #数分下/第十四章/注意点 
			- $b_{n}=\frac{1}{l}\int^{l}_{-l}f(x) \sin \frac{n \pi}{l}xdx \quad n=1\ , \ 2\ , \ 3\ , \ \cdots$ #数分下/第十四章/注意点 
				- $\frac{1}{\pi} \rightarrow \frac{1}{l}$
				- $\int^{\pi}_{-\pi} \rightarrow \int^{l}_{-l}$
				- $\sin nx \rightarrow \sin \frac{n \pi}{l}x$
# 四、$Flourier$级数的平均收敛性质

1. 定义(  [[平方可积]]  )
	- $\int^{\pi}_{-\pi}|f(x)|^{2}dx \textcolor{orange}{\underline{\textbf{存在}}}$
2. 断言(  $f在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{平方可积}}}\quad \Rightarrow \quad f在[-\pi,\pi]上\textcolor{red}{\underline{\textbf{绝对可积}}}$  )
	1. 断言(  $2个条件\quad \Rightarrow \quad f(x) \sim \frac{a_{0}}{2}+ \sum\limits_{n=1}^{\infty}(a_{n}\cos nx +b_{n} \sin nx)$  )
		- **2个条件**
			1. $f以2\pi为\textcolor{orange}{\underline{\textbf{周期}}}$
			2. $f在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{平方可积}}}$

> [!error]+ **衔接**
> $$为了回答\lim\limits_{n \rightarrow \infty}(\frac{1}{2 \pi}\int^{\pi}_{-\pi}|f(x)-S_{n}(x)|^{2}dx)^{\frac{1}{2}}=0 是否成立?$$
> $$\quad \Downarrow \quad $$
> $$\textcolor{orange}{\underline{\textbf{平方可积}}}的\textcolor{pink}{\underline{\textbf{2条性质}}}$$


1. [[平方可积]]的性质
	1. **性质1**(  $f(x)\ , \ g(x)在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{平方可积}}}\quad \Rightarrow \quad f(x)g(x)在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{可积}}}+结论$  )
		- **结论**
			- $|\int^{\pi}_{- \pi}f(x)g(x)dx| \ \ \leq \ \  \int^{\pi}_{-\pi}|f(x)g(x)|dx \ \ \leq \ \  (\int^{\pi}_{-\pi}|f(x)|^{2}dx)^{\frac{1}{2}}(\int^{\pi}_{-\pi}|g(x)|^{2}dx)^{\frac{1}{2}}$
			- $Cauchy-Schwarz不等式$
	3. **性质2**(  $f(x)\ , \ g(x)在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{平方可积}}}\quad \Rightarrow \quad f(x)+g(x)在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{可积}}}+结论$  )
		- **结论**
			- $(\int^{\pi}_{-\pi}|f(x)+g(x)|^{2}dx)^{\frac{1}{2}} \ \ \leq \ \ (\int^{\pi}_{-\pi}|f(x)|^{2}dx)^{\frac{1}{2}} + (\int^{\pi}_{-\pi}|g(x)|^{2})^{\frac{1}{2}}$
3. 定义(  [[n阶三角多项式]]  )
	- $T_{n}(x)=\frac{\alpha_{0}}{2}+\sum\limits_{k=1}^{n}(\alpha_{k}\cos kx + \beta_{k} \sin kx)$
		- $\alpha_{0}\ , \ \alpha_{k}\ , \ \beta_{k}(k=1\ , \ 2\ , \ \cdots \ , \ n)为\textcolor{pink}{\underline{\textbf{常数}}}$

>[!error] **衔接**
> $$我们利用T_{n}(x)\textcolor{orange}{\underline{\textbf{逼近}}}f(x)$$
> $$\quad \Downarrow \quad $$
> $$如何使\textcolor{pink}{\underline{\textbf{误差}}}\textcolor{orange}{\underline{\textbf{最小}}}?$$
> $$\quad \Updownarrow \quad$$
> $$\textcolor{orange}{\underline{\textbf{均方误差}}}\triangle_{n}=(\frac{1}{2 \pi}\int^{\pi}_{- \pi}|f(x)-T_{n}(x)|^{2}dx)^{\frac{1}{2}}何时最小?$$
> $$\quad \Updownarrow \quad$$
> $$\alpha_{0}\ , \ \alpha_{k} \ , \ \beta_{k}(k=1\ , \ 2\ , \ \cdots \ , \ n)\textcolor{pink}{\underline{\textbf{怎么取}}}\quad S.t. \quad \triangle_{n}\textcolor{red}{\underline{\textbf{最小}}}?$$


1. 定理14.8(  $2个条件\quad \Rightarrow \quad 1个结论$  )
	- **2个条件**
		1. $f(x)以2\pi为\textcolor{pink}{\underline{\textbf{周期}}}$
		2. $f(x)在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{平方可积}}}$
	- **1个结论**
		1. $all\ of \  \textcolor{orange}{\underline{\textbf{n阶三角多项式}}}T_{n}(x)中 \ , \ T_{n}(x)取f(x)的\textcolor{orange}{\underline{\textbf{Flourier级数}}}的\textcolor{orange}{\underline{\textbf{n阶部分和}}}S_{n}(x)时\ , \ f(x)与T_{n}(x)的\textcolor{orange}{\underline{\textbf{均方误差}}}\textcolor{red}{\underline{\textbf{最小}}}$

>[!error]+ **衔接**
>$$于是: \quad 只要T_{n}(x)取f(x)的\textcolor{pink}{\underline{\textbf{Flourier级数}}}的\textcolor{orange}{\underline{\textbf{n阶部分和}}}S_{n}(x)时 \ , \ \triangle_{n}\textcolor{red}{\underline{\textbf{最小}}}$$
>$$\quad \Updownarrow \quad$$
>$$\alpha_{k}=a_{k} \quad k=0 \ , \ 1\ , \ \cdots \ , \ n$$
>$$\beta_{k}=b_{k} \quad k=1\ , \ 2\ , \ \cdots \ , \ n$$
1. 定理14.9(  $2个条件\quad \Rightarrow \quad f(x)的Flourier系数a_{k}\ , \ b_{k}满足结论$  )
	- **2个条件**
		1. $f(x)以2\pi为\textcolor{pink}{\underline{\textbf{周期}}}$
		2. $f(x)在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{平方可积}}}$
	- **结论**
		- $\frac{a_{0}^{2}}{2}+\sum\limits_{k=1}^{\infty}(a^{2}_{k}+b^{2}_{k}) \leq \frac{1}{\pi}\int^{\pi}_{-\pi}|f(x)|^{2}dx$

> [!error]+ **衔接**
> $$到底什么时候\lim\limits_{n \rightarrow \infty}(\frac{1}{2 \pi}\int^{\pi}_{-\pi}|f(x)-S_{n}(x)|^{2}dx)^{\frac{1}{2}}=0 才成立呢?$$
> $$\quad \Downarrow \quad $$
> $$利用上面进行分析并且回答该问题$$
1. 引理1(  $1个条件 \quad \Rightarrow \quad 2个结论$  )
	- **1个条件**
		1. $f(x) \in \mathbb{R}[a,b]$
	- **2个结论**
		1. $\forall \ \xi>0 \ , \ \exists \ \textcolor{orange}{\underline{\textbf{连续函数}}}g(x)(x \in [a,b]) \quad S.t. \quad \int^{b}_{a}|f(x)-g(x)|^{2}dx <\xi$
		2. $g(a)=f(a) \quad 且 \quad g(b)=f(b)$
2. 定理14.10(  $2个条件\quad \Rightarrow \quad 1个结论$  )
	- **2个条件**
		1. $f(x)以2 \pi为\textcolor{pink}{\underline{\textbf{周期}}}$
		2. $f(x)在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{平方可积}}}$
	- **1个结论**
		1. $\forall \ \xi>0 \ , \ \exists \ \textcolor{orange}{\underline{\textbf{三角多项式}}}T(x) \quad S.t. \quad (\frac{1}{2\pi}\int^{\pi}_{-\pi}|f(x)-T(x)|)^{\frac{1}{2}}<\xi$
3. 定理14.11(  $2个条件\quad \Rightarrow \quad 1个结论$  )
	- **2个条件**
		1. $f(x)以2 \pi为\textcolor{pink}{\underline{\textbf{周期}}}$
		2. $f(x)在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{平方可积}}}$
	- **1个结论**
		1. $S_{n}(x)在[-\pi,\pi]上\textcolor{orange}{\underline{\textbf{平均收敛}}}到f(x)$
			- $即 \quad \lim\limits_{n \rightarrow \infty}(\frac{1}{2\pi}\int^{\pi}_{-\pi}|f(x)-S_{n}(x)|^{2}dx)^{\frac{1}{2}}=0$
				- $S_{n}(x)  \ \  \overset{\triangle}{=} \ \ f(x)的\textcolor{orange}{\underline{\textbf{Flourier级数}}}的\textcolor{orange}{\underline{\textbf{部分和}}}$
	- **推论**
		- $\frac{a_{0}^{2}}{2}+\sum\limits_{k=1}^{\infty}(a^{2}_{k}+b^{2}_{k})=\frac{1}{\pi}\int^{\pi}_{-\pi}|f(x)|^{2}dx$
			- $Paseval等式$

>[!attention]+ **总结**
>$$\textcolor{orange}{\underline{\textbf{定理14.11}}}回答了上述问题$$
>$$\quad \Updownarrow \quad$$
>$$\lim\limits_{n \rightarrow \infty}(\frac{1}{2 \pi}\int^{\pi}_{-\pi}|f(x)-S_{n}(x)|^{2}dx)^{\frac{1}{2}}=0 \quad when \quad \textcolor{orange}{\underline{\textbf{定理14.11}}}成立$$