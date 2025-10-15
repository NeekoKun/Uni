#GAL 
> [!error] Teorema
> Sia $H \subseteq V$, allora:
>1. $\mathrm{Dim}(H) \leq \mathrm{Dim}(V)$
>2. $\mathrm{Dim}(H) = \mathrm{Dim}(V) \implies H = V$

> [!error] Dimostrazione
> Sia $\{ \underline{v}_{1},\dots,\underline{v}_{n} \}$ una base di $H$- ($n = \mathrm{Dim}(V)$)
> 1. $\underline{v}_{1}, \dots, \underline{v}_{n}$ sono n vettori in $V$ linearmente indipendenti
> $\implies \mathrm{Dim}(H) = n \leq$ max numero di vettori L.I. in $V = \mathrm{Dim}(V)$
> 2. Supponiamo per assurdo che $\mathrm{Dim}(H) = \mathrm{Dim}(V)$ e $H \neq V$. Cioè $H = Span(\underline{v}_{1}, \dots, \underline{v}_{n}) \subset V$
> [[Lemma di Aggiunta]]: $\exists \underline{v}_{n+1} \in V : \underline{v}_{1},\dots,\underline{v}_{n+1} \in V$ sono Linearmente Indipendenti
> $\implies n+1 \leq$ max numero di vettori L.I. in $V = \mathrm{Dim}(V) = \mathrm{Dim}(H) = n$
> $\implies$ assurdo