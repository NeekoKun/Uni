#FCI 

## Flags
- [[Flags#SYN|SYN]]
- [[Flags#ACK|ACK]]
- [[Flags#FIN|FIN]]
- [[Flags#PSH|PSH]]
- [[Flags#URG|URG]]
## Controllo dell'Errore
- Meccanismo di ritrasmissione [[Go-Back-N#Timeout|Go-Back-N con Timeout]]
	- Mantiene nel buffer anche i segmenti fuori ordine
	- Viene mandato un [[Flags#ACK|ACK]] che controlla anche i segmenti fuori ordine

## Controllo di Congestione
- Diversi [[Problemi di Congestione]]
- Controlla la velocità massima di output delle macchine sulla rete
- Funziona su **TUTTO L'INTERNET**
- Completamente End-to-End, tratta la rete come una scatola nera
- Metodo
	- Limita la dimensione di una finestra ad un massimo uguale a **Congestion Window** (CWND)
	- Se non si perdono pacchetti, la velocità corrente è inferiore alla velocità massima supportata dalla rete
	- Se si perdono pacchetti, la velocità corrente è superiore alla velocità massima (overflow di qualche buffer)
	- La variabile SSTRESH determina la distinzione tra 2 fasi:
		- [[Slow start]] se CWND < SSTRESH 
		- [[Congestion avoidance]] se CWND > SSTRESH