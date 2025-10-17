#analisi 
> [!error] Teorema
> Se la serie $\sum_{n=1}^{\infty} a_{n}$ Converge Assolutamente allora essa converge anche semplicemente. Inoltre in tal caso, $$\left| \sum_{n=1}^{\infty} a_{n} \right| \leq \sum_{n=1}^{\infty} |a_{n}| $$

> [!error] Dimostrazione
> $\forall\ n \in \mathbb{N}:$ $$0 \leq a_{n} + |a_{n}| \leq 2|a_{n}|$$
> Poichè $\sum_{n=1}^{\infty} |a_{n}|$ converge per ipotesi, per [[Criterio del Confonto per Serie a Termini non-negativi]], converge anche $$\sum_{n=1}^{\infty} a_{n} + |a_{n}|$$ inoltre $$\sum_{n=1}^{\infty} a_{n} = \sum_{n=1}^{\infty} (a_{n} + |a_{n}| - |a_{n}|)$$ $$=\sum_{n=1}^{\infty} (a_{n} + |a_{n}|) - \sum_{n=1}^{\infty} |a_{n}|$$
> Entrambe le serie all'ultimo membro convergono $$\implies \sum_{n=1}^{\infty} a_{n} \text{ converge}$$ 

> [!info] Osservazione
> Convergenza Assoluta -> Convergenza Semplice. Non viceversa.
> Esempio:
> - $\sum_{n=1}^{\infty} \frac{(-1)^n}{n^\alpha}:\alpha \in (0;1)$