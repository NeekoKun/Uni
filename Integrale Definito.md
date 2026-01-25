#analisi 
## Definizioni
- [[Integrale di Riemann]]
- [[Integrale di Riemann Generalizzato]]

## Proprietà
### Linearità

> [!error] Proprietà
> Siano $f, g : [a,b] \to \mathbb{R}$ e siano Riemann-Integrabili in $[a,b]$ e $\alpha, \beta \in \mathbb{R}$.
> Allora $\alpha f + \beta g : [a,b] \to \mathbb{R}$ è Riemann-Integrabile in $[a,b]$ e 
> $$\int_{a}^b \alpha f(x) + \beta g(x) dx = \alpha \int_{a}^b f(x) dx + \beta \int_{a}^b g(x) dx$$

### Additività sul Dominio
> [!error] Proprietà
> Data $f : [a,b] \to \mathbb{R}, c \in [a,b]$
> Allora $f$ è Riemann Integrabile in $[a,b]$ se e solo se lo è in $[a,c]$ ed in $[c,b]$. Inoltre:
> $$\int_{a}^b f(x) dx = \int_{a}^c f(x) dx + \int_{c}^b f(x) dx$$

> [!info] Convenzione
> Se $a < b$ si pone
> $$\int_{b}^a f(x)dx = - \int_{a}^b f(x) dx$$
> Con questa convenzione, vale qualunque sia l'orientamento di $a,b,c \in \mathbb{R}$

### Concatenazione dell'Integrale

> [!error] Proprietà
> Sia $f : [a,b] \to \mathbb{R}$ Riemann-integrabile in $[a,b]$. Sia $\psi : [c,d] \to \mathbb{R}$ tale che $\Im f \subseteq [c,d]$. Allora $\psi \circ f : [a,b] \to \mathbb{R}$ è a sua volta Riemann-Integrabile in $[a,b]$

> [!error] Corollario
> Si $f: [a,b] \to \mathbb{R}$ è Riemann-Integrabile in $[a,b]$ allora lo sono anche $|f|, f^2, f^3, e^f, \sin f, \dots$

> [!error] Corollario
> Se $f,g : [a,b] \to \mathbb{R}$ sono Riemann-integrabili in $[a,b]$, allora lo è anche $f(x) \cdot g(x)$

### Positività e Monotonia dell'Integrale di Riemann

> [!error] Proprietà
> 1. Se $f:[a,b] \to \mathbb{R}$ è Riemann-integrabile in $[a,b]$ e se $f \geq 0$ in $[a,b]$, allora
> $$\int_{a}^b f(x) dx \geq 0$$
> 2. Se $f,g : [a,b] \to \mathbb{R}$ sono Riemann-integrabili in $[a,b]$ e se $f \geq g$ in $[a,b]$ allora
> $$\int_{a}^b f(x)dx \geq \int_{a}^b g(x) dx$$
> 3. Se $f :[a,b] \to \mathbb{R}$ è Riemann-Integrabile in $[a,b]$ allora
> $$\left|\int_{a}^b f(x) dx\right| \leq \int_{a}^b |f(x)| dx$$

### Media Integrale

> [!error] Teorema
> Sia $f:[a,b] \to \mathbb{R}$ continua in $[a,b]$ allora $\exists\ x_{0} \in [a,b]$ tale che 
> $$f(x_{0}) = \frac{1}{(b-a)} \int_{a}^b f(x) dx$$

> [!warning] Definizione
> Se $f: [a,b] \to \mathbb{R}$ è Riemann-Integrabile in $[a,b]$ allora
> $$\frac{1}{b-a} \int_{a}^b f(x) dx$$
> si dice **Valore Medio** di $f$ in $[a,b]$

> [!error] Dimostrazione
> Essendo $f$ continua essa è integrabile in $[a,b]$. Inoltre per il [[Teorema di Weierstrass]] essa ammette massimo e minimo assoluto in $[a,b]$, cioè
> $$M = \mathrm{max}(f), m = \mathrm{min}(f)$$
> ovviamente
> $$m \leq f(x) \leq M\ \forall\ x \in [a,b]$$
> Poiché le funzioni costanti sono integrabili, per Monotonia dell'Integrale 
> $$\int_{a}^b m\ dx \leq \int_{a}^b f(x)\ dx \leq \int_{a}^b M\ dx$$
> $$\implies m(b-a) \leq \int_{a}^b f(x)\ dx \leq M(b-a) $$
> $$\implies m \leq \frac{1}{b-a}\int_{a}^b f(x)\ dx \leq M $$
> Essendo $f$ continua, per il [[Teorema dei Valori Intermedi]] $\Im f = [m,M]$
> $$\implies \frac{1}{b-a} \int_{a}^b f(x)\ dx \in \Im f$$
> $\implies \exists\ x_{0} \in [a,b] :$
> $$\boxed{f(x_{0}) = \frac{1}{b-a} \int_{a}^b f(x)\ dx}$$

### Integrale per Parti

> [!error] Proprietà
> Siano $f,g : [a,b] \to \mathbb{R}$ derivabili in $[a,b]$, con $f', g' : [a,b] \to \mathbb{R}$ Riemann-Integrabili in $[a,b]$ allora:
> $$\int_{a}^b f(x) g(x)\ dx = f(b)g(b) - f(a)g(a) - \int_{a}^b f(x)g'(x)\ dx$$

### Integrare per Sostituzione
> [!error] Proprietà
>  #TODO 