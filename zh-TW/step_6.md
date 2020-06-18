## 翻跟斗飛行

讓我們為你的直升機編碼來進行360度旋轉。

--- task ---

我們希望每當按下空白鍵時，直升機都會進行360度旋轉。 請記住，你程式中的數字加起來需要為360。

![直升機](images/helicopter-sprite.png)

```blocks3
when [space v] key pressed
repeat (360)
turn ccw (1) degrees
end
```

--- /task ---

--- task ---

按空格鍵測試程式碼，你會發現直升機旋轉非常緩慢。 那是因為它只轉了1度並轉360次。

--- /task ---

--- task ---

為了加快直升機的旋轉速度，請更改程式中的數字，以使其旋轉角度增加，旋轉次數減少。 設定多少數字都沒關係，只要它們加起來等於360！

![直升機](images/helicopter-sprite.png)

```blocks3
when [space v] key pressed
+repeat (45)
+turn ccw (8) degrees
end
```

--- /task ---

--- task ---

如果你想讓直升機移動以及旋轉，只需添加`移動`{:class=“block3motion”}積木到你的程式中。

```blocks3
when [space v] key pressed
repeat (45)
+ move (5) steps
turn ccw (8) degrees
end
```

--- /task ---

--- task ---

再次按空白鍵來測試你的程式。 你應該會看到直升機轉了一圈。 如果你更改`移動`{:class=“block3motion”}積木裡的數字會怎樣？

![直升機翻跟斗飛行](images/toys-helicopter-360-move-test.png)

--- /task ---

