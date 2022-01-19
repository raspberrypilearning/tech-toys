## Draaiende vlinderdas

Laten we een vlinderdas coderen die draait wanneer erop wordt geklikt.

--- task ---

Open het Scratch startproject.

**Online**: open het [startproject](https://scratch.mit.edu/projects/397684878){:target="_blank"}.

Als je een Scratch-account hebt, kun je een kopie maken door op **Remix** te klikken.

**Offline**: open het [startproject](https://rpf.io/p/nl-NL/tech-toys-go){:target="_blank"} in de offline editor.

Als je de Scratch offline editor wilt downloaden en installeren dan kun je die vinden op [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

In het startproject zou je 2 karakters, een laptop en een helikopter moeten zien.

![startprojecten](images/toys-starter.png)

--- /task ---

--- task ---

Klik op de 'Vlinderdas'-sprite en voeg deze code toe:

![vlinderdassprite](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
turn cw (15) degrees
end
```

--- /task ---


--- task ---

Klik op de vlinderdas om je code uit te voeren. Je zou moeten zien dat je vlinderdas 10 keer 15 graden met de klok mee draait, in totaal 150 graden.

![vlinderdas die 150 graden draait](images/toys-bowtie-test.png)

--- /task ---

--- task ---

Vind het `richt naar`{:class="block3motion"}-blok en, _zonder het te slepen_, klik op het blok om de vlinderdas terug te zetten naar de beginpositie.

```blocks3
point in direction (90 v)
```

Tip: In Scratch kun je op een blok klikken om het meteen uit te voeren. Je hoeft het niet eens eerst naar het scriptgebied te slepen!

--- /task ---

--- task ---

Om de vlinderdas 1 volledige draai te laten maken, moeten de getallen in je code tot 360 graden optellen. Wijzig je code zodat de vlinderdas 10 keer `36` graden draait (36 x 10 = 360).

![vlinderdassprite](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
+turn cw (36) degrees
end
```

--- /task ---

--- task ---

Test je code opnieuw. Deze keer zou je vlinderdas 1 keer de volledige 360 graden moeten draaien en eindigen waar hij begon.

--- /task ---

Als je wilt dat je vlinderdas 4 keer volledig ronddraait, kun je het getal in het `herhaal`{:class="block3control"}-blok veranderen van `10` naar `40`.

```blocks3
when this sprite clicked
+repeat (40)
turn cw (36) degrees
end
```
