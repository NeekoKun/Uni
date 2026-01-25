#analisi 

 Vogliamo definire l'integrale di Riemann anche per funzioni $f: I \subseteq \mathbb{R} \to \mathbb{R}$ con $I$ intervallo che possa essere non chiuso o non limitato e dove $f$ possa essere illimitata in $I$

> [!warning] Definizione (Integrale di Riemann Generalizzato)
> Sia $f: [a,b) \to \mathbb{R}$ con $a \in \mathbb{R}$, $b \in \mathbb{R} \cup \{  +\infty \}$, $a<b$, $f$ possibilmente illimitata
> Sia $f$ Riemann-Integrabile in $$[a,h]\ \forall\ h \in (a,b)$$
> Definiamo $$\int_{a}^b f(x)\ dx = \lim_{ h \to b^- }\int_{a}^h f(x)\ dx$$
> se tale limite $\exists \in \overline{\mathbb{R}}$

> [!warning] Definizione
> Sia $f: (a,b ] \to \mathbb{R}$ con $a \in \mathbb{R} \cup \{ - \infty \}$, $b \in \mathbb{R}$, $a < b$, $f$ possibilmente illimitata
> Sia $f$ Riemann-Integrabile in $$[k,b]\ \forall\ k \in (a,b)$$
> Definiamo
> $$\int_{a}^b f(x)\ dx = \lim_{ k \to a^+ } \int_{k}^b f(x)\ dx$$
> - Se $\lim \in \mathbb{R}$ allora $f(x)$ di dice integrabile impropriamente o generalmente in $(a,b]$ e converge
> - Se $\lim \in \{ -\infty,+\infty \}$ allora $f(x)$ di dice integrabile impropriamente o generalmente in $(a,b]$ e diverge
> - Se $\lim \not\in \overline{\mathbb{R}}$ allora $f$ non è Riemann-Integrabile in $(a,b]$ in senso improprio o generalizzato e l'integrale non esiste