## Πέταξε το ελικόπτερό σου

Ας χρησιμοποιήσουμε τα πλήκτρα βέλους για να πετάξει το ελικόπτερό σου.

--- task ---

Ας ξεκινήσουμε γράφοντας κώδικα ώστε το ελικόπτερό σου να μετακινηθεί προς τα πάνω όταν πατηθεί το πλήκτρο πάνω βέλος.

![αντικείμενο ελικόπτερο](images/helicopter-sprite.png)

```blocks3
when [up arrow v] key pressed
change y by (5)
```

--- /task ---

--- task ---

Δοκίμασε τον κώδικά σου και θα δεις ότι η θέση `y`{:class="block3motion"} του ελικοπτέρου (πάνω/κάτω) αλλάζει κάθε φορά που πατάς το πλήκτρο επάνω βέλος.

--- /task ---

--- task ---

Για να κινηθεί το ελικόπτερο πιο ομαλά, μπορείς αντ' αυτού να προσθέσεις κώδικα για να μετακινηθεί προς τα πάνω μέσα στο μπλοκ `για πάντα`{:class="block3motion"} του ελικοπτέρου σου.

![αντικείμενο ελικόπτερο](images/helicopter-sprite.png)

```blocks3
when I receive [εκκίνηση v]
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

Μπορείς επίσης να γράψεις κώδικα ώστε το ελικόπτερο να μετακινείται προς τα αριστερά όταν πατήσεις το πλήκτρο αριστερό βέλος. Αυτή τη φορά θα πρέπει να αλλάξεις τη θέση `x`{:class="block3motion"} του ελικοπτέρου κατά `-5`.

![αντικείμενο ελικόπτερο](images/helicopter-sprite.png)

```blocks3
when I receive [εκκίνηση v]
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

Τώρα γράψε τον κώδικά σου ώστε το ελικόπτερο να ανταποκρίνεται στα πλήκτρα κάτω και δεξιό βέλος.

--- hints ---


--- hint ---

Αντίγραψε τον κώδικα που χρησιμοποίησες για να κάνεις το ελικόπτερο να κινηθεί προς τα πάνω και προς τα αριστερά, αλλάζοντας τα `πλήκτρα`{:class="block3sensing"} που χρησιμοποιήθηκαν και τις τιμές `x`{:class="block3motion"} & `y`{:class="block3motion"}

--- /hint ---

--- hint ---

Θα χρειαστείς αυτά τα μπλοκ:

![αντικείμενο ελικόπτερο](images/helicopter-sprite.png)

```blocks3
if <> then

end

change y by (-5)

change x by (5)

<key [right arrow v] pressed ?>
```

--- /hint ---

--- hint ---

Ο κώδικας θα πρέπει να μοιάζει κάπως έτσι:

![αντικείμενο ελικόπτερο](images/helicopter-sprite.png)

```blocks3
when I receive [εκκίνηση v]
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
