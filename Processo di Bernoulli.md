#IeS 
> [!warning] Definizione
> Una sequenza di [[Variabile Aleatoria|Variabili Aleatorie]] di [[Distribuzioni di Probabilità#Distribuzione Bernoulliana|Bernoulli]] [[iid]].
> Sia $X_{i} \textasciitilde \mathrm{Bern}(p), X_{i}$ [[iid]],
> $$\mathrm{BP}(p) = \{ X_{1}, X_{2}, X_{3}, \dots X_{n} \}$$

> [!warning] Interpretazione del Processo di Bernoulli
> $$
> \Omega  = \begin{cases}
> 000\dots \\
> 001\dots \\
> \vdots \\
> 111\dots
> \end{cases}
> $$
> $$P(111\dots) = \lim_{ k \to \infty } P(\underset{k}{\underbrace{11\dots}}) = \lim_{ k \to \infty } (P(1))^k = \begin{cases}
> 1 & p=1 \\
> 0 & p<1
> \end{cases}$$
> $$P(000\dots) = \lim_{ k \to \infty } P(\underset{k}{\underbrace{00\dots}}) = \lim_{ k \to \infty } (P(0))^k = \begin{cases}
> 1 & p=0 \\
> 0 & p>0
> \end{cases}$$
> $0$ per tutti gli altri casi. $\Omega$ può quindi essere interpretato come uno spazio campionario uniforme tra $0$ ed $1$

## Splitting

> [!warning] Definizione
> Sia $X_{i}$ in un $\mathrm{BP}(p)$, $M_{1} \textasciitilde \mathrm{BP}(q)$ una [[Variabile Aleatoria]] [[Distribuzioni di Probabilità#Distribuzione Bernoulliana|Bernoulliana]] ausiliaria, e $Y_{i};\ Z_{i}$ due [[Variabile Aleatoria|Variabili Aleatorie]] in output dello splitting
> $$Y_{i} = \begin{cases}
> 0 & X_{i} = 0 \lor X_{i} = 1 \land M_{i} = 0 \\
> 1  & X_{i} = 1 \land M_{i} = 1
> \end{cases}$$
> $$Z_{i} = \begin{cases}
> 0 & X_{i} = 0 \lor X_{i} = 1 \land M_{i} = 1 \\
> 1  & X_{i} = 1 \land M_{i} = 0
> \end{cases}$$
> $$\implies P(Y_{i}) = P(X_{i}) \cdot P(M_{i}) = p\cdot q \textasciitilde \mathrm{BP}(p \cdot q)$$
> $$\implies P(Z_{i}) = P(X_{i}) \cdot (1- P(M_{i})) = p \cdot (1-q) \textasciitilde \mathrm{BP}(p \cdot (1-q))$$
> $$$$

#TODO 
> [!warning] Definizione
> Si può fare l'opposto, partendo da 2 Processi di Bernoulli, e ottenendo un processo $X$ tale che
> $$X \textasciitilde \mathrm{Bern}(p + q - p\cdot q)$$
## Esempi

> [!info] Esempio
> Numero di successi $S$ in $n$ istanti temporali
> $$S = \sum^n X_{i} \implies S \textasciitilde \mathrm{Binom}(n, p)$$
> $$\implies p_{S}(k) = \binom{n}{k}p^k(1-p)^{n-k}$$

> [!info] Esempio
> Tempi di Interarrivo: $T_{n}$ conta il numero di prove fino al successo $n$
> $$\mathrm{BP}(p) \implies T_{1} \textasciitilde \mathrm{Geom}(p) \iff p_{T_{1}}(t) = (1-p)^{t-1}p$$
> Ma per **Perdita di Memoria**, $T_{n}\textasciitilde T_{1} \implies T_{n}\textasciitilde \mathrm{Geom}(p)$

- > Chiedere per $T_{i} \textasciitilde \mathrm{Geom}(p) \textasciitilde L$

> [!info] Esercizio
> Calcolare il numero di prove per il $k$-esimo successo
> Sarebbe $$Y_{k} = \sum^kT_{i}$$
> Ma richiederebbe convoluzioni di [[Variabile Aleatoria|Variabili Aleatorie]] Infinite.
> Calcolando $P(Y_{k}=t) = P(BP[t] = 1\ \cap\ \text{k-1 successi nei primi t-1 slot} )$
> $$P(Y_{k} = t) = p \cdot \binom{t-1}{k-1}p^{k-1}(1-p)^{t-1-(k-1)} = \binom{t-1}{k-1}p^k (1-p)^{t-k}$$
> $$\mathrm{E}[Y_{k}] = \sum_{t=k}^\infty t\binom{t-1}{k-1}p^k(1-p)^{t-k}$$
> Ma questo è difficile, conviene il primo metodo:
> $$\mathrm{E}[Y_{k}] = \sum_{i=1}^k E[T_{i}] = k \cdot \frac{1}{p} = \frac{k}{p}$$
> $$\mathrm{Var}[Y_{k}] = \sum_{i=1}^k \mathrm{Var}[T_{i}] = k \cdot \frac{1-p}{p^2}$$
> $$Y_{k} \textasciitilde \mathrm{Pascal}(k, p)$$