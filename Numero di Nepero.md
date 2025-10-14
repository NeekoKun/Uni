#analisi 
> [!error] Teorema
> La successione $$a_{n} = \left( 1 + \frac{1}{n} \right)^n$$ è monotona crescente e limitata.
> In particolare essa ammette limite in $\mathbb{R}$

> [!info] definizione
> $e$ è quel limite

> [!info] Osservazione
> $e = \mathrm{Sup}_{n\in \mathbb{N}}\left( 1+\frac{1}{n} \right)^n$
> $e > \left( 1+\frac{1}{n} \right)^n\ \forall\ n\geq 1$

> [!warning] Dimostrazione
> Si dimostra che $a_{n}$ è crescente, cioè che $$a_{n}\geq a_{n-1}\ \forall\ n\in \mathbb{N},\ n \geq 2$$
> cioè $$\frac{a_{n}}{a_{n-1}} \geq 1$$
> infatti $$\frac{a_{n}}{a_{n-1}} = \frac{\left( 1+\frac{1}{n} \right)^n}{\left( 1+\frac{1}{n-1} \right)^{n-1}} \geq \overset{\text{Disuguaglianza di Bernulli}}{\dots} \geq 1$$
> Si dimostra che $a_{n}$ sia limitata ponendo $$a_{n}\leq b_{n}\leq b_{1}$$ dove $$b_{n} = \left( 1+\frac{1}{n} \right)^{n+1}$$

> [!info] Corollario
> $\lim_{ n \to \infty }\left( 1+\frac{a}{n} \right)^n = e^a$