---
aliases:
  - Equazioni Lineari
---
#GAL 
> [!warning] Definizione
> Un'**Equazione Lineare** nelle variabili
> $x_{1},\ x_{2},\ \dots,\ x_{n} \in \mathbb{R}$ 
> è un'equazione del tipo:
> $a_{1}x_{1}+a_{2}x_{2}+\dots+a_{n}x_{n}=b$
> dove $\underbrace{a_{1},\ a_{2},\ \dots,\ a_{n}}\limits_{\text{coefficienti}},\ \underbrace{b}\limits_{\text{termine noto}} \in \mathbb{R}$ sono numeri fissati

> [!info] Osservazione
> $n=1 \implies$
> - 1 soluzione se $a \neq 0$
> - 0 soluzioni se $a = 0\ \land\ b \neq 0$
> - $\infty$ soluzioni se $a = 0\ \land\ b = 0$

> [!info] Osservazione
> $n=2 \implies$
> - $a_{1} \neq 0 \implies S=\{ \binom{-\frac{a_{2}}{a_{1}}t+\frac{b}{a_{1}}}{t}: t \in \mathbb{R} \} \subseteq \mathbb{R}^2$
> - $a_{1} = 0\ \land\ a \neq 0\implies S=\{ \binom{t}{\frac{b}{a_{2}}}:t\in \mathbb{R} \} \subseteq \mathbb{R}^2$
> - $a_{1}=a_{2}=0\ \land\ b\neq 0 \implies \overline{S} = 0$
> - $a_{1}=a_{2}=0\ \land\ b =0 \implies S=\mathbb{R}^2$

> [!info] Osservazione
> $n \geq 2 \implies$  
> - $a_{i} \neq 0 \implies \overline{S} = \infty$
> - $a_{1}=a_{2}=\dots=a_{n}=0$
> 	- $b\neq 0 \implies \overline{S}=0$
> 	- $b = 0 \implies \overline{S}=\infty$