$$\begin{eqnarray}
条件: \quad
&①& \quad f(x)以 2 \pi 为 \textcolor{pink}{\underline{\textbf{周期}}} \\
&②& \quad f(x) 在[-\pi \ , \ \pi]上\textcolor{orange}{\underline{\textbf{绝对可积}}}
\end{eqnarray}$$
$$S_{n}(f;x)= \frac{1}{\pi} \int^{\pi}_{-\pi}f(u) \cdot \frac{\sin\left(n+ \frac{1}{2}\right) \cdot \frac{(u-x)}{2}}{\sin \frac{u-x}{2}}du$$$$S_{n}(f;x) \ \  \overset{\triangle}{=} \ \  f(x)的\textcolor{orange}{\underline{\textbf{Dirichlet积分}}}$$
##### 引入过程 :

设

$$f(x) \sim \frac{a_{0}}{2} + \sum\limits_{n=1}^{\infty} (a_{n} \cos nx
+ b_{n} \sin nx)$$
记右式前n项部分和

$$S_{n}(x)=S_{n}(f;x)= \frac{a_{0}}{2} + \sum\limits_{k=1}^{n}(a_{k} cos 
 kx + b_{n} \sin nx)$$
$Flourier$系数

$$a_{k}= \frac{1}{\pi} \int^{\pi}_{-\pi}f(x) \cos kxdx \quad k=0 \ , \ 1 \ , \ 2 \ , \ \cdots$$
$$b_{k}= \frac{1}{\pi} \int^{\pi}_{-\pi} f(x) \sin kx dx \quad k= 1 \ , \ 2 \ , \  \cdots $$\
代入得

$$\tag{1}S_{n}(f;x)= \frac{1}{\pi} \int^{\pi}_{-\pi}f(u)[ \frac{1}{2} + \sum\limits_{k=1}^{n}\cos k(u-x)]du$$
利用$\textcolor{pink}{\underline{\textbf{恒等式}}}$
$$\frac{1}{2} + \sum\limits_{k=1}^{n}\cos kt = \frac{\sin(n+ \frac{1}{2})t}{2\sin \frac{t}{2}}\tag{核心手法}$$
代入到(1)得

$$S_{n}(f;x)= \frac{1}{\pi} \int^{\pi}_{-\pi}f(u) \frac{\sin(n+ \frac{1}{2})(u-x)}{2\sin \frac{u-x}{2}}du$$
$$\quad \Updownarrow \quad$$
$$S_{n}(f;x)= \frac{1}{\pi} \int^{\pi}_{-\pi}f(u) \cdot \frac{\sin\left(n+ \frac{1}{2}\right) \cdot \frac{(u-x)}{2}}{\sin \frac{u-x}{2}}du$$
因此 , 定义$\textcolor{orange}{\underline{\textbf{f(x)的Dirichlet积分}}}$
$$S_{n}(f;x) \ \  \overset{\triangle}{=} \ \ \textcolor{orange}{\underline{\textbf{f(x)的Dirichlet积分}}}$$


##### 第一次处理 :

根据[[Dirichlet核]]中的"换元"

$$t= \frac{u-x}{2}$$
$$\quad \Downarrow \quad $$
$$dt=du$$
$t = \pi时$
$$t= \frac{\pi-x}{2}$$
$t=-\pi时$
$$t=\frac{-\pi-x}{2}$$
代入$f(x)的Dirichlet$积分得

$$S_{n}(f;x)= \frac{1}{\pi} \int^{\pi}_{-\pi}f(x+t) \cdot D_{n}(t)dt$$
$\textcolor{pink}{\underline{\textbf{对区间继续拆解}}}$ , 得

$$\tag{1}\frac{1}{\pi} \int^{\pi}_{0}f(x+t) \cdot D_{n}(t) dt$$
$$和$$
$$\tag{2}\frac{1}{\pi} \int^{0}_{-\pi}f(x+t) \cdot D_{n}(t)dt$$


换元

$$\tag{核心手法}令t=-t$$
代入(2)得

