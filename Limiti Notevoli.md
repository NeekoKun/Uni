#analisi 
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

> [!error] $\lim_{ x \to 0 } \frac{\log(1 + x)}{x} = 1$
> Poichè $\log t$ è funzione continua, per cambio di variabile ($\dfrac{1}{t} = x$)
> $1 = \lim_{ t \to \infty } t \log\left( 1+\frac{1}{t} \right) = \lim_{ x \to 0 } \frac{\log(1+x)}{x}$

> [!error] $\lim_{ x \to 0 } \frac{e^x-1}{x} = 1$
> Per cambio di variabile $e^x -1 = t \Leftrightarrow e^x = t + 1 \Leftrightarrow x = \log(1 + t)$
> $$\lim_{ x \to 0 } \frac{e^x + 1}{x} = \lim_{ t \to 0 } \frac{t}{\log (1 + t)} = \frac{1}{1} = 1$$

> [!error] $\lim_{ x \to 0 } \frac{(1 + x)^\alpha - 1}{x} = \alpha$
> Ovvio per $\alpha = 0$. Se $\alpha \neq 0$
> $$(1+x)^\alpha = e^{\alpha \log(1 + x)} - 1$$
> $$\lim_{ x \to 0 } \frac{(1+x)^\alpha - 1}{x} = \lim_{ x \to 0 } \frac{e^{\alpha \log(1 + x)} - 1}{x}$$ $$\lim_{ x \to 0 } \frac{e^{\alpha \log(1 + x)} - 1}{x} = \lim_{ x \to 0 } \frac{e^{\alpha \log(1 + x)} - 1}{\alpha \log(1+x)} \cdot \frac{\alpha \log(1 + x)}{x}$$
> $$= 1 \cdot \alpha \cdot 1 = \alpha$$

> [!error] $\lim_{ x \to 0 } \frac{\sin x}{x} = 1$
> $$0 \leq \sin x \leq x \leq \tan x \implies \cos x \leq \frac{\sin x}{x} \leq 1$$
> $$\cos 0 = 1 \implies \lim_{ x \to 0 } \frac{\sin x}{x} = 1$$
> Per [[Teorema dei due Carabinieri]]

> [!error] $\lim_{ x \to 0 } \frac{1 - \cos x}{x^2} = \frac{1}{2}$
> $\cos x = 1 - 2\sin^2\left( \frac{x}{2} \right)$
> $$\implies \frac{1 - \cos x}{x^2} = \frac{ 1 - ( 1 - 2\sin^2\left( \frac{x}{2} \right))}{x^2}$$
> $$= \frac{2 \sin \frac{x}{2} \sin \frac{x}{2}}{4 \frac{x}{2} \frac{x}{2}} = \frac{2}{4} = \boxed{\frac{1}{2}}$$