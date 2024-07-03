###### 证明

$$x^{n}在(-1,1)上\textcolor{orange}{\underline{\textbf{不一致收敛}}}到0$$
###### Proof

$$\textcolor{pink}{\underline{\textbf{函数序列}}}\textcolor{red}{\underline{\textbf{一致收敛}}}的\xi-N语言$$
$$\quad \Updownarrow \quad$$$$\forall \ \xi>0 \ , \ \exists \ N=N(\xi) \quad S.t. \quad \forall \ n >N  \ , \ \forall \ x \in X$$
$$有\quad  \ | x^{n}-0| \ <\xi$$
$$\quad \Downarrow \quad $$
$$\exists \ \xi_{0} >0 \ , \ \forall \ N \ , \ \exists \ n_{0}>N \ , \  \exists \ x_{0} \in X$$
$$\quad S.t. \quad  \ | \  x_{0}^{n_{0}} -0 \ | \  \geqslant \xi_{0}$$
$$\quad \Updownarrow \quad$$
$$\textcolor{pink}{\underline{\textbf{函数序列}}}\textcolor{red}{\underline{\textbf{不一致收敛}}}的\xi-N语言$$
只需令

$$n_{0}= N+1$$
$$\tag{核心手法}x_{0}= \sqrt[n_{0}]{\frac{1}{2}} = \left(\frac{1}{2}\right)^{n_{0}} \in (-1,1) $$
$$\quad \Downarrow \quad $$
$$x_{0}^{n_{0}} = \left(\left(\frac{1}{2}\right)^{\frac{1}{n_{0}}}\right)^{n_{0}} = \frac{1}{2} = \xi_{0}$$
$$\quad \Downarrow \quad $$
因此
$$\exists \ \xi_{0}=\frac{1}{2} \ , \ \forall \ N \ , \ \exists \ n_{0}=N+1>N \ , \ \exists \ x_{0}= \sqrt[n_{0}]{\frac{1}{2}} \in X=(-1,1)$$
$$\quad S.t. \quad |x_{0}^{n_{0}}-0 \ | \ = \frac{1}{2}  \geqslant \xi_{0} = \frac{1}{2}$$
$$\quad \Updownarrow \quad$$
$$x^{n}在(-1,1)上\textcolor{orange}{\underline{\textbf{不一致收敛}}}到0 \qquad QED\ !$$