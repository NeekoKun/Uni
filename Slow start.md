#FCI 
> [!warning] Algoritmo
> - Si inizia settand CWND = 1 * MSS e la SSTRESH ad un valore elevato
> - Ogni [[Flags#ACK|ACK]] ricevuto aumenta di 1 la CWND
> 	- $\to$ incremento esponenziale

> [!info] Osservazione
> L'accelerazione di connessione varia con l'RTT

> [!error] Evento di Congestione
> SSTRESH viene posto a 
> $$\mathrm{Max} \left ( 2 \mathrm{MSS}, \frac{\mathrm{FlightSize}}{2} \right )$$
> e CWND viene posto a $1 \mathrm{MSS}$