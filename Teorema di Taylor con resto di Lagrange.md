#analisi 
> [!error] Teorema
> Sia $f:(a,b) \to \mathbb{R},\ x_{0}\in(a,b)$, $f$ derivabile n-volte in $x_{0}$, $n \geq 0$
> Allora per $x \to x_{0}$
> $\forall\ x \in [a,b]\ \exists\ c \in [x, x_{0}] :$
> $$f(x) = P_{n}(x) + \frac{f^{(n+1)}(c)}{(n+1)!}(x-x_{0})^{n+1}$$
> $$\implies f(x) = \sum_{k=0}^{n} \frac{f^{(k)}(x_{0})}{k!}(x-x_{0})^k + \frac{f^{(n+1)}(c)}{(n+1)!}(x-x_{0})^{n+1}$$
> Dove $P_{n}(x)$ + il [[Polinomio di Taylor]] e $\frac{f^{(n+1)}(c)}{(n+1)!}(x-x_{0})^{n+1}$ è il **Resto di Lagrange**
> Questa formula prende il nome di **Serie di Taylor con Resto di Lagrange**