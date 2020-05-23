## 宙返（ちゅうがえ）りする

ヘリコプターが360度回るようにプログラムを書きましょう。

--- task ---

スペースキーが押されるたびにヘリコプターが360度回るようにしたいです。 プログラムの中の数値は360まで足し込まれる必要があることに注意してください。

![ヘリコプターのスプライト](images/helicopter-sprite.png)

```blocks3
when [space v] key pressed
repeat (360)
turn ccw (1) degrees
end
```

--- /task ---

--- task ---

スペースキーを押して試してみると、ヘリコプターがかなりゆっくり回ることがわかります。 それは1度ずつ360回繰り返すからです。

--- /task ---

--- task ---

ヘリコプターが回る速度を上げるためには、少ない回数でより多くの角度を回るようにプログラムの数値を変更します。 合計が360になれば、どんな数を選んでもよいです。

![ヘリコプターのスプライト](images/helicopter-sprite.png)

```blocks3
when [space v] key pressed
+repeat (45)
+turn ccw (8) degrees
end
```

--- /task ---

--- task ---

ヘリコプターを回すだけではなく動かしたい場合は、`(10)歩動かす`{:class="block3motion"}ブロックをプログラムに追加するだけです。

```blocks3
when [space v] key pressed
repeat (45)
+ move (5) steps
turn ccw (8) degrees
end
```

--- /task ---

--- task ---

もう一度スペースキーを押して、プログラムを試します。 ヘリコプターが円を描（えが）くように動くはずです。 `(5)歩動かす`{:class="block3motion"}ブロックの中の数値を変えたらどうなりますか？

![ヘリコプターのループ](images/toys-helicopter-360-move-test.png)

--- /task ---

