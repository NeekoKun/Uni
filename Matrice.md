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