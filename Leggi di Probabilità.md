---
aliases:
  - Probability Mass Function
---
#IeS 
> [!error] Obiettivo:
> Passare da una notazione con gli eventi ad una con le [[Variabile Aleatoria|Variabili Aleatorie]]

> [!info] Esempio
> Evento: {Lo studente è alto 180 cm} $\to$ {H = 180}
> In generale, nel caso $\{ X=x \}$:
> $$P(\{ X=x \}) = P(\{ \omega \in \Omega: X(\omega) = x\}) = p_{X}(x)$$

> [!info] Osservazione
> $$\int_{-\infty}^\infty p_{X}(x) = 1;\ \forall\ X$$

---
> [!info] Esempio
> Sia $\Omega$ lo spazio campionario dei lanci di una moneta fino ad ottenere $T$, e sia $X(\omega):\Omega \to \mathbb{R}$ la variabile aleatoria che conta il numero di lanci fino ad ottenere la prima $T$, con $P(T) = p$.
> [[Leggi di Probabilità]]:
> $$
> P(X=k) = P(C\overset{k-1}{\dots} CT) =
> \begin{cases}
> (1-p)^{k-1}\cdot p & k=1,2,3,\dots \\
0 & \text{altrimenti}
> \end{cases}$$
> O anche definibile come 
> $$(1-p)^{k-1} \cdot p \cdot \mathbb{1}(k\in \mathbb{N})$$
> Utilizzando la [[Funzione Indicatrice]]

> [!warning] Notazione
> Se $X$ è una [[Variabile Aleatoria]], possiamo dire che $X$ si comporta come una [[Serie Geometrica]]:
> $$X \textasciitilde\  \mathrm{Geom}(p)$$
> Dove $p$ è il valore del primo elemento della serie

> [!info] Esempio
> Probabilità di ottenere $k$ teste in $n$ lanci con $P(T) = p$
> $$\binom{n}{k}p^k(1-p)^{n-k}$$
> quindi $X \textasciitilde \mathrm{Bin}(n,p)$

# Leggi di Probabilità Condizionata
> [!warning] Definizione
> Siano $A$, $B$ [[Evento|Eventi]], vogliamo definire $P(A|B)$ come operazioni su [[Variabile Aleatoria|Variabili Aleatorie]].
> $$A = \{ X=x \};\ B=\{ Y=y \}$$
> $$P(\{ X=x \} | \{ Y=y \}) = p_{X|Y}(x|y)$$
### Legge di Perdita di Memoria

> [!info] Esempio
> Siano $X$ numero di lanci di una moneta fino alla prima testa $T$, $Y$ il numero di lanci di una moneta a partire da 2 lanci dopo $X$, fino alla prima testa $T$.
> $$X \textasciitilde\ \mathrm{Geom}(p);\ Y \textasciitilde\ \mathrm{Geom}(p)$$
> Allora $\{ X - 2 | X > 2\ \} \textasciitilde\ \mathrm{Geom}(p)$, quidni
> $$p_{X-2|X > 2}(x) = p_{X}(x) = p_{Y}(x)$$

> [!warning] Legge
> Sia $X$ [[Variabile Aleatoria]] tale che $X \textasciitilde\ \mathrm{Geom}(p)$,
> $$p_{X - t | X > t}(k) = p_{X}(k)\ \ \forall\ t \in \mathbb{N}; k \in \mathbb{R}$$

> [!warning] Corollario
> Sia $X$ [[Variabile Aleatoria]] tale che $X \textasciitilde\ \mathrm{Geom}(p)$,
> $$E[X-t|X>t] = E[X]$$

---
> [!warning] [[Variabile Aleatoria Continua]]
> Nel caso di [[Variabile Aleatoria Continua]], l'equivalente vale per leggi $X \textasciitilde \mathrm{Exp}(\lambda)$
### Legge dell'Aspettativa Totale
> [!info] Esempio
> $A_{1}, A_{2}, A_{3}$ partizioni di $\Omega$.
> Probabilità totale di $B$:
> $$P(B) = P(A_{1})P(B|A_{1}) + P(A_{2})P(B|A_{2}) + P(A_{3})P(B|A_{3})$$
> Sia $B = \{ X = x \}$
> $$p_{X}(x) = P(A_{1})p_{X|A_{1}}(x) + P(A_{2})p_{X|A_{2}}(x) + P(A_{3})p_{X|A_{3}}(x)=$$
> $$\sum_{x\in \mathbb{R}} x\cdot p_{X}(x) =\sum_{x \in \mathbb{R}} x \cdot P(A_{1})p_{X|A_{1}}(x) +x \cdot P(A_{2})p_{X|A_{2}}(x) + x \cdot P(A_{3})p_{X|A_{3}}(x)=$$
> $$E[X] = P(A_{1})E[X|A_{1}] + P(A_{2})E[X|A_{2}] + P(A_{3})E[X|A_{3}]$$

> [!warning] Legge
> Siano $A_{1}, \dots, A_{n}$ partizioni di $\Omega$.
> $$E[X] = \sum_{i=1}^n p(A_{i})E[X|A_{i}]$$

### Legge di Probabilità Congiunta
[...]

### Legge di Probabilità Condizionata
> [!warning] Legge
> $$P_{X|Y}(x|y) = \dfrac{P(\{ X=x \} \cap \{  Y = y \})}{P(\{ Y=y \})}$$
> $$\frac{P_{X,Y}(x,y)}{P_{Y}(y)}$$