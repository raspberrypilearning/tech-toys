## Haz volar tu helicóptero

Vamos a usar las teclas de flecha para hacer volar el helicóptero.

--- task ---

Empecemos por codificar tu helicóptero para moverlo hacia arriba cuando se presione la flecha hacia arriba.

![objeto helicóptero](images/helicopter-sprite.png)

```blocks3
when [up arrow v] key pressed
change y by (5)
```

--- /task ---

--- task ---

Prueba tu código y verás que la posición de tu helicóptero `y`{:class="block3motion"} (arriba/abajo) cambia cuando se presiona la flecha hacia arriba.

--- /task ---

--- task ---

Para que tu helicóptero se mueva con más fluidez, en su lugar puedes añadir código para que se mueva hacia arriba dentro del giro de tu helicóptero `para siempre`{:class="block3motion"}.

![objeto helicóptero](images/helicopter-sprite.png)

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

You can also code your helicopter to move to the left when the left arrow is pressed. Esta vez tendrás que cambiar la posición `x`{:class="block3motion"} del helicóptero por `-5`.

![objeto helicóptero](images/helicopter-sprite.png)

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

Now code your helicopter to respond to the down and right arrow keys.

--- hints ---

--- hint ---

Copia el código que utilizaste para hacer que el helicóptero se mueva hacia arriba e izquierda, al cambiar las `claves`{:class="block3sensing"} y los valores `x`{:class="block3motion"} & `y`{:class="block3motion"}

--- /hint ---

--- hint ---

Necesitarás estos bloques:

![objeto helicóptero](images/helicopter-sprite.png)

```blocks3
if <> then

end

change y by (-5)

change x by (5)

<key [right arrow v] pressed ?>
```

--- /hint ---

--- hint ---

Tu código debería verse así:

![objeto helicóptero](images/helicopter-sprite.png)

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
