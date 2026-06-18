#ELT 
> [!error] Teorema
> Ipotesi:
> - Bipolo Lineare adinamico
> - Bipolo è Comandabile in Corrente: $\exists\ f: V = f(i)$
>
> Tesi:
> La relazione costitutiva $v = f(i)$ è la retta $$\boxed{V = V_{T} - R_{T}i}$$ e quindi il bipolo $\beta$ è esternamente equivalente al seguente generatore non ideale di tensione:
> ```tikz
>\usepackage{circuitikz}
>\begin{document}
>
>\begin{circuitikz}[american, voltage shift=0.5]
>\draw (6,0)
>to[short, *-] (0,0)
>to[vsource, v=$V_T$] (0,3)
>to[R=$R_T$, -*] (6,3);
>\draw (6,0) to[short, i=$V$] (6,3);
>\draw[->] (6,3) -- (7,3);
>\end{circuitikz}
>
>\end{document}
>```