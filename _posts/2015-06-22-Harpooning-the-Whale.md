---
layout: post
title: Harpooning the Whale
---

A few weeks ago now I wrote a small python program that analyzed word occurences in the text of [Moby Dick](https://www.gutenberg.org/files/2701/2701-h/2701-h.htm). I love Melville's book and this project was a fun way to do some text analysis on it. What follows is part of my code where I analyzed occurences of the word *whale(s)* in the text:

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

**Yes, the [Number of the Beast](https://en.wikipedia.org/wiki/Number_of_the_Beast), tied to the whale, is hidden in the text!** If we're splitting hairs my analysis was oversimplified. The **666** result ignores all instances split with punctuation attached--i.e. *whales,* or *whales.* or *whales;*. Acknowledging the gaps in my program, I still love this whale count. 

In Moby Dick, Melville confronted many big ideas such as fate and free-will as well as the relationship between God and Man. So its funny that I found the beast, another major mythological icon, lurking within the whale. Connecting these two symbols reveals yet another allegory extracted from Melville's text, one I imagine few people know about.

This program gave me the amazing feeling of successfully programming a solution x1000. It showed me just how much enjoyment and understanding I can derive from the programming. 

You can find my full program [here](https://github.com/luna-c/moby-dick-word-analysis). This blog isn't called **lunacy** for nothing!

