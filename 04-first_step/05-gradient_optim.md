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