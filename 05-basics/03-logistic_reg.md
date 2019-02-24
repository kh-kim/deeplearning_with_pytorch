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

## 확률 관점에서 결과를 해석하기

$$\begin{gathered}
y=\begin{bmatrix}
y_1 \\
y_2 \\
y_3
\end{bmatrix}=\begin{bmatrix}
1 \\
1 \\
0
\end{bmatrix}\text{, }
\hat{y}=\begin{bmatrix}
.4 \\
.7 \\
.2
\end{bmatrix}
\end{gathered}$$

$$\begin{gathered}
\begin{aligned}
f_\theta(x_i)=\hat{y}_i&=P_\theta(\text{y}_i=1) \\
&=1-P_\theta(\text{y}_i=0)
\end{aligned}
\end{gathered}$$

## Precision

## Recall
