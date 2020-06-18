## Fliege deinen Hubschrauber

Lass uns die Pfeiltasten verwenden, um den Hubschrauber zu fliegen.

--- task ---

Fangen wir damit an den Hubschrauber nach oben zu bewegen, wenn die Pfeil nach oben Taste gedrückt wird.

![Hubschrauber Sprite](images/helicopter-sprite.png)

```blocks3
when [up arrow v] key pressed
change y by (5)
```

--- /task ---

--- task ---

Teste deinen Code um zu sehen, wie sich die Position deines Hubschraubers `y`{:class="block3motion"} (auf/ab) ändert, wenn die Pfeil nach oben Taste gedrückt wird.

--- /task ---

--- task ---

Um deinen Hubschrauber flüssiger zu bewegen, kannst du stattdessen den Code zum „Sich nach oben bewegen“ der `wiederhole fortlaufend`{:class="block3motion"} Schleife des Hubschraubers hinzufügen.

![Hubschrauber Sprite](images/helicopter-sprite.png)

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

Du kannst auch programmieren, dass sich der Hubschrauber nach links bewegt, wenn die Pfeil nach links Taste gedrückt wird. Diesmal musst du die Position des Hubschraubers `x`{:class="block3motion"} um `-5` ändern.

![Hubschrauber Sprite](images/helicopter-sprite.png)

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

Programmiere als nächstes die Reaktion des Hubschraubers für die Pfeil nach unten und Pfeil nach rechts Tasten.

--- hints ---

--- hint ---

Kopiere den Code, den du benutzt hast, um den Helikopter nach oben und nach links zu bewegen und ändere die verwendeten `Tasten`{:class="block3sensing"} und die `x`{:class="block3motion"} & `y`{:class="block3motion"} Werte

--- /hint ---

--- hint ---

Du wirst diese Blöcke benötigen:

![Hubschrauber Sprite](images/helicopter-sprite.png)

```blocks3
if <> then

end

change y by (-5)

change x by (5)

<key [right arrow v] pressed ?>
```

--- /hint ---

--- hint ---

Dein Code sollte so aussehen:

![Hubschrauber Sprite](images/helicopter-sprite.png)

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
