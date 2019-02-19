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

$$\begin{gathered}
\begin{aligned}
\frac{\partial\mathcal{L}(\theta)}{\partial{W}}&=\frac{\partial}{\partial{W}}\cdot\frac{1}{k}\sum_{i=1}^k{\big|y^i-f(x^i)\big|_2} \\
&=\frac{\partial}{\partial{W}}\cdot\frac{1}{k}\sum_{i=1}^k{\big(y^i-f(x^i)\big)^2} \\
&=\frac{\partial}{\partial{W}}\cdot\frac{1}{k}\sum_{i=1}^k{\big({y^i}^2-2{y^i}\cdot{f(x^i)}+f(x^i)^2\big)} \\
&=\frac{\partial}{\partial{W}}\cdot\frac{1}{k}\sum_{i=1}^k{\big({y^i}^2-2{y^i}(x^i\cdot{W}+b)+(x^i\cdot{W}+b)^2\big)} \\
&=\frac{\partial}{\partial{W}}\cdot\frac{1}{k}\sum_{i=1}^k{\big({y^i}^2-2{y^i}x^i\cdot{W}+2y^i{b}+(x^i\cdot{W})^2+2x^i\cdot{W}\cdot{b}+b^2\big)} \\
&=\frac{\partial}{\partial{W}}\cdot\frac{1}{k}\sum_{i=1}^k{\big(-2{y^i}(x^i\cdot{W})+(x^i\cdot{W})^2+2(x^i\cdot{W})\cdot{b}\big)}
\end{aligned}\\
\text{, where }|x^i|=(1,n)\text{ and }|y^i|=(1,m).
\end{gathered}$$