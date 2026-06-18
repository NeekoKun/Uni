#IeS 

## Densità di Probabilità Condizionata
Sappiamo che:
$$P(x \leq X \leq x + \delta)\ \tilde{=}\ \delta \cdot f_{X}(x)$$
per analogia, vogliamo trovare
$$P(x \leq X \leq x + \delta_{x} | y \leq Y \leq y + \delta_{y})\ \tilde{=}\ \delta_{x}f_{X|Y}(x|y)$$
> [!error] Dimostrazione
> $$P(x \leq X \leq x + \delta_{x} | y \leq Y \leq y + \delta_{y}) = \frac{P(x \leq X \leq x + \delta_{x} , y \leq Y \leq y + \delta_{y})}{P(y \leq Y \leq y + \delta_{y})}=$$
> $$=\frac{f_{X,Y}(x,y)\delta_{x}\delta_{y}}{f_{Y}(y)\delta_{y}}=\frac{f_{X,Y}(x,y)\delta_{x}}{f_{Y}(y)}\implies$$
> $$\implies \lim_{ \delta_{x} \to 0 } \frac{P(x \leq X \leq x + \delta_{x} | y \leq Y \leq y + \delta_{y})}{\delta_{x}} = \frac{f_{X,Y}(x,y)}{f_{Y}(y)} = \boxed{f_{X|Y}(x|y)}$$

> [!warning] Utilizzo
> $$f_{Y|X}(y|x) = \frac{f_{X,Y}(x,y)}{f_{X}(x)} = \frac{f_{X,Y}(x,y)}{\int\limits_{\mathbb{R}}f_{X,Y}(x,t)dt}$$