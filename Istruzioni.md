#AXO 
- Istruzioni per la lettura dalla memoria
- Istruzioni per l'input e l'output
- RISC-V 64i
	- Little Endian
	- 64i = 64 bit per indirizzo di memoria nel registry
		- 32 Indirizzi in totale
	- Riduced Instruction Set Computer
		- Stessa lunghezza: 32bit/4 byte per informazione
- DOC dell'Abstract Binary Interface (ABI)
	- Convenzioni semantiche per utilizzo condiviso dei programmi

## Assembly
- Scritte come codice operativo + operandi dell'istruzione
- e.g.
```assembly
add    s0,s1,s2
```
-> somma s0 = s1 + s2
- Formato immediato
	- dev'essere un numero decimale con al massimo 12 bit
	- (-s^11; 2^11 + 1)
- e.g.
```
addi    s0,s1,5
```
-> s0 = s1 + 5
- Formato unsigned (aggiunta di u)
- non esiste con add pk stesso circuito
	- error control è in funzione al segno con i (int overflow)

### Sintassi
```
ld    S0, 5(a2) se a2 <- 10: somma 5 a 10, controlla ram[15], copia i prox 8 byte in S0
sd    S1, 5(a2) se a2 <- 10: somma 5 a 10, scrivi s1 in ram[15]
```
- ld = load double
- sd = save double
- double -> 8 byte
- word -> 4 byte
- half -> 2 byte

- ==Estensione del segno nel registro==


-0d26_{dec} = 0b101000_{bin} :
(011000 xor 111111) + 1

in hex:
0b11101000 -> 0xE8