# 피드 포워드 연산

$$\begin{gathered}
y=f(x) \\
\text{where }f:\mathbb{R}^{n}\rightarrow\mathbb{R}^{m}\text{, }x\in\mathbb{R}^n\text{ and }y\in\mathbb{R}^m.
\end{gathered}$$

$$\begin{gathered}
y=W\cdot{x}\\
\text{where }W\in\mathbb{R}^{m\times{n}}
\end{gathered}$$

$$\begin{gathered}
y={x}\cdot{W}\\
\text{where }x\in\mathbb{R}^{k\times{n}}\text{, }y\in\mathbb{R}^{k\times{m}}\text{, }W\in\mathbb{R}^{n\times{m}}\text{ and }k=\text{\#samples}.
\end{gathered}$$

$$\begin{gathered}
x\in\mathbb{R}^{k\times{n}}\longrightarrow|x|=(k,n)\\
y\in\mathbb{R}^{k\times{m}}\longrightarrow|y|=(k,m)\\
W\in\mathbb{R}^{n\times{m}}\longrightarrow|W|=(n,m)
\end{gathered}$$

```python
x
```

$$\begin{gathered}
y={x}\cdot{W}+b\\
\text{where }b\in\mathbb{R}^m.
\end{gathered}$$

$$b\in\mathbb{R}^m\longrightarrow|b|=(m,)$$

$$\begin{gathered}
y=[x;1]\cdot{W}\\
\text{where }W\in\mathbb{R}^{(n+1)\times{m}}.
\end{gathered}$$

```python
x
```