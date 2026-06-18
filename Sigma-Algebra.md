#IeS 
> [!warning] Definizione
> SI dice **Sigma-Algebra** di $\Omega$ una famiglia di sottoinsiemi di $\Omega$, Chiamata $\mathfrak{F}$ tale che:
> - $\Omega \in \mathfrak{F}$
> - $A \in \mathfrak{F} \implies (A^C = \Omega \setminus A) \in \mathfrak{F}$
> - $A_{i} \in \mathfrak{F};\ \forall\ i \in \mathbb{N} \implies  \bigcup\limits_{i=1}^\infty A_{i} \in \mathfrak{F}$

> [!info] Osservazione
> Una **Sigma-Algebra** di $\Omega$ è l'insieme dei sottoinsiemi "misurabili" di $\Omega$, quindi di [[Evento|Eventi]] di $\Omega$

> [!warning] Assiomi
> - **Non-negatività**: $P(A) \geq 0$
> - **Normalizzazione**: $P(\Omega) = 1$
> - **Additività**: $A \cap B = \emptyset \implies P(A\cup B) = P(A) + P(B)$
> Addendum:
> - $P\left( \bigcup\limits_{i=1}^\infty A_{i} \right) = \sum\limits_{i=1}^\infty P(A_{i})$

## Teoremi
- [[Teorema delle Probabilità Totali]]
- [[Teorema delle Probabilità Totali (Esteso)]]
- 