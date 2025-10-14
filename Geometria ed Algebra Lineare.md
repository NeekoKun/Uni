#GAL
# [[Vettori]], [[Matrice|Matrici]], [[Sistemi Lineari]]
### Definizione
- $\mathbb{R}$ ([[Numeri Reali]])
- Sia $n \in \mathbb{N}$:
	- $\mathbb{R}^n = \left\{\begin{pmatrix}x_{1} \\ x_{2} \\ \vdots \\ x_{n}\end{pmatrix} \ :\ x_{1}\dots x_{n} \in \mathbb{R} \right\}$
- Due interpretazioni geometriche (e.g. $n=2$):
	1. Punti dello Spazio $\left(P=\binom{1}{2}\in \mathbb{R}\right)$
	2. Segmenti Orientati $\left(\overrightarrow{OP} = \binom{1}{2} \in \mathbb{R}\right)$
		- "[[Vettori]]"

### Operazioni
- ==Somma==
	- $\begin{pmatrix}x_{1} \\ x_{2} \\ \vdots \\ x_{n}\end{pmatrix},\begin{pmatrix}y_{1} \\ y_{2} \\ \vdots \\ y_{n}\end{pmatrix} \in \mathbb{R}^n: \begin{pmatrix}x_{1} \\ x_{2} \\ \vdots \\ x_{n}\end{pmatrix} + \begin{pmatrix}y_{1} \\ y_{2} \\ \vdots \\ y_{n}\end{pmatrix} = \begin{pmatrix}x_{1} + y_{1} \\ x_{2} + y_{2} \\ \vdots \\ x_{n} + y_{n}\end{pmatrix} \in \mathbb{R}$
- ==Prodotto per uno scalare==
	- $\begin{pmatrix}x_{1} \\ x_{2} \\ \vdots \\ x_{n}\end{pmatrix} \in \mathbb{R}: c\begin{pmatrix}x_{1} \\ x_{2} \\ \vdots \\ x_{n}\end{pmatrix} = \begin{pmatrix}cx_{1} \\ cx_{2} \\ \vdots \\ cx_{n}\end{pmatrix} \in \mathbb{R}$

### Proprietà
- Somma
	- Commutatività
	- Associatività
	- Esistenza dell'**elemento neutro**
	- Esistenza dell'**elemento opposto**
- Prodotto
	- Associatività
		- $A(BC)=(AB)C$
	- Esistenza dell'**elemento neutro**
- Distributività
	- $A(B+C) = AB+AC$
	- $(A+B)C = AC+BC$

> [!info] Esempio
> Dati $\underline{v},\underline{w} \in \mathbb{R}^2$
> $\{ \underline{v} + t \underline{w} : t \in \mathbb{R} \}$ è una [[Retta]] descritta in forma parametrica
> $\underline{w}$ è chiamato "==Vettore Direzione==" della [[Retta]]

> [!info] Osservazione
> Una forma parametrica di una retta *non è unica*
> Esempio:
> - $r = \left\{ \binom{1}{3} + t\binom{1}{-1} : t \in \mathbb{R}\right\}$
> - $r = \left\{ \binom{2}{2} + s\binom{-2}{2} : s \in \mathbb{R}\right\}$

### Risultati
- Dalla forma parametrica di 2 vettori otteniamo una [[Retta]]
- Dalla forma parametrica di 3 vettori otteniamo un [[Piano]]

# [[Spazi Vettoriali]]
