#GAL 
> [!error] Proposizione
> $L$ è diagonalizzabile $\Leftrightarrow$ esiste una base di $V$ composta da [[Endomorfismi#Autovalori, Autovettori|autovettori]] di $L$.
> In questo caso, $M_{i, i}$ è l'i-esimo [[Endomorfismi#Autovalori, Autovettori|autovalore]] di $L$

> [!error] Dimostrazione
> Sia $B = \{ \underline{b}_{1}, \dots, \underline{b}_{n} \}$ una base di $V$
> $\underline{b}_{i}$ è autovettore di $L \Leftrightarrow L(\underline{b}_{i}) = \lambda_{i}\underline{b}_{i}$ per qualche $\lambda_{i} \in \mathbb{R}$
> $\Leftrightarrow \left[ L(\underline{b}_{i}) \right]_{B} = \begin{pmatrix}0 \\ \vdots \\ \lambda_{i} \\ \vdots \\ 0\end{pmatrix}$
> Quindi $\underline{b}_{1}, \dots, \underline{b}_{n}$ sono tutti autovettori di $L$
> $\Leftrightarrow \left(  [L(\underline{b}_{1})]_{B}, \dots, L(\underline{b}_{n})_{B} \right) = \begin{pmatrix}\lambda_{1} & 0 & \dots & 0 \\ 0 & \lambda_{2} & \dots & 0 \\ \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & \dots & \lambda_{n}\end{pmatrix}$