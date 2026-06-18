#IeS 
> [!warning] Presentazione
> Come faccio a determinare una preferenza in una popolazione campionando tale popolazione?

> [!error] Definizione
> Sia $f$ la frazione di persone che soddisfa un'evento $A$, $n$ il numero di persone selezionate dal sondaggista.
> Per l'$i$-esima persona estratta, registriamo la risposta:
> $$X_{i} = \begin{cases} 1 & \text{Se A verificato per la persona i-esima} \\
> 0  & \text{Altrimenti}\end{cases}$$
> Quindi $X_{i} \textasciitilde \mathrm{Bern}(f)$, [[iid]], e sappiamo che
> $$p_{X_{i}}(1) = f,\ \ \ E[X_{i}] = f,\ \ \ \mathrm{Var}[X] = f \cdot(1 - f)$$
> Utilizzando la [[Media Campionaria]]
> $$M_{n} = \frac{\sum_{1}^nX_{i}}{n} = \hat{f} \text{ stima di } f$$
> Volendo massimizzare $P(|\hat{f} - f| < \epsilon)$
> $$P(|M_{n} - f| \leq \epsilon) \geq P_{min}$$
> Dove $P_{min}$ è detto "Livello Fiduciario" (Confidence Level) ed $\epsilon$ è detto "accuratezza"
> Cerchiamo $n$ min tale che $P_{min} >$ di un certo valore, diciamo $0.95$
> Per [[Disuguaglianza di Chebyshev]]
> $$P(|M_{n} - E[M_n]| \geq \epsilon) \leq \frac{\mathrm{Var}[M_{n}]}{\epsilon^2}$$
> $$\mathrm{Var}[M_{n}] = \frac{\mathrm{Var}[X_{i}]}{n} = \frac{f \cdot (1-f)}{n}$$
>$$\implies P(|M_{n} - E[M_n]| \geq \epsilon) \leq \frac{f \cdot (1 - f)}{n \epsilon^2}$$
>Ma sappiamo che $\mathrm{Max}(\mathrm{Bern}(f)) = \frac{1}{4}$
>$$\implies P(|M_{n} - E[M_n]| \geq \epsilon) \leq \frac{1}{4 n \epsilon^2}$$
>$$\implies \frac{1}{4 n \epsilon^2} \leq 1 - P_{min}$$

> [!info] Ottimizzazione
> Vogliamo usare una disuguaglianza migliore per le [[Media Campionaria|Medie Campionarie]], utilizzando il [[Teorema Fondamentale del Limite]]
> $$|M_{n} - f| \geq \epsilon \implies \left| \frac{S_{n} - nf}{n}\right| \geq \epsilon$$
> $$\implies \left|\frac{{S_{n} - nf|}}{\sqrt{ n } \sigma} \right| \geq \frac{\epsilon \sqrt{ n }}{\sigma}$$
> $$P\left(|Z_{n}| \geq  \frac{\epsilon \sqrt{ n }}{\sigma}\right) = P\left( |Z_{n} \geq \epsilon \sqrt{ \frac{n}{f(1-f)} } \right) = P(|Z_{n}| \geq 2\epsilon \sqrt{ n } )$$
> E per il [[Teorema Fondamentale del Limite]]
> $\approx P(|Z| \geq 2 \epsilon \sqrt{ n }); \ \ \ Z \textasciitilde N(0, 1)$
> $= 2(1 - \Phi(2\epsilon \sqrt{ n })) \leq 1 - P_{min}$
> $= \Phi(2 \epsilon \sqrt{ n }) \geq 1 - \frac{1 - P_{min}}{2}$