#FCI 

## Timeout
> [!warning] Definizione
> In caso di utilizzo di Timeout, il go-back-n viene chiamato solamente dopo lo scadere di un timeout dall'inzio del pacchetto

> [!error] Problema
> Come scegliere dinamicamente il **Timeout**?
> - Il valore minimo deve essere leggermente maggiore di $2 \cdot \mathrm{RTT}$
> - Viene stimato tramite gli [[Algoritmi di Karn e Jacobson]]