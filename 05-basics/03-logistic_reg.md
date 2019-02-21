# 로지스틱 회귀

$$\begin{gathered}
\mathcal{D}=\{x^i,y^i\}_{i=1}^k \\
\text{where }x^i\in\mathbb{R}^n\text{ and }y^i\in\{0,1\}^m.
\end{gathered}$$

$$\begin{gathered}
\begin{aligned}
\hat{y}&=f(x) \\
&=\sigma(x\cdot{W}+b)
\end{aligned} \\
\text{where }x\in\mathbb{R}^{k\times{n}}\text{ and }\hat{y}\in\{0,1\}^{k\times{m}}. \\
\text{Thus, }W\in\mathbb{R}^{n\times{m}}\text{ and }b\in\mathbb{R}^{m}.
\end{gathered}$$

$$\begin{gathered}
\mathcal{L}(\theta)=-\frac{1}{k}\sum_{i=1}^k{y\cdot\log\hat{y}+(1-y)\cdot\log{(1-\hat{y})}} \\
\text{where }\theta=\{W,b\}.
\end{gathered}$$

$$\begin{gathered}
\theta\leftarrow\theta-\alpha\nabla_\theta\mathcal{L(\theta)}
\end{gathered}$$
