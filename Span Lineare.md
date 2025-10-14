#GAL 
> [!warning] Definizione
> Dati $v_{1}, v_{2}, \dots, v_{n}\in V$ il loro **Span Lineare** è l'insieme di tutte le loro [[Combinazione Lineare|combinazioni lineari]]
> $$\mathrm{Span}(\underline{v_{1}},\dots, \underline{v_{n}}) = \{ \underline{u} \in V: \underline{u}=c_{1}\underline{v_{1}}+c_{2}\underline{v_{2}}+\dots+c_{n}\underline{v_{n}} \text{ per qualche } c \in \mathbb{R} \}$$
> $$= \left\{  \sum c_{i}\underline{v_{i}}: c\in \mathbb{R}  \right\}$$
### Proprietà
- Dati $\underline{v_{1}}, \underline{v_{2}},\dots, \underline{v_{n}} \in V, \mathrm{Span}(\underline{v_{1}}, \underline{v_{2}}, \dots, \underline{v_{n}})$ è uno [[Spazi Vettoriali|Spazio Vettoriale]]

> [!error] Dimostrazione
> 1. $\underline{0} \in \mathrm{Span} \Leftrightarrow \underline{0} = 0\underline{v_{1}}+0\underline{v_{2}}+\dots+0\underline{v_{n}}$
> 2. Dati $\underline{u}, \underline{w} \in H \implies \underline{u}+\underline{w}\in H$
> $$
> \underline{u} = \sum c_{i}\underline{v_{i}}, \underline{w} = \sum d_{i}\underline{v_{i}} \\
> \implies \underline{u} + \underline{w} = \boxed{\sum (c_{i} + d_{i}) \underline{v_{i}} \in H}
> $$
> 3. Dato $\underline{u} \in H, c \in \mathbb{R} \implies c \underline{u} \in H$
> $$\underline{u} = \sum b_{i} \underline{u_{i}} \\
> \implies c \underline{u} = c \sum b_{i} \underline{u_{i}} \\
> \implies c \underline{u} = \boxed{\sum (c b_{i}) \underline{u_{i}} \in H}
> $$