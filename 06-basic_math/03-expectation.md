# 샘플링과 기대값

## 샘플링

$$x\sim{P(\text{x})}$$

## 기대값

$$\begin{gathered}
\frac{1}{k}\sum_{i=1}^k{x_i}=\frac{x_1}{k}+\frac{x_2}{k}+\cdots+\frac{x_k}{k} \\
\text{where }x_1,x_2,\cdots,x_k\sim{P(\text{x})}.
\end{gathered}$$

$$\begin{gathered}
\mathbb{E}_{x\sim{P(\text{x})}}[x]
\end{gathered}$$

$$\begin{gathered}
\mathbb{E}_{x\sim{P(\text{x})}}[x]=\sum_{x\in\mathcal{X}}{x}\cdot{P(x)} \\
\\
\mathbb{E}_{x\sim{p(\text{x})}}\big[f(x)\big]=\int{p(x)\cdot{f(x)}}~dx
\end{gathered}$$

### 주사위 홀짝 도박 게임

$$f(x)=\begin{cases}
+100\text{, if }x\text{ is even.} \\
-100\text{, otherwise.}
\end{cases}$$

$$\begin{gathered}
\mathbb{E}_{x\sim{P(\text{x})}}\big[f(x)\big]=\sum_{x\in\mathcal{X}}{P(x)\cdot{f(x)}} \\
\text{where }\mathcal{X}=\{1,2,3,4,5,6\}.
\end{gathered}$$

However, if the dice is unfair?

$$\begin{gathered}
P(\text{x}=1)=P(\text{x}=2)=P(\text{x}=3)=\frac{2}{9}, \\
P(\text{x}=4)=P(\text{x}=5)=P(\text{x}=6)=\frac{1}{9}.
\end{gathered}$$

## 몬테카를로 샘플링

$$\begin{gathered}
\mathbb{E}_{\text{x}\sim{P(x)}}\big[f(x)\big]\approx\frac{1}{k}\sum_{i=1}^k{f(x_i)}
\end{gathered}$$
