## 곡예 비행

헬리콥터가 360도 회전을 하게 코딩해봅시다.

--- task ---

우리는 스페이스바가 눌러져있을 때마다 헬리콥터가 360도 회전하기를 원합니다. 코드 안의 숫자는 360도가 되어야 한다는 걸 기억하세요.

![헬리콥터 스프라이트](images/helicopter-sprite.png)

```blocks3
when [space v] key pressed
repeat (360)
turn ccw (1) degrees
end
```

--- /task ---

--- task ---

스페이스바를 눌러 코드를 테스트하면 헬리콥터가 아주 천천히 회전하는 것을 볼 수 있을 것입니다. 이 이유는 1도씩 360번 회전하기 때문입니다.

--- /task ---

--- task ---

헬리콥터의 회전을 빠르게 하기 위해서 코드 안의 숫자를 바꿔서 각도는 늘이고 횟수는 줄여서 회전하게 만드세요. 총 회전하는 각도가 360도인 이상 무슨 숫자가 들어가던 상관 없습니다!

![헬리콥터 스프라이트](images/helicopter-sprite.png)

```blocks3
when [space v] key pressed
+repeat (45)
+turn ccw (8) degrees
end
```

--- /task ---

--- task ---

헬리콥터가 회전할 뿐만 아니라 이동까지 하게 하려면 `움직이기`{:class="block3motion"} 블록을 코드에 추가하기만 하면 됩니다.

```blocks3
when [space v] key pressed
repeat (45)
+ move (5) steps
turn ccw (8) degrees
end
```

--- /task ---

--- task ---

스페이스바를 눌러 다시 코드를 테스트하세요. 헬리콥터가 원 모양으로 움직이는 것을 볼 수 있습니다. `움직이기`{:class="block3motion"} 블록 안의 숫자를 바꾸면 무슨 일이 일어나나요?

![헬리콥터 반복문](images/toys-helicopter-360-move-test.png)

--- /task ---

