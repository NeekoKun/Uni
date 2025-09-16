#analisi
- Serve per dimostrare la verità di una implicazione universale della forma $\forall\ n \in \mathbb{N}\ P(n)$
1) Dimostrare che è vera $P(0)$
2) Dimostrare che $P(n) \implies P(n+1)$

#### Esempio (Disuguaglianza di Bernoulli)
$$\forall\ x \in \mathbb{R}\ con\ x>-1$$
$$(1+x)^n \ge 1+nx$$
1) verifichiamo $P(0)$
$$(1+x)^0 \ge 1+0x$$
$$1 \ge 1$$
2) Verifichiamo  $P(n) \implies P(n+1)$
$$(1+x)^{n+1} = (1+x)^n\ (1+x)$$
$$\ge\ (1+nx)(1+x)$$
$$= 1+nx+x+nx^2$$
$$=(1+(n+1)x)+nx^2$$
$$\ge 1+(n+1)x$$
$$(1+x)^{n+1}\ge 1+(n+1)x$$