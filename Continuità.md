#analisi 
> [!info] Osservazione
> Se $f$ non è definita in $x_{0}$ ma esiste $\lim_{ x \to x_{0} }f(x) = l \in \mathbb{R}$
> si può estendere per continuità di $f$ in $x_{0}$: $$\tilde{f}(x) = \begin{cases}f(x) & x \neq x_{0} \\ l & x = x_{0}\end{cases}$$
> La funzione $\tilde{f}$ ha dominio più grande del dominio di $f$ perché è definita anche in $x_{0}$, conincide con $f$ del dominio di $f$ ed è continua su $x_{0}$
> Vedremo che $$\lim_{ x \to 0 } \frac{\sin(x)}{x} = 1$$ quindi possiamo estendere per continuità $f(x) = \frac{\sin(x)}{x}$ in $x = 0$

## Classificazione
> [!warning] Definizione
> Se $\exists \lim_{ x \to x_0^+ } f(x) = l_{1},\ \lim_{ x \to x_0^- } f(x) = l_{2},\ l_{1} \neq l_{2}$ allora $x_{0}$ si dice **Punto di Discontinuità di I specie** o di tipo **salto** per $f$, con salto $$s(x_{0}) = l_{1} - l_{2}$$
> Se $f(x_{0}) = \lim_{ x \to x_{0}^- } f(x) = l_{2}$ diremo che $f$ è continua da destra, e viceversa

> [!warning] Definizione
> Se $\exists \lim_{ x \to x_{0}^+ } f(x) = l_{1},\ \lim_{ x \to x_{0}^- }f(x) = l_{2},\ l_{1} \neq l_{2}$ ed almeno uno dei due è uguale ad infinito o se uno dei due non esiste allora $x_{0}$ si dice **Punto di Discontinuità di II specie**
