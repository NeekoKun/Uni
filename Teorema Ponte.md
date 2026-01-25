#analisi 
> [!error] Teorema
> La [[Limite#Definizione|Definizione Successionale]] di $\lim_{ x \to x_{0} } f(x) = l$ e la [[Limite#Definizione|Definizione Topologica]] di $\lim_{ x \to x_{0} }$ sono equivalenti, per $f, I \subseteq \mathbb{R} \to \overline{\mathbb{R}}, x_{0}\in \overline{\mathbb{R}}$ punto di accumulazione per $I,l\in \overline{\mathbb{R}}$

>[!info] Osservazione
>Il caso $f:\mathbb{N} \subset \mathbb{R} \to \mathbb{R}$ delle successioni è incluso della definizione topologica di limite con $I = N$, $x_{0} = +\infty$ e $\lim_{ n \to \infty }f(n) = l \in \overline{\mathbb{R}}$
>Recuperiamo così la definizione già data. Infatti: 
>1. $l = +\infty, u(+\infty)=(M,\infty), M \in \mathbb{R}$
>$\forall\ M \in \mathbb{R}\ \exists\ N \in \mathbb{R} :$
>$$n \in \mathbb{N},\ n > N \implies f(n) > M$$
>2. $l = -\infty,\ \ u(+\infty) = (N, +\infty),\ N \in \mathbb{R},\ \ u(-\infty) = (-\infty, M),\ M \in \mathbb{R}$
>$\forall\ M \in \mathbb{R}\ \exists\ N \in \mathbb{R} :$
>$$n \in \mathbb{N},\ n > N \implies f(n) < M$$
>3. $l \in \mathbb{R},\ \ \ u(l) = (l-\epsilon,\ l + \epsilon)$
>Specificando la forma esplicita degli intorni $u(x_{0}), u(l)$ nei casi $x_{0}\in \overline{\mathbb{R}}$ e $l \in \overline{\mathbb{R}}$ si trovano le definizioni metriche di limite