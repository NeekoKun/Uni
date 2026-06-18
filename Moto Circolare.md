#FIS 
Caso particolare del [[Moto Curvilineo]]

#TODO graph

Coordinate Intrinseche:
$\hat{u}_{t} \perp\text{raggio}$
$\hat{u}_{n} \parallel\text{raggio}$
$v(t) = \dfrac{ds}{dt}\hat{u}_{t}$

Coordinate Polari:
$\hat{u}_r \parallel\text{raggio}$
$\hat{u}_{\theta} \perp\text{raggio}$

$r(t) = R =\text{costante}$
$s(t) = R\cdot\theta(t)$

$v(t) = \dfrac{dr}{dt}\hat{u}_{r} + r(t) \dfrac{d\theta}{dt}\hat{u}_{\theta} = R \dfrac{d\theta}{dt}\hat{u}_{t}$
Qui $\dfrac{d\theta}{dt} = \omega$, detta "==Velocità Angolare==", dove $[\omega] = \dfrac{\text{rad}}{\text{s}}$

## Accelerazione

- Coordinate Intrinseche

$a = a_{t} + a_{N} = \frac{dv}{dt}\hat{u}_{t} + \frac{v^2(t)}{\rho}\hat{u}_{N}$

- Coordinate Polari

$a = R \frac{dw}{dt} \hat{u}_{t} + \omega^2(t)R \hat{u}_{N} = R \frac{dw}{dt} \hat{u}_{\theta }- \omega^2(t)R \hat{u}_{r}$

Quindi:

$$\boxed{\begin{cases}
s(t) = \theta(t) R \\
v(t) = \omega(t) R \\
a(t) = \alpha(t) R
\end{cases}}
$$

> [!warning] Definizione
> - $\vec{\omega} \perp$ $\{ \vec{v}, \vec{r}(t) \}$
> - verso $\implies$ attraverso la regola della mano destra
> - $v = \omega R$
> $\implies \vec{v} = \vec{\omega} \times \vec{r}$

## Casi Particolari

- [[Moto Circolare Uniforme]]
- [[Moto Circolare Uniformemente Accelerato]]