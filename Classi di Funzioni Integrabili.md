#analisi 
> [!error] Teorema
> Se $f: [a,b] \to \mathbb{R}$ monotona allora essa è [[Integrali#Integrale Definito|Riemann-Integrabile]] in $[a,b]$

> [!info] Osservazione
> Sotto queste ipotesi, $f$ è automaticamente limitata:
> - Se $f$ crescente $$f(a) \leq f(x) \leq f(b)$$
> - Se $f$ decrescente $$f(b) \leq f(x) \leq f(a)$$

> [!error] Teorema (Di Heine-Cantor)
> Se $f: [a,b] \to \mathbb{R} è continua in $[a,b]$ allora essa è [[Integrali#Integrale Definito|Riemann-Integrabile]] in $[a,b]$

> [!info] Osservazione
> Sotto questa ipotesi, $f$ è automaticamente limitata perché ammette massimo e minimo assoluti per il [[Teorema di Weierstrass]]

> [!error] Teorema
> Se $a < c < b$, $a,b,c \in \mathbb{R}$, e se $f_{1}: [a,c] \to \mathbb{R},\ f_{2}:[c,b] \to \mathbb{R}$ sono funzioni [[Integrali#Integrale Definito|Riemann-Integrabili]] in $[a,c]$ e $[c,b]$ rispettivamente allora $\forall\ \alpha \in \mathbb{R}$
> $$f(x) = \begin{cases}f_{1}(x) & x \in [a, c) \\ \alpha & x = c \\ f_{2}(x) & x \in (c, b] \end{cases}$$
> è [[Integrali#Integrale Definito|Riemann-Integrabile]] in $[a,b]$

> [!info] Osservazione
> Vale un risultato analogo anche nel caso di un numero finito di punti $c_{1},\ \dots,\ c_{n} \in [a,b], n \in \mathbb{N}$