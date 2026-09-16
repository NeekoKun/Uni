#ELT 
## 1. Risoluzione di circuiti semplici e tecniche fondamentali

### Leggi di Kirchhoff

- **LKC (leggi ai nodi):** la somma algebrica delle correnti entranti in un nodo è nulla. $\sum I = 0$.
- **LKT (legge alle maglie):** la somma algebrica delle tensioni lungo una maglia chiusa è nulla. $\sum V = 0$.

### Serie e parallelo

- **Resistori in serie:** $R_{eq} = R_{1} + ... + R_{n}$
- **Resistori in parallelo:** $\frac{1}{R_{eq}} = \frac{1}{R_{1}}+ ... + \frac{1}{R_{n}}$ (stessa tensione). Per due soli: $R_{eq} = \frac{R_{1}R_{2}}{R_{1}+R_{2}}$
- **Partitore di tensione:** V_k = V_tot · R_k / (R_tot serie)
- **Partitore di corrente:** I_k = I_tot · R_altro / (R_k + R_altro) — attenzione: usa la resistenza dell'_altro_ ramo (o la conduttanza propria su conduttanza totale: I_k = I_tot · G_k / G_tot).
- Condensatori: **serie** come resistori in parallelo (1/C_eq), **parallelo** come resistori in serie (C_eq = ΣC).
- Induttori: si comportano come i resistori (serie: somma, parallelo: reciproci).

### Metodo dei nodi (Nodal Analysis)

1. Scegli un nodo di riferimento (massa, V=0).
2. Assegna un'incognita di tensione a ogni altro nodo.
3. Scrivi LKC per ogni nodo (esprimendo le correnti coi rami tramite legge di Ohm generalizzata: I = (V_a - V_b)/R).
4. Se c'è un generatore di tensione tra due nodi non di massa → **supernodo** (unisci i due nodi in un'unica equazione + equazione di vincolo V_a - V_b = V_gen).
5. Risolvi il sistema lineare.

### Metodo delle maglie (Mesh Analysis)

1. Definisci correnti di maglia (tutte in senso orario, per convenzione).
2. Scrivi LKT per ogni maglia in termini delle correnti di maglia.
3. Se c'è un generatore di corrente condiviso tra due maglie → **supermaglia**.
4. Risolvi il sistema.

### Sovrapposizione degli effetti (solo circuiti lineari)

- Si calcola l'effetto di **ogni generatore indipendente separatamente**, spegnendo gli altri:
    - generatore di tensione spento → cortocircuito
    - generatore di corrente spento → circuito aperto
- **I generatori pilotati (dipendenti) NON si spengono mai** — restano sempre attivi in ogni passo.
- La risposta totale è la somma algebrica delle risposte parziali.

### Trasformazione di sorgenti

- Un generatore di tensione V in serie con R è equivalente a un generatore di corrente I = V/R in parallelo con R (e viceversa). Utile per semplificare rapidamente reti.

---

## 2. Doppi bipoli e generatori pilotati (dipendenti)

### I quattro tipi di generatori pilotati

| Tipo                          | Sigla | Grandezza pilotante | Grandezza generata |
| ----------------------------- | ----- | ------------------- | ------------------ |
| Tensione pilotata in tensione | VCVS  | Tensione (altrove)  | Tensione = A·V_x   |
| Tensione pilotata in corrente | CCVS  | Corrente (altrove)  | Tensione = R·I_x   |
| Corrente pilotata in tensione | VCCS  | Tensione (altrove)  | Corrente = G·V_x   |
| Corrente pilotata in corrente | CCCS  | Corrente (altrove)  | Corrente = β·I_x   |

### Trattamento nell'analisi

- Si scrivono le equazioni nodali/di maglia esattamente come per i generatori indipendenti, MA in più serve **un'equazione di vincolo** che lega la grandezza pilotante (V_x o I_x) alle incognite del circuito.
- Non si possono spegnere nella sovrapposizione degli effetti.
- Per Thevenin/Norton con pilotati: niente spegnimento "furbo", serve il metodo del generatore di prova (vedi sotto).

### Doppi bipoli compositi

