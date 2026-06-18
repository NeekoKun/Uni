#FCI 
> [!info] Carrier Sense Multiple Access (CSMA)
> Protocollo "educato":
> - Una stazione che ha un frame da trasmettere, prima verifica che il canale sia libero rilevando la presenza di segnale a livello fisico (carrier o portante)
> - Se il canale è libero, la stazione trasmette il frame
> - Se il canale è occupato:
> 	- La trasmissione viene rimandata ripetendo il sensing dopo un tempo casuale
> 	- In altre implementazioni, [...]

> [!warning] Problemi di trasmissioni contemporanea
> Se il canale è libero, due client possono inizializzare comunicazione in contemporanea
> La probabilità che ciò accada scala con la latenza di propagazione del segnale nel medium, quindi il CSMA viene adottato in network di dimensioni ridotte come le reti di casa
>
>---
> Il protocollo diminuisce ciò nonostante la probabilità di collisione

### Calcolo dell'Errore
Il throughput è:
$$S = \frac{Ge^{-aG}}{G(1+2a) + e^{-aG}}$$
Dove $$a = \frac{\tau}{T}$$

## CSMA-CD
> [!info] Carrier Sense Multiple Access - Collision Detection
> Tramite questo protocollo, il CSMA rileva eventuali collisioni ed attende un certo $\delta$ before sending the packet again

### Calcolo dell'Errore
Il throughput è:
$$S = \frac{Ge^{-aG}}{G(1+2a) + a^{-aG} - G(1 - \delta)(1- e^{-aG})}$$
Ne può anche essere approssimato il massimo come
$$S_{max} = \frac{1}{1+5a}$$
> [!error] Applicazioni
> Il guadagno è marginale nel throughput, tuttavia permette al sender di sapere se la connessione è stata tagliata e quindi abilita l'implementazione di meccanismi di ridondanza o recupero dell'errore sender-side