#analisi 
> [!error] Teroema di Permanenza del Segno
> 1) Data $a_{n}$ successione, $\exists\ \lim_{ n \to \infty }a_{n}=l\in \mathbb{\overline{R}},\ l > 0\implies \exists\ n_{0}:a_{n}>0\ \forall\ n > n_{0}$
> 2) $\exists \lim_{ n \to \infty }a_{n}\in \overline{\mathbb{R}},\exists\ n_{0} : a_{n>n_{0}}\geq 0\implies l \geq 0$

> [!info] Osservazione
> - Può essere $l\geq 0$ con $a_{n}<0$
> 	- e.g.: $a_{n}=-\frac{1}{n}$
> - Se $a_{n}>0$ ed esiste $\lim_{ n \to \infty }a_{n}=l\in\overline{\mathbb{R}}$ allora $l\geq_{0}$ ma può essere $l=0$
> -> Le disuguaglianze strette passano a larghe al limite

> [!warning] Dimostrazione
> 1) Sia $l=\lim_{ n \to \infty }a_{n}\in(0,+\infty]$
> Se $l=+\infty$, per definizione $\forall\ M > 0 \exists  N \in \mathbb{N}:\forall\ n\geq N$
> $$a_{n}>M>0$$
> $\implies a_{n} > 0$ definitivamente in $n \in \mathbb{N}$
> Se $l \in (0, +\infty)$, scegliamo $\epsilon = \frac{l}{n} > 0$ nella definizione di limite, allora $\exists N \in \mathbb{N}: n\geq N$
> $$l-\epsilon<a_{n}$$
> Quindi $\forall\ n \geq N$
> $$a_{n}> l-\epsilon = l - \frac{l}{2} = \frac{l}{2} > 0$$
> $\implies a_{n}>0$ definitivamente in $n\in \mathbb{N}$
> 2) Se $a_{n}\geq 0$ difinitivamente e $\exists l = \lim_{ n \to \infty }a_n \in \overline{\mathbb{R}}$ vogliamo provare che $l \geq 0$
> Per assurdo sia $l<0$
> Per la parte (1) del teorema, deve essere definiticamente $a_{n}<0$ in $n\in \mathbb{N}$
> Assurdo perché dovrebbe essere
> $$a_{n}\geq 0 \land\ a_{n} < 0$$
> Definitivamente in $n\in \mathbb{N}$
> Quindi deve essere $l\geq 0$

## Corollario
1. Date due successioni $a_{n}, b_n:$ $$\exists\ \lim_{ n \to \infty } a_{n}=a, \lim_{ n \to \infty } b_{n} = b \in \mathbb{R}$$
	1) Se $a>b$ allora definitivamente un $n\in \mathbb{N}$ vale $a_{n}> b_{n}$
	2) Se $a_{n} \geq b_{n}$ definitivamente in $n\in \mathbb{N}$, allora $a \geq b$

> [!error] Dimostrazione
> 1) Se $c_{n} = a_{n} - b_{n}$ allora per algebra dei limiti $$\exists c = \lim_{ n \to \infty } a_{n} - b_{n} = a - b \in \mathbb{R}$$
> Quindi se $a > b$ alllora $c > 0$ e per permanenza del segno definitivamente in $n \in \mathbb{N}$ vale che $$a_{n} - b_{n} = c_{n} > 0$$
> 2) Sia ancora $a_{n} - b_{n} = c_{n}$ e $c = \lim_{ n \to \infty }c_{n} = a - b \in \mathbb{R}$
> 			se $a_{n} \geq b_{n}$ definitiamente allora $c_{n} \geq 0$ definiticamente in $n \in \mathbb{N}$, per permanenza del segno. $c=\lim_{ n \to \infty }c_n \geq 0$
> $\implies a- b = c \geq 0$
> $\implies a \geq b$