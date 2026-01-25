#analisi 
> [!error] Teorema
> Sia $f: (a,b) \to \mathbb{R}, x_{0} \in (a,b)$. Allora, **se** $x_{0}$ è un punto di esremo per $f$ e **se** $f$ è derivabile in $x_{0}$, allora $$f'(x_{0}) = 0$$

> [!error] Dimostrazione
> Proviamo il teorema solo nel caso in cui $x_{0}$ sia [[Massimi, Minimi ed Estremanti#Massimo/Minimo|Massimo Locale]].
> Essendo $x_{0}$ punto di Massimo Locale, per $|h|$ sufficientemente piccolo avremo $$f(x_{0} + h) \leq f(x_{0})$$
> Allora se $h > 0$ $$\frac{f(x_{0} + h) - f(x_{0})}{h} \leq 0$$
> Essendo $f$ derivabile in $x_{0}$, per [[Teorema di Permanenza del Segno dei Limiti]] avremo $$f'(x_{0}) = f'_{+}(x_{0}) = \lim_{ h \to o^+ } \frac{f(x_{0}+h) - f(x_{0})}{h} \leq 0$$
> Invece, se $h < 0$: $$\frac{f(x_{0} + h) - f(x_{0})}{h} \geq 0$$
> essendo $f$ derivabile in $x_{0}$, per [[Teorema di Permanenza del Segno dei Limiti]] avremo $$f'(x_{0}) = f'_{-}(x_{0}) = \lim_{ h \to 0^- } \frac{f(x_{0} + h) - f(x_{0})}{h} \geq 0 $$
>Entrambi i limiti esistono per ipotesi. quindi: $$f'(x_{0}) \leq 0 \land f'(x_{0}) \geq 0$$ $$\implies \boxed{f'(x_{0}) = 0}$$ 