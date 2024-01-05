## घूमता हुए बो टाय

आइए एक बो टाई को कोड करें जो क्लिक करने पर घूमता है।

--- task ---

Scratch स्टार्टर प्रोजेक्ट खोलें।

**Online**: open the [starter project](https://rpf.io/tech-toys-on){:target="_blank"}.

यदि आपके पास एक Scratch खाता (account) है तो आप **Remix** पर क्लिक करके प्रतिलिपि बना सकते हैं |

**Offline**: open the [starter project](https://rpf.io/p/en/tech-toys-go){:target="_blank"} in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

स्टार्टर प्रोजेक्ट में, आपको 2 चीज़े, एक लैपटॉप और एक हेलीकॉप्टर दिखाई देना चाहिए।

![स्टार्टर प्रोजेक्ट](images/toys-starter.png)

--- /task ---

--- task ---

'Bow Tie' (बो टाय) स्प्राइट पर क्लिक करें और इस कोड को जोड़ें:

![बो टाय स्प्राइट](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
turn cw (15) degrees
end
```

--- /task ---


--- task ---

अपने कोड को चलाने के लिए बो टाई पर क्लिक करें। आपको दिखाई देना चाहिए कि आपका बो टाई 10 बार 15 डिग्री घूमता है, यानी कुल मिलाकर 150 डिग्री।

![बो टाय 150 डिग्री घूमता हैं](images/toys-bowtie-test.png)

--- /task ---

--- task ---

`point in direction`{:class="block3motion"} ब्लॉक को खोजें और, _इसे खींचे बिना_ क्लिक करें, यह बो टाई को अपनी शुरुआती स्थिति में वापस सेट करता हैं।

```blocks3
point in direction (90 v)
```

टिप: Scratch में आप इसे ब्लॉक पर क्लिक कर चला सकते हैं। आपको इसे पहले स्क्रिप्ट क्षेत्र पर खींचने की भी आवश्यकता नहीं है!

--- /task ---

--- task ---

बो टाई को 1 पूर्ण स्पिन करने के लिए, आपके कोड में संख्याओं का जोड़ 360 डिग्री तक होना होगा। अपना कोड बदलें ताकि बो टाई `36` डिग्री 10 बार (36 x 10 = 360) बदलें।

![बो टाय स्प्राइट](images/bowtie-sprite.png)

```blocks3
when this sprite clicked
repeat (10)
+turn cw (36) degrees
end
```

--- /task ---

--- task ---

अपने कोड का फिर से परीक्षण करें। इस बार, आपके बो टाई को 1 पूर्ण 360 डिग्री घुमाना पड़ेगा ताकि वह जहां से आया है वहीं वापस रुक जाएं।

--- /task ---

यदि आप चाहते हैं कि आपका बो टाय 4 बार पूर्ण घूमें, तो आपको `repeat`{:class="block3control"} ब्लॉक की संख्या को `10` से `40` में बदलनी होगी।

```blocks3
when this sprite clicked
+repeat (40)
turn cw (36) degrees
end
```
