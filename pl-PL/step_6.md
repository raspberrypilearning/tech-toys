## Zapętlić pętlę

Zakodujmy helikopter, aby wykonał obrót o 360 stopni.

--- task ---

Chcemy, aby helikopter wykonywał 360 stopni za każdym razem, gdy naciśnięty zostanie klawisz spacja. Pamiętaj, że liczby w kodzie muszą sumować się do 360.

![ikona helikoptera](images/helicopter-sprite.png)

```blocks3
when [space v] key pressed
repeat (360)
turn ccw (1) degrees
end
```

--- /task ---

--- task ---

Przetestuj swój kod, naciskając spację, a zobaczysz, że Twój helikopter obraca się bardzo wolno. To dlatego, że obraca się tylko o 1 stopień 360 razy.

--- /task ---

--- task ---

Aby przyspieszyć obrót helikoptera, zmień liczby w kodzie, aby obracał się o kilka wiecej stopni mniej razy. Nie ma znaczenia, jakie liczby wybierzesz, o ile sumują się one do 360!

![ikona helikoptera](images/helicopter-sprite.png)

```blocks3
when [space v] key pressed
+repeat (45)
+turn ccw (8) degrees
end
```

--- /task ---

--- task ---

Jeśli chcesz, aby Twój helikopter poruszał się tak samo, jak wirował, po prostu dodaj `przesuń`{:class="block3motion"} bloku do twojego kodu.

```blocks3
when [space v] key pressed
repeat (45)
+ move (5) steps
turn ccw (8) degrees
end
```

--- /task ---

--- task ---

Ponownie naciśnij spację, aby przetestować kod. Powinieneś zobaczyć jak twoj helikopter lata w okręgu. Co się stanie, jeśli zmienisz numer w swoim `ruchu`{:class="block3motion"} blok?

![zapętlenie helikoptera](images/toys-helicopter-360-move-test.png)

--- /task ---

