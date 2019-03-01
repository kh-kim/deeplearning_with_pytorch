# 쿨러 라이블러 다이버전스

## Equation

$$\begin{aligned}\text{KL}(P||Q)&=-\mathbb{E}_{\text{x}\sim{P}}\bigg[\log{\frac{Q(x)}{P(x)}}\bigg] \\
&=-\sum_{x\in\mathcal{X}}P(x)\log{\frac{Q(x)}{P(x)}} \\
&=-\sum_{x\in\mathcal{X}}\Big(P(x)\log{Q(x)}-P(x)\log{P(x)}\Big)
\end{aligned}$$
