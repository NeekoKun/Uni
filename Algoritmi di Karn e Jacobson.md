#FCI 
> [!warning] Obiettivo
> Stima l'**Expected RTT** in base al campionamento di $\Delta t$ tra SYN ed ACK in una connessione

## Algoritmo di Jacobson
> [!info] Metodo
> Il *sender* [[TCP]] calcola lo **Smoothed Round Trip Time** (SRTT) e la **Smoothed Deviation** (SDEV) come:
> $$\mathrm{SRTT} ^{(i)} = (1 - \alpha)\mathrm{SRTT}^{(i - 1)} + \alpha \mathrm{SRTT}^{(i)}$$
> SDEV calc #TODO
>  ed il Timeout viene settato a $$\mathrm{Timeout} = \mathrm{SRTT} + 4 \mathrm{SDEV}$$
