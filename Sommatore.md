#ELT 

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[american voltages] 
% Amplificatore operazionale
\draw (4,2) node[op amp] (opamp) {}; 

% Resistenze di ingresso
\draw (0,3.5)
to[R, l=$R_1$, o-] (2,3.5) -- (2,2.3) -- (opamp.-);
\draw (0,2.5)
to[R, l=$R_2$, o-] (2,2.5) -- (2,2.3);
\draw (0,1.5) to[R, l=$R_3$, o-] (2,1.5) -- (2,2.3);

% Etichette ingressi
\draw (0,3.5) node[left] {$V_1$};
\draw (0,2.5) node[left] {$V_2$};
\draw (0,1.5) node[left] {$V_3$};

% Resistenza di feedback
\draw (opamp.out) -- (6,2) -- (6,4)
to[R, l=$R_f$] (2,4) -- (2,2.3);

% Collegamento ingresso non invertente a massa
\draw (opamp.+) -- (3.3,1.7) node[ground] {}; 

% Uscita
\draw (opamp.out)
to[short, -o] (7,2) node[right] {$V_{out}$};

% Annotazioni
\draw[dashed, gray] (2,2.3) circle (0.1);
\draw (2,2.3) node[above right, xshift=0.2cm] {$V_-$};
\end{circuitikz}

\end{document}
```