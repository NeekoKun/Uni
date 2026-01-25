#analisi 
> [!error] Teorema
> Sia $f: [a,b] \subseteq \mathbb{R} \to \mathbb{R}$ continua in $[a,b]$ e derivabile in $(a,b)$. Allora $\exists c \in (a,b) :$ $$f'(c) = \frac{f(b) - f(a)}{b-a}$$

```tikz
\begin{document}
	\begin{tikzpicture}[domain = 1:5.8, every node/.style={scale=1.5}]
		\draw[very thin,color=gray] (0,0) grid (7,6);
		\draw[->] (-0.5,0) -- (7.3,0) node[right] {$x$};
		\draw[->] (0,-0.5) -- (0,6.3) node[above] {$f(x)$};
		\draw[color=black]   plot (\x,{0.2 * (\x - 5)^(3) + (\x - 5)^(2) + \x - 2});
		
		\coordinate (A) at (1, 2.2);
		\draw[dashed] (A) -- (1,0) node[below] {$a$};
		\draw[dashed] (A) -- (0,2.2) node[left] {$f(a)$};
		
		\coordinate (B) at (5.8, 4.5424);
		\draw[dashed] (B) -- (5.8,0) node[below] {$b$};
		\draw[dashed] (B) -- (0,4.5424) node[left] {$f(b)$};
		
		\draw[color=blue] plot (\x, {((8.2176 + 2.3424 *\x)/(4.8))});
		
		\coordinate (C) at (1.94608, 3.5760747538407);
		\coordinate (D) at (4.72057, 2.7942874831538);
		
		\draw[dashed, color=red] (C) -- (1.94608, 0) node[below] {$c_1$};
		\draw[dashed, color=red] (D) -- (4.72057, 0) node[below] {$c_2$};
		
		\coordinate (C') at ({1.94608 - 1}, {3.5760747538407 - 2.3424 / 4.8});
		\coordinate (C'') at ({1.94608 + 1}, {3.5760747538407 + 2.3424 / 4.8});
		
		\coordinate (D') at ({4.72057 - 1}, {2.7942874831538 - 2.3424 / 4.8});
		\coordinate (D'') at ({4.72057 + 1}, {2.7942874831538 + 2.3424 / 4.8});
		
		\draw[color=red] (C') -- (C'');
		\draw[color=red] (D') -- (D'');
	\end{tikzpicture}
\end{document}
```

> [!info] Osservazione
> $f(a) = f(b) = 0 \implies \exists\ c \in (a,b):f'(c) = 0$
> Questo teorema prende il nome di **Teorema di Rolle**

> [!error] Dimostrazione
> Introduciamo la funzione ausiliaria $g: [a,b] \to \mathbb{R}$ definita come $$g(x) = f(x) - \frac{f(b) - f(a)}{b - a} (x - a) + f(a)$$
> Allora:
> - $g$ è [[Continuità|Continua]] perché somma di funzioni continue
> - $g$ è Derivabile in $(a,b)$ perché somma di funzioni derivabili
> - $g(a) = g(b) = 0$
> 
> Poiché $g$ è continua in $[a,b]$, ammette massimo $M$ e minimo $m$ in $[a,b]$.
> - Se $M = m$ allora $g$ è costante in $[a,b]$ e $g'(x) = 0\ \forall\ x \in (a,b)$
> - Se $M \neq m \implies m \neq 0 \lor M \neq 0$, quindi esso non viene assunto nei due estremi (essendo $g(a) = g(b) = 0$) ma in un punto $c \in (a,b)$.
>
> Essendo $c$ estremante di $g$, $g$ continua e derivabile in $g(c)$, allora per [[Teorema di Fermat]] $g'(c) = 0$
> $$0 = g'(c) = f'(c) - \frac{f(b) - f(a)}{b - a}$$ $$\implies \boxed{f'(c) = \frac{f(b) - f(a)}{b - a}}$$