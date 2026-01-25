#analisi 

> [!warning] Definizione (Integrale di Riemann)
> per $f: [a,b] \to \mathbb{R}$, con $f$ limitata
> Per ogni $n \in N$, dividiamo $[a,b]$ in $n$ parti di uguale lunghezza $\frac{b-a}{n}$ ($n \geq 2$) tramite i punti:
> $$x_{0} = a < x_{1} < x_{2} < \dots < x_{n} = b$$
> Equivalenti e a distanza $\frac{b-a}{n}$ dal precedente e dal successivo, dove $$x_{k} = a + \frac{b-a}{n}k$$
> In ogni intervallo $[x_{k-1}, x_{k}]$ scegliamo poi arbitrariamente un punto $t_{k}^{(n)} \in [x_{k-1}, x_{k}]$
> costruiamo la **Somma di Cauchy-Riemann**
> $$\mathcal{S}_{n} = \sum_{k=1}^{n} (x_{k} - x_{k-1})f(t_{k}^{(n)})$$
> $$= \frac{b-a}{n} \sum_{k=1}^{n} f(t_{k}^{(n)})$$
> Ad ogni passo della costruzione, in generale variano sia i punti $x_{0}, \dots, x_{n}$ che realizzano la partizione di $[a,b]$, che i punti $t_{k}^{(n)} \in [x_{k-1}, x_{k}]$ per $k \in [1, \dots, n]$.
> La Somma di Cauchy-Riemann $\mathcal{S}_{n}$ da un'approssimazione di ciò che vogliamo definire come "**Integrale di Riemann**" di $f$ in $[a,b]$, ottenuta come somme di rettangoli $R_{k}$ avente base [...] ed altezza [...]

> [!warning] Definizione
> Diciamo che $f: [a,b] \to \mathbb{R}$ limitata in $[a,b]$ e integrabile secondo Riemann in $[a,b]$ (in senso proprio) se detta $\mathcal{S}_{n}$ una qualsiasi successione di somme di cauchy-riemann (costruita come sopra) esiste finito $$\lim_{ n \to \infty } \mathcal{S}_{n} = L \in \mathbb{R}$$
> ed inoltre tale limite $L \in \mathbb{R}$ **NON** dipende dalla scelta dei punti $t_{k}^{(n)}$ operata ad ogni passo $n$ della costruzione.
> Chiameremo
> $$L = \lim_{ n \to \infty } \mathcal{S}_{n} = \int_{a}^b f(x) dx$$
> Integrale di Riemann di $f$ in $[a,b]$

> [!warning] Definizione
> Se $f: [a,b] \to \mathbb{R}$ è Riemann-Integrabile in $[a,b]$ e se $f(x) \geq 0\ \forall\ x \in [a,b]$ e
> $$D = \{ (x,y) \in \mathbb{R}^2 : a \leq x \leq b, 0 \leq y \leq f(x) \}$$
> definiamo
> $$\mathrm{Area}(D) = \int_{a}^b f(x) dx$$

> [!info] Osservazione
> Se $f :[a,b] \to \mathbb{R}$ è Riemann-Integrabile in $[a,b]$ e può cambiare segno ($f(x) < 0$ per qualche $x \in [a,b]$) l'area ottenuta con l'integrale di Riemann ha segno positivo o negativo, a seconda

> [!info] Osservazione
> Esistono altre 4 definizioni equivalenti dell'integrale di Riemann
