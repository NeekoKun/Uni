#analisi 
> [!error] Teorema
> $\sum_{n=0}^{\infty} a_{n}$ converge $\implies \lim_{ n \to \infty }a_{n} = 0$

> [!error] Dimostrazione
> Sia $S_{N} = \sum_{n=0}^{N} a_{n}$ successione delle somme parziali di $a_{n}$. Per ipotesi $\exists S = \lim_{ N \to \infty } S_{N}\in \mathbb{R}$
> Osserviamo che $$S_{N} = \sum_{n=0}^{N} a_{n} = \sum_{n=0}^{N-1} a_{n} + a_{n} = S_{N-1} + a_{n}$$
> $$\implies a_{n} = S_{N} - S_{N-1} \forall\ N \geq 1$$
> Poiché $\lim_{ N \to \infty } [\dots]$

> [!info] Osservazione
> Se $\lim_{ n \to \infty }a_{n} = 0 \not\implies \sum_{n=0}^{\infty} a_{n}$ converge

> [!error] Controesempio
> $\sum_{n=1}^{\infty} \frac{1}{n}$ (serie armonica)
> $\lim_{ n \to \infty }a_{n} = \lim_{ n \to \infty } \frac{1}{n} = 0$ ovvio
> Osserviamo che $\forall\ n \geq 1$ vale $$\frac{1}{n} > \log\left( 1 + \frac{1}{n} \right)$$
> Infatti $$e = \lim_{ n \to \infty } \left( 1 + \frac{1}{n} \right)^n = \mathrm{sup}\left( 1 + \frac{1}{n} \right)^n$$
> $$\implies \left( 1 + \frac{1}{n} \right)^n$$
> $$\implies 1 = \log \left( 1 + \frac{1}{n} \right)^n$$
> $$\implies \frac{1}{n} \geq \log \left( 1 + \frac{1}{n} \right)$$
> Allora $S_{N} = \sum_{n=1}^{N} \frac{1}{n} = \sum_{n=1}^{N} \log\left( 1 + \frac{1}{n} \right)$
> $$= \sum_{n=1}^{N} \log\left(  \frac{n+1}{n}  \right)$$
> $$= \sum_{n=1}^{N} [\dots]$$
> $$= \log (N+1) = \log(N+1) - \log(1) = \log(N+1)$$
> $\implies S_{N} \geq \log(N+1)$
