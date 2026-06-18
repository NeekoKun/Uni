#IeS 
> [!error] Teorema di Shannon
> $$\mathrm{E}[l] = \sum_{j=1}^m l_{j} p_{X}(x_{j}) \geq H(X)$$

> [!error] Dimostrazione
> Questa viene come diretta conseguenza della [[Disuguaglianza di Kraft-McMillan]]
> $$H(X) = \mathrm{E}\left[ \frac{\log_{2}1}{p_{X}(X)} \right] = \mathrm{E}\left[ \log_{2} \frac{2^{l(x)}}{p_{X}(x)2^{l(X)}} \right]$$
> $$= \mathrm{E}[\log_{2}2^{l(x)}] + \mathrm{E}\left[ \log_{2} \frac{1}{p_{X}(x)2^{l(x)}} \right] = \mathrm{E}[L] + E\left[ \log_{2} \frac{1}{p_{X}(x) 2^{l(x)}} \right]$$
> Cerchiamo di dimostrare che $E\left[ \log_{2} \frac{1}{p_{X}(x) 2^{l(x)}} \right] \leq 0$
> $$E\left[ \log_{2} \frac{1}{p_{X}(x) 2^{l(x)}} \right] \leq \log_{2}\mathrm{E}\left[ \frac{1}{p_{X}(x) 2^{l(x)}} \right] = \log_{2}\left( \sum_{j=1}^m p_{X}(x_{j}) \cdot \frac{1}{p_{X}(x_{j})2^{l(x_{j})}} \right)$$
> $$\implies E\left[ \log_{2} \frac{1}{p_{X}(x) 2^{l(x)}} \right] = \log_{2}\left( \sum_{j=1}^m 2^{-l(x_{j})} \overset{Kraft-McMillen}{\leq} 1 \right) \implies \boxed{\leq 0}$$

> [!info] Osservazione
> In generale, $i(x_{j})$ è un numero non intero di bit.
> $$i(x_{j}) \in \mathbb{N}\ \forall\ j \implies \mathrm{E}[L] = H(X)$$

> [!info] Osservazione
> Al più, ogni risultato spreca 1 bit (per arrotondamento dato da $\lceil i(x_{j}) \rceil - i(x_{j})$)
