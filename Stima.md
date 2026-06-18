#IeS 

## Come stimare un valore da una distribuzione sondaggistica?

### Least Mean Square
> [!error] Least Mean Square (LMS)
> Vogliamo minimizzare $$E[(\Theta - \hat{\Theta})^2]$$ che possiamo ridurre ad una generica $h(c)$ dove $c = \hat{\Theta}$ che è la nostra stima

> [!warning] Risoluzione
> Per trovare il minimo di $h(c)$:
> $$\frac{dh(c)}{dc} = \frac{d}{dc}E[(\Theta - c)^2] = \frac{d}{dc}(E[\Theta^2] - 2cE[\Theta] + c^2)$$
> $$-2E[\Theta] + 2c \overset{!}{=} 0 \implies c = E[\Theta]$$

> [!info] Conclusione
> Il valore atteso ($E[\Theta]$) è dunque il valore che minimizza l'errore quadratico medio. Peraltro, $$h(E[\Theta]) = E[(\Theta - E[\Theta])^2] = \mathrm{Var}[\Theta]$$
> E quindi $\mathrm{Var}[\Theta]$ è detto **Minimum Mean Square Error** (MMSE)

> [!warning] Osservazione
> Nel caso di una probabilità $\Theta$ condizionata ad $X$, $$h(c) = \mathrm{Var}[\Theta|X=x]$$ ed in generale, per tutte le realizzazioni di $X$: $$h(c) = E[\mathrm{Var}[\Theta | X]]$$
> E peraltro, $$\mathrm{Var}[\Theta] = E[\mathrm{Var}[\Theta|X]] + \mathrm{Var}[E[\Theta|X]]$$
> $$\implies \boxed{\mathrm{Var}[\Theta] \geq E[\mathrm{Var}[\Theta|X]]}$$
> E dunque a posteriori l'incertezza diminuisce

#### Least Mean Square con $n$ osservazioni
> [!error] Definizione
> $$\hat{\Theta}(X_{1},X_{2},\dots,X_{n}) = E[\Theta | X_{1},X_{2},\dots,X_{n}] = \int_{\mathbb{R}}\theta f_{\Theta|X_{1},X_{2},\dots,X_{n}}(\Theta|X_{1},X_{2},\dots,X_{n})d\theta$$

> [!warning] Risoluzione
> $$f_{\Theta|X_{1},\dots,X_{n}} = \frac{f_{X_{1},\dots,X_{n}|\Theta}(\dots|\dots)f_{\Theta}(\theta)}{f_{X_{1},\dots,X_{n}}(\dots)}$$
> Se c'è indipendenza condizionata delle $X_{i} |\Theta$
> $$f_{X_{1},\dots,X_{n}|\Theta}(\dots|\dots) = \prod_{i=1}^nf_{X_{i}|\Theta}(x_{i}|\theta)$$
> Se $X_{i}|\Theta$ sono [[iid]] allora
> $$f_{X_{1},\dots,X_{n}|\Theta}(\dots|\dots) = \prod_{i=1}^n f_{X|\Theta}(x_{i}|\theta)$$

#### Proprietà
Sia $\hat{\Theta}_{LMS}(X) = E[\Theta|X]$ la stima in Least Mean Square, e l'errore di stima $\tilde{\Theta} = \hat{\Theta}_{LMS} - \Theta$
> [!error] Stima Non Polarizzata
> $E[\tilde{\Theta}] = 0$
> 
>---
> $$E[\tilde{\Theta}|X=x] = E[\hat{\Theta}_{LMS}(X) - \Theta| X = x]$$
> $$= \hat{\Theta}_{LMS}(x) - E[\Theta|X=x] = \hat{\Theta}_{LMS}(x) - \hat{\Theta}_{LMS}(x) = 0\ \ \forall\ x \in \mathbb{R}$$
> $$\implies p(E[\tilde{\Theta}|X] = 0) = 1$$
> $$\implies E[E[\tilde{\Theta}|X]] = \boxed{E[\tilde{\Theta}] = 0}$$

> [!error] Ignota
> $E[\tilde{\Theta} \cdot h(X)] = 0$ per ogni $h$ deterministica
>
> ---
> $$E[\tilde{\Theta} \cdot h(X)|X=x] = E[\tilde{\Theta} \cdot h(x) | X=x] = h(x)\cdot E[\tilde{\Theta}|X=x] = 0\ \ \forall\ x \in \mathbb{R}$$
> $$\implies E[E[\tilde{\Theta} \cdot h(x) | X]] = E[0] = 0$$

> [!error] Ignota
> $\mathrm{Cov}[\tilde{\Theta}, \hat{\Theta}_{LMS}] = 0$
>
> ---
> $$\mathrm{Cov}[\tilde{\Theta}, \hat{\Theta}_{LMS}] = E[\tilde{\Theta} \cdot \hat{\Theta}_{LMS}(X)] - E[\tilde{\Theta}] \cdot E[\hat{\Theta}_{LMS}(X)]$$
> Per proprietà $II$ ed $I$
> $E[\tilde{\Theta} \cdot \hat{\Theta}_{LMS}(X)] = 0$
> $E[\tilde{\Theta}] = 0$
> $$\implies \mathrm{Cov}[\tilde{\Theta}, \hat{\Theta}_{LMS}] = 0 - 0 = 0$$

> [!error] Ignota
> $\mathrm{Var}[\tilde{\Theta}] = E[\mathrm{Var}[\Theta|X]]$
>
> ---
> $$\mathrm{Var}[\Theta] = \mathrm{Var}[\hat{\Theta}_{LMS} - \tilde{\Theta}] = \mathrm{Var}[\hat{\Theta}_{LMS}] + \mathrm{Var}[\tilde{\Theta}] - 2 \mathrm{Cov}[\hat{\Theta}_{LMS}, \tilde{\Theta}]$$
> $$\mathrm{Var}[\Theta] = \mathrm{Var}[E[\Theta|X]] + E[\mathrm{Var}[\Theta|X]]$$
> $$\mathrm{Var}[\hat{\Theta}_{LMS}] = \mathrm{Var}[E[\Theta|X]] \implies \boxed{\mathrm{Var}[\tilde{\Theta}] = E[\mathrm{Var}[\Theta|X]]}$$

> [!info] Volendo minimizzare $\mathrm{Var}[\tilde{\Theta}]$
> Voglio avere $$\mathrm{Var}[\tilde{\Theta}_{LMS}] \approx \mathrm{Var}[\Theta]$$

[[Stimatori Lineari]]
