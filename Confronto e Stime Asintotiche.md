#analisi 
> [!warning] Definizione
> - $\lim_{ n \to \infty } a_{n} = \pm \infty$, $\lim_{ n \to \infty }b_{n}=\pm \infty \lor \mp \infty$, se 
> $$
> \lim_{ n \to \infty } \frac{a_{n}}{b_{n}} = 
> \begin{cases}
> 0 & a_{n}\ \text{è infinito di ordine inferiore rispetto a }b_n \\ \\ 
> l \in \mathbb{R}\setminus \{0\} & a_{n},\ b_{n} \text{ sono infiniti dello stesso ordine} \\ \\
> \pm \infty & b_{n} \text{ è infinito di ordine inferiore rispetto ad } a_{n} \\ \\
> \not\exists & a_{n},\ b_{n} \text{ non sono controntabili}
> \end{cases} \\
> $$
> - $\lim_{ n \to \infty }a_{n}=\lim_{ n \to \infty }b_{n} = 0$ se
> $$
> \lim_{ n \to \infty } \frac{a_{n}}{b_{n}} = 
> \begin{cases}
> 0 & a_{n} \text{ infinitesimo di ordine superiore rispetto a } b_{n} \\ \\
> l\in \mathbb{R}\setminus \{ 0 \} & a_{n},\ b_{n} \text{ infinitesimi dello stesso ordine} \\ \\
> \pm \infty & b_{n} \text{ è infinitesimo di ordine superiore rispetto ad } a_{n} \\ \\
> \not\exists & a_{n},\ b_{n} \text{ non sono confrontabili}
> \end{cases}
> $$

> [!warning] Definizione
> - $\sigma$-piccolo $$a_{n} = \sigma(b_{n}) \leftrightarrow \lim_{ n \to \infty } \frac{a_{n}}{b_{n}}=0$$
> - Asintotico $$a_{n} \textasciitilde\ b_{n} \leftrightarrow \lim_{ n \to \infty } \frac{a_{n}}{b_{n}}=1$$

> [!info] Osservazione
> - $\lim_{ n \to \infty }\frac{a_{n}}{b_{n}} = l\in \mathbb{R}\setminus\{ 0 \} \implies a_{n} \textasciitilde\ b_{n}$

> [!info] Osservazione
> - $a_{n}$ ~ $a_{n}$
> - $a_{n}$ ~ $b_{n}$, $b_{n}$ ~ $c_{n} \implies a_{n}$ ~ $c_{n}$
> - $a_{n}$ ~ $b_{n} \implies b_{n}$ ~ $a_{n}$
> 
> Quindi l'asintotico è una relazione di equivalenza

### Proprietà
1) $a_{n}$ ~ $a'_{n}$, $b_{n}$ ~ $b'_{n}$ $\implies$ $a_{n}b_{n}$ ~ $a'_{n}b'_{n}$
2) $a_{n}$ ~ $a'_{n}$, $b_{n}$ ~ $b'_{n}$ $\implies$ $\dfrac{a_{n}}{b_{n}}$ ~ $\dfrac{a'_{n}}{b'_{n}}$
3) $a_{n}$ ~ $a'_{n}$, $\alpha \in \mathbb{R}$ $\implies$ $(a_{n})^\alpha$ ~ $(a'_{n})^\alpha$
4) $a_{n}$ ~ $a'_{n}$ $\implies$ le due successioni hanno lo stesso carattere:
	- Convergono entrambe allo stesso limite $l$
	- Divergono entrambe allo stesso infinito
	- Sono entrambe irregolari
> [!warning] Dimostrazione
> 1. $a_{n}$ ~ $a'_{n}$, $b_{n}$ ~ $b'_{n}$ $\implies$ $a_{n}b_{n}$ ~ $a'_{n}b'_{n}$
> $$\frac{a_{n}b_{n}}{a'_{n}b'_{n}} = \frac{a_{n}}{a'_{n}} \cdot \frac{b_{n}}{b'_{n}} = 1 \cdot 1 = 1$$
> 2. $\dfrac{a_{n}}{b_{n}}$ ~ $\dfrac{a'_{n}}{b'_{n}}$
> $$\frac{\frac{a_{n}}{b_{n}}}{\frac{a'_{n}}{b'_{n}}} = \frac{a_{n}}{b'_{n}} \cdot \frac{a'_{n}}{b_{n}} = 1 \cdot 1 = 1 $$
> 3. $(a_{n})^\alpha$ ~ $(a'_{n})^\alpha$
> $$\frac{(a_{n})^\alpha}{(a'_{n})^\alpha} = \frac{a_{n}}{a'_{n}}^\alpha = 1^\alpha = 1$$
> 4. $a_{n},\ a'_{n}$ hanno lo stesso comportamento al limite
> Se $\lim_{ n \to \infty } a'_{n} = l \in \mathbb{R}$
> $$a_{n} = \frac{a_{n}}{a'_{n}} \cdot a'_{n} \to 1\cdot l = l$$
> $\implies \lim_{ n \to \infty }a_{n} = l$
> [...]
> Segue che $\not\exists \lim_{ n \to \infty }a'_{n} \implies \not\exists \lim_{ n \to \infty }a_{n}$

> [!info] Osservazione
> - $a_{n} \cdot \sigma(b_{n}) = \sigma(a_{n}b_{n})$
> - $c \cdot \sigma(a_{n}) = \sigma(a_{n})$
> - $\pm \sigma(a_{n}) = \mp \sigma(a_{n})$
> - $\sigma\left( \frac{1}{n} \right) + \sigma\left( \frac{1}{n^2} \right) = \sigma\left( \frac{1}{n} \right)$
> - $\sigma(n) + \sigma(n^2) = \sigma(n^2)$
> - $a_{n}$ ~ $b_{n} \implies \sigma(a_{n}) = \sigma(b_{n})$

> [!info] Osservazione
> è possibile usare la relazione di asintotico con le funzioni composte, partendo dalla più esterna quando si fa lo sviluppo