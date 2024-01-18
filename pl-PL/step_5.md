## Latanie twoim helikopterem

Użyjmy klawiszy strzałek, aby latać twoim helikopterem.

--- task ---

Zacznijmy od kodowania helikoptera, aby poruszał się w górę po naciśnięciu strzałki w górę.

![ikona helikoptera](images/helicopter-sprite.png)

```blocks3
when [up arrow v] key pressed
change y by (5)
```

--- /task ---

--- task ---

Przetestuj swój kod, a zobaczysz, że pozycja `y`{:class="block3motion"} (góra/dół) Twojego helikoptera zmienia się po każdym naciśnięciu strzałki w górę.

--- /task ---

--- task ---

Aby twój helikopter poruszał się płynniej, możesz zamiast tego dodać kod umożliwiający poruszanie się w górę wewnątrz pętli `zawsze`{:class="block3motion"} Twojego helikoptera.

![ikona helikoptera](images/helicopter-sprite.png)

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

Możesz również zakodować swój helikopter, aby poruszać się w lewo po naciśnięciu strzałki w lewo. Tym razem musisz zmienić helikoptera `x`{:class="block3motion"} pozycji od `-5`.

![ikona helikoptera](images/helicopter-sprite.png)

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

Teraz zaprogramuj swój śmigłowiec, aby odpowiedzieć na klawisze strzałek w dół i w prawo.

--- hints ---

--- hint ---

Skopiuj kod użyty do uruchomienia helikoptera w górę i w lewo, zmieniając`klawisze`{:class="block3sensing"} użytku i `x`{:class="block3motion"} i `y`{:class=„block3motion”} wartości

--- /hint ---

--- hint ---

Będziesz potrzebował tych bloków:

![ikona helikoptera](images/helicopter-sprite.png)

```blocks3
if <> then

end

change y by (-5)

change x by (5)

<key [right arrow v] pressed ?>
```

--- /hint ---

--- hint ---

Twój kod powinien wyglądać tak:

![ikona helikoptera](images/helicopter-sprite.png)

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
