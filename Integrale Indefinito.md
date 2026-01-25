#analisi 

> [!warning] Definizione
> L'insieme di tutte le primitive di $f:I \subseteq \mathbb{R} \to \mathbb{R}$ prende il nome di **Integrale Indefinito** di $f$ in $I$ e si indica con $$\int f(x) dx$$

> [!info] Osservazione
> Se $F(x)$ è una primitiva di $f :I \subseteq \mathbb{R} \to \mathbb{R}$ in $I$, $I$ intervallo, spesso si scrive $$\int f(x) dx = F(x) + c$$ $c \in \mathbb{R}$ arbitrario

## Proprietà
### Linearità

> [!error] Teorema
> Datr $f, g : I \subseteq \mathbb{R} \to \mathbb{R}$, $\alpha, \beta \in \mathbb{R}$, allora $$\int \alpha f(x) + \beta g(x) dx = \alpha \int f(x) dx + \beta \int g(x) dx$$

> [!error] Dimostrazione
> Se $F,G$ sono primitive di $f,g$ rispettivamente in $I$, $\alpha, \beta \in \mathbb{R}$ allora $\alpha F + \beta G$ è derivabile in $I$ per linearità della derivata. Inoltre $\forall\ x \in I$
> $$(\alpha F + \beta G)'(x) = \alpha F'(x) + \beta G'(x) = \boxed{\alpha f(x) + \beta g(x)}$$
### Integrale per Parti
> [!error] Teorema
> Siano $f, g : I \subseteq \mathbb{R} \to \mathbb{R}$, $I$ intervallo, derivabile in $I$. Allora:
> $$\int f'(x)g(x)dx = f(x)g(x) - \int f(x)g'(x)dx$$

> [!error] Dimostrazione
> Sia $H$ primitiva di $f\cdot g'$ in $I$, allora $f\cdot g - H$ è derivabile in $I$. Inoltre, $\forall\ x \in I$
### Integrale per Sostituzione

> [!error] Teorema
> Sia $f: I \subseteq \mathbb{R} \to \mathbb{R}$, $I$ intervallo, $\psi : J \to I$, $\psi$ derivabile in $J$. Allora
> $$\int f(\psi(t))\psi'(t) dt = \int f(x) dx$$
> con $x = \psi(t)$

> [!error] Dimostrazione
> Sia $F$ primitiva di $f$ in $I$. Allora $F \circ \psi$ è derivabile in $I$ . Inoltre $\forall\ t \in I$ 28/11 #TODO 
> 
