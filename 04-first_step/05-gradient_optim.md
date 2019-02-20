# 그래디언트 기반 최적화

$$\begin{gathered}
\begin{aligned}
\mathcal{L}(f)&=\text{MSE}(y,\hat{y})\\
&=\mathcal{L}(W,b)\\
&=\mathcal{L}(\theta)
\end{aligned}\\
\text{where }\theta=\{W,b\}.
\end{gathered}$$

$$\theta=\underset{\theta\in\Theta}{\text{argmin }}{\mathcal{L}(\theta)}$$

$$\begin{gathered}
\theta\leftarrow\theta-\alpha\nabla_\theta\mathcal{L}(\theta)\\
\text{where }\alpha\text{ is learning rate.}
\end{gathered}$$

$$\nabla_\theta\mathcal{L}(\theta)=\frac{\partial\mathcal{L}(\theta)}{\partial\theta}$$

$$\begin{gathered}
W\leftarrow{W}-\alpha\frac{\partial\mathcal{L}(\theta)}{\partial{W}} \\
b\leftarrow{b}-\alpha\frac{\partial\mathcal{L}(\theta)}{\partial{b}}
\end{gathered}$$

<!--
$$\begin{gathered}
\begin{aligned}
\frac{\partial\mathcal{L}(\theta)}{\partial{W}}&=\frac{\partial}{\partial{W}}\cdot\frac{1}{k}\sum_{i=1}^k{\big\|y^i-f(x^i)\big\|_2} \\
&=\frac{\partial}{\partial{W}}\cdot\frac{1}{k}\sum_{i=1}^k{\big(y^i-f(x^i)\big)\cdot\big(y^i-f(x^i)\big)^T} \\
&=\frac{\partial}{\partial{W}}\cdot\frac{1}{k}\sum_{i=1}^k{\big({y^i}\cdot{y^i}^T-f(x^i)\cdot{y^i}^T-{y^i}\cdot{f(x^i)}^T+f(x^i)\cdot{f(x^i)}^T\big)} \\
&=\frac{\partial}{\partial{W}}\cdot\frac{1}{k}\sum_{i=1}^k{\big({y^i}\cdot{y^i}^T-(x\cdot{W}+b)\cdot{y^i}^T-{y^i}\cdot{(x\cdot{W}+b)}^T+(x\cdot{W}+b)\cdot{(x\cdot{W}+b)}^T\big)} \\
&=\frac{\partial}{\partial{W}}\cdot\frac{1}{k}\sum_{i=1}^k{\big(-(x\cdot{W}+b)\cdot{y^i}^T-{y^i}\cdot{(x\cdot{W}+b)}^T+(x\cdot{W}+b)\cdot{(x\cdot{W}+b)}^T\big)} \\
&=\frac{\partial}{\partial{W}}\cdot\frac{1}{k}\sum_{i=1}^k{\big(-x\cdot{W}\cdot{y^i}^T-b\cdot{y^i}^T-{y^i}\cdot{x\cdot{W}}-{y^i}\cdot{b}^T+x\cdot{W}\cdot{W}^T\cdot{x}^T+b\cdot{W}^T\cdot{x}^T+x\cdot{W}\cdot{b}^T+b\cdot{b}^T\big)} \\
&=\frac{\partial}{\partial{W}}\cdot\frac{1}{k}\sum_{i=1}^k{\big(-x\cdot{W}\cdot{y^i}^T-{y^i}\cdot{x\cdot{W}}+x\cdot{W}\cdot{W}^T\cdot{x}^T+b\cdot{W}^T\cdot{x}^T+x\cdot{W}\cdot{b}^T\big)} \\
\end{aligned}\\
\text{, where }|x^i|=(1,n)\text{ and }|y^i|=(1,m).
\end{gathered}$$
-->