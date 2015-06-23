---
layout: post
title: Harpooning the Whale
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

Yes, the [Number of the Beast](https://en.wikipedia.org/wiki/Number_of_the_Beast) equals the word occurrences of whale(s) in Moby Dick. **Yes, the Number of the Beast directly linked to the whale is hidden in the text!** 

There are obvious gaps in my program. For example, the **666** count ignores all instances split with punctuation attached--i.e. *whales,* or *whales.* or *whales;*. Nevermind, how all the occurences might not be talking about **THE WHALE**(Moby Dick). Overlooking its many shortcomings while using my dramatic simplification, I love this whale count because I found a connection betwee the Beast, a major mythological icon, and the whale. By doing so, I created--with the help of Python--yet another allegory concealed in Melville's text.

So I got that amazing feeling of successfully programming a solution x1000. Creating this program showed me just how much enjoyment and understanding I can potentially derive from programming. I create what is meaningful--in programs and in narratives.

You can find my full program [here](https://github.com/luna-c/moby-dick-word-analysis). This blog is associated with **lunacy** for a reason!