- Un doppio bipolo (2-porte) può essere descritto da matrici Z, Y, H (ibride) o T (trasmissione), a seconda delle grandezze indipendenti scelte.
- **Collegamento in serie** di due doppi bipoli → si sommano le matrici Z.
- **Collegamento in parallelo** → si sommano le matrici Y.
- **Cascata** → si moltiplicano le matrici di trasmissione T.
- Per risolvere un doppio bipolo composito pilotato: isola il blocco, scrivi le relazioni caratteristiche (es. V1 = Z11 I1 + Z12 I2, ecc.), poi applica i vincoli esterni (carico, generatore) e risolvi il sistema.

---

## 3. Thevenin e Norton

### Procedura standard

1. **Rimuovi il carico** (il ramo di cui vuoi conoscere V-I).
2. **V_th** = tensione a vuoto ai morsetti aperti (con tutti i generatori attivi).
3. **R_th** (= R_norton):
    - Se **non ci sono generatori pilotati**: spegni tutti i generatori indipendenti (V→cortocircuito, I→aperto) e calcola la resistenza equivalente vista dai morsetti.
    - Se **ci sono generatori pilotati**: spegni solo gli indipendenti, poi applica un **generatore di prova** ai morsetti (V_test o I_test) e calcola R_th = V_test / I_test (i pilotati restano attivi e reagiscono al test).
4. **I_norton** = I_cc = corrente di cortocircuito ai morsetti = V_th / R_th.
5. Il circuito equivalente Thevenin: generatore V_th in serie con R_th. Norton: generatore I_n in parallelo con R_th.

### Nota utile

- Se R_th risulta negativa o nulla con circuito attivo → possibile in presenza di pilotati (il bipolo può erogare potenza o comportarsi da resistenza negativa).
- Massima trasferimento di potenza al carico: R_carico = R_th (per carichi puramente resistivi).

---

## 4. Amplificatori operazionali (op-amp ideali)

### Regole dell'op-amp ideale (in retroazione negativa)

