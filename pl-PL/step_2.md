## Muszka spinningowa

Zakodujmy muszkę, która będzie się kręcić po kliknięciu.

--- task ---

Otwórz projekt startowy Scratch.

**Online**: otwórz [projekt początkowy](https://rpf.io/tech-toys-on){:target="_blank"}.

Jeśli masz konto Scratch, możesz wykonać kopię klikając **Remiks**.

**Offline**: otwórz projekt początkowy [ ](https://rpf.io/p/pl-PL/tech-toys-go){:target="_blank"} w edytorze offline.

Jeśli chcesz pobrać i zainstalować edytor Scratch, znajdziesz go w [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

W projekcie startowym powinieneś zobaczyć 2 postacie, laptopa i helikopter.

![projekty początkowe](images/toys-starter.png)

--- /task ---

--- task ---

Kliknij „Muszke” duszka i dodaj ten kod:

![duszek muszki](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
turn cw (15) degrees
end
```

--- /task ---


--- task ---

Kliknij muszkę, aby uruchomić kod. Powinieneś zobaczyć, że Twoja muszka obraca się o 15 stopni zgodnie z ruchem wskazówek zegara 10 razy, w sumie obracajac sie 150 stopni.

![muszka obracająca się o 150 stopni](images/toys-bowtie-test.png)

--- /task ---

--- task ---

Znajdź `ustaw kierynek na`{:class="block3motion"} bloku i _bez przeciągania go_, kliknij go, aby ustawić muszkę z powrotem w pozycji początkowej.

```blocks3
point in direction (90 v)
```

Wskazówka: w Scratch możesz kliknąć blok, aby go uruchomić od razu. Nawet nie musisz przeciągać go do obszaru skryptów najpierw!

--- /task ---

--- task ---

Aby muszka wykonała 1 pełny obrót, liczby w kodzie muszą sumować się do 360 stopni. Zmień swój kod, aby muszka obrócił się `36` stopni 10 razy (36 x 10 = 360).

![muszka duszka](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
+turn cw (36) degrees
end
```

--- /task ---

--- task ---

Przetestuj swój kod ponownie. Tym razem Twoja muszka powinna wykonać 1 pełny obrót o 360 stopni i skończyć w miejscu, w którym się rozpoczęła.

--- /task ---

Jeśli chcesz, aby twoja muszka wykonała 4 pełne obroty, możesz zmienić liczbę w `powtórz`{:class="block3control"} bloku z `10` do `40`.

```blocks3
when this sprite clicked
+repeat (40)
turn cw (36) degrees
end
```
