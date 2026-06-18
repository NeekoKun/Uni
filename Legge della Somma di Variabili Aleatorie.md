---
aliases:
  - Somma di Convoluzione
---
#IeS 
> [!warning] [[Variabile Aleatoria|Variabili Aleatorie]] Discrete
> Siano $X$, $Y$ [[Variabile Aleatoria|Variabili Aleatorie]] discrete, con $X \perp Y$
> Sia $W = X + Y$, allora:
> $$P(W = w) = P(X+Y = w) = \sum_{x+y=w}P_{X,Y}(x,y)=$$
> $$= \sum_{x+y=w}p_{X}(x)p_{Y}(y) = \boxed{\sum_{x}p_{X}(x)p_{Y}(w-x)}$$
> chiamata "**Somma di Convoluzione**"

> [!warning] [[Variabile Aleatoria|Variabili Aleatorie]] Continue
> Siano $X$, $Y$ [[Variabile Aleatoria Continua|Variabili Aleatorie Continue]], $X \perp Y$
> Sia $W = X + Y$, quindi
> $$f_{W}(w) =\boxed{ \int_{-\infty}^\infty f_{X}(x)f_{Y}(w-x)dx}$$
> chiamato "**Integrale di Convoluzione**"

> [!warning] [[Variabile Aleatoria|Variabili Aleatorie]] Gaussiane
> #TODO 
