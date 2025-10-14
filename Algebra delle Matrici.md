#GAL 
### Trasposta di una Matrice
> [!warning] Definizione
> Data $A=(a_{i,\ j}) \in Mat(m,\ n)$
> Definiamo $A^T = (a_{j,\ i}) \in Mat(n,\ m)$
> Cioè $(A^T)_{i,\ j} = (A)_{j,\ i}$

> [!info] Proprietà
> 1) $(A^T)^T = A$
> 2) $(A+B)^T = A^T + B^T$
> 3) $(cA)^t = c(A^t)$

> [!info] Esempio
> $A = \begin{pmatrix}1 & 2 & 3 \\0 & 2 & 0\end{pmatrix}\implies A^T = \begin{pmatrix}1 & 0 \\ 2 & 2 \\ 3 & 0\end{pmatrix}$
##### Distribuzione della Trasposizione
> [!warning] Definizione
> $(AB)^T = B^TA^T$ 

### Prodotto tra Matrici
> [!info] Caso Speciale
> $\underline{a} = (a_{1},\ a_{2},\ \dots,\ a_{n}),\ \underline{b}=\begin{pmatrix}b_{1} \\ b_{2} \\ \vdots \\ b_{n}\end{pmatrix}$
> 
>$\underline{a}\underline{b} = a_{1}b_{1} + a_{2}b_{2}+\dots+a_{n}b_{n} =\displaystyle\sum_{k=1}^n a_{k}b_{k}$

> [!warning] Definizione
> Dati $m,\ n,\ p \in \mathbb{N}:A=Mat(m,\ n), B=Mat(n,\ p)$ definiamo
> $AB \in Mat(m,\ p) : (AB)_{i,j} = a_{i,1}b_{1,j} + a_{i,2}b_{2,j}+\dots+a_{i,n}b_{n,j} = \displaystyle\sum_{k=1}^n a_{i,k}b_{k,j}$

> [!info] Osservazione
> $AB=0 \not\implies A=0\ \lor\ B=0$

### Elemento Neutro
 > [!warning] Definizione
 > Sia $A \in Mat(m,\ n)$ abbiamo $I_{m}A = AI_{n} = A$
 > Verifichiamo che $I_{m}A = A$
 > $(I_mA)_{i,j} = \displaystyle\sum_{k=1}^n (I_{m})_{i,k}(A)_{k,j}$
 > Poniamo $I_{m} \in Mat(m,\ m) = (I_{m})i,j = 1\ i==j?\ 0$
 > allora $\displaystyle\sum_{k=1}^n(I_{m})_{i,i}(A)_{i,j} = \displaystyle\sum_{k=1}^n1(A)_{i,j} = A$
 