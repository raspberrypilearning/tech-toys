## Faire voler ton hélicoptère

Utilise les touches fléchées pour piloter ton hélicoptère.

--- task ---

Commençons par coder ton hélicoptère pour qu'il monte lorsque la flèche vers le haut est enfoncée.

![sprite d'hélicoptère](images/helicopter-sprite.png)

```blocks3
when [up arrow v] key pressed
change y by (5)
```

--- /task ---

--- task ---

Teste ton code et tu verras que la position `y`{:class="block3motion"} (haut/bas) de ton hélicoptère change quand la flèche vers le haut est enfoncée.

--- /task ---

--- task ---

Pour que ton hélicoptère se déplace plus doucement, tu peux à la place ajouter du code pour monter vers le haut à l'intérieur de la boucle `répéter indéfiniment` de ton hélicoptère{:class="block3motion"}.

![sprite d'hélicoptère](images/helicopter-sprite.png)

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

Tu peux aussi programmer ton hélicoptère pour se déplacer vers la gauche lorsque la flèche gauche est enfoncée. Cette fois, tu devras changer la position `x`{:class="block3motion"} de l'hélicoptère par `-5`.

![sprite d'hélicoptère](images/helicopter-sprite.png)

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

Maintenant, code ton hélicoptère pour qu'il réponde aux touches fléchées droite et bas.

--- hints ---

--- hint ---

Copie le code que tu as utilisé pour faire avancer l'hélicoptère vers le haut et vers la gauche, en changeant les `touches`{:class="block3sensing"} utilisées et les valeurs `x`{:class="block3motion"} & `y`{:class="block3motion"}

--- /hint ---

--- hint ---

Tu auras besoin de ces blocs :

![sprite d'hélicoptère](images/helicopter-sprite.png)

```blocks3
if <> then

end

change y by (-5)

change x by (5)

<key [right arrow v] pressed ?>
```

--- /hint ---

--- hint ---

Ton code devrait ressembler à ceci :

![sprite d'hélicoptère](images/helicopter-sprite.png)

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
