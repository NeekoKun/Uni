#AXO 
```MAIN
        eqv     MID, 12288
        .data
TENSOR: .space  2048
IDX:    .word   512
        .text
        .global MAIN
MAIN:	la      t3, TENSOR
		beq     t1, t3, PROX
		li      t4, MID
PROX:   jal     BACKUP
		bne     t1, t2, SUCC
		ld      t1, (zero)
END:    mv      t5, t1
```
```BACKUP
        .data
VECTOR: .space  256
        .text
        .global BACKUP
BACKUP: bne     a3, zero, MAIN
        ld      a2, (t0)
SUCC:   la      t3, IDX
        beq     t1, t3, SUCC
	    ret
```

### 
```assembly
0  |MAIN:	auipc   t3, 00000
4  |  		addi    t3, t3, 000
8  |    	beq     t1, t2, 006
C  |	    lui     t4, 00003
10 |        addi    t4, t4, 000
14 |PROX:   jal     00000
18 |	    bne     t1, t2, 000
1C |	    ld      t1, (zero)
20 |END:    addi    t5, t1, zero
```

### Tabella Simboli

| Indirizzo | Simbolo | Type |
| --------- | ------- | ---- |
| 0         | MAIN    | T    |
| 14        | PROX    | T    |
| 20        | END     | T    |
| 0         | TENSOR  | D    |
|           | IDX     | T    |

### Tabella di Rilocazione

| Indirizzo | Comando      |
| --------- | ------------ |
| 0         | auipc        |
| 4         | addi         |
| C         | lui %hi(MID) |
| 10        |              |
| 14        |              |
| 18        |              |