$$\tag{3}\frac{1}{\pi} \int^{0}_{-\pi} f(x-t) \cdot D_{n}(-t) d(-t)$$
由于$Dirichlet$核的性质得

$$D_{n}(t)=D_{n}(-t)$$

代入(3)得

$$\tag{4}\frac{1}{\pi} \int^{\pi}_{0}f(x-t) \cdot D_{n}(t)dt$$
合并(1)(4)得

$$S_{n}(f;x)=\frac{1}{\pi} \int^{\pi}_{-\pi}[f(x+t)+f(x-t)] \cdot D_{n}(t)dt$$

##### 第二次处理

根据$f(x)的Dirichlet积分和Dirichlet核$的性质得

$$\tag{1}1= \frac{1}{\pi} \int^{\pi}_{-\pi}D_{n}(t)dt$$
同乘$S$得

$$\tag{2}S= \frac{S}{\pi} \int^{\pi}_{-\pi}D_{n}(t)dt$$
根据"第一次处理"的结果

$$S_{n}(f;x)=\frac{1}{\pi} \int^{\pi}_{-\pi}[f(x+t)+f(x-t)] \cdot D_{n}(t)dt$$
令$x=x_{0}$代入得
$$\tag{3}S_{n}(f;x_{0})= \frac{1}{\pi} \int^{\pi}_{-\pi}[f(x_{0}+t)+f(x_{0}-t)] \cdot D_{n}(t)dt$$
令(3)-(2)得
$$\tag{4}S_{n}(f;x_{0})-S= \frac{1}{\pi} \int^{\pi}_{0}[f(x_{0}+t)+f(x_{0}-t)-2S] \cdot D_{n}(t)dt$$
换元
$$\varphi_{x_{0}}(t)=f(x_{0}+t)+f(x_{0}-t)-2S$$
代入(4)得

$$S_{n}(f;x_{0})-S = \frac{1}{\pi} \int^{\pi}_{0}\varphi_{x_{0}} \cdot D_{n}(t)dt$$

##### 对处理结果进行观察

对于 $\varphi_{x_{0}}$

$$\varphi_{x_{0}}=f(x_{0}+t)+f(x_{0}-t)-2S$$
$①\quad if \quad f(x)在x_{0}点\textcolor{orange}{\underline{\textbf{连续}}}$

$$f(x_{0})= \lim\limits_{x \rightarrow x_{0}}f(x)$$
只需要
$$\tag{核心手法}令S=f(x_{0})$$
$② \quad if \quad f(x)在x_{0}点\textcolor{orange}{\underline{\textbf{不连续}}}$

但是

$$f(x_{0}-0)和f(x_{0}+0)存在$$
$$\quad \Updownarrow \quad$$
$$x_{0}是\textcolor{pink}{\underline{\textbf{第一类间断点}}}$$
$$\quad \Updownarrow \quad$$
$$\textcolor{pink}{\underline{\textbf{可去间断点}}}或\textcolor{pink}{\underline{\textbf{跳跃间断点}}}$$
只需要
$$\tag{核心手法}令S= \frac{f(x_{0}+0)+f(x_{0}-0)}{2}$$

此时

$$令t \rightarrow 0^{+}$$

那么“第二次处理”的结果就化为

$$\frac{1}{\pi} \int^{\delta}_{0}\varphi_{x_{0}} \cdot D_{n}(t)dt$$
$$和$$
$$\frac{1}{\pi} \int^{\pi}_{\delta}\varphi_{x_{0}} \cdot D_{n}(t)dt$$
###### 理由

$$D_{n}(t) = \frac{\sin \left(n+ \frac{1}{2}\right) \cdot \frac{t}{2}}{\sin \frac{t}{2}}$$
$if \quad t \rightarrow 0^{+}$

$$D_{n}(t)\textcolor{orange}{\underline{\textbf{无意义}}}$$
因此

$$需要拆解区间$$
$$\quad \Updownarrow \quad$$
$$[0\ , \ \delta ] \quad 和 \quad[ \delta \ , \ \pi]$$