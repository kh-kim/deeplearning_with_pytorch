# 딥러닝이란

$$\begin{gathered}
h=\{h_0,h_1,h_2,\cdots,h_r\}\text{ and }|h|=r+1.\\
\\
\begin{aligned}
\hat{y}&=f(x) \\
&=f_{r}\circ{f_{r-1}}\circ\cdots\circ{f_1}(x)
\end{aligned} \\
\\
\text{where } \\
z_i=f_i(z_{i-1})=\sigma(z_{i-1}\cdot{W_i}+b_i) \\
\text{ and } \\
\hat{y}=z_r=f_r(z_{r-1}).
\end{gathered}$$
