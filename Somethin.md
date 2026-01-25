#analisi 
> [!warning] Definizione
> Data $f: (a,b) \to \mathbb{R}$, $a < b$, $a,b \in \overline{\mathbb{R}}$, con $f$ possibilmente illimitata
> Sia $f$ [[Integrale di Riemann|Riemann-Integrabile]] in $[k,h]$ $\forall\ k <h \in (a,b)$
> Diremo che $f$ è [[Integrale di Riemann|Riemann-Integrabile]] in senso improprio o generalizzato in $(a,b)$ se
> $$\int_{a}^b f(x)\ dx = \lim_{\overset{h \to b^-}{k \to a^+ }} \int_{k}^h f(x)\ dx$$
> - Se ale doppio limite esiste infinito, $f$ non è [[Integrale di Riemann|Riemann-Integrabile]] in senso improprio e
> $$\int_{a}^b f(x)\ dx \text{ diverge}$$
> - Se tale doppio limite non esiste in $\overline{\mathbb{R}}$ allora $f$ non è [[Integrale di Riemann|Riemann-Integrabile]] e nin senso improprio e
> $$\int_{a}^b f(x)\ dx \text{ non esiste}$$

> [!info] Osservazione
> Equivale a chiedere che comunque sia fissato $c \in (a,b)$ $f$ sia [[Integrale di Riemann|Riemann-Integrabile]] in senso improprio separatamente in $[c, b)$ e $(a, c]$. I due limiti vengono presi in maniera indipendente e
> $$\int_{a}^b f(x)\ dx = \int_{a}^c f(x)\ dx + \int_{c}^b f(x)\ dx$$

> [!info] Osservazione
> Siano
> $$F = \int_{a}^b f(x)\ dx,\ \ G = \int_{a}^c f(x)\ dx,\ \ H = \int_{c}^b f(x)\ dx$$
> - Se $G$ e $H$ convergono, allora $F$ converge a $G + H$
> - Se $F$ o $G$ divergono, allora $F$ diverge anche lui