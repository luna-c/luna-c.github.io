---
layout: post
title: Harpooning the Whale
category: programming
---

A few weeks ago I wrote a small python program that analyzed word occurences in the text of [Moby Dick](https://www.gutenberg.org/files/2701/2701-h/2701-h.htm). I love Melville's book and this project was a fun way to do some text analysis on it. What follows is part of my code where I analyzed occurences of the word *whale(s)* in the text:

    original = open('mobydick.txt').read()
    txt_split = original.split()
    whalecount = 0
    whale_forms = ['whale', 'whales', 'Whale', 'Whales']

    for word in txt_split:
      if word in whale_forms:
        whalecount += 1
    print("The whale count is %d" % (whalecount))

This returned:

>The whale count is **666**.

The [Number of the Beast](https://en.wikipedia.org/wiki/Number_of_the_Beast) equals the word occurrences of whale(s) in Moby Dick. **Yes, the Number of the Beast directly linked to the whale is hidden in the text!** 

There are obvious gaps in my module. For example, the **666** count ignores all instances split with punctuation attached--i.e. 'whales,' or 'whales.' or 'whales;'. And all the occurences might not be referencing THE whale(Moby Dick). So I am overlooking many shortcomings while employing dramatic simplification. But I love this whalecount because I found a connection between the Beast, a major mythological icon, and the whale. I created--with the help of Python--yet another allegory concealed in Melville's text.

I got that amazing feeling x1000 from successfully programming this module.

You can find my complete program [here](https://github.com/luna-c/moby-dick-word-analysis). This blog is associated with **lunacy** for a reason!

