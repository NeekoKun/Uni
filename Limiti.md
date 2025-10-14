#analisi 
## Formule
- Siano $a_{n}$, $b_{n}$ due successioni, ed esistano
	- $a=\lim_{ n \to \infty } a_{n}$, $b=\lim_{ n \to \infty }b_{n} \in \mathbb{R}$
- Allora
	1. $\lim_{ n \to \infty }(a_{n} \pm b_{n}) = a \pm b$
	2. $\lim_{ n \to \infty } (a_{n} \cdot b_{n}) = a \cdot b$
	3. $\lim_{ n \to \infty }\frac{a_{n}}{b_{n}}=\frac{a}{b}$
	4. $\lim_{ n \to \infty }a_{n}^{b_{n}}=a^b$

> [!error] Dimostrazione
> 1) Osserviamo che vale: $$|(a_{n} + b_{n}) - (a + b)| = |(a_{n} - a) + (b_{n} - b)| \leq |a_{n} - a| + |b_{n} - b|$$ per disuguaglianza triangolare.
> Per definizione di limite, $\forall\ \epsilon > 0$
> $$\exists\ N_{1} \in \mathbb{N}:\forall\ n\geq N_{1} |a_{n} - a| > \frac{\epsilon}{2}$$
> $$\exists\ N_{2} \in \mathbb{N}:\forall\ n\geq N_{2} |a_{n} - a| > \frac{\epsilon}{2}$$
> allora se $n \geq max\{ N_{1},N_{2} \}$
> $|(a_{n} + b_{n}) - (a + b)| \leq |a_{n} - a| + |b_{n} - b| <\frac{\epsilon}{2} + \frac{\epsilon}{2} = \epsilon$
> $\implies \lim_{ n \to \infty }(a_{n} + b_{n}) = a + b$
> 2) Osserviamo $$|a_{n}b_{n} - ab| = |a_{n}b_{n} - a_{n}b + a_{n}b - ab|$$$$= |a_{n}(b_{n} - b) + b(a_{n} - a)|$$$$\leq |a_{n}(b_{n} - b)| + |b(a_{n} - a)|$$$$ \leq |a_{n}||b_{n} - b| + |b||a_{n} - a|$$ per disuguaglianza triangolare
> Poichè converge, $\exists\ M \in \mathbb{R}:|a_{n}|\leq \mathbb{N} \forall\ n\in \mathbb{N}$
> $$|a_{n}b_{n} - ab| \leq |a_{n}||b_{n} - b| + |b||a_{n} - a| \leq M|b_{n} - b|+|b||a_{n} - a|$$ per definizione di limite, $\forall\ \epsilon > 0$
> [...]

## Teoremi
> [!warning] Definizione
> Diremo che una [[Successione]] che converge a $l \in \mathbb{R}$ e scriveremo
> $$\lim_{ n \to \infty } a_{n} = 0$$
> Se $\forall\ \epsilon > 0\ \exists\ N \in \mathbb{N} : \forall\ n \geq N$
> $$|a_n - l| < \epsilon\ \ \ \ \ \ (l-\epsilon < a_n < l + \epsilon)$$

> [!error] Teorema dell'Unicità del Limite
> [...]

> [!warning] Definizione
> - Se $\lim_{ n \to \infty } a_{n} = l \in \mathbb{R}$ diremo che $a_{n}$ converge a $l\in \mathbb{R}$
> - Se $\lim_{ n \to \infty } a_{n} = \pm \infty$ diremo che $a_{n}$ diverge a $\pm \infty$
> - Se $a$ non converge né diverge diciamo che essa è irregolare $\implies \not\exists \lim_{ n \to \infty } a_{n}$
> 	- Oscillante
> 	- Indeterminata

> [!warning] Definizione
> Chiamiamo $\overline{\mathbb{R}} = \mathbb{R}^* = \mathbb{R}\cup \{ \pm \infty \} = \mathbb{R}$ esteso 

> [!error] Teorema dell'Unicità del Limite in $\overline{\mathbb{R}}$
> $\exists! \lim_{ n \to \infty }a_{n}\in\overline{\mathbb{R}}$

> [!warning] Definizione
> - Se $\lim_{ n \to \infty }a_{n} = 0$ diremo che $a_{n}$ è una successione infinitesima
> - Se $\lim_{ n \to \infty } a_{n} = \pm \infty$ diremo che $a_{n}$ è una successione infinita

> [!warning] Definizione
> Diremo che $a_{n}$ converge a $l \in \mathbb{R}$ per eccesso se [...]

> [!error] Teorema di Esistenza del Limite di Successioni Monotone Limitate
> Sia $a_{n}$ una successione monotona e limitata
> $\implies \exists \lim_{ n \to \infty }a_{n} = l\in \mathbb{R}$
> Inoltre:
> - Se $a_{n}$ è crescente, $\lim_{ n \to \infty }a_{n} = l^-, l = \mathrm{sup}\ a_{n}\in \mathbb{R}$
> - Se $a_{n}$ è decrescente, $\lim_{ n \to \infty }a_{n} = l^+, l = \mathrm{inf}\ a_{n}\in \mathbb{R}$

> [!error] Dimostrazione
> $a_{n}$ crescente 
> $\implies a_{n}\geq a_{0}\ \forall\ n>0$
> $\implies$ è illimitata dall'alto
> $\implies\ \forall\ M>0\ \exists\ n_{0}\in \mathbb{N}:a_{n_{0}}>M$
> $\implies \forall\ n\geq n_{0},a_{n}>a_{n_{0}}$
> $\implies a_{n}\geq a_{n_{0}}>M$
> $\implies M>0\ \exists n_{0}\in \mathbb{N}:\ \forall\ n\geq n_{0}$
> $$a_{n}>a_{n_{0}}$$
> $\implies \boxed{\lim_{ n \to \infty }a_{n}=+\infty=\mathrm{sup}a_{n}}$

> [!info] Osservazione
> $a_{n}$ monotona $\implies$ $a_{n}$ regolare
> $a_{n}$ regolare $\not\implies$ $a_{n}$ monotona

> [!error] Teorema
> Data una successione $a_{n}$ convergente, cioè $\exists \lim_{ n \to \infty }a_{n}=l\in \mathbb{R}$, allora $a_{n}$ è limitata

> [!info] Osservazione
> $\exists\ \lim_{ n \to \infty } a_{n}= l\in \mathbb{R}\implies a_{n}$ limitata

- [[Teorema di Permanenza del Segno]]
- [[Teorema dei due Carabinieri]]
- [[Teorema del Confronto tra successioni divergenti]]
- [[Teorema di Gerarchia degli Infiniti]]
- [[Teorema di Aritmetizzazione Parziale di Infinito]]
- [[Teorema di ???]]
- [[Teorema del Rapporto per Successioni]]