#IeS 
## Storia
- Pascal
- Francesi
- Kolmogorov - [[Teoria Assiomatica delle Probabilità]]

## I Capitolo
- [[Spazio Campionario]]
- [[Sigma-Algebra]]
- [[Evento]]
- [[Indipendenza]]
- [[Indipendenza Condizionata]]
- [[Disposizioni]]
- [[Teorema di Weiss]]
- [[Distribuzioni di Probabilità#Discrete|Distribuzioni di Probabilità Discrete]]
## II Capitolo
- [[Variabile Aleatoria]]
- [[Leggi di Probabilità]]
- [[Funzione Indicatrice]]
- [[Valore Atteso]]
- [[Varianza]]
- [[Indipendenza Condizionata]]
- [[Variabile Aleatoria Continua]]
- [[Funzione Cumulativa di Probabilità]]
- [[Densità di Probabilità]]
- [[Regola di Bayes]]
- [[Delta di Dirac]] #TODO 
- [[Legge della Somma di Variabili Aleatorie]]
- [[Covarianza]]
- [[Disuguaglianza di Chebyshev]]
- [[Disuguaglianza di Markov]]
- [[Convergenza di Probabilità]]
- [[Media Campionaria]]
- [[Problema del Sondaggista]]
	- [[Teorema Fondamentale del Limite]]
- [[Stima]]
- [[Monte Carlo]]

## III Capitolo
- [[Processi Casuali]]
- 

## Appunti 1° Parziale
- Calcolo momento di Grado $n$
$$E[X^n] = \int x^nf_{X}(x)dx$$
- [[Disuguaglianza di Chebyshev]]
- [[Disuguaglianza di Markov]]
- $$\sum^n\mathcal{B}(p) = \mathrm{Bin}(n, p)$$
- $f_{Y|X}(y|x) = \frac{f_{X,Y}(x,y)}{F_{X}(x)}$
- Sia $Y = g(X)$, allora $$f_{Y}(y) = \frac{f_{X}(g^{-1}(y))}{\left|\frac{dg(x)}{dx}\right|_{x=g^{-1}(y)}}$$
- Bayes: $$f_{X|Y}(x|y) = \frac{f_{Y|X}(y|x)p_{X}(x)}{f_{Y}(y)}$$
- $E[XY|X] = XE[Y|X]$
- Convergenza di $\{ Y_{n} \}_{n}$ $$\lim_{ n \to \infty } P(|Y_{n} - \alpha| > \epsilon) = 0$$
- $$P(f(X)|f(Y)) \land X \perp Y \implies P(f(X))$$
- $$\mathrm{Var}[X+Y] = \mathrm{E}[\mathrm{Var}[X+Y|X]] + \mathrm{Var}[\mathrm{E}[X+Y|X]]$$
- $$\mathrm{Var}[M_{n}]  = \frac{\mathrm{Var}[X]}{n}$$
- $$X_{i} \perp X_{j}\ \forall\ i\neq j \in \mathbb{N} \implies  \mathrm{E}\left[ \prod_{i} X_{i} \right] = \prod_{i} \mathrm{E}[X_{i}]$$
- [[Covarianza]]
- $$\mathrm{Var}[X+Y] = \mathrm{Var}[X] + \mathrm{Var}[Y] + 2\mathrm{Cov}[X,Y]$$
- Coefficiente di Correlazione Lineare: $$p[X,Y] = \frac{\mathrm{Cov}[X,Y]}{\sqrt{ \mathrm{Var}[X]\mathrm{Var}[Y] }}$$
## Appunti 2° Parziale

- $S=\sum_{i=1}^NX_{i}$ $$\mathrm{E}[S] = \mathrm{E}[X]\cdot \mathrm{E}[N]$$$$\mathrm{Var}[S] = \mathrm{E}[N]\cdot \mathrm{Var}[X] + \mathrm{E}^2[X]\cdot \mathrm{Var}[N]$$
- $\mathrm{I}[A] = -\log_{2}{P(A)}\ [\text{bits}]$
- $\mathrm{E}[X] = \mathrm{E[\mathrm{E}[X|Y]]}$
- $\mathrm{Var}[X] = \mathrm{Var}[\mathrm{E}[X|Y]] + \mathrm{E}[\mathrm{Var}[X|Y]]$
- $\eta = \frac{1}{M}$
- $$\hat{\Theta}_{LIN}(X) = \mathrm{E}[\Theta] + \frac{\mathrm{Cov}(\Theta,X)}{\mathrm{Var}[X]} \cdot (X - \mathrm{E}[X]) $$
- Interarrivo $\mathrm{BP}[\lambda] = \mathrm{Geom}[\lambda]$
- $\mathrm{BP}[\lambda] + \mathrm{BP}[\gamma] = \mathrm{BP[\lambda + \gamma - \lambda \gamma]}$
- $P(X>Y) = \int_{-\infty}^\infty F_{Y}(X)f_{X}(x)dx$
- Puoi modellare $\mathrm{PP}$ congiunti come $\mathrm{BP}(\lambda)$ con $\lambda$ come rapporto dei carattere interessato sulla somma
- [[Stima]]
	- $\hat{\Theta}_{MAP}(X=x) = \underset{\theta}{argmax} f_{\Theta|X}(\theta|x)$
	- $\hat{\Theta}_{LMS}(X=x) = E[\Theta|X=x]$
- Entropia:
	- $H(X) = -\sum p(x)\log p(x) = -\int f_{X}(x)\log f_{X}(x)dx$
	- $H(X|Y) = H(X,Y) - H(Y)$
- Autoinformazione:
	- $i(A) = -\log(P(A))$
	- $i(x,y) = i(x|y) + i(y)$