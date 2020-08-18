## Giro della morte

Scriviamo il codice per far eseguire al tuo elicottero un giro a 360 gradi.

--- task ---

Vogliamo che l'elicottero esegua una rotazione di 360 gradi ogni volta che viene premuto il tasto spazio. Ricorda che i numeri nel tuo codice devono sommare 360.

![sprite elicottero](images/helicopter-sprite.png)

```blocks3
when [space v] key pressed
repeat (360)
turn ccw (1) degrees
end
```

--- /task ---

--- task ---

Prova il tuo codice premendo lo spazio, e vedrai che il tuo elicottero gira molto lentamente. Questo perché gira 1 solo grado per 360 volte.

--- /task ---

--- task ---

Per accelerare la rotazione dell'elicottero, modifica i numeri nel codice in modo che giri più gradi ma meno volte. Non importa quali numeri si scelgono, basta che la somma faccia 360!

![sprite elicottero](images/helicopter-sprite.png)

```blocks3
when [space v] key pressed
+repeat (45)
+turn ccw (8) degrees
end
```

--- /task ---

--- task ---

Se vuoi che il tuo elicottero si sposti mentre ruota, aggiungi un blocco `fai`{:class="block3motion"} al tuo codice.

```blocks3
when [space v] key pressed
repeat (45)
+ move (5) steps
turn ccw (8) degrees
end
```

--- /task ---

--- task ---

Premi di nuovo il tasto spazio per testare il tuo codice. Dovresti vedere il tuo elicottero muoversi lungo una circonferenza. Cosa succede se cambi il numero nel blocco `fai`{:class="block3motion"}?

![giro dell´elicottero](images/toys-helicopter-360-move-test.png)

--- /task ---

