## Fai volare il tuo elicottero

Usa i tasti freccia per far volare l'elicottero.

--- task ---

Iniziamo scrivendo il codice che faccia salire il tuo elicottero quando viene premuta la freccia in alto.

![sprite elicottero](images/helicopter-sprite.png)

```blocks3
when [up arrow v] key pressed
change y by (5)
```

--- /task ---

--- task ---

Prova il tuo codice e vedrai che la posizione del tuo elicottero `y`{:class="block3motion"} cambia (su/giù) ogni volta che la freccia in alto viene premuta.

--- /task ---

--- task ---

Per far muovere il tuo elicottero in modo più fluido, puoi in alternativa aggiungere del codice per spostarti verso l'alto all'interno del ciclo `per sempre`{:class="block3motion"}.

![sprite elicottero](images/helicopter-sprite.png)

```blocks3
when I receive [inizio v]
forever
next costume
+ if <key [up arrow v] pressed ?> then
change y by (5)
end
end

-when [up arrow v] key pressed
-change y by (5)
```

--- /task ---

--- task ---

Puoi anche scrivere il codice per muovere il tuo elicottero a sinistra quando viene premuta la freccia sinistra. Questa volta dovrai cambiare la posizione `x dell'elicottero`{:class="block3motion"} di `-5`.

![sprite elicottero](images/helicopter-sprite.png)

```blocks3
when I receive [inizio v]
forever
next costume
if <key [up arrow v] pressed ?> then
change y by (5)
end
+if <key [left arrow v] pressed ?> then
change x by (-5)
end
end
```

--- /task ---

--- task ---

Ora scrivi il codice per muovere il tuo elicottero quando usi i tasti freccia giù e freccia destra.

--- hints ---


--- hint ---

Copia il codice che hai usato per far muovere l'elicottero verso l'alto e verso sinistra, modificando i `tasti`{:class="block3sensing"} usati e i valori `x`{:class="block3motion"} & `y`{:class="block3motion"}

--- /hint ---

--- hint ---

Avrai bisogno di questi blocchi:

![sprite elicottero](images/helicopter-sprite.png)

```blocks3
if <> then

end

change y by (-5)

change x by (5)

<key [right arrow v] pressed ?>
```

--- /hint ---

--- hint ---

Il tuo codice dovrebbe assomigliare a questo:

![sprite elicottero](images/helicopter-sprite.png)

```blocks3
when I receive [inizio v]
forever
next costume
if <key [up arrow v] pressed ?> then
change y by (5)
end
if <key [left arrow v] pressed ?> then
change x by (-5)
end
+if <key [down arrow v] pressed ?> then
change y by (-5)
end
+if <key [right arrow v] pressed ?> then
change x by (5)
end
end
```

--- /hint ---

--- /hints ---

--- /task ---
