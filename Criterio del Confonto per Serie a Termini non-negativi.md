#analisi #finire
> [!error] Teorema
> Date due successioni $a_{n}$ e $b_{n}$ tali che (definitivamente in $n \in \mathbb{N}$) sia $$0 \leq a_{n} \leq b_{n}\ \ \forall\ n$$ allora:
> 1. Se $\sum_{n=1}^{\infty} a_{n}$ diverge a $+\infty$, allora anche $\sum_{n=1}^{+\infty} b_{n}$ diverge a $+\infty$
> 2. Se $\sum_{n=1}^{+\infty} b_{n}$ converge, allora anche $\sum_{n=1}^{+\infty} a_{n}$ converge.
> Inoltre se $a_{n} \leq b_{n} \forall\ n \in \mathbb{N}$, allora $$0 \leq \sum_{n=1}^{+\infty} a_{n} \leq \sum_{n=1}^{+\infty} b_{n} \leq +\infty$$

> [!error] Dimostrazione
> Per semplicità supponiamo che $$0 \leq a_{n} \leq b_{n},\ \ \forall\ n \in \mathbb{N}$$
> consideriamo le somme parziali $$_{N} = \sum_{n=1}^{N} a_{n},\ \ \ \sigma_{N} = \sum_{n=1}^{N} b_{n}$$ Segue che $$0 \leq S_{N} \leq \sigma_{N}$$ Inoltre $s_{N}$, $\sigma_{N}$ sono monotone crescenti, quindi esistono $$S = \lim_{N \to \infty } S_{N},\ \ \ \sigma = \lim_{ N \to \infty } \sigma_{N} \in \mathbb{R} \cup \{  +\infty \}$$
> 1. Se $\sum_{n=1}^{\infty}a_{n}$ diverge, $$\sum_{n=1}^{\infty}a_{n} = \lim_{ N \to \infty } S_{N}= S = +\infty $$ Perché $S_{N} \leq \sigma_{N}, \forall\ N \in \mathbb{N}$, per il teorema del [[Confronto per Successioni Divergenti]] vale anche $$\lim_{ N \to \infty }  $$
> 2. Se $\sum_{n=1}^{\infty}b_{n}$ converge allora $$\sigma = \lim_{ N \to \infty } \sigma_{N} \in \mathbb{R}$$ Poiché $\sigma_{N}$ crescente, $\sigma = \mathrm{sup}\sigma_{N}$. Quindi $$S_{N} \leq \sigma_{N} \leq 0 \forall\ N \in \mathbb{N}$$ $$\implies S_{N} \text{}$$
> 3. Essendo $\sigma_{N} \geq S_{N} \forall\ N \in \mathbb{N}$ e poiché esistono $$S = \lim_{ N \to \infty } S_{N}, \sigma = \lim_{ N \to \infty } \sigma_{N}$$ vale per permanenza del segno $$S = \lim_{ N \to \infty } S_{N} \leq \lim_{ N \to \infty } \sigma_{N} = \sigma $$

## Esempi
- Serie geometrica: $$\sum_{n=1}^{\infty} q^n =
\begin{cases} \frac{1}{1-q}  & se  & 0 \leq q < 1 \\
+\infty  & se & q\geq_{1}
\end{cases}$$
- Serie armonica generalizzata, $\alpha \in \mathbb{R}$ $$\sum_{n=1}^{\infty} \frac{1}{n^\alpha} =
\begin{cases} \text{converge} & se & \alpha > 1 \\
\text{diverge}  &  se & a \leq 1
\end{cases}$$
- Serie armonica generalizzata II $$
\sum_{n=1}^{\infty} \frac{1}{n^\alpha(\log n)^\beta} = \begin{cases}
\text{converge} & se & \alpha > 1, \beta \in \mathbb{R}\ ||\ \alpha = 1, \beta > 1 \\
\text{diverge}  & se & \alpha < 1, \beta \in \mathbb{R}\ ||\ \alpha = 1, \beta \leq 1
\end{cases}
$$