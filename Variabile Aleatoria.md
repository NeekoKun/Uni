---
aliases:
  - Variabili Aleatorie
---
#IeS 
> [!warning] Definizione
> Sia $\Omega$ uno spazio di probabilità, possiamo definire una funzione $H: \Omega \to \mathbb{R}$, chiamata "**Variabile Aleatoria**", che mappa ad ogni evento $\omega$ un valore in $\mathbb{R}$

> [!info] Esempio
> Sia $\bar{H}(\omega) = \dfrac{H(\omega)}{100}$, questa rimane una **Variabile Aleatoria**.

> [!info] Osservazione
> Sia $H: \Omega\to \mathbb{R};\ f:\mathbb{R}\to \mathbb{R}$, allora $f \circ H$ è una **Variabile Aleatoria**

> [!warning] Variabili Aleatorie Indipendenti
> Siano $X$, $Y$ [[Variabile Aleatoria|Variabili Aleatorie]]. Queste sono indipendenti se e solo se:
> $$P_{X,Y}(x,y) = P_{X}(x)P_{Y}(y)\ \ \forall\ (x, y) \in \mathbb{R}^2$$

## Trasformazione Monotona di Variabile Aleatoria
> [!warning] Definizione
> Sia $Y = g(x)$ con $g$ funzione nota e deterministica, strettamente monotona
> Allora se prendiamo un intervallo $[x, x+\delta]$, questo verrà mappato a $[y, y+\epsilon]$, dove:
> $$y = g(x)$$
> $$y+\epsilon = g(x+\delta)$$
> $$\implies [y, y+\epsilon] = [g(x), g(x+\delta)]$$.
> Gli eventi possono essere rappresentati come
> $$\{ x \leq X \leq x + \delta_{x} \} = \{ y \leq Y \leq g(x + \delta_{x}) \}$$
> Ma per un $\delta_{x}$ abbastanza piccolo, abbiamo
> $$\{  g(x) \leq Y \leq g(x + \delta_{x}) \} = \left\{  g(x) \leq Y \leq g(x) + \delta_{x}\cdot\left| \frac{dg(x)}{dx}\right|  \right\}$$
> Dove per definizione $$\delta_{x} \cdot \left|\frac{dg(x)}{dx}\right| = \delta_{y}$$
> ---
> Riscrivendo con $\delta_{y}$:
> $$P(x \leq X \leq x + \delta_{x}) = P(g(x) \leq Y \leq g(x) + \delta_{y})$$
> $$\implies \delta_{x}f_{X}(x) = \delta_{y}f_{Y}(g(x))$$
> $$\implies f_{Y}(g(x)) = \frac{f_{X}(x)}{\left|\frac{dg(x)}{dx}\right|}$$
> Notiamo che $y = g(x)$ e $x = g^{-1}(y)$ in quanto $g$funzione strettamente monotona, quindi, in $y$:
> $$f_{Y}(y) = \frac{f_{X}(g^{-1}(y))}{\left| \frac{dg}{dx} (g^{-1}(y)) \right|}$$

## Esempi
$Y = X^3$
$g(x) = x^3$, $g^{-1}(y) = y^{\frac{1}{3}}$
$\frac{dg}{dx} = 3x^2$, 
$$f_{Y}(y) = \frac{f_{X}(y^{1/3})}{| 3y^{2/3} |}$$
---
$Y = X^2$
$g(x) = x^2$

$$f_{Y}(y) = P(X < 0)f_{Y|X<0}(y) + P(X \geq 0)f_{Y|X\geq0}(y)$$

## Notazione
- Lettere maiuscole indicano la **Variabile Aleatoria**
- Lettere minuscole indicano i valori numerici, anche chiamati ==Realizzazioni==