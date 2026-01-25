\#GAL 
> [!error] Teorema
> Sia $q(\underline{x}) = \underline{x}^TA\underline{x}$ con $q: \mathbb{R}^n \to \mathbb{R}$, $A \in \mathrm{Mat}(n,n)$ simmetrica.
> Siano:
> - $p$ numero di autovalori positivi di $A$
> - $r$ numero di autovalori negativi di $A$
> - $n - p - r$ numero di autovalori $= 0$
> 
> (Contati con Molteplicità)
> Allora:
> 1. $A$ è congruente alla matrice
> $$Y = \begin{pmatrix}
> I_{p} & 0 & 0 \\
> 0 & -I_{r} & 0 \\
> 0 & 0 & 0
> \end{pmatrix}$$
> detta **Forma Canonica di Sylvester**, quindi $q(\underline{x})$ è equivalente a
> $$S(\underline{x}) = x_{1}^2 + \dots + x_{p}^2 - (x_{p+1}^2 + \dots + x_{p+r}^2)$$
> 2. La [[Segnatura]] di $A$/$q(\underline{x})$ vale
> $$(n_{+}, n_{-}, n_{0}) = (p, r, n-p-r)$$
> 3. Due forme [[Quadratiche]] sono equivalenti $\Leftrightarrow$ hanno la stessa [[Segnatura]]

> [!error] Dimostrazione
> $\boxed{1.}$
> $A$ simmetrica $\implies S^TAS = D$ con $S$ ortogonale e $D$ diagonale con autovalori di $A$ per [[Teorema Spettrale]]
> Possiamo supporre che gli autovalori siano ordinati, quindi
> $$\lambda_{1}, \dots, \lambda_{p} > 0,\ \lambda_{p+1}, \dots, \lambda_{p+r} < 0,\ \lambda_{p+r+1}, \dots, \lambda_{n} = 0$$
> Cerchiamo quindi $W$ invertibile tale che $W^TDW = Y$. Consideriamo
> $$W = \begin{pmatrix}
> \frac{1}{\sqrt{ |\lambda_{1}| }} & \dots & 0 & 0 & 0 & 0 \\
> \vdots & \ddots & 0 & 0 & 0 & 0 \\
> 0 & \dots & \frac{1}{\sqrt{ |\lambda_{p+r}| }} & 0 & 0 & 0 \\
> 0 & \ddots & 0 & 1 & 0 & 0 \\
> \vdots & \dots & \vdots & \vdots & \ddots & 0 \\
> 0 & \dots & 0 & 0 & \dots & 1
> \end{pmatrix}$$
> allora $W^TDW$ è diagonale con
> $$(W^TDW)_{ii} = \begin{cases}
> 1 & \lambda_{i} > 0 \\
> -1 & \lambda_{i} < 0 \\
> 0 & \lambda_{i} = 0
> \end{cases}$$
> cioé:
> $$W^TDW = Y \implies W^T(S^TAS)W = Y \implies \boxed{(SW)^TA(SW) = Y}$$
> $\boxed{3.}$
> Se $q_{1}(\underline{x}), q_{2}(\underline{x})$ hanno la stessa segnatura
> $\implies$ per $\boxed{1.}$ hanno la stessa forma canonica di Sylvester $S(\underline{x})$ $\implies$ sono equivalenti alla stessa forma canonica $\implies \boxed{\text{sono equivalenti tra di loro}}$

## Corollari

> [!error] Corollario (Rappresentazione di un Prodotto scalare)
> 1. Sia $A \in \mathrm{Mat}(n,n)$ l'operazione $\left<\underline{x}, \underline{y}\right> = \underline{x}^TA\underline{y}$ con $\underline{x},\underline{y} \in \mathbb{R}^n$ è un prodotto scalare $\Leftrightarrow$ $A$ è simmetrica e definita positiva
> 2. Sea $V$ uno [[Spazi Euclidei|Spazio Euclideo]], $B = \{ \underline{b}_{1}, \dots, \underline{b}_{n} \}$ base qualsiasi.
> La matrice $A$ tale che $(A)_{ij} = \left<\underline{b}_{1}, \underline{b}_{j}\right>$ è simmetrica e definita positiva, e $\left<\underline{v}, \underline{w}\right> = [\underline{v}]^T_{B}A[\underline{w}]_{B}$

> [!error] Dimostrazione
> $\boxed{1.}$
> $\underline{x}^TA\underline{y} \overset{1 \times 1}{=} (\underline{x}^TA\underline{y})^T = \underline{y}^TA^T\underline{x}$
> quindi $\left<\underline{x},\underline{y}\right> = \left<\underline{y}, \underline{x}\right> \Leftrightarrow \underline{x}^TA\underline{y} = \underline{y}^TA\underline{x} \Leftrightarrow \underline{y}^TA\underline{x} = \underline{y}^TA\underline{x}\ \forall\ \underline{x},\underline{y}$
> bilineare segue dalle proprietà del prodotto tra matrici
> definita positiva: $\left<\underline{x}, \underline{x}\right> > 0\ \forall\ \underline{x} \neq \underline{0} \Leftrightarrow \underline{x}^TA\underline{x} > 0\ \forall\ \underline{x} \neq \underline{0} \Leftrightarrow A$ definitivamente positiva