#analisi
- $\mathbb{C}: \{z = a + ib:\ a, b \in \mathbb{R}, i^2 = -1\}$
- Otteniamo polinomi algebricamente completi
- è un [[Campi|Campo]]

> [!info] Osservazione
> $x^2 + 1 = 0$ non ha soluzioni in ==nessun [[Campi|Campo]] Ordinato==
> Infatti in un Campo Ordinato X cale sempre che
> - $x^2 \geq 0\ \forall\ x \in X$
> - $1 > 0$
> - $\implies 1 \geq 1$
> - $\implies 1 + x^2 \geq 1 > 0$
> - $\implies 1 + x^2 > 0$
> - $\implies 1 + x^2 \neq 0\ \forall\ x \in X$

### Costruzione del [[Campi|Campo]]
È possibile costruire un campo (non ordinato) che estenda $\mathbb{R}$ tale che $x^2 + 1 =0$ ammetta una soluzione?
> [!warning] Definizione di $i$
> $i^2 = -1$

> [!warning] Definizione di Parte **Reale** e Parte **Immaginaria**
> $\mathbb{C} = \{ z = a+ib : a,b \in \mathbb{R} \}$
> $z = a+ib$ prende il nome di "Forma Algebrica" del numero complesso
> $a = \mathrm{Re}\ z$
> $b = \mathrm{Im}\ z$ 

> [!warning] Definizione di **Somma** e **Prodotto**
> $\forall\ z = a+ib,\ w =x+iy \in \mathbb{C}$
> $\implies z+w=(a+x)+i(b+y)$
> $\implies z \cdot w = (ax-by) + i(bx+ay)$

> [!info] Osservazione
> Le operazioni + e $\cdot$ in $\mathbb{C}$ sono definite formalmente come somme e prodotti di polinomi a coefficienti reali id grado 1 in $i$, con in più una regola aggiuntiva: $i^2 = -1$

> [!error] Teorema
> $\mathbb{C}$ con $+$ e $\cdot$ è un [[Campi|Campo]]
> Non lo dimostreremo, le proprietà di somme e prodotto derivano dalle loro stesse proprietà in $\mathbb{R}$

- In $\mathbb{C}$ l'elemento neutro di + è $0 = 0+i0$
- In $\mathbb{C}$ l'elemento neutro di $\cdot$ è $1 = 1+i 0$

> [!info] Osservazione
> $z = a+ib \in \mathbb{C}$
> $\implies -z = -a-ib$
> $z \in \mathbb{C}, z \neq 0$
> $\implies z^{-1} = \frac{1}{z} = \frac{a}{a^2+b^2} -i \frac{b}{a^2 + b^2}$

> [!info] Osservazione
> $\mathbb{R} \subset \mathbb{C}$
> $\implies$ R è un sottocampo di $\mathbb{C}$:
> Le strutture sopra coincidono con le strutture sottostanti

> [!info] Osservazione
> Ogni punto $z \in \mathbb{C}$ può essere rappresentato su un piano cartesiano con coordinate:
> 
> $$(a,b) \in \mathbb{R}^2:a=\mathrm{Re}\ z,\ b = \mathrm{Im}\ z$$
> 
> In particolare, ogni numero complesso $z = a+ib$ può anche essere pensato come vettore nel piano applicato in 0 ed avente altro estremo in $(a,b)$, orientato da 0 ad $(a,b)$

> [!info] Osservazione
> Sommare due numeri complessi corrisponde a sommare i corrispondenti vettori che li rappresentano tramite la regola del parallelogramma

> [!warning] Definizione di **Coniugato** e **Modulo**
> Dato $z = x+iy \in \mathbb{C}$:
> Chiamiamo $\overline{z} = x-iy$ "Complesso Coiugato" di $z \in \mathbb{C}$.
> Chiamiamo $|z| = \sqrt{ x^2 + y^2 }$ "Modulo" di $z \in \mathbb{C}$ 

> [!info] Osservazione
>- $z \cdot \overline{z} = |z|^2$
>- $z^{-1} = \frac{1}{z} \cdot \frac{\overline{z}}{z} = \frac{\overline{z}}{|z|}$
>- $\overline{(z + w)} = \overline{z} + \overline{w}$
>- $\overline{(z \cdot w)} = \overline{z} \cdot \overline{w}$

> [!warning] Definizione di **Forma Trigonometrica** e **Forma Esponenziale**
> Per individuare $z =a+ib\in \mathbb{C}$ possiamo assegnare $\theta = arg(z),\ \rho=\sqrt{ a^2+b^2 }=|z|$

> [!info] Osservazione
> - $arg(0)$ non è ben definito
> - $arg(z)$ è definito a meno di multipli interi di $2\pi$