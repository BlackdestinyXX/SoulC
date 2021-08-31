# Avvertimento
Io mi sono solo occupato della traduzione del readme del linguaggio, che è stato interamente creato da ThaMessia.
# SoulC
Dunque, stavo guardando come è stato fatto l'interprete di Brainfuck, e ho visto che più semplice di quanto pensassi.
Pensavo di poter creare un nuovo linguaggio di programmazione esoterico simile a brainfuck e l'ho fatto.

![SoulC](https://user-images.githubusercontent.com/68974876/130805678-5868d748-4d36-4f00-8261-95478d273c9c.png)

Come ho detto prima, SoulC è simile a Brainfuck ma con alcune differenze. 
Non conosci Brainfuck ma vorresti comunque imparare il SoulC? Tranquillo, ho preparato una documentazione che include anche alcuni esempi (resta comunque un linguaggio di programmazione esoterico :D).

# Documentazione:

Vediamo le basi del linguaggio:
```yml
xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
.p
xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
.p
xxxxxxxxxx
.
```
Questo programma stampa "Hi" e a questo punto, va a capo.
Ogni 'x' rappresenta una lettera (o solo un carattere se vuoi semplificare) in ASCII, quindi significa che
per **memorizzare** una lettera, devi digitare quante 'x' per quanti caratteri in ASCII sarà quella lettera.

Esempio: 
```yml
xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```
Questo **memorizzerà** una "a" perché ci sono 97 "x" e "a" in ASCII è 97.

Per capire cosa ".p" significa, possiamo dividerlo in due parti: '.' e 'p'. '.' è molto semplice da capire, stampa solamente l'output.

Perché per tutto questo tempo ho parlato di "memorizzare"? Perchè ogni carattere nel file .soulc è in un array.
Se voglio stampare più caratteri devo avanzare nell'array.
Ora che abbiamo questo concetto chiaro nella mente, andiamo avanti.

'p' sta per **pointeradvance**, questo signifca che ogni volta che scriviamo 'p' nel nostro programma dopo l'output ('.')
possiamo andare avanti nell'array, permettendoci di stampare più caratteri.

Ma cosa succede se volessimo tornare nell'array? Possiamo semplicemente usare 'q'.

Andiamo avanti!

```yml
,[.,]
```

Ok, questo potrebbe essere particolare da capire. ',' è un input e queste parentesi quadre significano conteggi come strutture di controllo.
Se hai notato che questo codice accetta input e quindi stampa l'input fornito in un ciclo, hai ragione.

Per le persone che non capiscono come funziona questo codice, lo spiego in modo semplice.
Tutto questo codice si svolge in **un elemento di un grande array**,
ciò significa che possiamo usare l'input fornito come variabile da stampare.

La struttura di controllo qui conta come un ciclo, quindi è ovvio che si ripeterà all'infinito poiché non vengono fornite istruzioni.

# Altri esempi (da altri programmatori)
[ComeTiChiami.soulc](https://github.com/AndreaGennaioli/ComeTiChiami.soulc) fatto da [AndreaGennaioli](https://github.com/AndreaGennaioli/)

# Sommario
Se hai imparato tutto questo, hai compreso appieno le basi di SoulC e puoi dire di aver imparato un linguaggio di programmazione esoterico.

Posso dire solo una cosa ora: **Goditi il linguaggio!**
