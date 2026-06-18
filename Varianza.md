#IeS 

> [!warning] Definizione
> La **Varianza** è
> $$\mathrm{Var}(x) = E[(X - E[X])^2] = E[X^2] - E[X]^2$$

## Proprietà

- $\mathrm{Var}[X] \geq 0$
- $\mathrm{Var}[aX + b] = \mathrm{Var}[aX] = a^2\mathrm{Var}[X]$
### Varianza della [[Variabile Aleatoria]] Binomiale

> [!warning] Definizione
> Sia $X: \Omega \to \mathbb{R} \textasciitilde \mathrm{Bin}(n,p)$
> $$\mathrm{Var}[X] = n \cdot p \cdot (1 - p)$$

# Varianza per [[Variabile Aleatoria|Variabili Aleatorie]] Multiple

> [!warning] Definizione
> Consideriamo $X,Y:\Omega \to \mathbb{R}$
> $$\mathrm{Var}[X + Y] = \mathrm{Var}[X] + \mathrm{Var}[Y] + 2(E[XY] - E[X]E[Y])$$

> [!info] Osservazione
> $$X \perp Y \implies \mathrm{Var}[X+Y] = Var[X] + Var[Y]$$


# Varianza per [[Variabile Aleatoria]] Continua

> [!warning] Definizione
> Stessa identica cosa.
> $$\mathrm{Var}[X] = E[X^2] - E[X]^2$$