## हेलीकॉप्टर को उड़ाना

चलिएं, हेलीकाप्टर को उड़ाने के लिए ऊपर, निचे, दाएं, बाएं (तीर) वाले कुंजियों का इस्तमाल करे।

--- task ---

चलो अभी हेलीकॉप्टर को कोड करना शुरू करें, जब भी ऊपर तीर कुंजी (Up Arrow Key) दबाया जाए तब हेलीकॉप्टर तो ऊपर जाना चाहिए।

![हेलीकॉप्टर स्प्राइट](images/helicopter-sprite.png)

```blocks3
when [up arrow v] key pressed
change y by (5)
```

--- /task ---

--- task ---

अपने कोड का परीक्षण करें और आप देखेंगे कि जब भी ऊपर तीर कुंजी (Up Arrow Key) दबाई जाती है तब आपके हेलीकॉप्टर का `y`{:class="block3motion"} स्थान बदल जाता है।

--- /task ---

--- task ---

अपने हेलिकॉप्टर को अधिक आसानी से ले जाने के लिए, ऊपर जाने के लिए आप इसके बजाय अपने हेलिकॉप्टर के `forever`{:class="block3motion"} लूप के अंदर कोड जोड़ सकते हैं।

![हेलीकॉप्टर स्प्राइट](images/helicopter-sprite.png)

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

बाएं तीर कुंजी (Left Arrow Key) को दबाए जाने आप अपने हेलीकॉप्टर को बाईं ओर ले जाने के लिए कोड भी कर सकते हैं। इस बार आपको हेलीकॉप्टर के `x`{:class="block3motion"} स्थान को `-5` से बदलना होगा।

![हेलीकॉप्टर स्प्राइट](images/helicopter-sprite.png)

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

अब अपने हेलिकॉप्टर को कोड करें ताकि जब निचे और दाए तीर के कुंजी दबाएं जाय तब हेलीकॉप्टर उस दिशा में जाए।

--- hints ---


--- hint ---

हेलीकॉप्टर को ऊपर और बाएं ओर उड़ाने के लिए आपके द्वारा उपयोग किए गए कोड को कॉपी करें, `keys`{:class="block3sensing"} (कुंजियों) को बदलते हुए `x`{:class="block3motion"} & `y`{:class="block3motion"} के मान को बदलिएं।

--- /hint ---

--- hint ---

आपको इन ब्लॉक्स की आवश्यकता होगी:

![हेलीकॉप्टर स्प्राइट](images/helicopter-sprite.png)

```blocks3
if <> then

end

change y by (-5)

change x by (5)

<key [right arrow v] pressed ?>
```

--- /hint ---

--- hint ---

आपका कोड इस प्रकार दिखना चाहिए:

![हेलीकॉप्टर स्प्राइट](images/helicopter-sprite.png)

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
