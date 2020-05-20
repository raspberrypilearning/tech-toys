## Met je helikopter vliegen

Laten we de pijltjestoetsen gebruiken om met je helikopter te vliegen.

--- task ---

Laten we beginnen met het coderen van je helikopter om omhoog te bewegen wanneer de pijl omhoog-toets wordt ingedrukt.

![helikopter sprite](images/helicopter-sprite.png)

```blocks3
when [up arrow v] key pressed
change y by (5)
```

--- /task ---

--- task ---

Test je code en je zult zien dat je `y`{:class="block3motion"} positie (omhoog / omlaag) van de helikopter verandert wanneer de pijl omhoog-toets wordt ingedrukt.

--- /task ---

--- task ---

Om je helikopter soepeler te laten bewegen, kun je in plaats daarvan code toevoegen om omhoog te gaan binnen de `herhaal`{:class="block3motion"}-lus van de helikopter.

![helikopter sprite](images/helicopter-sprite.png)

```blocks3
when I receive [start v]
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

Je kunt ook je helikopter coderen om naar links te gaan wanneer de pijl naar links wordt ingedrukt. Deze keer moet je de `x`{:class="block3motion"} positie van de helikopter wijzigen met `-5`.

![helikopter sprite](images/helicopter-sprite.png)

```blocks3
when I receive [start v]
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

Codeer nu je helikopter om te reageren op de pijl omlaag- en pijl rechts-toetsen.

--- hints ---

--- hint ---

Kopieer de code die je hebt gebruikt om de helikopter naar boven en naar links te laten bewegen, door de `toetsen`{:class="block3sensing"} en `x`{:class="block3motion"} & `y`{:class="block3motion"} waarden te wijzigen

--- /hint ---

--- hint ---

Je hebt deze blokken nodig:

![helikopter sprite](images/helicopter-sprite.png)

```blocks3
if <> then

end

change y by (-5)

change x by (5)

<key [right arrow v] pressed ?>
```

--- /hint ---

--- hint ---

Je code zou er als volgt uit moeten zien:

![helikopter sprite](images/helicopter-sprite.png)

```blocks3
when I receive [start v]
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
