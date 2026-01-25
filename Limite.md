#analisi 
## Definizione
> [!warning] Definizione Topologica di Limite
> Sia $f: I \subseteq \mathbb{R} \to \mathbb{R}, x_{0} \in \overline{\mathbb{R}}$ punto di accumilazione di $I$,$l \in \overline{\mathbb{R}}$ diremo che
> $$\lim_{ x \to \infty } f(x)=l$$
> se e solo se per ogni intorno $u(l)$ di $l$ esiste un intorno $u(x_{0})$ di $x_{0}$ tale che
> $$
>\begin{cases} x \in u(x_{0})  \\
 x \in I \\
 x \neq x_{0}
\end{cases} \implies f(x) \in u(l)$$
> a.k.a.
$$x \in (u(x_{0}) \cap I) \setminus \{ x_{0} \}$$

> [!warning] Definizione Metrica
> 1. Limite finito all'infinito ($l \in \mathbb{R}, x_{0} = \pm \infty$)
> 	- $\lim_{ x \to +\infty } f(x) = l$
> 	$\forall\ \epsilon > 0\ \exists\ M \in \mathbb{R} : x > +M \implies l - \epsilon < f(x) < l + \epsilon$
> 	- $\lim_{ x \to -\infty } f(x) = l$
> 	$\forall\ \epsilon > 0\ \exists\ M \in \mathbb{R} : x < -M \implies l-\epsilon < f(x) < l + \epsilon$
> 2. Limite infinito all'infinito ($l = \pm \infty, x_{0} = \pm \infty$)
> 	- $\lim_{ x \to +\infty } f(x) = +\infty$
> 	$\forall\ M > 0\ \exists\ N > 0 : x > +N \implies f(x) > +M$
> 	- $\lim_{ x \to +\infty } f(x) = -\infty$
> 	$\forall\ M > 0\ \exists\ N > 0 : x > +N \implies f(x) < -M$
> 	- $\lim_{ x \to -\infty } f(x) = +\infty$
> 	$\forall\ M > 0\ \exists\ N > 0 : x < -N \implies f(x) > +M$
> 	- $\lim_{ x \to -\infty } f(x) = -\infty$
> 	$\forall\ M > 0\ \exists\ N > 0 : x < -N \implies f(x) < -M$
> 3. Limite infinito al finito ($l = \pm \infty, x_{0} \in \mathbb{R}$)
> 	- $\lim_{ x \to x_{0} } f(x) = +\infty$
> 	$\forall\ M > 0\ \exists\ \delta > 0 : \begin{cases} x_{0} - \delta < x < x_{0} + \delta \\ x \neq x_{0} \end{cases} \implies f(x) > +M$
> 	- $\lim_{ x \to x_{0} } f(x) = -\infty$
> 	$\forall\ M > 0\ \exists\ \delta > 0 : \begin{cases} x_{0} - \delta < x < x_{0} + \delta \\ x \neq x_{0} \end{cases} \implies f(x) < -M$
> 4. Limite finito al finito ($l \in \mathbb{R}, x_{0} \in \mathbb{R}$)
> 	- $\lim_{ x \to x_{0} }f(x) = l$
> 	$\exists\ \epsilon > 0\ \exists\ \delta > 0 : \begin{cases} x_{0} - \delta < x < x_{0} + \delta \\ x \neq x_{0} \end{cases} \implies l - \epsilon < f(x) < l + \epsilon$

> [!info] Osservazione
> Talvolta è necessario distinguere il comportamento al limiti di $f$ a seconda che $x$ si avvicini ad $x_{0}$ da destra o da sinistra

> [!warning] Definizione
> Data $f: I \subseteq \mathbb{R} \to \mathbb{R},\ x_{0} \in \mathbb{R}$ di accumulazione per $I$, diremo che
> - $$\lim_{ x \to x_{0}^+ } f(x) = +\infty$$
> $\forall\ M > 0\ \exists\ \delta > 0 :$ 
> $$x_{0} < x < x_{0} + \delta \implies f(x) > M$$
> - $$\lim_{ x \to x_{0}^- } f(x) = +\infty$$
> $\forall\ M > 0\ \exists\ \delta > 0 :$ 
> $$x_{0} - \delta < x < x_{0} \implies f(x) > M$$

