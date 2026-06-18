---
aliases:
  - Expected Value
---
#IeS 

> [!info] Esempio
> Scommettendo €1 ad un gioco, abbiamo la seguente [[Leggi di Probabilità]] per la vittoria:
> $$p_{X}(x) = \begin{cases}
> \frac{1}{6} & x=1 \\
> \frac{1}{2} & x=2 \\
> \frac{1}{3} & x=4 \\
> 0 & altrimenti
> \end{cases}$$
> Su $n$ giocate, il valore atteso è
> $$n\left( \frac{1}{6} \cdot 1 + \frac{1}{2} \cdot 2 + \frac{1}{3} \cdot 3 \right) = 2.5n$$
> ovverosia la media pesata delle Realizzazioni, dove i pesi sono le probabilità

> [!warning] Definizione
> In generale, il valore atteso è:
> $$E[X] = \sum_{x \in \mathbb{R}} x p_{X}(x)$$
> Informalmente, $E[X]$ è il baricentro delle $p_{X}$

> [!warning] Definizione
> $E[X], E[X^2], E[X^3], \dots, E[X^n]$ sono detti **Momenti della [[Variabile Aleatoria]] X**, dove
> $E[X^n]$ è il Momento di Ordine n
> $E[(X-E[X])^n]$ è detto il **Momento Centrato di Ordine n della [[Variabile Aleatoria]] X**, [[Varianza]] nel caso $n = 2$

## Proprietà

### Linearità
> [!warning] Proprietà
> Sia $X: \Omega\to \mathbb{R}$, allora
> $$E[aX+b] = aE[X] + E[b]$$

### Legge dello Statistico Inconsapevole (Law of the Unconscious Statistician - LOTUS)
Siano $X:\Omega\to \mathbb{R};\ g:\mathbb{R} \to \mathbb{R};\ Y = g(X)$
Calcoliamo $E[Y]$ conoscendo $p_{X}$ e $g$
$$E[Y] = \sum_{y\in \mathbb{R}} y \cdot p_{Y}(y)$$
$$= \sum_{y\in \mathbb{R}} y \cdot \sum_{x : g(x) = y} p_{X}(x) = \sum_{y\in \mathbb{R}} \sum_{x : g(x) = y} y p_{X}(x) = \sum_{y\in \mathbb{R}} \sum_{x : g(x) = y} g(x) p_{X}(x)$$
ma visto che eventualmente sommeremo ogni $x \in \mathbb{R}$:
$$\sum_{x \in \mathbb{R}} g(x)p_{X}(x) = E[g(X)]$$
> [!info] Esempio
> Abbiamo $X$ rappresentante temperatura in °C
> $Y$ rappresentante la temperatura in °F
> dove $g(x) = ax + b$ e $Y = g(x)$
> allora
> $$E[Y] = E[g(X)] = E[aX + b] = \sum_{x\in \mathbb{R}} axp_{X}(x) + \sum_{x \in \mathbb{R}} bp_{X(x)}$$
> $$ = a \sum_{x \in \mathbb{R}} xp_{X}(x) + b\sum_{x \in \mathbb{R}} p_{X}(x)$$
> $$ = aE[X] + b = g(E[X])$$

> [!warning] Proprietà
> Se $g(x)$ è lineare in $\mathbb{R}$, allora $E[g(X)] = g(E[X])$

### Valore Atteso della [[Variabile Aleatoria]] Binomiale

> [!warning] Definizione
> Sia $X: \Omega \to \mathbb{R} \textasciitilde \mathrm{Bin}(n,p)$
> $$E[X] = n \cdot p$$ 

# Valore Atteso Condizionato
> [!warning] Definizione
> Siano $A$, $B$ eventi, dove
> $$A = \{ X=x \};\ B=\{ Y=y \}$$
> $$E[X|B] = \sum_{ x \in \mathbb{R}} x \cdot p_{{X|B}}(x)$$

# Valore Atteso per [[Variabile Aleatoria|Variabili Aleatorie]] Multiple

> [!warning] Definizione
> $$E[g(X,Y)] = \sum_{(x,y) \in \mathbb{R}^2} g(x,y)\cdot p_{X,Y}(x,y)$$

## Casi Particolari
- $g(X,Y) = X^kY^i \to E[X^kY^i]$ sono detti "**Momenti Congiunti di $X$ e $Y$**"
	- $E[g(X,Y)] \neq g(E[X],E[Y])$ a meno che:
		- $g(X,Y) = aX+bY+c;\ \ a,b,c \in \mathbb{R}$
		- $X \perp Y \implies E[XY] = E[X]E[Y]$


# Valore Atteso per [[Variabile Aleatoria]] Continua

> [!warning] Definizione
> $$E[X] = \int_{-\infty}^\infty xf_{X}(x) dx$$