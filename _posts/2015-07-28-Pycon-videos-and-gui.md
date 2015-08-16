---
layout: post
title: Pycon Videos and Gui
category: programming
---

I was listening to the [Talk Python To Me](http://www.talkpythontome.com/episodes/show/4/enterprise-python-and-large-scale-projects) podcast and came across Allison Kaptur's Pycon Talk [Bytes in the Machine](https://www.youtube.com/watch?v=HVUTjQzESeo). I enjoyed her talk. Like most Python talks I've watched in the past, speakers do an incredible job of simplifying techniques while leaving out a lot of the complexities that I drown in. I also watched Guido Van Rossum's keynote and that was fun. 

I fooled around with this Fun GUI today thats in [Programming Python](http://kysmykseka.net/koti/wizardry/Programming/Python/Programming%20Python,%204th%20Edition%20(2010).pdf)...

```
from tkinter import *
import random
fontsize = 30
colors = ['red', 'green', 'blue', 'yellow', 'orange', 'cyan', 'purple']

def onSpam():
	popup = Toplevel()
	color = random.choice(colors)
	Label(popup, text='Popup', bg='black', fg=color).pack(fill=BOTH)
	mainLabel.config(fg=color)

def onFlip():
	mainLabel.config(fg=random.choice(colors))
	main.after(100, onGrow)

def onGrow():
	global fontsize
	fontsize += 5
	mainLabel.config(font=('arial', fontsize, 'italic'))
	main.after(100, onGrow)

main = Tk()
mainLabel = Label(main, text='Fun Gui!', relief=RAISED)
mainLabel.config(font=('arial', fontsize, 'italic'), fg='cyan',bg='navy')
mainLabel.pack(side=TOP, expand=YES, fill=BOTH)
Button(main, text='spam', command=onSpam).pack(fill=X)
Button(main, text='flip', command=onFlip).pack(fill=X)
Button(main, text='grow', command=onGrow).pack(fill=X)
main.mainloop()
```
Programming Python is the perfect book for where I'm at right now and I'm loving it.

Also I found the [Zen Mode](https://github.com/blog/1379-zen-writing-mode) of writing on Github which I love! It should significantly increase my post output. Do check it out!