1. **I+ = I− = 0** (nessuna corrente entra negli ingressi).
2. **V+ = V−** ("corto circuito virtuale", valido solo se c'è retroazione negativa dall'uscita all'ingresso invertente).
3. L'uscita fornisce la corrente necessaria (guadagno ad anello aperto → ∞).

### Configurazioni classiche

- **Invertente:** V_out = − (R_f/R_in) · V_in. Ingresso non invertente a massa.
- **Non invertente:** V_out = (1 + R_f/R_1) · V_in.
- **Inseguitore di tensione (buffer):** V_out = V_in (guadagno 1, alta impedenza in ingresso).
- **Sommatore invertente:** V_out = −R_f (V1/R1 + V2/R2 + ...).
- **Differenziale (sottrattore):** V_out = (R_f/R1)(V2 − V1) se le resistenze sono scelte simmetricamente.
- **Integratore:** V_out = −(1/RC) ∫V_in dt.
- **Derivatore:** V_out = −RC (dV_in/dt).

### Metodo di risoluzione

- Applica le regole ideali per trovare le tensioni ai nodi di ingresso.
- Scrivi LKC ai nodi (di solito il nodo invertente, dato che lì spesso confluiscono le resistenze) usando I=0 negli ingressi.
- Risolvi come circuito nodale normale.

---

## 5. Trasformatori ideali

### Relazioni fondamentali (rapporto spire n = N1/N2)

- **V1 / V2 = n**
- **I1 / I2 = 1/n** (quindi V1·I1 = V2·I2 → potenza conservata, nessuna perdita)
- Polarità: i pallini (dot convention) indicano i terminali con la stessa polarità istantanea.

### Riflessione di impedenze

- Un'impedenza Z2 collegata al secondario appare al primario come: **Z1 = n² · Z2**
- Utile per "portare" tutto il circuito su un solo lato (primario o secondario) ed eliminare il trasformatore, risolvendo poi un circuito equivalente più semplice.
- Attenzione al verso dei pallini: se le convenzioni non sono concordi, si introduce un segno meno nelle relazioni.

---

## 6. Condensatori e induttori in DC (regime permanente e transitori)

### Comportamento a regime permanente (DC, t→∞, tutto costante)

- **Condensatore → circuito aperto** (I_C = C dV/dt = 0 se V costante).
- **Induttore → cortocircuito** (V_L = L dI/dt = 0 se I costante).

### Condizioni iniziali e continuità

- La **tensione sul condensatore** non può variare istantaneamente: V_C(0⁻) = V_C(0⁺).
- La **corrente sull'induttore** non può variare istantaneamente: I_L(0⁻) = I_L(0⁺).
- (Tensione su L e corrente su C **possono** invece variare bruscamente.)

### Transitori — circuiti del primo ordine

- **Circuito RC:** costante di tempo τ = R·C.
    - Carica: V_C(t) = V_∞ + (V_0 − V_∞)·e^(−t/τ)
- **Circuito RL:** costante di tempo τ = L/R.
    - I_L(t) = I_∞ + (I_0 − I_∞)·e^(−t/τ)
- Ricetta generale per qualunque grandezza x(t) in un circuito del 1° ordine: **x(t) = x(∞) + [x(0⁺) − x(∞)] · e^(−t/τ)** dove x(∞) si calcola sostituendo C→aperto o L→corto (regime), x(0⁺) dalle condizioni iniziali/continuità, τ = R_eq·C oppure L/R_eq (R_eq vista dai morsetti dell'elemento reattivo, con generatori indipendenti spenti).

---

## 7. Circuiti in AC e dominio dei fasori

### Fasori

- Una grandezza sinusoidale $v(t) = V_m cos(\omega t + \phi)$ si rappresenta come fasore: $V = V_m\ ∠\ \phi$ (ampiezza e fase; spesso si usa il valore efficace $V_{rms} = \frac{V_m}{\sqrt{ 2 }}$ al posto di V_m).
- Vantaggio: le equazioni differenziali diventano algebriche (nel dominio dei fasori, $\frac{d}{dt}$ → moltiplicazione per $j \omega$).

### Impedenze

- **Resistore:** $Z_R = R$ (nessuno sfasamento)
- **Induttore:** $Z_L = j\omega L$ (tensione in anticipo di 90° sulla corrente)
- **Condensatore:** $Z_C = \frac{1}{j\omega C} = \frac{−j}{\omega C}$ (corrente in anticipo di 90° sulla tensione)
- Le leggi di Kirchhoff, serie/parallelo, partitori, nodi, maglie, Thevenin/Norton, sovrapposizione: **valgono identiche**, sostituendo $R$ con $Z$ (impedenza complessa) e lavorando con numeri complessi invece che con numeri reali.

### Metodo simbolico — procedura

1. Trasforma tutti i generatori sinusoidali in fasori.
2. Trasforma $R$, $L$, $C$ nelle rispettive impedenze $Z$ (funzione di $\omega$ — attenzione: $\omega$ deve essere la stessa per tutti i generatori, altrimenti serve sovrapposizione con un'analisi per ogni frequenza).
3. Risolvi il circuito come un normale circuito resistivo, ma con numeri complessi (nodi, maglie, Thevenin, ecc.).
4. Ritrasforma il fasore risultato in una sinusoide nel tempo, se richiesto.

### Potenza in AC

- **Potenza istantanea:** $p(t) = v(t)·i(t)$.
- **Potenza attiva (media):** $P = V_{rms} · I_{rms} · cos(\phi) [W]$, dove $\phi = \phi_v − \phi_i$ è lo sfasamento tra tensione e corrente.
- **Potenza reattiva:** $Q = V_{rms} · I_{rms} · sin(\phi)\ [VAR]$.
- **Potenza apparente:** $S = V_{rms} · I_{rms} = \sqrt{  P^2 + Q^2 } [VA]$.
- **Potenza complessa:** $S = V · I*$ (fasore tensione per il coniugato del fasore corrente) = $P + jQ$.
- **Fattore di potenza:** $cos(\phi) = \frac{P}{S}$. Carichi induttivi → $\phi>0$ (corrente in ritardo); carichi capacitivi → φ<0 (corrente in anticipo).
- Il **rifasamento** (aggiunta di un condensatore in parallelo al carico induttivo) serve a portare $cos(\phi)$ vicino a 1, riducendo la corrente reattiva richiesta alla linea.
