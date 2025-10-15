#analisi 
> [!error] Teorema
> Siano $a_{n}$, $b_{n}$ due successioni con termini (definitivamente) positivi. Supponiamo che $a_{n}$ ~ $b_{n}$
> Allora $\sum_{n=1}^{\infty}a_{n}$ e $\sum_{n=1}^{\infty}b_{n}$ hanno lo stesso carattere

> [!error] Dimostrazione
> Poiché $\lim_{ n \to \infty } \frac{a_{n}}{b_{n}} = 1$, per $\epsilon = \frac{1}{2}$ $$\exists N_{1} \in \mathbb{N} : \forall\ n \geq N$$ $$\frac{1}{2} = 1 - \frac{1}{2} < \frac{a_{n}}{b_{n}} < 1 + \frac{1}{2} = \frac{3}{2}$$
> Perché definitivammente $a_{n}$, $b_{n}$ sono positive, $\exists N_{2} \in \mathbb{N}: \forall\ n \geq N_{2}$ $$a_{n} > 0,\ b_{n} > 0$$
> Allora $op n \geq N = \mathrm{max} \{  N_{1}, N_{2} \}$
> segue che $$0 < a_{n} < \frac{3}{2}b_{n}$$ e $$0 < \frac{1}{2}b_{n} < a_{n}$$
> per il criterio del confronto
> - Dalla prima segue che $\sum_{n=1}^{\infty} a_{n}$ diverge $\implies \sum_{n=1}^{\infty} b_{n}$ diverge, $\sum_{n=1}^{\infty}b_{n}$ converge $\implies\sum_{n=1}^{\infty} a_{n}$ converge.
> - Dalla seconda segue che $\sum_{n=1}^{\infty} a_{n}$ converge $\implies \sum_{n=1}^{\infty}b_{n}$ converge, $\sum_{n=1}^{\infty}b_{n}$ diverge $\implies \sum_{n=1}^{\infty}a_{n}$ diverge 
>
> $\implies$ le serie o convergono o divergono entrambe