#analisi 
> [!error] Teorema
> Sia $f:(a,b) \to \mathbb{R}$ derivabile in $(a,b)$. Allora:
> 1. $f$ crescente in $(a,b) \Leftrightarrow f'(x) \geq 0\ \forall\ x \in (a,b)$
> 2. $f$ decrescente in $(a,b) \Leftrightarrow f'(x) \leq 0\ \forall\ x \in (a,b)$
> 3. $f'(x) > 0\ \forall\ x \in (a,b) \implies f$ strettamente crescente in $(a,b)$
> 4. $f'(x) < 0\ \forall\ x \in (a,b) \implies f$ strettamente decrescente in $(a,b)$

> [!info] Osservazione
> Esempio:
> $$f(x) = x^3$$ è una funzione strettamente crescente ma la sua derivata si annulla in $x = 0$

> [!info] Osservazione
> Esistono funzioni monotone strette e derivabili in $(a,b)$ tali che $$f'(x) \geq 0$$ ma tali che $f'(x) = 0$ per qualche $x_{0}\in (a,b)$
> Quindi in 3. e 4. non vale "Se e solo se" 

> [!info] Osservazione
> Il Test di Monotonia permette di individuare massimi e minimi locali per $f$:
> - Se $f$ cresce in $[x_{0}-\delta, x_{0}]$ e decresce in $[x_{0}, x_{0} + \delta]$ allora $x_{0}$ è Massimi, [[Massimi, Minimi ed Estremanti#Massimo/Minimo|Massimo Locale]] di $f$
> - Viceversa per il [[Massimi, Minimi ed Estremanti#Massimo/Minimo|Minimo Locale]]

> [!error] Dimostrazione
> Solo in casi in cui $f$ è crescente in $(a,b)$
> - Sia $f:(a,b) \to \mathbb{R}$ derivabile e crescente in $(a,b)$. Allora vogliamo dimostrare che $f'(x) \geq 0\ \forall\ x \in (a,b)$
> Sia $x \in (a,b), h \in \mathbb{R} : |h|$ abbastanza piccolo in modo che $x+h \in (a,b), h\neq 0$.
> Se $h > 0 \implies x + h > x \Leftrightarrow f(x + h) > f(x)$ perché $f$ monotona
> Allora $\forall\ h \neq 0$ $$\frac{f(x+h) - f(x)}{h} \geq 0$$
> Poiché $f$ è derivabile $\exists$ $$f'(x) = \lim_{ h \to 0 } \frac{f(x+h)-f(x)}{h}$$
> per [[Teorema di Permanenza del Segno dei Limiti]] $f'(x) \geq 0$ 
> - Se $f:(a,b) \to \mathbb{R}$ derivabile e $f'(x)  \geq 0\ \forall\ x \in (a,b)$ allora $f$ è crescente in $(a,b)$
> Siano $x_{1},x_{2} \in (a,b)$, con $x_{1} < x_{2}$.
> Vogliamo dimostrare che $f(x_{1}) \leq f(x_{2})$
> Poiché $[x_{1}, x_{2}] \subseteq (a,b)$, essendo $f$ derivabile e quindi continua in $(a,b)$, $f$ sarà continua e derivabile anche in $[x_{1},x_{2}]$
> Per il [[Teorema del Valore Medio di Lagrange]] $\exists$ $c \in (x_{1}, x_{2}) \subseteq (a,b)$ tale che:
> $$\frac{f(x_{2}) - f(x_{1})}{x_{2} - x_{1}} = f'(c) \geq 0$$
> perché $f'(x) \geq 0\ \forall\ x \in (a,b)$ per ipotesi
> $\implies f(x_{2}) - f(x_{1}) = f'(c)(x_{2} - x_{1}) \geq 0$
> $\implies f(x_{2}) \geq f(x_{1})$
> Poiché ciò è vero $\forall\ x_{1}, x_{2} \in (a,b)$ con $x_{1} < x_{2}$, per definizione $f$ è crescente in $(a,b)$
> - Se $f:(a,b) \to \mathbb{R}$ derivabile e $f'(x)  > 0\ \forall\ x \in (a,b)$ allora $f$ è crescente in $(a,b)$
> Siano $x_{1},x_{2} \in (a,b)$, con $x_{1} < x_{2}$.
> Vogliamo dimostrare che $f(x_{1}) < f(x_{2})$
> Poiché $[x_{1}, x_{2}] \subseteq (a,b)$, essendo $f$ derivabile e quindi continua in $(a,b)$, $f$ sarà continua e derivabile anche in $[x_{1},x_{2}]$
> Per il [[Teorema del Valore Medio di Lagrange]] $\exists$ $c \in (x_{1}, x_{2}) \subseteq (a,b)$ tale che:
> $$\frac{f(x_{2}) - f(x_{1})}{x_{2} - x_{1}} = f'(c) > 0$$
> perché $f'(x) > 0\ \forall\ x \in (a,b)$ per ipotesi
> $\implies f(x_{2}) - f(x_{1}) = f'(c)(x_{2} - x_{1}) > 0$
> $\implies f(x_{2}) > f(x_{1})$
> Poiché ciò è vero $\forall\ x_{1}, x_{2} \in (a,b)$ con $x_{1} < x_{2}$, per definizione $f$ è crescente in $(a,b)$
