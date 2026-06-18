#analisi 
> [!error] Teorema
> Sia $a_{n}$ una serie con termini (definitivamente) positivi, e supponiamo $\exists\ l = \lim_{ n \to \infty } \frac{a_{n+1}}{a_{n}} \in \overline{\mathbb{R}}$
> Allora
> 1. Se $l > 1$ allora $$\sum_{n=1}^{\infty} a_{n} \text{ diverge } (\lim_{ n \to \infty } a_{n} = +\infty)$$
> 2. Se $0 \leq l < 1$ allora $$\sum_{n=1}^{\infty} a_{n} \text{ converge}$$
> 3. Se $l = 1$ allora non si può concludere nulla, cioè esistono serie che convergono e serie che divergono tali che $$\lim_{ n \to \infty } \frac{a_{n+1}}{a_{n}} = 1$$

> [!error] Dimostrazione
> Per semplicità supponiamo $a_{n} > 0 \forall\ n \in \mathbb{N}$, e $$l = \lim_{  n \to \infty } \frac{a_{n+1}}{a_{n}}$$
> 1. Se $l > 1$ ci sono 2 casi:
> 	1. se $l \in (1; +\infty)$, scegliamo $\epsilon = l - 1 > 0$ nella definizione di limite. Allora $$\exists N \in \mathbb{N} : l - \epsilon < \frac{a_{n+1}}{a_{n}} < l + \epsilon$$
> 	$\implies \forall\ n \geq N$ $$\frac{a_{n+1}}{a_{n}} > \frac{l+1}{2} > 1$$
> 	Se chiamiamo $q = \frac{l+1}{2}$ vale che $$a_{n+1} > qa_{n} \forall\ n \geq N$$
> 	$\implies \forall\ n \geq N$ $$a_{n+1} > q^{n + 1 - N}a_{N}$$
> 	$$\implies a_{n+1} > \frac{a_{N}}{q_{N}} \cdot q^{n+1}$$
> 	Per il [[Criterio del Confronto per Serie a Termini non-negativi]], Poichè $\sum_{n=1}^{\infty}q_{n}$ diverge, diverge anche $\sum_{n=1}^{\infty}a_{n}$ (Serie Geometrica di ragione $q = \frac{l + 1}{2} > 1$)
> 	2. Se $l = +\infty$, per definizione di limite infinito per $M=2$ esiste $N \in \mathbb{N}$ tale che $\forall\ n \geq N$ $$\frac{a_{n+1}}{a_{n}} > M = 2$$
> 	$\implies a_{n+1} > qa_{n}$ con $q = 2$, $\forall\ n \geq N$, e da qui si ripete la dimostrazione del punto 1.
> 2. Se $0 \leq l < 1$, per $\epsilon = \frac{1-l}{2} > 0$ $$\exists N \in \mathbb{N} : \forall\ n \geq N$$ $$l - \epsilon < \frac{a_{n+1}}{a_{n}} < l + \epsilon = \frac{1+l}{2} < 1$$
> $$\implies \frac{a_{n+1}}{a_{n}} < \frac{1+l}{2} < 1 \forall\ n \geq N$$
> definiamo $q = \frac{1+l}{2} < 1$, allora
> $$\frac{a_{n+1}}{a_{n}} < q < 1 \forall\ n \geq N$$
> $$0 < a_{n+1}<qa_{n} \forall\ n \geq N$$
> $\implies \forall\ n \geq N$
> $$0 < a_{n+1} < qa_{n} < q^2a_{n-1} < \dots < q^{n+1-N}a_{N}$$
> $\implies \forall\ n \geq N$
> $$0 < a_{n+1} < \frac{a_{N}}{q^N} \cdot q^{n+1}$$
> $\implies \forall\ n \geq N+1$
> $$0 < a_{n} < \frac{a_{N}}{q^N} \cdot q^{n}$$
> Poiché $q \in (0, 1)$ oer il [[Criterio del Confronto per Serie a Termini non-negativi]], essendo $\sum_{n=0}^{\infty} q^n = \frac{1}{1-q}$ convergente, deve essere convergente anche $\sum_{n=1}^{\infty}a_{n}$
> Per [[Teorema dei due Carabinieri]], essendo $\lim_{ n \to \infty }q^n = 0$, deve essere anche $\lim_{ n \to \infty }a_{n} = 0$

