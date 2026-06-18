#IeS 
# Discrete

## Distribuzione Geometrica
> [!warning] Somme
> Calcolare la $k$-esima riuscita di una distribuzione geometrica risulta in una Pascal di carattere $\mathrm{Pascal}(k, \lambda)$, dove $\lambda$ è il parametro della geometrica

## Distribuzione Binomiale

## Distribuzione Bernoulliana

## Distribuzione Uniforme

## Distribuzione di Pascal

## Distribuzione di Poisson
$$f(k) = \frac{\lambda \tau}{k!}^k e^{-\lambda \tau}$$
$$E[N_{[0,\tau]}] = \sum_{k=0}^\infty k f(k) = \lim_{ n \to \infty } \mathrm{E}\left[ \mathrm{Binom}\left[ n, \frac{\lambda \tau}{n} \right] \right] = \lim_{ n \to \infty } n \frac{\lambda \tau}{n} = \lambda \tau$$
$$\mathrm{Var}[N_{[0, \tau]}] = \lim_{ n \to \infty } \mathrm{Var}\left[ \mathrm{Binom}\left[ n, \frac{\lambda \tau}{n} \right] \right] = \lim_{ n \to \infty } n \frac{\lambda \tau}{n} \left( 1- \frac{\lambda \tau}{n} \right) = \lambda \tau$$
## Erlang
> [!warning] Definizione
> Un process di $\mathrm{Erlang}(k, \lambda)$ descrive la probabilità del $k$-esimo successo di un processo di Poisson $\mathrm{Pois(\lambda)}$
# Continue


## Distribuzione Uniforme


## Distribuzione Normale


## Distribuzione Esponenziale

| Proprietà                     | $\mathrm{E}[X]$     | $\mathrm{Var}[X]$         | PDF $(X=x)$                                                                      | CDF                                       |
| ----------------------------- | ------------------- | ------------------------- | -------------------------------------------------------------------------------- | ----------------------------------------- |
| $\mathrm{Geom}(p)$            | $\frac{1}{p}$       | $\frac{1-p}{p^2}$         | $(1-p)^{x-1}p$                                                                   | $1-(1-p)^k$                               |
| $\mathrm{Binom}(n, p)$        | $np$                | $np(1-p)$                 | $\binom{n}{x}p^x(1-p)^{n-x}$                                                     | $\sum_{i=0}^k \binom{n}{i}p^i(1-p)^{n-1}$ |
| $\mathrm{Pascal}(k, p)$       | $\frac{k}{p}$       | $\frac{k\cdot(1-p)}{p^2}$ | $\binom{x-1}{k-1}p^k(1-p)^{x-k}$                                                 |                                           |
| $\mathrm{Pois}(\lambda)$      | $\lambda$           | $\lambda$                 | $\frac{\lambda^xe^{-\lambda}}{x!}$                                               |                                           |
| $\mathrm{Bern}(p)$            | $p$                 | $p(1-p)$                  | ---                                                                              |                                           |
| $\mathcal{U}[a, b]$           | $\frac{a+b}{2}$     | $\frac{(b-a)^2}{12}$      | ---                                                                              |                                           |
| $\mathcal{N}[\mu, \sigma^2]$  | $\mu$               | $\sigma^2$                | $\frac{1}{\sigma^2\sqrt{ 2\pi }}\exp\left( -\frac{(x-\mu)^2}{2\sigma^4} \right)$ |                                           |
| $\mathrm{Exp}(\lambda)$       | $\frac{1}{\lambda}$ | $\frac{1}{\lambda^2}$     | $\lambda e^{-\lambda x}$                                                         | $1-e^{-\lambda x}$                        |
| $\mathrm{Erlang}(k, \lambda)$ | $\frac{k}{\lambda}$ | $\frac{k}{\lambda^2}$     | $\frac{\lambda^kx^{k-1}e^{-\lambda x}}{(k-1)!}$                                  |                                           |

