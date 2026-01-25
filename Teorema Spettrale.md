#GAL
> [!error] Teorema
> $V$ [[Spazi Euclidei|Spazio Euclideo]]
> $L:V\to V$ è un [[Endomorfismi|Endorfismo]]
> $L$ è simmetrico $\Leftrightarrow L$ è ortogonalmente diagonalizzabile

> [!error] Dimostrazione (3/4)
> $\boxed{\Leftarrow}$
> Supponiamo esiste $B = \{ \underline{b}_{1}, \dots, \underline{b}_{n} \}$ base di $V$ di autovettori di $L$. Dati
> $$\underline{v} = \sum_{i=1}^{n} v_{i} \underline{b}_{i},\ \underline{w} = \sum_{j=1}^{n} w_{j}\underline{b}_{j}\ \in V $$
> Verifichiamo che $<L(\underline{v}), \underline{w}> = <\underline{v}, L(\underline{w})>$
> $$<L(\underline{v}), \underline{w}> = \left<L\left( \sum_{i=1}^{n} v_{i} \underline{b}_{i} \right), \sum_{j=1}^{n} w_{j} \underline{b}_{j}\right> = \left< \sum_{i=1}^{n} v_{i} L\left( \underline{b}_{i} \right), \sum_{j=1}^{n} w_{j} \underline{b}_{j}\right>$$
> $$= \sum_{i,j}  v_{i}w_{j} \left< L(\underline{b}_{i}), \underline{b}_{j}\right> = \sum_{i,j}  v_{i}w_{j} \left< \lambda_{i}\underline{b}_{i}, \underline{b}_{j}\right> = \sum_{i,j}  v_{i}w_{j} \lambda_{i}\left< \underline{b}_{i}, \underline{b}_{j}\right> $$
> $$= \sum_{i}^n  v_{i}w_{i}\lambda_{i} $$
> 
> $$<\underline{v}, L(\underline{w})> = \left<\sum_{i=1}^{n} v_{i} \underline{b}_{i}, L\left(\sum_{j=1}^{n} w_{j} \underline{b}_{j}\right)\right> = \left< \sum_{i=1}^{n} v_{i} \underline{b}_{i}, \sum_{j=1}^{n} w_{j} L(\underline{b}_{j})\right>$$
> $$= \sum_{i,j}  v_{i}w_{j} \left< \underline{b}_{i}, L(\underline{b}_{j})\right> = \sum_{i,j}  v_{i}w_{j} \left< \underline{b}_{i}, \lambda_{j}\underline{b}_{j}\right> = \sum_{i,j}  v_{i}w_{j} \lambda_{j}\left< \underline{b}_{i}, \underline{b}_{j}\right> $$
> $$= \sum_{i}^n  v_{i}w_{i}\lambda_{i} $$
> Risultati uguali $\implies$ $L$ è simmetrico
> $\boxed{\Rightarrow}$
> Supponiamo $L$ [[Endomorfismo Simmetrico]]
> Per lemma, $\exists$ autovalore $\lambda \in \mathbb{R} \implies \exists$ autovettore $\underline{0} + \underline{v}_{1} \in E_{\lambda}$. Cioè $L(\underline{v}_{1}) = \lambda \underline{v}_{1}$
> Possiamo supporre $||\underline{v}_{1}|| = 1$.
> Consideriamo $W = \mathrm{Span}(\underline{v}_{1})^\perp$, e dimostriamo che $L(W) \subseteq W$:
> $\left< L(\underline{w}), \underline{v}_{1}\right> = \left< \underline{w}, L(\underline{v}_{1})\right> = \left<\underline{w}, \lambda\underline{v}_{1}\right> = \lambda \left<\underline{w}, \underline{v}_{1}\right> = 0\ \forall\ \underline{w} \in W$
> $\implies L(\underline{w}) \in \mathrm{Span}(\underline{v}_{1})^\perp = W$
> $\implies L(W) \subseteq W$
> qualcosa qualcosa induzione [...] #TODO 


> [!error] Lemma
> Se $L:V \to V$ è un [[Endomorfismo Simmetrico]] allora esiste almeno un autovalore

> [!error] Corollario
> $L:V\to V$ simmetrico se $\lambda_{i} \neq \lambda_{j}$ autovalori distinti
> $\implies E_{\lambda_{i}} \perp E_{\lambda_{j}}$

> [!error] Corollario
> Le seguenti condizioni sono equivalenti per $A \in \mathrm{Mat}(n.n)$
> 1. $A$ è simmetrica
> 2. $\exists$ base $\{ \underline{b}_{1}, \dots, \underline{b}_{n} \}$ base ortogonale di $\mathbb{R}^n$ di autovettori di $A$
> 3. $\exists$ matrice $S = (\underline{b}_{1}, \dots, \underline{b}_{n})$ tale che $D = S^TAS$ è diagonale