#analisi 
> [!warning] Definizione
> Data una successione di [[Numeri Reali]], definiamo successione delle somme parziali di $a_{n}$ la successione $S_{N} = \sum_{i=0}^{N}a_{n}=a$
> Chiamiamo serie degli $a_{n}$ la successione formale $$\sum_{n=0}^{N} a_{n}$$ che si legge serie degli $a_{n}$.
> Indica formalmente la somma degli infiniti termini $a_{n}$.
> - Diremo che la serie degli $a_{n}$ converge a $S \in \mathbb{R}$ se $$\exists \lim_{ N \to \infty } S_{N} = S \in \mathbb{R}$$ dove $S_{N} = \sum_{n=1}^{N} a_{n}$.
> 	Scriveremo quindi $$\sum_{n=0}^{N} a_{n} = S \in \mathbb{R}$$
> - Diremo che la serie degli $a_{n}$ diverge a $\pm \infty$ se $\exists \lim_{ N \to \infty }S_{N} = S \in \{ -\infty,\infty \}$

> [!info] Osservazione
> - La somma della serie è $$S = \lim_{ N \to \infty } \sum_{n=0}^{N} a_{n}$$
> - Studiare una serie coinvolge due successioni: $a_{n}$ e $S_{N}$
> - Studiare il carattere di una serie significa stabilire seessa sia convergente, divergente ($a \pm \infty$) o irregolare
> - Se la serie è convergente, calcolare esplicitamente il valore $$S = \lim_{ N \to \infty } \sum_{n=0}^{N} a_{n} \in \mathbb{R}$$ è in generale un problema molto difficile.
> Il problema è che spesso non si riesce a determinare una forma pi+ "semplice ed esplicita" per $$S_{N} = \sum_{n=0}^{N} a_{n}$$ Diventa quindi fondamentale trovare condizioni necessarie o sufficienti affinché una serie converga o diverga.
> Successivamente, se la serie converge si può provare a calcolare un valore approssimato della sua somma

> [!info] Osservazione
> I primi $n_{0}\in \mathbb{N}$ termini della successione $a_{n}$ sono indifferenti per determinare il carattere di $\sum_{n=0}^{N}a_{n}$.
> Se la serie converge, ogni valore è necessario per calcolare il calore di convergenza

> [!info] Osservazione
> Non vale la proprietà commutativa - non si può alterare l'ordine di una serie -

> [!warning] Serie note
> - Serie geometrica
> $$\sum_{n=0}^{N} q^n = S_{N} = \begin{cases} + \infty & q \geq 1 \\ \frac{1}{1-q} & |q| < 1 \\ \not\exists\ & q \leq 1 \end{cases}$$

> [!info] Osservazione 
> Dal [[Teorema dell'Algebra dei Limiti]] e dal [[Teorema di Aritmetizzazione Parziale di Infinito]] segue che date 2 serie regolari $$\sum_{n=0}^{\infty} a_{n},\ \sum_{n=0}^{\infty} b_{n}$$ e $\alpha, \beta \in \mathbb{R}$ vale $$\sum_{n=0}^{\infty} (\alpha a_{n} + \beta b_{n}) = \alpha \sum_{n=0}^{\infty} a_{n} + \beta \sum_{n=0}^{\infty} b_{n}$$

> [!error] Dimostrazione
> $$\sum_{n=0}^{\infty} (\alpha a_{n} + \beta b_{n}) = \lim_{ N \to \infty } \sum_{n=0}^{N} (\alpha a_{n} + \beta b_{n})$$
> $$= \lim_{ N \to \infty } \left[  \alpha \sum_{n=0}^{N} a_{n} + \beta \sum_{n=0}^{N} b_{n}  \right]$$
> $$= \alpha \lim_{ N \to \infty } \sum_{n=0}^{N} a_{n} + \beta \lim_{ N \to \infty } \sum_{n=0}^{N} b_{n} $$
> $$= \alpha \sum_{n=0}^{\infty} a_{n} + \beta \sum_{n=0}^{\infty} b_{n} $$

## Teoremi
- [[Condizione Necessaria affinchè una serie converga]]
- [[Resto Ennesimo]]
- Condizioni Sufficienti affinché una serie ammetta limite:
	- [[Serie a Termini Positivi]]