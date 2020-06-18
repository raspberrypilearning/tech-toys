## Looping

Lass uns deinen Hubschrauber programmieren, um einen Looping zu fliegen.

--- task ---

Wir wollen, dass der Hubschrauber jedesmal eine 360 Grad Drehung macht, wenn die Leertaste gedrückt wird. Denk daran, dass die Zahlen in deinem Code 360 ergeben müssen.

![Hubschrauber Sprite](images/helicopter-sprite.png)

```blocks3
when [space v] key pressed
repeat (360)
turn ccw (1) degrees
end
```

--- /task ---

--- task ---

Teste deinen Code durch drücken der Leertaste. Du solltest sehen, dass der Hubschrauber sich sehr langsam dreht. Das liegt daran, dass er sich 360 Mal nur um 1 Grad dreht.

--- /task ---

--- task ---

Ändere die Zahlen in deinem Code, damit er sich in weniger Schritten mehr dreht, um die Drehung des Hubschraubers zu beschleunigen. Es ist egal welche Zahlen du wählst, solange die Summe 360 beträgt!

![Hubschrauber Sprite](images/helicopter-sprite.png)

```blocks3
when [space v] key pressed
+repeat (45)
+turn ccw (8) degrees
end
```

--- /task ---

--- task ---

Wenn der Hubschrauber sich zu der Drehung auch Bewegen soll, füge einfach einen `gehe`{:class="block3motion"} Block zu deinem Code hinzu.

```blocks3
when [space v] key pressed
repeat (45)
+ move (5) steps
turn ccw (8) degrees
end
```

--- /task ---

--- task ---

Drücke die Leertaste um deinen Code erneut zu testen. Der Hubschrauber sollte sich nun in einem Kreis bewegen. Was passiert, wenn du die Nummer im `gehe`{:class="block3motion"} Block änderst?

![Hubschrauber Looping](images/toys-helicopter-360-move-test.png)

--- /task ---

