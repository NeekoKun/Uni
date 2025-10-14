#GAL 
> [!error] Teorema
> Dati $\underline{v_{1}},\dots,\underline{v_{n}} \in V$ **Linearmente Indipendenti** ma non generatori di $V$, allora $\exists\ \underline{v_{n+1}} \in V : \underline{v_{1}},\dots,\underline{v_{n+1}}$ sono ancora **Linearmente Indipendenti**

> [!error] Dimostrazione
> Per Ipotesi: $\mathrm{Span}(\underline{v_{1}}, \dots, \underline{v_{n}}) \neq V$
> $\implies \exists\ \underline{v_{n+1}}\in V: \underline{v_{n+1}}\not\in \mathrm{Span}(\underline{v_{1}}, \dots, \underline{v_{n}})$
> Supponiamo $$c_{1}\underline{v_{1}} + \dots + c_{n}\underline{v_{n}} + c_{n+1}\underline{v_{n+1}} = \underline{0}$$
> Devo dimostrare che $c_{1}=\dots=c_{n} = c_{n+1} = 0$
> $$c_{1}\underline{v_{1}} + \dots + c_{n}\underline{v_{n}} = -c_{n+1}\underline{v_{n+1}}$$
> $\implies c_{n+1} = 0$, altrimenti possiamo dividere ed ottenere $\underline{v_{n+1}}$ come combinazione lineare, ma $\underline{v_{n+1}}\not\in \mathrm{Span}(\underline{v_{1}},\dots,\underline{v_{n}})$
> $$\implies c_{1}\underline{v_{1}} + \dots + c_{n}\underline{v_{n}} = \underline{0}$$
> $\implies c_{1}=\dots=c_{n}=0$ perché sappiamo che sono Linearmente Indipendenti ==per Ipotesi== $\square$