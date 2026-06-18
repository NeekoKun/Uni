#IeS 
## Definizione
> [!warning] Definizione
> Vogliamo mantenere le proprietà di un [[Processo di Bernoulli]] ma esteso ad un tempo **Continuo**
> 1. **Omogeneità Temporale**: L'intensità degli arrivi è ==costante nel tempo==
> 2.
> 2. Numero di arrivi in un intervallo di tempo infinitesimo $$P(k, \delta) = \begin{cases} 1-\lambda \delta + \sigma(\delta) & k=0 \\ \lambda \delta + \sigma(\delta) & k=1 \\ \sigma(\delta) & k>1
\end{cases}$$ dove $\lambda = \lim_{ \delta \to 0 } \frac{E[\text{arrivi}]}{\delta}$
>
> Indicato come $\mathrm{PP}(\lambda)$
> Questo risulta in:
> $$f_{\mathrm{Pois}(\lambda\tau)}() = \frac{(\lambda \tau)^k e^{-\lambda \tau}}{k!}$$

> [!info] Osservazione
> Il modello tempo-discreto equivale ad un [[Processo di Bernoulli]] se $\delta$ è sufficientemente piccolo. In quel caso:
> $$\mathrm{PP}(\lambda) = \mathrm{BP}(\lambda \delta + \sigma(\delta)) = \mathrm{BP}(\lambda \frac{\tau}{n} + \sigma(\frac{\tau}{n}))$$
> $$P(\text{k arrivi in [0,t]}) = P(N_{[0,\tau]} = k) = \lim_{ n \to \infty } \binom{n}{k} \left( \frac{\lambda \tau}{n} \right)^k\left( 1 - \frac{\lambda \tau}{n} \right)^{n-k} = \frac{(\lambda \tau)^k}{k!}e^{-\lambda \tau}$$
> $$\implies N_{[0, \tau]} \textasciitilde \mathrm{Poisson}(\lambda \tau)$$

## Legge di Erlang

> [!info] Esempio
> Calcolo del tempo al $k$-esimo arrivo.
> Sia $Y_{k}$ una [[Variabile Aleatoria]] descrivente il tempo al $k$-esimo arrivo.
> $$f_{Y_{k}}(t) = \lim_{ \delta \to 0 } \frac{P(t < Y_{k} < t + \delta)}{\delta}$$
> $$P(t < Y_{k} < t + \delta) = P(k-1 \text{ arrivi in }[0,t]) \cdot P(1 \text{ arrivo in }[t, t+\delta])$$
> $$= \frac{(\lambda t)^{k-1} e^{-\lambda t}}{(k-1)!} \cdot (\lambda \delta + \sigma(\delta))$$
> $$\implies f_{Y_{k}} = \frac{(\lambda t)^{k-1} e^{-\lambda t}}{(k-1)!} \cdot \lambda$$
> $$\implies Y_{k} \textasciitilde \mathrm{Erlang}(k,\lambda)$$