## تحليق طائرتك العمودية

دعونا نستخدم مفاتيح الأسهم لطيران طائرتك العمودية.

--- task ---

دعونا نبدأ ببرمجة مروحيتك للتحرك للأعلى عندما يتم الضغط على السهم لأعلى.

![كائن الطائرة العامودية](images/helicopter-sprite.png)

```blocks3
when [up arrow v] key pressed
change y by (5)
```

--- /task ---

--- task ---

اختبر التعليمات البرمجية الخاصة بك وسترى أن الموقع `ص`{:class="block3motion"} (للاعلى/للاسفل) للطائرة العمودية يتغير كلما تم الضغط على السهم الأعلى.

--- /task ---

--- task ---

لجعل مروحيتك تتحرك بسلاسة، يمكنك بدلاً من ذلك إضافة تعليمة برمجية للتحرك إلى الأعلى داخل تعليمة الطائرة `للأبد`{:class="block3motion"}.

![كائن الطائرة العامودية](images/helicopter-sprite.png)

```blocks3
when I receive [البداية v]
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

يمكنك أيضا برمجة الطائرة للتحرك إلى اليسار عند الضغط على السهم الأيسر. هذه المرة ستحتاج إلى تغيير موقع الطائرة العمودية `س`{:class="block3motion"} بمقدار `-5`.

![كائن الطائرة العامودية](images/helicopter-sprite.png)

```blocks3
when I receive [البداية v]
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

الآن برمج طائرتك للاستجابة الى مفاتيح الأسهم للأسفل واليمين.

--- hints ---


--- hint ---

انسخ التعليمات البرمجية التي استخدمتها لجعل الطائرة العمودية تتحرك للأعلى والأيسر، وتغيير قيم `المفاتيح `{:class="block3sensing"} المستخدمة و موقعي `س`{:class="block3motion"} و `ص`{:class="block3motion"}

--- /hint ---

--- hint ---

ستحتاج إلى هذه التعليمة البرمجية:

![كائن الطائرة العامودية](images/helicopter-sprite.png)

```blocks3
if <> then

end

change y by (-5)

change x by (5)

<key [right arrow v] pressed ?>
```

--- /hint ---

--- hint ---

يجب أن تبدو التعليمات البرمجية خاصتك بالشكل التالي:

![كائن الطائرة العامودية](images/helicopter-sprite.png)

```blocks3
when I receive [البداية v]
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
