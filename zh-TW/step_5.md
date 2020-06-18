## 操控你的直升機

讓我們使用方向鍵來操控你的直升機。

--- task ---

讓我們開始編碼，當按下『向上鍵』時，直升機會向上移動。

![直升機](images/helicopter-sprite.png)

```blocks3
when [up arrow v] key pressed
change y by (5)
```

--- /task ---

--- task ---

測試你的代碼，你將會看到每當按下『向上鍵』時，直升機的`y`{:class=“block3motion”}的位置(上/下)會改變。

--- /task ---

--- task ---

為了使直升機更平穩地移動，你可以改成在`重複無限次`{:class=“block3motion”}迴圈中添加程式碼來向上移動直升機。

![直升機](images/helicopter-sprite.png)

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

你還可以對直升機進行編碼，在按下左鍵時向左移動。 這次你需要更改直升機的`x`{:class=“block3motion”}的位置為`-5`。

![直升機](images/helicopter-sprite.png)

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

現在，為你的直升機編碼，以響應上下鍵。

--- hints ---

--- hint ---

複製你用來使直升機向上和向左的程式碼，更改使用的`鍵`{:class=“block3sensing”}，以及`x`{:class=“block3motion”}和`y`{:class=“block3motion”}的值。

--- /hint ---

--- hint ---

你會需要這些積木：

![直升機](images/helicopter-sprite.png)

```blocks3
if <> then

end

change y by (-5)

change x by (5)

<key [right arrow v] pressed ?>
```

--- /hint ---

--- hint ---

你的程式應該會像這樣：

![直升機](images/helicopter-sprite.png)

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
