## Loopings

Laten we je helikopter coderen om een draai van 360 graden te maken.

--- task ---

We willen dat de helikopter 360 graden draait wanneer de spatietoets wordt ingedrukt. Onthoud dat de getallen in je code tot 360 moeten optellen.

![helikopter sprite](images/helicopter-sprite.png)

```blocks3
when [space v] key pressed
repeat (360)
turn ccw (1) degrees
end
```

--- /task ---

--- task ---

Test je code door op de spatiebalk te drukken en je zult zien dat je helikopter heel langzaam draait. Dat komt doordat het 360 keer maar 1 graad verandert.

--- /task ---

--- task ---

Om de draai van je helikopter te versnellen, verander je de getallen in je code zodat deze minder vaak meer graden draait. Het maakt niet uit welke getallen je kiest, zolang ze maar optellen tot 360!

![helikopter sprite](images/helicopter-sprite.png)

```blocks3
when [space v] key pressed
+repeat (45)
+turn ccw (8) degrees
end
```

--- /task ---

--- task ---

Als je wilt dat je helikopter zowel beweegt als draait, voeg je gewoon een `neem stappen`{:class="block3motion"}-blok toe aan je code.

```blocks3
when [space v] key pressed
repeat (45)
+ move (5) steps
turn ccw (8) degrees
end
```

--- /task ---

--- task ---

Druk nogmaals op de spatiebalk om je code te testen. Je zou je helikopter in een cirkel moeten zien bewegen. Wat gebeurt er als je het getal in je `neem stappen`{:class="block3motion"}-blok verandert?

![helikopter in een looping](images/toys-helicopter-360-move-test.png)

--- /task ---

