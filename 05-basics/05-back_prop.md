# 역전파 알고리즘

$$\begin{gathered}
y=f\circ{g}(x) \\
\text{where }z=g(x).
\end{gathered}$$

$$\begin{gathered}
f(x)=x\cdot{W_f}+b_f \\
g(x)=x\cdot{W_g}+b_g \\
\theta=\{W_f,b_f,W_g,b_g\}
\end{gathered}$$

$$\frac{\partial\mathcal{L}(\theta)}{\partial{W_g}}$$

$$\frac{\partial\mathcal{L}(\theta)}{\partial{W_g}}=\frac{\partial\mathcal{L}(\theta)}{\partial{z}}\cdot\frac{\partial{z}}{\partial{W_g}}$$
