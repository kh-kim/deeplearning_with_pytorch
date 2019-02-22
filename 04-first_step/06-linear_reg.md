# 선형 회귀

$$\begin{gathered}
\mathcal{D}=\{x^i,y^i\}_{i=1}^k \\
\text{where }x^i\in\mathbb{R}^n\text{ and }y^i\in\mathbb{R}^m.
\end{gathered}$$

```py
```

$$\begin{gathered}
\theta=\{W,b\} \\
\text{where }f(x)=x\cdot{W}+b.
\end{gathered}$$

```py
```

$$\begin{gathered}
\begin{aligned}
\mathcal{L}(\theta)&=\frac{1}{k}\sum_{i=1}^k{\|y^i-\hat{y}^i\|_2}\\
&=\text{MSE}(y,\hat{y})
\end{aligned}\\
\text{where }\hat{y}^i=f(x^i).
\end{gathered}$$

```py
```

$$\theta\leftarrow\theta-\alpha\nabla_\theta\mathcal{L}(\theta)$$

```py
```