[...]
## Algebra dei Limiti
> [!warning] Definizione
> Siano $$\lim_{ x \to x_{0} } f(x) = l_{1}, \lim_{ x \to x_{0} }g(x) = l_{2}$$
> Allora:
> - $\lim_{ x \to x_{0} } f(x) + g(x) = l_{1} + l_{2}$
> - $\lim_{ x \to x_{0} } f(x) \cdot g(x) = l_{1} l_{2}$
> - $\lim_{ x \to x_{0} } \cfrac{f(x)}{g(x)} = \cfrac{l_{1}}{l_{2}}$
> - $\lim_{ x \to x_{0} }f(x)^{g(x)} = l_{1}^{l_{2}}$
> - $\lim_{ x \to x_{0} } f(x)^\alpha = l_{1}^\alpha$
> 
> A meno di **Forme di Indeterminazione**
> - $\infty - \infty$
> - $0 \cdot \infty$
> - $\frac{0}{0}$
> - $\frac{\infty}{\infty}$
> - $1^{\pm \infty}$
> - $\infty^0$
> - $0^0$

## Asintotici e $\sigma$
> [!warning] Definizione
> Date due funzioni $f, g$ e $x_{0} \in \overline{\mathbb{R}}$ diremo che:
> - $f(x)$ ~ $g(x)$ per $x \to x_{0}$ se $$\lim_{ x \to x_{0} } \frac{f(x)}{g(x)} = 1$$
> - $f(x)$ = $\sigma(g(x))$ per $x \to x_{0}$ se $$\lim_{ x \to x_{0} } \frac{f(x)}{g(x)} = 0$$

> [!warning] Definizione
> Data $f$ e $x_{0} \in \overline{\mathbb{R}}$ diremo che:
> - $f$ è infinitesima per $x \to x_{0}$ se $$\lim_{ x \to x_{0} } f(x) = 0$$
> - $f$ è infinita per $x \to x_{0}$ se $$\lim_{ x \to x_{0} } f(x) = \pm \infty$$

> [!info] Osservazione
> - Se $\lim_{ x \to x_{0} } \frac{f(x)}{g(x)} = \lambda \in \mathbb{R} \setminus \{ 0 \}$
> allora $f(x)$ ~ $\lambda g(x)$ per $x \to x_{0}$
> - Se $\lim_{ x \to x_{0} } \frac{f(x)}{g(x)} = \pm \infty$
> allora $\lim_{ x \to x_{0} } \frac{g(x)}{f(x)} = 0$ per $x \to x_{0}$
> allora $g(x) = \sigma(f(x))$

> [!info] Osservazione
> $f(x)$ ~ $g(x)$ per $x \to x_{0}$
> se e solo se $f(x) = g(x) + \sigma(g(x))$ per $x \to x_{0}$

> [!error] Proposizione
> 1. $f_{1}$ ~ $f_{2}$ e $g_{1}$ ~ $g_{2}$ per $x \to x_{0}$
> $$\implies f_{1} \cdot g_{1} ~ f_{2} \cdot g_{2}$$
> $$\implies \frac{f_{1}}{g_{1}} ~ \frac{f_{2}}{g_{2}}$$
> $$\implies f_{1}^\alpha ~ f_{2}^\alpha$$
> 2. $f$ ~ $g$ per $x \to x_{0}$
> $$\implies \exists\ \lim_{ x \to x_{0} } f(x) \in \overline{\mathbb{R}}$$
> $$\Leftrightarrow $$

