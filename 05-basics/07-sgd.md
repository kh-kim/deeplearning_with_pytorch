# 스토캐스틱 그래디언트 디센트

$$\begin{gathered}
\mathcal{D}=\{x^i,y^i\}_{i=1}^k \\
\text{where }x^i\in\mathbb{R}^n\text{ and }y^i\in\mathbb{R}^m. \\
\downarrow\\
\text{batchify}\\
\downarrow\\
\begin{aligned}
\tilde{\mathcal{D}}&=\{(x^{1:b+1},y^{1:b+1}),(x^{b+1:2b+1},y^{b+1:2b+1}),\cdots\} \\
&=\{(\tilde{x}^1,\tilde{y}^1),(\tilde{x}^2,\tilde{y}^2)\cdots\}
\end{aligned} \\
\text{where }\tilde{x}^i\in\mathbb{R}^{b\times{n}}\text{ and }\tilde{y}^i\in\mathbb{R}^{b\times{m}}.
\end{gathered}$$

$$\begin{gathered}
\theta\leftarrow\theta-\alpha\nabla_\theta\frac{1}{b}\sum_{x\in\tilde{x},y\in\tilde{y}}\mathcal{L(x,y,\theta)}, \\
\forall(\tilde{x},\tilde{y})\in\tilde{\mathcal{D}}.
\end{gathered}$$
