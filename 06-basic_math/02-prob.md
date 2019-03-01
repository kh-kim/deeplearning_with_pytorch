# 확률과 확률 분포

$$P(\text{x}=x)$$

## Discrete Variables

$$\begin{gathered}
\sum_{i=1}^N{P(\text{x}=x_i)=\sum_{i=1}^N{P(x_i)=1}}
\end{gathered}$$

## Continuous Variables

$$\begin{gathered}
\forall{x}\in\text{x}\text{, }p(x)\ge{0}. \\
\text{We don't require that }p(x)\le{1}. \\
\\
\int_{-\infty}^{\infty}{p(x)}~dx=1
\end{gathered}$$

## Distribution Function

$$\begin{gathered}
f(x)=P(\text{x}=x) \\
\\
y=\int_{-k}^{k}{f(x)}~dx
\end{gathered}$$

### Binomial Distribution

$$\begin{aligned}
f(k,n,\theta)=P(K=k;n,\theta)&=\begin{pmatrix}n \\ k\end{pmatrix}\cdot\theta^k(1-\theta)^{n-k} \\
&=\frac{n!}{k!\cdot(n-k)!}\cdot\theta^k(1-\theta)^{n-k}
\end{aligned}$$

### Gaussian Distribution

$$\begin{gathered}
f(x,\theta)=p(x;\theta)=\frac{1}{\sigma\sqrt{2\pi}}\exp{\Bigg(-\frac{(x-\mu)^2}{2\sigma^2}\Bigg)}, \\
\text{where }\theta=\{\mu,\sigma\}.
\end{gathered}$$

## Joint Distribution

$$\begin{gathered}
P(\text{x},\text{y})
\end{gathered}$$

### Marginal Distribution

$$\begin{gathered}
P(x)=\sum_{y\in\mathcal{Y}}{P(\text{x}=x,\text{y}=y)} \\
\\
p(x)=\int{p(x,y)}~dy
\end{gathered}$$

### Independant

$$\begin{gathered}
P(x,y)=P(x)P(y)\text{, }\forall{x, y}
\end{gathered}$$

$$\begin{gathered}
\frac{P(x,y)}{P(x)P(y)}=1\text{, }\forall{x, y}
\end{gathered}$$

## Conditional Distribution

$$\begin{gathered}
P(y|x)=\frac{P(x,y)}{P(x)}
\end{gathered}$$

$$\begin{aligned}
P(y|x)&=\frac{P(x,y)}{P(x)} \\
&=\frac{P(x)P(y)}{P(x)} \\
&=P(y)
\end{aligned}$$

$$\begin{aligned}
\int{P(y|x)}~dx&=\int{\frac{P(x,y)}{P(x)}}~dx \\
&=P(y)
\end{aligned}$$

$$\begin{gathered}
P(x,y)=P(y|x)P(x) \\
\\
\begin{aligned}
\int{P(x,y)}~dx&=\int{P(y|x)P(x)}~dx \\
&=\int{P(x|y)P(y)}~dx \\
&=P(y)
\end{aligned}
\end{gathered}$$

## Bayes Theorem

$$\begin{gathered}
P(y|x)=\frac{P(x|y)P(y)}{P(x)}
\end{gathered}$$
