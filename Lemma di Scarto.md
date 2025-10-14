#GAL 
> [!error] Teorema
> Dati $\underline{v_{1}},\underline{v_{2}},\dots,\underline{v_{n}} \in V$ linearmente dipendenti
> Allora uno di loro può essere scartato senza cambiare il loro $\mathrm{Span}$

> [!error] Dimostrazione
> $\underline{v_{1}},\dots, \underline{v_{n}} \in V$ L.D.
> $\implies$ uno di essi è combinazione lineare degli altri (possiamo supporre l'ultimo a meno di riordinarli)
> $\implies \sum_{i=1}^{n-1}c_{i}\underline{v_{i}}$ per qualche $c$
> Dobbiamo dimostrare che $\mathrm{Span}(\underline{v_{1}},\dots,\underline{v_{n}}) = \mathrm{Span}(\underline{v_{1}},\dots,\underline{v_{n-1}})$
> - "$\subseteq$": $\forall\ \underline{w} \in \mathrm{Span}(\underline{v_{1}},\dots,\underline{v_{n}})$
> $$\implies \underline{w} = \sum_{i=1}^{n} a_{i}\underline{v_{i}}$$
> $$= \sum_{i=1}^{n-1} a_{i}\underline{v_{i}} + a_{n}\underline{v_{n}}$$
> $$= \sum_{i=1}^{n-1} a_{i}\underline{v_{i}} + a_{n}\sum_{i=1}^{n-1}  c_{i}\underline{v_{i}}$$
> $$=\sum_{i=1}^{n-1} (a_{i} + a_{n}c_{i})\underline{v_{i}} $$
> $\implies \mathrm{Span}(\underline{v_{n}}) \subseteq \mathrm{Span}(\underline{v_{n-1}})$
> - "$\supseteq$": $\forall\ \underline{u} \in \mathrm{Span}(\underline{v_{1}}, \dots, \underline{v_{n-1}})$
> $$\underline{u} = \sum_{i=1}^{n-1} b_{i}\underline{v_{i}}$$
> $$=b_{1}\underline{v_{1}} + \dots + b_{n-1}\underline{v_{n-1}} \boxed{ + 0 \underline{v_{n}}} \in \mathrm{Span}(\underline{v_{1}}, \dots, \underline{v_{n}})$$