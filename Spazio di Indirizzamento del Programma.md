#AXO
- Stack
- Heap
- Dati Globali e Statici
- Seg. Testo o Istruzioni
- Riservato

- Ipotizziamo inizi con 0x0<sup>4</sup> 0<sup>4</sup> 0<sup>4</sup> 0<sup>4</sup>
- Segmento di Testo: 0x0<sup>4</sup> 0<sup>4</sup> 0040 0<sup>4</sup>
	- Traduzione in stringhe binarie del linguaggio macchina
- Dati Globali e Statici: 0x0<sup>4</sup> 0<sup>4</sup> 1000 0<sup>4</sup>
	- Variabili Globali e Statiche
		- Globali: Accessibili da tutti i File del programma
		- Statiche Accessibili ad un solo File del programma
	- Contiene il BSS
		- Variabili Globali *Non Inizializzate*
- Heap
	- Variabili senza nome (Allocate con malloc())
- Stack
	- Parametri e variabili locali sono dette variabili automatiche
		- Automaticamente posizionate in stack
- Finisce con 0x0<sup>4</sup> 003F F<sup>4</sup> F<sup>4</sup>
	- In RISC-V sono **38 Bit**
	- I restanti indirizzi sono dedicati al Sistema Operativo
- Chiamati Indirizzi Virtuali Rilocabili
	- OS decide dove metterli nella RAM

> [!warning] ASLR
> Address Space Layout Randomization
> Utilizzata per evitare attacchi di memory overflow mirati,
> Randomizza gli indirizzi di inizio segmenti di memoria

## Processo
- RdA (Record di Attivazione)
	- Contiene valore di ritorno e variabili locali
- Esecuzione del Programma
	- Se genera un nuovo RdA, chiamando una funzione, viene piazzato al di sopra del primo nella stack
	- -> indirizzi sempre più bassi
	- array passate as reference (in C)