#analisi 
Sia $X=\mathbb{R} \lor X=\mathbb{Q}$, consideriamo sempre E sottoinsieme X  (non vuoto)
> [!warning] Definizione
> - L'insieme si dice limitato superiormente o dall'alto se esiste $k \in X\ |\ x \leq k, \forall\ x \in E$
> - L'insieme si dice limitato inferiormente o dal basso se esiste $k \in X\ |\ x \geq k\ \forall\ x \in E$
> - L'insieme si dice limitato se sia limitato superiormente che inferiormente

> [!warning] Definizione
>- Dato E in X non vuoto, $x_0 \in X, x_0$ si dice:
>	- Massimo di E se:
>		- $x_0 \in E$
>		- $x_0 \geq x\ \forall\ x \in E$
>	- Minimo di E se same thing
>- Condizione necessaria:
>	- L'insieme dev'essere limitato dal verso giusto

> [!info] Osservazione
>  Non sempre esistono $max E$, $min E$, seppure è sia limitato dal lato giusto

> [!info] Osservazione 
> - E sott X non vuoto, $k,h \in X$
> - k è maggiorante solo se $k \geq x\ \forall\ x \in E$
> - k è minorante solo se $h \leq  x\ \forall\ x \in E$

> [!info] Osservazione
> - Se esiste un maggiorante, l'insieme è limitato dall'alto
> - Se esiste un minorante, l'insieme è limitato dal basso

> [!info] Osservazione
> - Se k è maggiorante di E, ogni $a \geq k$ è maggiorante di E
> - Se h è un minorante di E, ogni $b \leq h$ è minorante di E
> - Se k è maggiorante di  E, e $k \in E$, $max E = k$
> - Se h è minorante di E, e $h \in E$, $min E=h$

> [!info] Esempio
> - $E = \{ r\in \mathbb{Q}: r\geq 0,\ r^2 \leq 2\}$ sott. $\mathbb{R}$
> - ogni $k \geq \sqrt2$ maggiorante
> - ogni $h \leq 0$ minorante
> - $inf E = 0 = min E$
> - $sup E =  \sqrt2\ \nexists\ max E$
> - $E = \{ r\in \mathbb{Q}: r\geq 0,\ r^2 \leq 2\}$ sott. $\mathbb{Q}$
> - ogni $k \geq \sqrt2$ maggiorante
> - ogni $h \leq 0$ minorante
> - $inf E = 0 = min E$
> - $\nexists\ sup E,\ \nexists\ max E$

> [!warning] Definizione
> - Sia E sott. X nn vuoto. Se esistono maggioranti, cioè se E è limitato dall'alto, chiameremo estremo superiore e lo indichiamo con sup E il minimo dei maggioranti
> - Sia E sott. X nn vuoto. Se esistono minoranti, cioè se E è limitato dal basso, chiameremo estremo inferiore e lo indichiamo con inf E il massimo dei minoranti

## Esempi
- e.g. $E = \mathbb{N}$
	- $\nexists sup\mathbb{N}$
	- $infE = 0 = minE$
- e.g. $E=\left\{  \frac{1}{n}: n\in \mathbb{N}, n\neq {0}  \right\}$
	- $E$ è limitato
	- $max\ E=1$
	- $min\ E$ non esiste
	- $sup E = max  E= 1$
	- $\nexists\ min E,\ inf E = 0$
## Proprietà dell'Estremo Superiore
- x soddisfa la proprietà dell'estremo superiore se ogni sottoinsieme non vuoto E, contenuto in x e limitato dall'alto possiede estremo superiore $supE \in X$
- Same with inferiore
- Prende il nome di [[Assioma di Completezza di R]]

> [!warning] Definizione ([[Assioma di Completezza di R]]):
> - $\mathbb{R}$ è l'unico campo ordinato che soddisfa la proprietà dell'estremo superiore

> [!info] Osservazione
> - Le proprietà dell'estremo superiore e dell'estremo inferiore sono equivalenti
> - $\mathbb{Q}$ non soddisfa la proprietà dell'Estremo Superiore
> - Dato $E \subset   R,\ maxE/minE \implies maxE=supE/minE=infE$
> - $supE \in E \implies maxE = supE$

> [!warning] Definizione
>- $\text{Insieme illimitato dall'Alto} \Leftrightarrow supE=+\infty$
> - $\text{Insieme illimitato dal Basso} \Leftrightarrow infE=-\infty$

> [!info] Osservazione
> - Dato E sott R nn vuoto, esistono sempre supE, infE in $\overline{\mathbb{R}}  =\mathbb{R}\ \cup \pm \infty$
> - E sott. R non vuoto e limitato dall'alto, x* << R è supE se
> 1) x <= x* po. x \in E
> 2) $\forall\ k < x^* \exists\ x \in E\ |\ k < x \leq x^*$
> 	- Cioè x* è il più piccolo dei maggioranti
> - E sott. R, limitato dal basso,allora x_* \in R + inE se
> 1) $x_{*} \leq x\ \forall\ x \in E$
> 2) $\forall\ h > x\ \exists\ x \in E\ |\ x_{*}\leq x<h$ 

