#GAL 
> [!warning] Definizione
> $A \in \mathrm{Mat(n, n)}$ è **Ortogonale** $\Leftrightarrow A^TA = I_{n}$

> [!info] Osservazione
> 1. $A$ ortogonale $\Leftrightarrow A^T = A^-1$
> 2. $A$ ortogonale $\implies A^T$ ortogonale
> 3. $A,B$ ortogonali $\implies AB$ ortogonale

> [!error] Proposizione
> Le seguenti 3 condizioni sono equivalenti per $A \in \mathrm{Mat}(n,n)$
> 1. $A$ è ortogonale
> 2. Le colonne di $A$ formano una [[Base Ortogonale e Ortonormale|Base Ortonormale]] di $\mathbb{R}^n$
> 3. Le righe di $A$ formano una [[Base Ortogonale e Ortonormale|Base Ortonormale]] di $\mathbb{R}^n$

> [!error] Dimostrazione (1. $\Leftrightarrow$ 2.)
> Poniamo $A = (\underline{a}_{1}, \dots, \underline{a}_{n})$
> $\implies A^T = \begin{pmatrix}\underline{a}_{1}^T \\ \vdots \\ \underline{a}_{n}^T\end{pmatrix}$ righe di $A^T$
> $(A^TA)_{i,j} = \left(\begin{pmatrix}\underline{a}_{1}^T \\ \vdots \\ \underline{a}_{n}^T\end{pmatrix}\begin{pmatrix}\underline{a}_{1}, \dots, \underline{a}_{n}\end{pmatrix}\right)_{i,j} = \underline{a}^T_{i}\underline{a}_{j} = \underline{a}_{i} \cdot \underline{a}_{j}$
> Quindi $A$ è una matrice ortogonale $\Leftrightarrow A^TA = I_{n} \Leftrightarrow (A^TA)_{ij} = (I_{n})_{ij} = \delta_{ij}$