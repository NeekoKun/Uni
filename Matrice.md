#GAL 
> [!warning] Definizione
> Una **matrice** mxn è una tabella rettangolare di numeri
>  m = numero di righe
>  n = numero di colonne
>  e.g.
>  $\begin{pmatrix}1 & 0 & 2 & 4 \\2 & -1 & \sqrt{ 3 } & 0 \\ 5 & 3 & \pi & 1\end{pmatrix}$

> [!info] Casi Speciali
> - m x 1 = Vettori Colonna
> - 1 x n = Vettori riga
> - 1 x 1 = Scalare

> [!warning] Definizione
> Dato un [[Sistemi Lineari|Sistema Lineare]] in forma standard definiamo
> - Matrice dei Coefficienti:
> $\begin{pmatrix}a_{11} & a_{12} & \dots & a_{1n} \\ a_{21} & a_{22} & \dots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ a_{m1} & a_{m2} & \dots & a_{mn} \end{pmatrix}$
> - Vettore dei Termini Noti
> $\begin{pmatrix}b_{1} \\ b_{2} \\ \vdots \\ b_{m}\end{pmatrix}$
> - Vettore delle Variabili
> $\begin{pmatrix}x_{1} \\ x_{2} \\ \vdots \\ x_{m}\end{pmatrix}$
> - Matrice Completa del Sistema
> $\begin{pmatrix}a_{11} & a_{12} & \dots & a_{1n} & b_{1} \\ a_{21} & a_{22} & \dots & a_{2n} & b_{2} \\ \vdots & \vdots & \ddots & \vdots & \vdots \\ a_{m1} & a_{m2} & \dots & a_{mn} & b_{m} \end{pmatrix}$

### Matrice Inversa (metodo di Gauss-Jordan)

$(A, I_{n}) \overset{\mathrm{Gauss-Jordan}}{\to}(I_{n}, A^{-1})$

## Determinante
> [!warning] Definizione
> Denotiamo $\widehat{A}_{ij}\in \mathrm{Mat(n-1,n-1)}$ la sottomatrice di $A$ ottenuta eliminando la riga $i$ e la colonna $j$



> [!warning] Definizione
> Il **Determinante** di una matrice *quadrata* $A = (a_{i,j}) \in \mathrm{Mat}(n,n)$ e definito ricorsivamente come:
> - Caso $n = 1;\ A = (a_{n}) \implies \det A \overset{\text{def}}{=} a_{n}$
> - Caso $n > 1 :$
> 	- Scegliamo una riga $i$ e "sviluppiamo lungo la riga $i$": $$\det A \overset{\text{def}}{=} \sum_{j=1}^{n} (-1)^{i+j} a_{ij} \cdot \det \widehat{A}_{ij}$$
> 	- Scegliamo una colonna $j$ e "Sviluppiamo lungo la colonna $j$": $$\det A \overset{\text{def}}{=} \sum_{i=1}^{n} (-1)^{i+j}a_{ij} \cdot \det \widehat{A}_{ij}$$