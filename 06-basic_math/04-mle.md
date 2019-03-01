# 최대 가능도 추정 (Maximum Likelihood Estimation)

## Likelihood

$$K\sim\mathcal{B}(n,\theta)$$

$$\begin{aligned}
P(K=k;n,\theta)&=\begin{pmatrix}n \\ k\end{pmatrix}\cdot\theta^k(1-\theta)^{n-k} \\
&=\frac{n!}{k!\cdot(n-k)!}\cdot\theta^k(1-\theta)^{n-k}
\end{aligned}$$

$$\begin{gathered}
\mathcal{D}=\{0,0,1,0,\cdots\} \\
|\mathcal{D}|=n\text{ and }\text{sum}(\mathcal{D})=k.
\end{gathered}$$

$$f_\mathcal{D}(\theta)=P(\mathcal{D};\theta)=\frac{n!}{k!\cdot(n-k)!}\cdot\theta^k(1-\theta)^{n-k}$$

## MLE란

$$\begin{gathered}\hat{\theta}=\underset{\theta\in\Theta}{\text{argmax }}J(\theta)\\
\\
\theta\leftarrow\theta+\alpha\nabla_\theta{J(\theta)}, \\
\text{where }J(\theta)=\mathbb{E}_{\mathcal{D}\sim{P(\text{x})}}\big[P(\mathcal{D};\theta)\big].
\end{gathered}$$

### 일반화

$$J(\theta)=\mathbb{E}_{x\sim{P(\text{x})}}\big[P(x;\theta)\big]$$

$$\mathcal{D}=\{x_i,y_i\}_{i=1}^N$$

$$P(y|x;\theta)$$

$$J(\theta)=\mathbb{E}_{x\sim{P(\text{x})}}\Big[\mathbb{E}_{y\sim{P(\text{y}|x)}}\big[P(y|x;\theta)\big]\Big]$$

## Log-likelihood

$$\begin{gathered}
P(x_1,x_2,\cdots,x_i)\approx{P(x_1)P(x_2)\cdots{P(x_i)}} \\
\downarrow \\
\log{P(x_1,x_2,\cdots,x_i)}\approx{\log{P(x_1)}+\log{P(x_2)}+\cdots+\log{P(x_i)}}
\end{gathered}$$

$$\begin{gathered}
p(x;\theta)=\frac{1}{\sigma\sqrt{2\pi}}\exp{\Bigg(-\frac{(x-\mu)^2}{2\sigma^2}\Bigg)}, \\
\text{where }\theta=\{\mu,\sigma\}.
\end{gathered}$$

$$\log{p(x;\theta)}=-\log{\sigma\sqrt{2\pi}}-\frac{(x-\mu)^2}{2\sigma^2}$$

$$J(\theta)=\mathbb{E}_{x\sim{P(\text{x})}}\Big[\log{P(x;\theta)}\Big]$$

## Negative Log-likelihood

$$\begin{gathered}\hat{\theta}=\underset{\theta\in\Theta}{\text{argmin }}\mathcal{L}(\theta)\\
\\
\theta\leftarrow\theta-\alpha\nabla_\theta{\mathcal{L}(\theta)}, \\
\text{where }\mathcal{L}(\theta)=-\mathbb{E}_{\mathcal{D}\sim{P(\text{x})}}\big[\log{P(\mathcal{D};\theta)}\big].
\end{gathered}$$