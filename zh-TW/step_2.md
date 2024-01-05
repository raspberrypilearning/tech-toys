## 旋轉領結

讓我們編寫一個點擊後會旋轉的領結

--- task ---

打開Scratch入門專案。

**Online**: open the [starter project](https://rpf.io/tech-toys-on){:target="_blank"}.

如果你有 Scratch 帳戶，你可以透過點擊**Remix**來創建副本並進行改編。

**Offline**: open the [starter project](https://rpf.io/p/en/tech-toys-go){:target="_blank"} in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

在入門專案中，你應該會看到2個人物、一台筆記型電腦和一架直升機。

![入門專案](images/toys-starter.png)

--- /task ---

--- task ---

點擊“領結”，然後添加以下程式碼：

![領結](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
turn cw (15) degrees
end
```

--- /task ---


--- task ---

點擊領結來執行你的程式碼。 你應該會看到領結順時針旋轉15度10次，總共旋轉150度。

![領結轉150度](images/toys-bowtie-test.png)

--- /task ---

--- task ---

找到`面朝角度`{:class="block3motion"}積木，先_不要拖曳它_，請點擊它來讓領結回到初始位置。

```blocks3
point in direction (90 v)
```

提示：在Scratch中，你可以點擊一個積木以立即執行它。 你甚至不需要先將它拖曳到程式區域！

--- /task ---

--- task ---

為了使領結完成1次完整旋轉，程式碼中的數字加起來需要為360度。 透過更改程式碼，讓領結旋轉` 36 `度10次(36 x 10 = 360)。

![領結](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
+turn cw (36) degrees
end
```

--- /task ---

--- task ---

再試試你的程式。 這次，你的領結應該進行1次完整的360度旋轉，並停止在初始位置。

--- /task ---

如果希望領結完成4次完整旋轉，可以把`重複` {:class=“block3control”}積木的數字從`10`改成至`40` 。

```blocks3
when this sprite clicked
+repeat (40)
turn cw (36) degrees
end
```
