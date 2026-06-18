#IeS 
> [!warning] Definizione
> Voglio trovare valori per $a$ e $b$ tali che 
> $$\hat{\Theta}_{LIN}(X) = aX+b$$
> minimizzi
> $$E[(\Theta - \hat{\Theta}_{LIN}(X))^2]$$
> quindi
> $$[a^*,b^*] = \underset{a,b}{\mathrm{argmin}}\ E[(\Theta - \hat{\Theta}_{LIN})^2]$$
> $$ = \underset{a,b}{\mathrm{argmin}}\ E[(\Theta - aX + b)^2]$$
> $$ = \underset{a,b}{\mathrm{argmin}}\ h(a,b)$$
> essendo un paraboloide, è sufficiente trovare il [[Punti Stazionari|Punto Stazionario]]
> $$\begin{cases}
> \frac{\partial}{\partial a}h(a,b) = 0 \\
> \frac{\partial}{\partial b}h(a,b) = 0
> \end{cases} \implies \begin{cases}
> a^* = \frac{\mathrm{Cov}[X,\Theta]}{\mathrm{Var}[X]} \\
> b^* = E[\Theta] - a^* E[X]
> \end{cases}$$
> $$\implies \hat{\Theta}_{LIN}(X) = E[\Theta] + \frac{\mathrm{Cov}[X,\Theta]}{\mathrm{Var}[X]} \cdot (X - E[X])$$

> [!info] Osservazione
> Per trovare $\hat{\Theta}_{LIN}$ devo solo valutare statistiche del primo ordine e del secondo ordine

---

### Stima con più Osservazioni
> [!warning] Definizione
> Impongo di trovare una stima lineare delle $X_{i}$:
> $$\hat{\Theta}_{LIN} = a_{1}X_{1} + a_{2}X_{3}+\dots + a_{n}X_{n} + b$$
> in modo da minimizzare $$E[(\Theta - \hat{\Theta}_{LIN})^2]$$
> Analogamente a prima, possiamo dimostrare che i coefficienti ottimi si possono calcolare utilizzando i momenti del primo e del secondo ordine di $X_{i}$ e $\Theta$

> [!info] Osservazioni
> Quando tutte le [[Variabile Aleatoria|Variabili Aleatorie]] sono Gaussiane, allora $$\hat{\Theta}_{LIN} = \hat{\Theta}_{LMS} = \hat{\Theta}_{MAP}$$