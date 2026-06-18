#IeS 
> [!error] Teorema
> Siano $X_{i}$ [[Variabile Aleatoria|Variabili Aleatorie]] [[iid]] con $\mathrm{Var}[X_{i}] < \infty$ e sia $Z_{n} = \frac{X_{1} + X_{2} + \dots + X_{n} - n \mathrm{E}[X_{1}]}{\sqrt{ n \mathrm{Var}[X_{1}] }}$ e sia $Z \textasciitilde N(0, 1)$, allora
> $$F_{Z_{n}}(c) \overset{n \to \infty}{ \to } F_{Z}(c) = \Phi(c)\ \forall\ c \in \mathbb{R}$$

> [!error] Corollario
> $$F_{Z_{n}} \to F_{Z} \implies Z_{n} \approx \mathcal{N}(0,1)$$
> $$Z_{n} = \frac{S_{n} - n\mu}{\sqrt{ n \sigma^2 }} \implies S_{n} \approx \sqrt{ n\sigma^2 }Z_{n} + n\mu = N(n\mu, n \sigma^2)$$

> [!warning] Applicazione
> $$P\left( Z \geq \frac{n - \mathrm{E}[X]}{\sqrt{ \mathrm{Var}[X] }} \right) = 1 - \Phi\left( \frac{n - \mathrm{E}[X]}{\sqrt{ \mathrm{Var}[X] }} \right)$$

> [!info] Osservazione
> La velocità di convergenza di $Z_{n}$ ad una gaussiana dipende dalla simmetria della distribuzione di partenza