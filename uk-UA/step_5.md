## Польоти на гелікоптері

Давай будемо використовувати клавіші зі стрілками для польотів на гелікоптері.

--- task ---

Розпочнімо із програмування руху гелікоптера вгору, коли натиснуто клавішу з відповідною стрілкою.

![спрайт гелікоптера](images/helicopter-sprite.png)

```blocks3
when [up arrow v] key pressed
change y by (5)
```

--- /task ---

--- task ---

Протестуй свій код і ти побачши, що позиція `y`{:class="block3motion"} (вгору/вниз) змінюється кожного разу, коли натиснуто на клавішу стрілка вгору.

--- /task ---

--- task ---

Щоб твій гелікоптер рухався більш плавно, тобі краще додати цей код всередину циклу гелікоптера `завжди`{:class="block3motion"}.

![спрайт гелікоптера](images/helicopter-sprite.png)

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

Також ти можеш запрограмувати свій гелікоптер рухатися вліво, коли натиснуто клавішу з відповідною стрілкою. Цього разу ти маєш змінити позицію гелікоптера `x`{:class="block3motion"} на `-5`.

![спрайт гелікоптера](images/helicopter-sprite.png)

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

Тепер запрограмуй свій гелікоптер реагувати на клавіші зі стрілками вниз та вправо.

--- hints ---

--- hint ---

Скопіюй код, який використовувався для руху гелікоптера вгору та вліво, змінивши в ньому `клавіші`{:class="block3sensing"} та значення `x`{:class="block3motion"} та `y`{:class="block3motion"}

--- /hint ---

--- hint ---

Тобі знадобляться наступні блоки:

![спрайт гелікоптера](images/helicopter-sprite.png)

```blocks3
if <> then

end

change y by (-5)

change x by (5)

<key [right arrow v] pressed ?>
```

--- /hint ---

--- hint ---

Твій код повинен виглядати так:

![спрайт гелікоптера](images/helicopter-sprite.png)

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
