## ちょうネクタイを回す

ちょうネクタイを押したら回るようにプログラムを書いてみましょう。

--- task ---

基本（きほん）のScratchプロジェクトを開きます。

**オンライン**: [基本（きほん）のプロジェクト](https://scratch.mit.edu/projects/399190901){:target="_blank"}を開きます。

スクラッチアカウントを持っている場合は、**リミックス**をクリックしてコピーを作成できます。

**オフライン**: オフラインエディターで[基本（きほん）のプロジェクト](http://rpf.io/p/ja-JP/tech-toys-go){:target="_blank"}を開きます。

[rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}からScratchオフラインエディターをダウンロードしてインストールできます。

基本（きほん）のプロジェクトには2人の人物とラップトップ、ヘリコプターがあります。

![基本（きほん）のプロジェクト](images/toys-starter.png)

--- /task ---

--- task ---

「ちょうネクタイ」のスプライトを押して、次のコードを追加します。

![ちょうネクタイのスプライト](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
turn cw (15) degrees
end
```

--- /task ---


--- task ---

ちょうネクタイを押してプログラムを実行します。 ちょうネクタイが時計回りに15度ずつ10回 回り、合計で150度回ります。

![150度回ったちょうネクタイ](images/toys-bowtie-test.png)

--- /task ---

--- task ---

`(90)度に向ける`{:class="block3motion"}ブロックを見つけて、_そのブロックをドラッグせずに_クリックし、ちょうネクタイを最初の位置に戻します。

```blocks3
point in direction (90 v)
```

ヒント：Scratchではブロックをクリックするとすぐに実行できます。 最初にブロックをスクリプトエリアにドラッグする必要さえありません！

--- /task ---

--- task ---

ちょうネクタイを一回転させるには、プログラムの中の数値を360度まで足していく必要があります。 ちょうネクタイを`36`度ずつ10回（36 x 10 = 360）回すようにプログラムを変更してみましょう。

![ちょうネクタイのスプライト](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
+turn cw (36) degrees
end
```

--- /task ---

--- task ---

もう一度試してみましょう。 今回はちょうネクタイが360度回って最初の位置に戻るはずです。

--- /task ---

ちょうネクタイを4回転させたいときは、`(10)回繰り返す`{:class"block3control"}ブロックの中の数値を`10`から`40`に変更します。

```blocks3
when this sprite clicked
+repeat (40)
turn cw (36) degrees
end
```
