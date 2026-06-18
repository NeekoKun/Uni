#IeS #TODO 
> [!warning] Definizione
> Sicuramente è non-negativa, ed è la media delle [[Autoinformazione|Autoinformazioni]] degli eventi di un sistema [???]

## Entropie Notevoli
---
#### Entropia di Bernoulliana
$$H_{b}(p) = p \log\left( \frac{1}{p} \right) + (1-p)\log\left( \frac{1}{1-p} \right) [\text{bit}]$$
$$\lim_{ p \to 0 \lor p \to 1 } \frac{d}{dp}H_{b}(p) = \pm \infty$$
#### Entropia di Geometrica
$$H_{g}(p) =  [\text{bit}]$$

## Interpretazione Statistica
- Stato termodinamico:
	- Funzione di [[Pressione]], [[Temperatura]], [[Volume]] etc
- Stato dinamico:
	- Coordinate e variabili meccaniche delle particelle di un sistema

==Più stati dinamici portano agli stessi stati termodinamici==

> [!warning] Formulazione
> Siano $n$ il numero di particelle in un sistema, ed $n_{r}$, $n_{l}$ rispettivamente il numero di particelle nella partizione destra e sinistra del sistema. Possiamo calcolare il numero di combinazioni possibili $\Gamma$ come:
> $$\Gamma = \frac{n!}{n_{r}! \cdot n_{l}!}$$

> [!info] Osservazione
> Il massimo di questo $\Gamma$ si ottiene con un bilanciamento tra $n_{r}$ e $n_{l}$, dunque uno stato di equilibrio è quello statisticamente più probabile. Questo è il significato statistico dell'entropia, ovverosia che i sistemi tendono allo stato **statisticamente più probabile**. Per calcolare $S$ da $\Gamma$;
> $$S = K_{B}\ln \Gamma$$
> dove
> $$K_{B} = \frac{R}{N_{A}} \approx 1.38 \cdot 10 ^ {-23} \frac{J}{K}$$