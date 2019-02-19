# 손실 함수

$$\begin{gathered}
\mathcal{D}=\{x^i,y^i\}_{i=1}^k \\
\text{where }x^i\in\mathbb{R}^n\text{ and }y^i\in\mathbb{R}^m.
\end{gathered}$$

```python
x
```

$$\begin{gathered}
\hat{y}^1=f(x^1)\\
\hat{y}^2=f(x^2)\\
\vdots\\
\hat{y}^k=f(x^k)
\end{gathered}$$

```python
x
```

$$\begin{gathered}
(y^1,\hat{y}^1)\\
(y^2,\hat{y}^2)\\
\vdots\\
(y^k,\hat{y}^k)
\end{gathered}$$

$$\begin{gathered}
\begin{aligned}
\mathcal{L}(f)&=\frac{1}{k}\sum_{i=1}^k{|y^i-f(x^i)|}\\
&=\frac{1}{k}\sum_{i=1}^k{|y^i-\hat{y}^i|}\\
&=\frac{1}{k}\big(|y^1-\hat{y}^1|+\cdots+|y^k-\hat{y}^k|\big)\\
\end{aligned}\\
\text{where }y\in\mathbb{R}^m
\end{gathered}$$

$$\mathcal{L}(f)=\frac{1}{k}\sum_{i=1}^k{|y^i-\hat{y}^i|_2}$$

$$
|y^i-\hat{y}^i|=|y_1^i-\hat{y}_1^i|+|y_2^i-\hat{y}_2^i|+\cdots+|y_m^i-\hat{y}_m^i|
$$

```python
x
```

$$\begin{gathered}
\begin{aligned}
\mathcal{L}(f)&=\frac{1}{k}\sum_{i=1}^k{|y^i-\hat{y}^i|_2}\\
&=\text{MSE}(y,\hat{y})
\end{aligned}\\
\text{where }y\in\mathbb{R}^{k\times{m}}\text{ and }\hat{y}\in\mathbb{R}^{k\times{m}}.
\end{gathered}$$

```python
x
```
