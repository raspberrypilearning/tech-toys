## Girar el Corbatín

Vamos a codificar un corbatín para que gire cuando se hace clic en él.

--- task ---

Abre el proyecto inicial de Scratch.

**Online**: open the [starter project](https://rpf.io/tech-toys-on){:target="_blank"}.

Si tienes una cuenta de Scratch puedes hacer una copia haciendo clic en **Reinventar**.

**Offline**: open the [starter project](https://rpf.io/p/en/tech-toys-go){:target="_blank"} in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

En el proyecto inicial, deberías ver 2 personajes, un notebook y un helicóptero.

![proyectos iniciales](images/toys-starter.png)

--- /task ---

--- task ---

Haz clic sobre el objeto «corbatín» y añade este código:

![objeto corbatín](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
turn cw (15) degrees
end
```

--- /task ---


--- task ---

Haz clic en el corbatín para ejecutar tu código. Deberías ver que tu corbatín gira 15 grados en sentido de las agujas del reloj 10 veces, girando 150 grados en total.

![corbatín girando 150 grados](images/toys-bowtie-test.png)

--- /task ---

--- task ---

Encuentra el bloque `apuntar en dirección`{:class="block3motion"} y _sin arrastrarlo_, hazle clic para volver a colocar el corbatín en su posición inicial.

```blocks3
point in direction (90 v)
```

Consejo: En Scratch puedes hacer clic en un bloque para ejecutarlo inmediatamente. ¡Ni siquiera necesitas arrastrarlo al área de scripts primero!

--- /task ---

--- task ---

Para hacer que el corbatín haga 1 giro completo, los números en tu código deben sumar hasta 360 grados. Cambia tu código para que el corbatín gire `36` grados 10 veces (36 x 10 = 360).

![objeto corbatín](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
+turn cw (36) degrees
end
```

--- /task ---

--- task ---

Vuelve a probar tu código. Esta vez, tu corbatín debe hacer 1 giro completo de 360 grados y terminar donde comenzó.

--- /task ---

Si quieres que tu corbatín haga 4 vueltas completas, puedes cambiar el número en el bloque `repetir`{:class="block3control"} desde `10` a `40`.

```blocks3
when this sprite clicked
+repeat (40)
turn cw (36) degrees
end
```
