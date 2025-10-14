#analisi 
> [!error] Teorema
> Se $\sum_{n=0}^{\infty} a_{n}$ converge, allora $\lim_{ n \to \infty }a_{n} = 0$

> [!error] Dimostrazione
> Sia $S_{N} = \sum_{n=0}^{N} a_{n}$ successione delle somme parziali di $a_{n}$. Per ipotesi $\exists S = \lim_{ N \to \infty } S_{N}\in \mathbb{R}$
> Osserviamo che $$S_{N} = \sum_{n=0}^{N} a_{n} = \sum_{n=0}^{N-1} a_{n} + a_{n} = S_{N-1} + a_{n}$$
> $$\implies a_{n} = S_{N} - S_{N-1} \forall\ N \geq 1$$
> Poiché $\lim_{ N \to \infty } [\dots]$

> [!info] Osservazione
> Se $\lim_{ n \to \infty }a_{n} = 0 \not\implies \sum_{n=0}^{\infty} a_{n}$ converge

> [!error] Controesempio
> $\sum_{n=1}^{\infty} \frac{1}{n}$ (serie armonica)
