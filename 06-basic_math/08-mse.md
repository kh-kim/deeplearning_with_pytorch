# MSE의 재해석

$$\mathcal{D}=\{x_i,y_i\}_{i=1}^N$$

$$\begin{gathered}
\begin{aligned}
\mathcal{L}(\theta)&=-\frac{1}{N}\sum_{i=1}^N{\log{f(x_i;\sigma,\theta)}} \\
&=-\frac{1}{N}\sum_{i=1}^N\log{\Bigg(\frac{1}{\sigma\sqrt{2\pi}}\exp{\bigg(-\frac{\big(x_i-\mu_\theta(x_i)\big)^2}{2\sigma^2}\bigg)}\Bigg)} \\
&=-\frac{1}{N}\sum_{i=1}^N{\Bigg(-\log{\sigma\sqrt{2\pi}}-\frac{\big(x_i-\mu_\theta(x_i)\big)^2}{2\sigma^2}\Bigg)}
\end{aligned} \\
\text{where }\hat{y_i}=\mu_\theta(x_i).
\end{gathered}$$

$$\begin{aligned}
\nabla_\theta\mathcal{L}(\theta)&=-\frac{1}{N}\sum_{i=1}^N{-\frac{1}{2\sigma^2}\cdot\nabla_\theta\Big(x_i-\mu_\theta(x_i)\Big)^2} \\
&=\frac{1}{N\cdot2\sigma^2}\sum_{i=1}^N{\nabla_\theta\Big(x_i-\mu_\theta(x_i)\Big)^2} \\
&\approx\frac{1}{N}\sum_{i=1}^N{\nabla_\theta\Big(x_i-\mu_\theta(x_i)\Big)^2}=\nabla_\theta\tilde{\mathcal{L}}(\theta)
\end{aligned}$$

$$\begin{aligned}
\tilde{\mathcal{L}}(\theta)&=\frac{1}{N}\sum_{i=1}^N{\Big(x_i-\mu_\theta(x_i)\Big)^2} \\
&=\text{MSE}\big(x_i,\mu_\theta(x_i)\big)_{i=1}^N
\end{aligned}$$
