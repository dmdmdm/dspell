# dspell
A spell checker with sugestions using only /usr/share/dict/words - emulates ispell and aspell

Other spell checkers are huge beasts.  But this one is pretty small.
It just uses /usr/share/dict/words which is available on all Linux systems.

Here is what happens when you send a correctly spelled word and an incorrected spelled word:

 ```
 echo apple orrange | ./dspell
 @(#) International Ispell Version 3.1.20 (but really dspell .1)
 *
 & orrange 6 6: arrange, cornage, orange, oranger, oranges, orangey
```

You get pretty much the same thing from big aspell:
```
echo apple orrange | aspell -a
@(#) International Ispell Version 3.1.20 (but really Aspell 0.60.8)
*
& orrange 13 6: Orange, orange, arrange, arranger, or range, or-range, oranges, range, arranged, arranges, grange, Orange's, orange's
```