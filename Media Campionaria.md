#IeS 

## Legge Debole dei Grandi Numeri
> [!warning] Definizione
> Prendiamo $x_{1},x_{2},\dots x_{n}$ n [[Variabile Aleatoria|Variabili Aleatorie]] [[iid]]
> Possiamo approssimare $$X \approx M_{n} = \frac{X_{1} + X_{2} + \dots + X_{n}}{n}$$
> dove $M_{n}$ è la **Media Campionaria**.
> Quindi:
> $$E[M_{n}] = E  \left[\frac{X_{1} + X_{2} + \dots + X_{n}}{n}\right] = \frac{{nE[X]}}{n} = E[X]$$
> $$\mathrm{Var}[M_{n}] = \mathrm{Var}\left[ \frac{{\sum_{1}^m X_{i}}}{n} \right] = \frac{1}{n^2} \sum_{1}^n\mathrm{Var}[X_{i}] = \frac{1}{n}\mathrm{Var}[X_{1}] = \frac{1}{n} \mathrm{Var}[X]$$
> Dunque:
> $$\lim_{ n \to \infty } \mathrm{Var}[M_{n}] = 0$$
> Per [[Disuguaglianza di Chebyshev]]:
> $$\lim_{ n \to \infty } P(|M_{n} - E[M_{n}]| > \epsilon ) \leq \lim_{ n \to \infty } \frac{\mathrm{Var}[X]}{E^2}$$
> E inoltre $$E[M_{n}] = E[X],\ \ \ \ \lim_{ n \to \infty } \frac{\mathrm{Var}[X]}{E^2} = 0$$
> $$\implies \lim_{ n \to \infty } P(|M_{n} - E[X]| > \epsilon) = 0\ \ \forall\ \epsilon > 0$$
> $$\implies \{ M_{n} \}_{n} \overset{P}{\to} E[X]$$