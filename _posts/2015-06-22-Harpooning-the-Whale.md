---
layout: post
title: Harpooning the Whale
---

A few weeks ago now I wrote a small program that analyzed word occurences in the text of [Moby Dick](https://www.gutenberg.org/files/2701/2701-h/2701-h.htm). I love the book and this project was a fun way to do some text analysis. What follows is part of my code where I analyzed occurences of the word *whale(s)* in the text:

```python

original = open('mobydick.txt').read()
txt_split = original.split()
whalecount = 0
whale_forms = ['whale', 'whales','Whale','Whales']

for word in txt_split:
    if word in whale_forms:
        whalecount += 1

print("The whale count is %d" % (whalecount))

```

This returned:

>The whale count is **666**.

**Yes, the [Number of the Beast](https://en.wikipedia.org/wiki/Number_of_the_Beast), tied to the :whale2:, is hidden in the text!** Now if we're splitting hairs my analysis was oversimplified. The 666 result ignores all instances of *whale(s)* coupled with punctuation--i.e. "whales," or "whales;" or "whales.". But I still find this to be incredible and prefer to think of it as 666 *standalone* instances of *whale* or *whales* in the text

Its happenstances like this that really invite me on this programming journey. You can find my full program [here](https://github.com/luna-c/moby-dick-word-analysis). Thanks for reading!

