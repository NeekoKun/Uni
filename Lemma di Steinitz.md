#GAL 
> [!error] Teorema
> Sia $V = \mathrm{Span}(\underline{v_{1}},\dots,\underline{v_{m}})$ uno spazio vettoriale.
> Siano $\underline{w_{1}}, \dots, \underline{w_{n}} \in V$.
> Allora $n > m \implies \underline{w_{1}},\dots, \underline{w_{n}}$ sono linearmente dipendenti

> [!error] Dimostrazione
> Per ipotesi, ogni $\underline{w_{j}} \in V =\mathrm{Span}(\underline{v_{1}},\dots,\underline{v_{m}})$
> $$\implies \underline{w_{j}} = a_{1j}\underline{v_{1}} + a_{2j}\underline{v_{2}} + \dots + a_{mj}\underline{v_{m}} \forall\ j \in [1,n]$$
> $$= \sum_{i=1}^{n} a_{ij}\underline{v_{i}}$$
> Consideriamo $A = (a_{ij})\in \mathrm{Mat}(m,n)$
> Per ipotesi, $n > m \implies \mathrm{rK}(A) \leq m < n$
> Il sistema $A \underline{x} = \underline{0}$ ho infinite soluzioni (Rochè-Capelli)
> $\implies$ esistono soluzioni non nulle:
> $$\exists\ \underline{c} = \begin{pmatrix} c_{1} \\ c_{2} \\ \vdots \\ c_{n} \end{pmatrix} \neq \underline{0}: A \underline{c} = \underline{0}$$
> Cioè $\forall\ i\in[i,m]$
> $$\sum_{i=1}^{n} a_{ij}c_{j}=0 $$
> Consideriamo la seguente combinazione lineare:
> $$\sum_{j=1}^{n} c_{j} \underline{w_{j}}$$
> $$=\sum_{j=1}^{n} \left( c_{j} \sum_{i=1}^{m} a_{ij}\underline{v_{i}}  \right)$$
> $$= \sum_{j=1}^{n} \sum_{i=1}^{m} c_{j}a_{ij}\underline{v_{i}}$$
> $$= \sum_{i=1}^{m} \sum_{j=1}^{n} c_{j}a_{ij}\underline{v_{i}}$$
> $$= \sum_{i=1}^{m} \left( \sum_{j=1}^{n} c_{i}a_{ij} \right) \underline{v_{i}}$$
> $$= \sum_{i=1}^{m} 0 \underline{v_{i}} = 0 $$