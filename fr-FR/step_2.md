## Nœud papillon tournant

Codons un nœud papillon qui tourne quand on clique dessus.

--- task ---

Ouvre le projet de démarrage Scratch.

**Online**: open the [starter project](https://rpf.io/tech-toys-on){:target="_blank"}.

Si tu as un compte Scratch, tu peux en créer une copie en cliquant sur **Remix**.

**Offline**: open the [starter project](https://rpf.io/p/en/tech-toys-go){:target="_blank"} in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

Dans le projet de démarrage, tu devrais voir 2 personnages, un ordinateur portable et un hélicoptère.

![projets de démarrage](images/toys-starter.png)

--- /task ---

--- task ---

Clique sur le sprite « Noeud papillon » et ajoute ce code :

![sprite nœud papillon](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
turn cw (15) degrees
end
```

--- /task ---


--- task ---

Clique sur le nœud papillon pour exécuter ton code. Tu devrais voir que ton nœud papillon tourne de 15 degrés dans le sens des aiguilles d'une montre 10 fois, tournant de 150 degrés au total.

![nœud papillon tournant de 150 degrés](images/toys-bowtie-test.png)

--- /task ---

--- task ---

Trouve le bloc `s'orienter à`{:class="block3motion"} et, _sans le glisser_, clique dessus pour replacer le nœud papillon à sa position de départ.

```blocks3
point in direction (90 v)
```

Astuce : Dans Scratch, tu peux cliquer sur un bloc pour l'exécuter immédiatement. Tu n'as même pas besoin de le faire glisser en premier dans la zone de script !

--- /task ---

--- task ---

Pour que le nœud papillon fasse 1 tour complet, les chiffres de ton code doivent totaliser 360 degrés. Change ton code pour que le nœud papillon tourne de `36` degrés 10 fois (36 x 10 = 360).

![sprite nœud papillon](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
+turn cw (36) degrees
end
```

--- /task ---

--- task ---

Teste ton code à nouveau. Cette fois, ton nœud papillon devrait faire 1 tour complet à 360 degrés et finir là où il a commencé.

--- /task ---

Si tu veux que ton nœud papillon fasse 4 tours complets, tu peux changer le nombre dans le bloc `répéter`{:class="block3control"} de `10` à `40` .

```blocks3
when this sprite clicked
+repeat (40)
turn cw (36) degrees
end
```
