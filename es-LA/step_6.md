## Loop-the-loop

Vamos a programar tu helicóptero para que haga un giro de 360 grados.

--- task ---

Queremos que el helicóptero gire 360 grados cada vez que se presiona la tecla de espacio. Recuerda que los números en tu código deben sumar hasta 360.

![objeto helicóptero](images/helicopter-sprite.png)

```blocks3
when [space v] key pressed
repeat (360)
turn ccw (1) degrees
end
```

--- /task ---

--- task ---

Test your code by pressing space, and you'll see that your helicopter spins very slowly. Esto se debe a que sólo gira 1 grado 360 veces.

--- /task ---

--- task ---

Para acelerar el giro de tu helicóptero, cambia los números en tu código, así girará más grados menos veces. ¡No importa qué números elijas mientras que sumen hasta 360!

![objeto helicóptero](images/helicopter-sprite.png)

```blocks3
when [space v] key pressed
+repeat (45)
+turn ccw (8) degrees
end
```

--- /task ---

--- task ---

Si quieres que tu helicóptero se mueva, además de girar, solo añade un bloque `mover`{:class="block3motion"} a tu código.

```blocks3
when [space v] key pressed
repeat (45)
+ move (5) steps
turn ccw (8) degrees
end
```

--- /task ---

--- task ---

Presiona otra vez espacio para probar tu código. Deberías ver que tu helicóptero se mueve en círculo. ¿Qué sucede si cambias el número en el bloque `mover`{:class="block3motion"}?

![el giro del helicóptero](images/toys-helicopter-360-move-test.png)

--- /task ---

