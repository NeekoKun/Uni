#analisi 
## Limite Incrementale
> [!warning] Definizione (Limite Incrementale)
> Il **Limite Incrementale** di una funzione $f$ in $x_{0}$ è dato da:
> $$\lim_{ h \to 0 } \frac{f(x_{0}+h) - f(x)}{h}$$

## Derivate

> [!warning] Condizioni di Esistenza
> La **Derivata Prima** di una funzione $f$ può esistere solo se esiste il Limite Incrementale con $h \to 0^+$ e con $h \to 0^-$ esistono e coincidono. Quindi:
> $$\lim_{ h \to 0^+ } \frac{f(x_{0}+h) - f(x_{0})}{h} = \lim_{ h \to 0^- } \frac{f(x_{0}+h) - f(x_{0})}{h} = f'(x_{0}) \in \mathbb{R}$$

> [!warning] Definizione (Derivata Generale)
> La Derivata Prima della Derivata Prima di una funzione è la **Derivata Seconda**, e così via

> [!warning] Derivata di Funzioni definite a Tratti
> Basta derivare i tratti e definire la derivata a tratti a sua volta.
> Gli insiemi chiusi diventano aperti quando derivati. E.g.:
> $$ f(x) = |x| =
> \begin{cases}
> -x & x < 0 \\
> x & x \geq 0
> \end{cases} \\
> \implies f'(x) = 
> \begin{cases}
> -1 & x < 0 \\
> 1 & x > 0
> \end{cases}
> $$

## Teoremi
- [[Teorema della Catena]]
- [[Teorema della Derivata della Funzione Inversa]]
- 