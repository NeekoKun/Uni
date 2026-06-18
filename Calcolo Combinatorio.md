#IeS 

## Operazioni
$$P(B \cup C | A) = P(B|A) + P(C|A)$$$$P(B \cap C | A) = P(B|A) \cdot P(C|A)$$

## Principi di Calcolo Combinatorio
- Spezzare il Problema in Stadi di Scelta
Supponiamo di Avere $r$ stadi di scelta
$n_{i}$: # scelte nello stadio $i$
$$\prod_{i=1}^rn_{i} = \text{Numero di Foglie}$$

e.g. Contare quante targhe possono esistere
$r = 7$
$n_{1} = n_{2} = n_{6}=n_{7}=26$
$n_{3}=n_{4}=n_{5} = 10$
$f = 26^4\cdot10^3$

e.g. Contare il numero di targhe che non contengono ripetizioni di lettere o cifre
$r=7$
$n_{1} = 26$
$n_{2} = 25$
$n_{3} = 10$
$n_{4}=9$
$n_{5}=8$
$n_{6}=24$
$n_{7} = 23$
$f=26\cdot 25 \cdot 24 \cdot 23 \cdot 10 \cdot 9 \cdot 8$

e.g. In quanti modi posso ordinare gli elementi di $A = \{ 1,2,3,4 \}$
$r=4$
$n_{1} = 4$
$n_{2} = 3$
$n_{3} = 2$
$n_{4} = 1$
$f=4! = 24$

e.g. Contare il numero di sottoinsiemi di un insieme $A:|A| = n$
$r=n$
$n_{i} = 2\ \forall\ i$
$f = 2^n$

e.g. Calcolare la probabilità che 6 lanci di un dado ben bilanciato diano 6 numeri diversi
$r = 6$
$n_{1} = 1$
$n_{2} = \frac{5}{6}$
$n_{3} = \frac{4}{6}$
$\vdots$
$f=\frac{6!}{6^6}$

## Coefficiente Binomiale

e.g. Contare il numero di sottoinsiemi con $k$ elementi distinti che si possono formare partendo da un insieme di $n$ elementi
$\dfrac{n!}{k!(n-k)!} = \binom{n}{k}$

e.g. $n$ lanci di moneta indipendenti, $P(T) = p$
$P(TCCTTT) = P(T)P(C)P(C)P(T)P(T)P(T) = p^4(1-p)^2$
generalmente:
$P(\text{una sequenza con kT, (n-k)C}) = p^k(1-p)^{n-k}$
$P(kT, n \text{ lanci}) = p^k(1-p)^{n-k} \cdot\text{n° sequenze con kT e (n-k)C} =$
$$=p^k(1-p)^{n-k}\cdot\binom{n}{k}$$

> [!warning] Schema Generale
> Ho $n$ prove indipendenti, probabilità di "successo" $p$.
> Qual'è la probabilità di avere $k$ successi su $n$ prove indipendenti? [[Probabilità Binomiale]]

e.g. Lanci di moneta indipendenti, $P(T) = p$
$B = \{ \text{3 lanci su 10 sono T} \}$
$A = \{ \text{primi 2 lanci sono T} \}$
$P(A|B) = \frac{P(A\cap B)}{P(B)}$

$B$ è uno spazio di probabilità Uniforme Discreto
$$\implies \frac{P(A\cap B)}{P(B)} = \frac{|A \cap B|}{|B|}$$
$|B| = \binom{10}{3}$
$|A\cap B| = \dfrac{8}{\binom{10}{3}}$

## Coefficiente Multinomiale

$n$ prove indipendenti
Generalizziamo oltre al binario
$n_{1}$ di tipo 1
$n_{2}$ di tipo 2
$n_{3}$ di tipo 3
$n_{4}$ di tipo 4
$n_{1} + n_{2}+n_{3}+n_{4} = n$

$r=4$
stadio 1: $\binom{n}{n_{1}}$
stadio 2: $\binom{n-n_{1}}{n_{2}}$
stadio 3: $\binom{n-n_{1}-n_{2}}{n_{3}}$
stadio 4: $\binom{n-n_{1}-n_{2}-n_{3}}{n_{4}} = \binom{n_{4}}{n_{4}} = 1$
scelte totali: $\binom{n}{n_{1}}\binom{n-n_{1}}{n_{2}}\binom{n-n_{1}-n_{2}}{n_{3}} = \dfrac{n!}{n_{1}!n_{2}!n_{3}!n_{4}!} = \dbinom{n}{n_{1},n_{2},n_{3},n_{4}}$

e.g. Anagrammi di MISSISSIPPI
$\dfrac{11!}{1!4!4!2!}$

e.g. Distribuisco 52 carte a 4 giocatori. Probabilità che ogni giocatore abbia un asso
casi favorevoli
2 stadi:
1° stadio: Distribuisco gli assi $\to 4!$
2° stadio: Distribuisco 48 carte $\to \dbinom{48}{12,12,12,12}$
casi totali:
$\dbinom{52}{13,13,13,13}$
$$\implies \frac{4!\dbinom{48}{12,12,12,12}}{\dbinom{52}{13,13,13,13}}$$

e.g. Superenalotto
Vengono estratti 6 numeri da 1 a 90 (senza reinserimento).
Supponendo di giocare 6 numeri, qual'è la probabilità di indovinarne 3, 4, 5, o 6?

Spazio di probabilità uniforme discreto
Casi totali:
$\binom{90}{6}$

Casi favorevoli:
1° stadio: scelgo k tra i 6 numeri vincenti: $\binom{6}{k}$
2° stadio: scelgo 6-k numeri tra gli 84 perdenti $\binom{84}{6-k}$
n° totale = $\binom{6}{k}\binom{84}{6-k}$

probabilità:
$\dfrac{\binom{6}{k}\binom{84}{6-k}}{\binom{90}{6}}$

[[Probabilità Ipergeometriche]]
