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