> [!error] Dimostrazione
> 1. nelle ipotesi $$\frac{f_{1}g_{1}}{f_{2}g_{2}} = \frac{f_{1}}{f_{2}} \cdot \frac{g_{1}}{g_{2}} \to 1$$
> per $x \to x_{0}$ (algebra dei limiti)
> $\implies f_{1} \cdot g_{1}$ ~ $f_{2} \cdot g_{2}$
> $$\frac{\frac{f_{1}}{g_{1}}}{\frac{f_{2}}{g_{2}}} = \frac{f_{1}g_{2}}{f_{2}g_{1}} = \frac{f_{1}}{f_{2}} \cdot \frac{g_{1}}{g_{2}}^{-1} \to 1$$ per $x \to x_{0}$
> $$\frac{f_{1}^\alpha}{f_{2}^\alpha} = \frac{f_{1}}{f_{2}}^\alpha \to 1$$
> per $x \to x_{0}$ (algebra dei limiti)
> 2. Per $x \to x_{0}$ scriviamo $f(x) = \frac{f(x)}{g(x)} \cdot g(x)$
> poichè $\lim_{ x \to x_{0} } \frac{f(x)}{g(x)} = 1$, se $$\exists\ \lim_{ x \to x_{0} }g(x) = l \in \overline{\mathbb{R}}$$ $$\implies \lim_{ x \to x_{0} } f(x) = \lim_{ x \to x_{0} } \frac{f(x)}{g(x)} \cdot g(x) = 1 \cdot l = l$$ Invertendo le funzioni troviamo che $$\exists\ \lim_{ x \to x_{0} } f(x) = l \in \overline{\mathbb{R}} \leftrightarrow \exists\ \lim_{ x \to x_{0} } g(x) = l \in \overline{\mathbb{R}}$$

## Limiti Notevoli
- $\lim_{ x \to 0 } \frac{\sin(x)}{x} = 1$
-> $\sin x$ ~ $x$
- $\lim_{ x \to 0 } \frac{1 - \cos(x)}{x^2} = \frac{1}{2}$
-> $\cos x = 1 - \frac{1}{2}x^2 + \sigma(x^2)$
- $\lim_{ x \to \pm \infty } (1 + \frac{1}{x})^x = e$
-> Questo risultato lo abbiamo enunciato ma non dimostrato
- $\lim_{ x \to 0 } \frac{\log(1 + x)}{x} = 1$
-> $\log(1 + x)$ ~ $x$
- $\lim_{ x \to 0 } \frac{e^x - 1}{x} = 1$
- $\lim_{ x \to 0 } \frac{(1+x)^\alpha -1}{x} = \alpha \forall\ \alpha \in \mathbb{R}$
-> $(1 + x)^\alpha -1$  ~ $\alpha x$
-> $(1 + x)^\alpha = 1 + \alpha x + \sigma(x)$
- $\lim_{ x \to 0 } \frac{\tan(x)}{x} = 1$
- $\lim_{ x \to 0 } \frac{\arctan(x)}{x} = 1$

> [!info] Osservazione
> Dalle formule precedenti e dal teorema di [[Cambio di Variabile nei Limiti]] segue che se $\varepsilon(x)$ è una funzione tale che $$\lim_{ x \to x_{0} } \varepsilon(x) = 0$$ allora per $x \to x_{0}$
> $$\lim_{ x \to x_{0} } \frac{\sin(\varepsilon(x))}{\varepsilon(x)} = \lim_{ t \to 0 } \frac{\sin(t)}{t} = 1$$
## Teoremi
- [[Teorema di Unicità del Limite]]
- [[Teorema Ponte]]
- [[Teorema sul Limite di Funzione]]
- [[Teorema del Confronto tra Limiti]]
- [[Teorema del Confronto per Limite Infinito]]
- [[Teorema di Permanenza del Segno dei Limiti]]
- [[Teorema di Gerarchia degli Infiniti]]
- [[Teorema degli Zeri]]
- [[Teorema di Weierstrass]]
- [[Teorema di Permanenza del Segno]]
- [[Teorema dei due Carabinieri]]
- [[Teorema del Confronto tra successioni divergenti]]
- [[Teorema di Aritmetizzazione Parziale di Infinito]]
- [[Teorema di ???]]
- [[Teorema del Rapporto per Successioni]]
- [[Limiti Notevoli]]
