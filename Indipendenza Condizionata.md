#IeS 
> [!warning] Definizione
> Siano $A$, $B$, $C$ eventi. Allora
> $$P(A\cap B | C) = P(A|C) \cdot P(B|C)$$

## Esempi
- In una famiglia ci sono 2 figli. Sapendo che almeno un figlio è maschio ed è nato di Martedì, qual'è la probabilità che anche l'altro figlio sia maschio ($\frac{13}{27}$)

Assunzioni:
- [[Indipendenza]] dei generi dei figli
- [[indipendenza]] dei giorni di nascita
- Equiprobabilità dei giorni di nascita e del genere
- $\to$ Spazio di probabilità uniforme

$M_{1}$: Primo figlio maschio
$M_{2}$: Secondo figlio maschio
$F_{1}$: Prima figlia femmina
$F_{2}$: Seconda figlia femmina

Lun$_{1}$ Figlio 1 nato di Lunedì
Lun$_{2}$ Figlio 2 nato di Lunedì
$\vdots$
Dom$_{1}$ Figlio 1 nato di Domenica
Dom$_{2}$ Figlio 2 nato di Domenica


|                   | $M_{2}\cap L_{2}$                                 | $\dots$  | $F_{2}\cap D_{2}$                                 |
| ----------------- | ------------------------------------------------- | -------- | ------------------------------------------------- |
| $M_{1}\cap L_{1}$ | $\frac{1}{2} \frac{1}{7} \frac{1}{2} \frac{1}{7}$ | $\dots$  | $\frac{1}{2} \frac{1}{7} \frac{1}{2} \frac{1}{7}$ |
| $M_{1}\cap M_{1}$ | $\frac{1}{2} \frac{1}{7} \frac{1}{2} \frac{1}{7}$ | $\dots$  | $\frac{1}{2} \frac{1}{7} \frac{1}{2} \frac{1}{7}$ |
| $\vdots$          | $\vdots$                                          | $\ddots$ | $\vdots$                                          |
| $F_{1}\cap D_{1}$ | $\frac{1}{2} \frac{1}{7} \frac{1}{2} \frac{1}{7}$ | $\dots$  | $\frac{1}{2} \frac{1}{7} \frac{1}{2} \frac{1}{7}$ |
