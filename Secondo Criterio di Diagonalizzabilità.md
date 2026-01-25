#GAL 
> [!error] Teorema
> $L: V \to V$ $\mathrm{dim}V = n$, $\lambda_{i},\ \dots,\ \lambda_{r}$ Autovalori di $V$
> $L$ è diagonalizzabile $\Leftrightarrow$ $$g_{\lambda_{i}} = a_{\lambda_{i}}\ \forall\ i, \sum_{i=1}^r a_{\lambda_{i}} = n$$ $$\sum_{i=1}^rg_{\lambda_{i}} = n$$
> In questo caso.:
> Se $B_{i}$ è una base di ciascu autospazio di $E_{\lambda_{i}}$ allora $B_{1} \cup B_{2} \cup \dots \cup B_{r}$ è una base di $V$ di autovettori di $L$

> [!info] Esempi
> 1. $A = \begin{pmatrix}1 & 1\\1 & 1\end{pmatrix}$ è diagonalizzabile
> $\chi_{A}(x) = -x(2-x)$
> $a_{0} = a_{2} = 1$
> $g_{0} = g_{2} = 1$
> 2. $A = \begin{pmatrix}0 & -1\\1 & 0\end{pmatrix}$ non è diagonalizzabile
> $\chi_{A}(x) = x^2 + 1$
> $\sum a_{\lambda} = 0 < 2 \implies$ Non abbiamo abbastanza autovettori
> 3. $A = \begin{pmatrix}1 & 1\\0 & 1\end{pmatrix}$ non è diagonalizzabile
> $\chi_{A}(x) = (1-x)^2$
> $a_{1} = 2 \implies \sum a_{\lambda} = 2$
> $g_{0} = g_{1} = 1$