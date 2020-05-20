## 헬리콥터 날리기

화살표를 눌러 헬리콥터를 비행시켜봅시다.

--- task ---

먼저 위쪽 화살표를 누르면 위로 이동하도록 헬리콥터를 코딩하는 것으로 시작하겠습니다.

![헬리콥터 스프라이트](images/helicopter-sprite.png)

```blocks3
when [up arrow v] key pressed
change y by (5)
```

--- /task ---

--- task ---

코드를 테스트하면 위쪽 화살표를 누를 때마다 헬리콥터의 `y`{:class="block3motion"} 좌표(위/아래)가 변경되는 것을 볼 수 있습니다.

--- /task ---

--- task ---

헬리콥터가 더 부드럽게 움직이도록 하려면 `무한 반복하기`{:class="block3motion"} 반복문 안에 코드를 추가하여 헬리콥터가 위로 이동할 수 있습니다.

![헬리콥터 스프라이트](images/helicopter-sprite.png)

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

왼쪽 화살표를 누르면 왼쪽으로 이동하도록 헬리콥터에 코딩할 수도 있습니다. 이번에는 헬리콥터의 `x`{:class="block3motion"} 좌표를 `5`만큼 변경해야 합니다.

![헬리콥터 스프라이트](images/helicopter-sprite.png)

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

이제 아래쪽 방향키와 오른쪽 방향키에도 응답하도록 헬리콥터를 코딩합니다.

--- hints ---

--- hint ---

헬리콥터를 위쪽과 왼쪽으로 움직이게 했던 코드를 복사하여 `방향키`{:class="block3sensing"}와 `x`{:class="block3motion"}&`y`{:class="block3motion"}의 값을 변경해줍니다.

--- /hint ---

--- hint ---

이 블럭들이 필요할겁니다.

![헬리콥터 스프라이트](images/helicopter-sprite.png)

```blocks3
if <> then

end

change y by (-5)

change x by (5)

<key [right arrow v] pressed ?>
```

--- /hint ---

--- hint ---

다음과 같은 코드가 될 것입니다:

![헬리콥터 스프라이트](images/helicopter-sprite.png)

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
