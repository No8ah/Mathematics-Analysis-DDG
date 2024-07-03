# 问题

$$讨论\quad \int^{+\infty}_{2} \frac{dx}{x^{\alpha} \ln x} \quad 的\textcolor{orange}{\underline{\textbf{收敛性}}} \quad \alpha \in \mathbb{R}$$
# 求解

## 处理

因为

$$\lim\limits_{x \rightarrow +\infty} \frac{1}{x^{\alpha} \ln x} \cdot x^{p} = \lim\limits_{x \rightarrow +\infty} \frac{x^{p-\alpha}}{\ln x}=\left\{\begin{matrix}
 0 \quad p  \leqslant \alpha \\
 +\infty \quad p > \alpha
 \end{matrix}\right.$$

## 讨论

### $p>1$

因为

$$\int^{+\infty}_{2 } \frac{dx }{x^{p}}\quad \textcolor{red}{\underline{\textbf{收敛}}}$$
$$\quad \Downarrow \quad $$
$$1 <p  \leqslant \alpha $$
$$\quad \Updownarrow \quad$$
$$\alpha >1$$
$$\quad \Downarrow \quad $$
$$\int^{+\infty}_{2} \frac{dx }{x^{\alpha}\ln x} \quad \textcolor{red}{\underline{\textbf{收敛}}}$$

### $p=1$

$$\int^{+\infty}_{2} \frac{dx}{x^{\alpha} \ln x}$$
$$\quad \Downarrow \quad $$
$$\int^{+\infty}_{2} \frac{dx}{x \cdot \ln x} = \int^{+\infty}_{2} \frac{d \ln x}{\ln x} = \ln \ln x  \ | \ ^{+\infty}_{2}= +\infty - \ln \ln 2$$
$$\quad \Downarrow \quad $$
$$\int^{+\infty}_{2} \frac{dx}{x^{\alpha}\ln x}\quad \textcolor{orange}{\underline{\textbf{发散}}}$$
$$\quad \Updownarrow \quad$$
$$\alpha =1 $$
$$\quad \Downarrow \quad $$
$$\int^{+\infty}_{2} \frac{dx}{x^{\alpha}\ln x} \quad \textcolor{orange}{\underline{\textbf{发散}}}$$
### $p<1$

因为
$$\int^{+\infty}_{2} \frac{dx}{x^{p}}\quad \textcolor{orange}{\underline{\textbf{发散}}}$$
$$\quad \Downarrow \quad $$

$$\int^{+\infty}_{2} \frac{dx}{x^{\alpha}\ln x} \quad \textcolor{orange}{\underline{\textbf{发散}}}$$
$$\quad \Updownarrow \quad$$
$$\alpha<p<1$$
$$\quad \Downarrow \quad $$
$$\alpha <1$$
$$\quad \Downarrow \quad $$
$$\int^{+\infty}_{2} \frac{dx}{x^{\alpha}\ln x} \quad \textcolor{orange}{\underline{\textbf{发散}}}$$

### 综上

$$\left\{\begin{matrix}
 \alpha>1 \quad \textcolor{red}{\underline{\textbf{收敛}}}\\
 \alpha\leqslant 1 \quad \textcolor{orange}{\underline{\textbf{发散}}}
\end{matrix}\right. \qquad QED\ !$$