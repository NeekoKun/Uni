#analisi 
> [!warning] Teorema
> - Sia $y\in \mathbb{R}, y\geq 0, n\in \mathbb{N}, n\geq 1$
> $\implies\exists! x\in \mathbb{R}\ |\ x\ge 0\ e\ x^n=y$
> - Segue dal fatto che la funzione $f: [0,+; +\infty) \to [0; +\infty), f(x) = x^n$ è monotona strettamente crescente, continua, con $f(0)=0, \lim_{ x \to +\infty }=+\infty$

> [!warning] Definizione
> Il numero reale x siffatto si chiama radice (reale) n-esima di y

> [!info] Osservazione
> $\sqrt{ 4 } = 2$
> $\xcancel{\sqrt{ 4 } = \pm 2}$

> [!warning] Definizione
> - $\forall\ a\in \mathbb{R}$
> 	- $a^0 = 1$
> 	- $a^m = a\cdot a \dots a\cdot a$
> 	- $a^{\frac{1}{n}} =\sqrt[n]{ a }$
> - $\forall\ a \in \mathbb{R}, a > 0$ definiamo.
> 	- a^-1 = 1/a
> - $\forall\ m,n \in \mathbb{N}, n \neq 0$
> 	- $a^{-m} = (a^{-1})^m$
> 	- $a^{m/n} = {a^{\frac{1}{n}}}^m$



> [!info] Osservazione
> - $\forall\ a^n \in \mathbb{R}, a > 0\ \forall\ a \in \mathbb{R}\ a > 0\ \forall\ r \in \mathbb{Q}$

Come definire $a^n \in \mathbb{R} \impliedby a \in \mathbb{R} \land a > 0 \land r \in \mathbb{R}$?
1) $b \in \mathbb{R} \implies b = \pm b_0,b_1b_2b_3b_4....b_k...\ con\ b_0 \in \mathbb{N}, n_k \in \{0...9\}\ \forall\ k \in \mathbb{N}, k \geq 1$
2) definiamo $a^b = \lim\limits_{ k \to +\infty }a^{\pm b_{0},b_{1}b_{2}\dots b_{k}}$
Si Dimostra che $a^b$ può anche essere caratterizzata dome $a^b = sup\{a^{\pm b_0,b_1b_2b_3b_4\dots b_k}: k \in \mathbb{N}\}$
oppure in dell'opposto a seconda che i valore della successione siano crescenti o decrescenti

> [!info] Osservazione
> -  è definito $\forall\ a\in \mathbb{R}, a>0,\ \forall\ b\in \mathbb{R}$ e vale $a^b>0$
> - $a^b$ può essere definito anche per alcuni valori $a\leq 0$ se $b\in \mathbb{R}$ è particolare

> [!error] Teorema
> - Dati $y,a \in \mathbb{R},\ y > 0\ \land a>0,\ a!=1 \implies \exists\ x \in \mathbb{R}\ |\ a^x = y$

Def di [[Logaritmi]]:
- Dati $y,a \in \mathbb{R},\ y>0,\ a>0,\ a!=1$
- Definiamo
	- $x = log_ay \implies a^x=y$
