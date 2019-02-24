# 소프트맥스 함수

$$\text{idx}=\underset{i\in\{1,2,\cdots,n\}}{\text{argmax}}(x)$$

$$\begin{gathered}
[0,0,0,1,0,0]\\
\text{if idx}=4\text{ and }n=6.
\end{gathered}$$

$$\text{softmax}_k(x)=\frac{e^{x_k}}{\sum_{i=1}^n{e^{x_i}}}$$

$$\begin{gathered}
\text{softmax}(x)=\Bigg[\frac{e^{x_0}}{\sum_{i=1}^n{e^{x_i}}};\cdots;\frac{e^{x_n}}{\sum_{i=1}^n{e^{x_i}}}\Bigg] \\
\text{where }x\in\mathbb{R}^n
\end{gathered}$$

## 결과를 확률 분포 관점에서 해석

$$\begin{gathered}
f_\theta(x)=\text{softmax}(z)=\hat{y}=\begin{bmatrix}\frac{e^{z_0}}{\sum_{i=1}^n{e^{z_i}}} \\
\frac{e^{z_0}}{\sum_{i=1}^n{e^{z_i}}} \\
\vdots \\
\frac{e^{z_0}}{\sum_{i=1}^n{e^{z_i}}}
\end{bmatrix} \\
\text{where }x\in\mathbb{R}^n\text{ and }z,y\in\mathbb{R}^m.
\end{gathered}$$

$$\begin{gathered}
\hat{y}=f_\theta(x)=P_\theta(\text{y}|x)
\end{gathered}$$