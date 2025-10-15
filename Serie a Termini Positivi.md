#analisi 
> [!warning] Definizione
> Data una [[Serie]] $\sum_{n=1}^{\infty} a_{n}$, essa si dice a termini (definitivamente) positivi se $a_{n} \geq 0$ (definitivamente) in $n \in \mathbb{N}$

> [!error] Teorema
> Se la [[Serie]] è a termini (definitivamente) positivi allora essa converge o diverge a $+\infty$.

> [!error] Dimostrazione
> Essendo $a_{n}$ definitivamente positiva, $\exists n_{0} \in \mathbb{N}: \forall\ n \geq n_{0},\  a_{n} \geq 0$
> Allora $\forall\ N \geq n_{0}$ $$S_{N} = \sum_{n=1}^{N} a_{n} = \sum_{n=1}^{N-1} a_{n}  + a_{N} = S_{N-1} + a_{N} \geq S_{N-1}$$
> $$\implies S_{N} \text{è definitivamente crescente in } N \in \mathbb{N}$$
> Quindi per il teorema di esistenza del limite per successioni (definitivamente) monotone varrà $$\exists \lim_{ n \to \infty } S_{N} = S \in \mathbb{R} \cup \{ +\infty \}$$
> Cioè $\sum_{i=1}^{\infty} S_{N} = \lim_{ N \to \infty } S_{N} = S \in \mathbb{R} + \{ +\infty \}$
> e la serie converge (se $S \in \mathbb{R}$) o diverge a $+\infty$ (se $S = +\infty$)

## Criteri
- [[Criterio del Confonto per Serie a Termini non-negativi]]
- [[Criterio del Confronto Asintotico]]
- [[Criterio del Rapporto per Serie]]
- [[Criterio della Radice]]