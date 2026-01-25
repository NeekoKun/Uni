#analisi 
> [!warning] Definizione
> Data $f: I \subseteq \mathbb{R} \to \mathbb{R}$ e $F: I \subseteq \mathbb{R} \to \mathbb{R}$ diremo che $F$ è **Primitiva** di $f$ in $I$ se:
> - $F$ derivabile in $I$
> - $F'(x) = f(x)\ \forall\ x \in I$

> [!info] Osservazione
> Data $f : I \subseteq \mathbb{R} \to \mathbb{R}$, $I$ intervallo, non è detto che essa ammetta primitiva in $I$. Ad esempio: $$f: [-1, +1] \to \mathbb{R}:$$ $$f(x) = \begin{cases} 0 & x \in [-1, 0) \\ 1 & x \in [0, +1]\end{cases}$$
> Perché ha punto di discontinuità di salto in $x_{0} = 0$
> Per i teoremi visto sui punti di [[Continuità#Classificazione|Discontinuità]] delle funzioni che sono derivate di altre funzioni su un intervallo, $f$ non puù essere derivata di alcuna funzione $F:[-1, +1] \to \mathbb{R}$

> [!info] Osservazione
> Vedremo che $f:I \subseteq \mathbb{R} \to \mathbb{R}$, $I$ intervallo, e se $f$ è continua in $I$ allora essa ammette primitive in $I$ ([[Teorema Fondamentale del Calcolo Integrale I]])

> [!info] Osservazione
> Esistono funzioni discontinue che ammettono primitive, ma le discontinuità devono essere di **II specie**

> [!error] Proposizione
> Se $F : I \subseteq R \to \mathbb{R}$ è una primitiva di $f: I \subseteq \mathbb{R} \to \mathbb{R}$ e $c \in \mathbb{R}$, allora anche $$F(x) + c$$ è una primitiva di $f$ in $I$

> [!error] Proposizione
> Se $F_{1}, F_{2} : I \subseteq \mathbb{R} \to \mathbb{R}$ sono primitive di $f: I \subseteq \mathbb{R} \to \mathbb{R}$ un $I$, con $I$ intervallo, allora $\exists\ c \in \mathbb{R}:$ $$F_{1}(x) = F_{2}(x) + c$$

> [!info] Osservazione
> Se $f: I \subseteq \mathbb{R} \to \mathbb{R}$, $I$ intervallo, allora $f$ può non ammettere primitive in $I$.
> Se esiste primitiva $F: I \subseteq \mathbb{R} \to \mathbb{R}$ di $f$ in $I$, allora ve ne sono infinite, tutte e sole della forma $$F(x) + c$$ per $c \in \mathbb{R}$

> [!error] Dimostrazione
> 1. Se $F: I \subseteq \mathbb{R} \to \mathbb{R}$ è primitiva di $f$ in $I$ e $c \in \mathbb{R}$ allora $\forall\ x \in I$ $$(F+c)'(x) = F'(x) + 0 = f(x)$$
> Per definizione, $F+c$ è primitiva di $f$ in $I$
> 2. Siano $F_{1}, F_{2} : I \subseteq \mathbb{R} \to \mathbb{R}$, con $I$ intervallo, primitive in $I$ di $f: I \subseteq \mathbb{R} \to \mathbb{R}$
> Definiamo $G = F_{1} - F_{2}$, $G : I \subseteq \mathbb{R} \to \mathbb{R}$.
> Allora $G$ è derivabile in $I$ e $\forall\ x \in R$ vale $$G'(x) = (F_{1} - F_{2})'(x) = F_{1}'(x) - F_{2}'(x) = f(x) - f(x) = 0$$
> Poiché $G$ è definita su un intervallo $I$, deve essere
> $$G(x) = c\ \forall\ x \in I$$
> $$\implies F_{1}(x) - F_{2}(x) = c$$
> $$\implies \boxed{F_{1}(x) = F_{2}(x) + c}$$

- [[Integrale Indefinito]]
- [[Integrale Definito]]
- [[Classi di Funzioni Integrabili]]