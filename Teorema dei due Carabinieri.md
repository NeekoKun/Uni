#analisi 
> [!error] Definizione
> Date tre successioni $a_{n}, b_{n}, c_{n}$ tali che $$a_{n} \leq b_{n} \geq c_{n}$$ definitivamente in $n \in \mathbb{N}$ e tali che $$\exists\ \lim_{ n \to \infty }a_{n}=\lim_{ n \to \infty }c_{n}=l \in \mathbb{R}$$
> Allora $\exists\ \lim_{ n \to \infty }b_{n} = l \in \mathbb{R}$

> [!warning] Dimostrazione
> Per definizione di limite, $\forall\ \epsilon>0$ 
> $\exists\ N_{1}\in \mathbb{N}:\forall\ n\geq N_{1}\ |a_{n} - l|<\epsilon$, cioè $$l-\epsilon < a_{n}$$
> $\exists\ N_{2}\in \mathbb{N}:\forall\ n\geq N_{2}\ |c_{n} - l|<\epsilon$, cioè $$c_{n} < l + \epsilon$$
> inlotre $N_{3}\in \mathbb{N}:n\geq N_{3}$ $$\implies a_{n} \leq b_{n} \leq c_{n}$$
> allora se $n \geq max\{ N_{1},N_{2},N_{3} \}$ $$l-\epsilon < a_{n} \leq b_{n} \leq c_{n} < l+\epsilon$$
> $\implies \forall\ \epsilon > 0\ \exists\ N = max\{ N_{1},N_{2},N_{3} \}:\forall\ n \geq N l[\dots]l$

## Corollari
1) Se $b_{n}, c_{n}$ sono successioni, tali che $$|b_{n}| \leq c_{n}$$ definitivamente in $n\in \mathbb{N}$ e se $\lim_{ n \to \infty }c_{n} =0$, allora $$\exists\ \lim_{ n \to \infty } b_{n} = 0$$
2) Se $b_{n},c_{n}$ sono successioni tali che $c_{n}$ sia limitata e $\lim_{ n \to \infty }b_{n} = 0$ allora $$\lim_{ n \to \infty } c_{n}\cdot b_{n}=0$$
> [!error] Dimostrazione
> 1) Per ipotesi $|b_{n}| \leq c_{n}$ definitivamente in $n\in \mathbb{N}$, cioè $$-c_{n}\leq b_{n}\leq c_{n}$$ inoltre $$\lim_{ n \to \infty } c_{n} = 0 \land \lim_{ n \to \infty } -c_{n} = 0$$ per algebra dei limiti.
> Per teorema dei due carabinieri: $$\exists\ \lim_{ n \to \infty } b_{n} = 0$$
> ---
> 2) Vogliamo dimostrare che $$\lim_{ n \to \infty } b_{n}c_{n} = 0$$Essendo $c_{n}$ limitato, $\exists\ M>0:\forall\ n\in \mathbb{N}$ $$|c_{n}| \leq M$$ quindi $\forall\ n\in \mathbb{N}$ vale $$|b_{n}c_{n}| \leq M|b_{n}|$$ inoltre, $$\lim_{ n \to \infty } |b_{n}| = 0$$ e quindi per algebra dei limiti $$\lim_{ n \to \infty } M|b_{n}| = 0$$ poiché $\lim_{ n \to \infty }b_{n}=0$ per ipotesi.
> Per il punto 1. allora $$\lim_{ n \to \infty } b_{n}c_{n}=0$$