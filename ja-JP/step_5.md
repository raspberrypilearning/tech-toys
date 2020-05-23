## ヘリコプターを飛ばす

矢印キーを使ってヘリコプターと飛ばしてみましょう。

--- task ---

上矢印が押されたときにヘリコプターが上昇するようにプログラムを書くところから始めましょう。

![ヘリコプターのスプライト](images/helicopter-sprite.png)

```blocks3
when [up arrow v] key pressed
change y by (5)
```

--- /task ---

--- task ---

プログラムを試してみると、上矢印を押すたびにヘリコプターの`y`{:class="block3motion"}座標（上／下）が変わることがわかります。

--- /task ---

--- task ---

ヘリコプターをもっと簡単に動かすために、このブロックに代えてヘリコプターの`ずっと`{:class="block3motion"}ループの中に上方向に動かすプログラムを追加します。

![ヘリコプターのスプライト](images/helicopter-sprite.png)

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

左矢印を押したときに左に移動するようにヘリコプターにプログラムを追加することもできます。 今度は`x`{:class="block3motion"}座標を`-5`ずつ変える必要があります。

![ヘリコプターのスプライト](images/helicopter-sprite.png)

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

では、ヘリコプターが下矢印キーと右矢印キーに反応するようにプログラムを書いてみてください。

--- hints ---

--- hint ---

ヘリコプターを上や左に動かすのに使ったプログラムをコピーし、使用した`キー`{:class="block3sensing"}と`x`{:class="block3motion"}と`y`{:class="block3motion"}の値を変更します。

--- /hint ---

--- hint ---

次のブロックが必要です：

![ヘリコプターのスプライト](images/helicopter-sprite.png)

```blocks3
if <> then

end

change y by (-5)

change x by (5)

<key [right arrow v] pressed ?>
```

--- /hint ---

--- hint ---

コードは以下のようになります：

![ヘリコプターのスプライト](images/helicopter-sprite.png)

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
