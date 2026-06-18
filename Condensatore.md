---
aliases:
  - Capacitore
  - Capacitor
---
#ELT 

## Scrittura

```tikz
\usepackage{circuitikz}

\begin{document}
\begin{circuitikz}[american, voltage shift=0.5]
  % Left pole
  \draw (0,0) node[circ] {};
  
  % Right pole
  \draw (3,0) node[circ] {};
  
  % Capacitor
  \draw (0,0) to[C] (3,0);
  
  % Charges on plates
  \node at (1.3,-0.5) {$+q$};
  \node at (1.7,-0.5) {$-q$};
  
  % Capacitance label
  \node at (1.5,-1.0) {$C$};
  
  % Curved voltage arrow and label
  \draw[->] (0,0.2) to[out=45, in=135] (3,0.2);
  \node at (1.5,1.2) {$V_c$};
  
  % Current label on left pole
  \node at (-0.5,0) {$i_C$};

\end{circuitikz}
\end{document}
```

## Relazioni Costitutive
- $q = C\cdot v_{C};\ [F]$ "Farad"
- $i_{C}(t) = C \dfrac{dv_{C}}{dt}$
	- $i_{C}dt = Cdv_{C} \implies \int i_{C}dt =\int Cdv_{C} \implies$ $$ \implies \boxed{v_{C}(t) = v_{C}(t_{0}) + \frac{1}{C}\int_{t_{0}}^t i_{C}(t')dt'}$$

## Proprietà

> [!warning] (a) Regime Costante
> $$v_{C}(t) \text{ costante} \implies i_{C} = 0$$
> Quindi, con $t \to \infty$, un condensatore a **Regime Costante** è un **Circuito Aperto**

> [!warning] (b) $v_{C}$ è continua in $t$
> $$\lim_{ t \to t_{0}^+ } v_{C}(t) = \lim_{ t \to t_{0}^- } v_{C}(t) = v_{C}(t_{0})$$
> in termini semplici:
> $$v_{C}(t_{0}^+) = v_{C}(t_{0}^-) = v_{C}(t_{0})$$

