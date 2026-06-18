#FIS 
> [!warning] Definizione
> Un **Pendolo Fisico** è un pendolo che, al posto di essere composto di un filo + un Punto Materiale, è composto da un punto rigido fissato nello spazio ad un punto diverso dal suo centro di massa, detto $\Omega$

$$\vec{M}_{e} = \vec{r} \times \vec{F}_{p} = -rmg\sin(\pi - \theta) \hat{u}_{z}$$
$$= -rmg \sin(\theta)\hat{u}_{z}$$
$$\vec{M}_{e} = I_{\Omega}\vec{\alpha} = I_{\Omega} \frac{d^2\theta}{dt^2}\hat{u}_{z}$$
$$\implies -rmg\sin \theta = I_{\Omega} \frac{d^2\theta}{dt^2}$$
Approssimando piccoli angoli ($\sin \theta = \theta$)
$$\implies -rmg\theta = I_{\Omega} \frac{d^2\theta}{dt^2}$$
$$\implies \frac{d^2\theta}{dt^2} = -\frac{rmg}{I_{\Omega}}\theta$$