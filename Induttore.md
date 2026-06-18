#ELT 

## Scrittura
```tikz
\usepackage{circuitikz}

\begin{document}
\begin{circuitikz}[american, voltage shift=0.5, scale=1.5]
  % Left pole
  \draw (0,0) node[circ] {};
  
  % Right pole
  \draw (3,0) node[circ] {};
  
  % Inductor
  \draw (0,0) to[L] (3,0);
  
  % Magnetic flux symbol (Φ)
  \node at (1.5,-0.5) {$\phi$};
  
  % Inductance label
  \node at (1.5,-1.0) {$L$};
  
  % Curved voltage arrow and label
  \draw[->] (0,0.2) to[out=45, in=135] (3,0.2);
  \node at (1.5,1.2) {$V_L$};
  
  % Current label on left pole
  \node at (-0.5,0) {$i_L$};
\end{circuitikz}
\end{document}
```
## Relazioni Costitutive
- $\phi = Li_{L};\ [H]$ "Farad"
- $V_{L} = \dot{\phi} = L \dot{i_{L}}$
	- $v_{L} = L \dfrac{di_{C}}{dt} \implies$ $$\implies \boxed{i_{L}(t) = i_{L}(t_{0}) + \frac{1}{L} \int_{t_{0}}^t v_{L}(t')dt'}$$

## Proprietà

> [!warning] (a) Regime Costante
> $$i_{C}(t) \text{ costante} \implies v_{C} = 0$$
> Quindi, con $t \to \infty$, un condensatore a **Regime Costante** è un **Cortocircuito**

> [!warning] (b) $i_{C}$ è continua in $t$
> $$\lim_{ t \to t_{0}^+ } i_{C}(t) = \lim_{ t \to t_{0}^- } i_{C}(t) = i_{C}(t_{0})$$
> in termini semplici:
> $$i_{C}(t_{0}^+) = i_{C}(t_{0}^-) = i_{C}(t_{0})$$