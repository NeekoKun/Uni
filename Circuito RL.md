#ELT 
```tikz
\usepackage{circuitikz}

\begin{document}
\begin{circuitikz}[american, scale=1.5, transform shape]
  % Draw the RC circuit with voltage source
  \draw (0,0) to[I, l=$V_0$, *-*] (0,3)     % Voltage source
        (0,3) to[R, l=$R$, *-*] (3,3)       % Resistor
        (3,3) to[L, l=$L$, *-*] (3,0)       % Capacitor
        (3,0) to (0,0);                 % Ground return
  
  % Add voltage labels
  \node[above] at (1.5, 2.3) {$V_R$};
  \node[right] at (2, 1.5) {$V_L$};
\end{circuitikz}
\end{document}
```
Dove
$$\tau = \frac{L}{R}$$