## ちょうネクタイを回す

ちょうネクタイを押したら回るようにプログラムを書いてみましょう。

--- task ---

基本（きほん）のScratchプロジェクトを開きます。

**オンライン**: [基本（きほん）のプロジェクト](http://rpf.io/tech-toys-on){:target="_blank"}を開きます。

スクラッチアカウントを持っている場合は、**リミックス**をクリックしてコピーを作成できます。

**オフライン**: オフラインエディターで[基本（きほん）のプロジェクト](http://rpf.io/p/en/tech-toys-go){:target="_blank"}を開きます。

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

Find the `point in direction`{:class="block3motion"} block and, _without dragging it_, click it to set the bow tie back to its starting position.

```blocks3
point in direction (90 v)
```

Tip: In Scratch you can click on a block to run it straight away. You don't even need to drag it onto the scripts area first!

--- /task ---

--- task ---

To make the bow tie do 1 complete spin, the numbers in your code need to add up to 360 degrees. Change your code so that the bow tie turns `36` degrees 10 times (36 x 10 = 360).

![bowtie sprite](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
+turn cw (36) degrees
end
```

--- /task ---

--- task ---

Test your code again. This time, your bow tie should do 1 complete 360 degree spin and end up where it started.

--- /task ---

If you want your bow tie to do 4 complete spins, you can change the number in the `repeat`{:class="block3control"} block from `10` to `40`.

```blocks3
when this sprite clicked
+repeat (40)
turn cw (36) degrees
end
```
