#IeS 
> [!warning] Definizione
> L'insieme di tutti i possibili risultati di un [[Esperimento Aleatorio]], indicato con $\Omega$


> [!warning] Proprietà
> - **Mutua Esclusività**: Si deve verificare uno ed un solo evento elementare
> - **Esaustività**: Lo spazio deve elencare tutti i possibili risultati

e,g,
- Lancio della Moneta
$$\Omega = \{ \text{Testa}, \text{Croce} \}$$
- Lancio di un Dado a 6 facce
$$\Omega = \{ 1,2,3,4,5,6 \}$$
- Lancio di un Dado a 4 facce
$$\Omega = \{ 1,2,3,\text{4 e tira vento}, \text{4 e non tira vento} \}$$
- Lancio di 2 Monete
$$\Omega = \{ T_{1}T_{2}, T_{1}C_{2}, C_{1}T_{2}, C_{1}C_{2} \}$$
- Lancio di 2 Dadi a 4 facce

```tikz

\begin{document}
\begin{tikzpicture}[scale=2,font=\huge]
\draw (0,0)--(1,-1) (0,-2)--(5,-2) (0,-3)--(5,-3) (0,-4)--(5,-4) (2,0)--(2,-5) (3,0)--(3,-5) (4,0)--(4,-5);
\draw[double,double distance=.5pt] (0,-1)--(5,-1) (1,0)--(1,-5) ;
\path[magenta]
(.7,-.3) node{II}
(.3,-.7) node{I}
                (1.5,-.5) node{1} ++(0:1) node{2} ++(0:1) node{3} ++(0:1) node{4}
(.5,-1.5) node{1} ++(0:1) node{1,1} ++(0:1) node{2,1} ++(0:1) node{3,1} ++(0:1) node{4,1}
(.5,-2.5) node{2} ++(0:1) node{1,2} ++(0:1) node{2,2} ++(0:1) node{3,2} ++(0:1) node{4,2}
(.5,-3.5) node{3} ++(0:1) node{1,3} ++(0:1) node{2,3} ++(0:1) node{3,3} ++(0:1) node{4,3}
(.5,-4.5) node{4} ++(0:1) node{1,4} ++(0:1) node{2,4} ++(0:1) node{3,4} ++(0:1) node{4,4}

;
\end{tikzpicture}
\end{document}

```
- Spazio Continuo
$$\Omega = \{ (x,y):0\leq x\leq1;\ 0\leq y\leq 1 \}$$
> [!info] Osservazione
> Non ha molto senso assegnare probabilità ad elementi elementari
> $\to$ Assegniamo quindi probabilità a ==Sottoinsiemi di $\Omega$==  creando la [[Sigma-Algebra]]