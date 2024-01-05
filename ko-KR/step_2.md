## 나비 넥타이 돌리기

클릭하면 회전하는 나비넥타이를 코딩해봅시다.

--- task ---

스크래치 스타터 프로젝트를 여세요.

**Online**: open the [starter project](https://rpf.io/tech-toys-on){:target="_blank"}.

스크래치 계정이 있는 경우 **리믹스**를 클릭하여 복사본을 만들 수 있습니다.

**Offline**: open the [starter project](https://rpf.io/p/en/tech-toys-go){:target="_blank"} in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

스타터 프로젝트에서는 노트북과 헬리콥터, 총 두개의 캐릭터가 나옵니다.

![스타터 프로젝트](images/toys-starter.png)

--- /task ---

--- task ---

'나비 넥타이' 스프라이트를 클릭하고 다음 코드를 입력하세요:

![나비 넥타이 스프라이트](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
turn cw (15) degrees
end
```

--- /task ---


--- task ---

나비 넥타이를 클릭하여 코드를 실행하세요. 나비넥타이가 시계방향으로 15도씩 10번, 총 150도 회전하는 것을 볼 수 있습니다.

![150도 회전하는 나비 넥타이](images/toys-bowtie-test.png)

--- /task ---

--- task ---

`방향 보기`{:class="block3motion"} 블록을 찾아 _드래그 하지 않고_ 클릭하여 나비넥타이를 시작 위치로 설정합니다.

```blocks3
point in direction (90 v)
```

팁: 스크래치에서 블록을 클릭하여 바로 실행할 수 있습니다. 스크립트 영역으로 먼저 드래그할 필요가 없습니다!

--- /task ---

--- task ---

나비넥타이를 1바퀴 회전시키려면 코드의 숫자를 360도까지 늘려야 합니다. 나비넥타이가 `36도`로 10회 회전하도록 코드를 변경합니다.(36 x 10 = 360)

![나비 넥타이 스프라이트](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
+turn cw (36) degrees
end
```

--- /task ---

--- task ---

코드를 다시 테스트 해 보세요. 이번에는 나비넥타이가 360도로 한 번 회전하고 원래 있던 자리로 돌아와야 합니다.

--- /task ---

나비넥타이를 4번 회전하려면 `반복`{:class="block3control"} 블록의 숫자를 `10`에서 `40`으로 변경할 수 있습니다.

```blocks3
when this sprite clicked
+repeat (40)
turn cw (36) degrees
end
```
