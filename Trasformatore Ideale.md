#ELT 
```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[american, scale=2, transform shape]
  \node[transformer, anchor=A1] (T) at (2,0) {}
	  (T.north) node{K}
	  (T.outer dot A1) node[circ]{}	
	  (T.outer dot B1) node[circ]{}
  ;
  \draw (T.A1) -- ++(-2,0) node[ocirc] (a1) {} node[midway, above] {$+$};
  \draw (T.B1) -- ++(+2,0) node[ocirc] (b1) {} node[midway, above] {$+$};
  \draw (T.A2) -- ++(-2,0) node[ocirc] (a2) {};
  \draw (T.B2) -- ++(+2,0) node[ocirc] (b2) {};
  \draw[->, shorten >= 4pt, shorten <= 4pt] (a2) -- (a1) node[midway, left] {$v_1$};
  \draw[->, shorten >= 4pt, shorten <= 4pt] (b2) -- (b1) node[midway, right] {$v_2$};
  \draw[<-, shorten <=4pt] (a1) -- ++(-1,0) node[midway, above] {$i_1$};
  \draw[<-, shorten <=4pt] (b1) -- ++(1,0) node[midway, above] {$i_2$};
\end{circuitikz}
\end{document}
```

## Trasformazione di Resistenze

### Da 2 a 1
```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[scale=2, transform shape]
  \node[transformer, anchor=A1] (T) at (2,0) {}
	  (T.north) node{K}
	  (T.outer dot A1) node[circ]{}	
	  (T.outer dot B1) node[circ]{}
  ;
  \draw (T.A1) -- ++(-2,0) node[ocirc] (a1) {};
  \draw (T.B1) -- ++(+2,0) node (b1) {};
  \draw (T.A2) -- ++(-2,0) node[ocirc] (a2) {};
  \draw (T.B2) -- ++(+2,0) node (b2) {};
  \draw[<-, shorten <=4pt] (a1) -- ++(-1,0) node[midway, above] {$i_1$};
  \draw[->, shorten >= 4pt, shorten <= 4pt] (a2) -- (a1) node[midway, left] {$v_1$};
  \draw (b2) to[R, l=$R_L$] (b1);
\end{circuitikz}
\end{document}
```

$$R_{eq} = \frac{v_{1}}{i_{1}} = \frac{Kv_{2}}{-\frac{i_{2}}{K}} = K^2\left( - \frac{v_{2}}{i_{2}} \right) \implies$$
$$\implies \boxed{R_{eq} = K^2R_{L}}$$
### Da 1 a 2

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[scale=2, transform shape]
  \node[transformer, anchor=A1] (T) at (2,0) {}
	  (T.north) node{K}
	  (T.outer dot A1) node[circ]{}	
	  (T.outer dot B1) node[circ]{}
  ;
  \draw (T.A1) -- ++(-2,0) node[ocirc] (a1) {};
  \draw (T.B1) -- ++(+2,0) node[ocirc] (b1) {};
  \draw (T.A2) -- ++(-2,0) node[ocirc] (a2) {};
  \draw (T.B2) -- ++(+2,0) node[ocirc] (b2) {};
  \draw[->, shorten >= 4pt, shorten <= 4pt] (a2) -- (a1) node[midway, left] {$v_1$};
  \draw[->, shorten >= 4pt, shorten <= 4pt] (b2) -- (b1) node[midway, right] {$v_2$};
  \draw[<-, shorten <=4pt] (a1) -- ++(-1,0) node[midway, above] {$i_1$};
  \draw[<-, shorten <=4pt] (b1) -- ++(1,0) node[midway, above] {$i_2$};
  \draw (a2) ++ (-1, 0) to[R, l=$R$] (a1) ++ (-1, 0);
\end{circuitikz}
\end{document}
```
$$R_{eq} = \frac{R_{L}}{K^2}$$
## Trasformazione di Generatori non-ideali di Tensione

### Da 2 a 1
```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[american, scale=2, transform shape]
  \node[transformer, anchor=A1] (T) at (2,0) {}
	  (T.north) node{K}
	  (T.outer dot A1) node[circ]{}	
	  (T.outer dot B1) node[circ]{}
  ;
  \draw (T.A1) -- ++(-2,0) node[ocirc] (a1) {};
  \draw (T.B1) to[R, l=$R_S$] ++(+2,0) node (b1) {};
  \draw (T.A2) -- ++(-2,0) node[ocirc] (a2) {};
  \draw (T.B2) -- ++(+2,0) node (b2) {};
  \draw[->, shorten >= 4pt, shorten <= 4pt] (a2) -- (a1) node[midway, left] {$v_1$};
  \draw[->, shorten >= 4pt, shorten <= 4pt] (T.B2) -- (T.B1) node[midway, left] {$v_2$};

  \draw (b2) to[V, invert, l=$V_S$] (b1);
\end{circuitikz}
\end{document}
```
Circuito Equivalente di Thevenin:
```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[american, scale=2, transform shape]
	\draw (0,0) node[ocirc] {} to[R, l=$K^2R_S$] (2,0)
	to[V, v=$KV_S$] (2,-2)
	-- (0, -2) node[ocirc] {};
\end{circuitikz}
\end{document}
```
### Da 1 a 2

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[american, scale=2, transform shape]
  \node[transformer, anchor=A1] (T) at (2,0) {}
	  (T.north) node{K}
	  (T.outer dot A1) node[circ]{}	
	  (T.outer dot B1) node[circ]{}
  ;
  \draw (T.A1) to[R, l=$R_S$] ++(-2,0) node (a1) {};
  \draw (T.B1) -- ++(+2,0) node[ocirc] (b1) {};
  \draw (T.A2) -- ++(-2,0) node (a2) {} to[V, v=$V_S$, invert] (a1);
  \draw (T.B2) -- ++(+2,0) node[ocirc] (b2) {};
  \draw[->, shorten >= 4pt, shorten <= 4pt] (T.A2) -- (T.A1) node[midway, left] {$v_1$};
  \draw[->, shorten >= 4pt, shorten <= 4pt] (b2) -- (b1) node[midway, right] {$v_2$};
\end{circuitikz}
\end{document}
```
