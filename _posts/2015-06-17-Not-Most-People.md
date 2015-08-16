---
layout: post
title: Not Most People
category: programming
---

I most definitely did **not** install Kivy the other day. That process seems to have gotten away from me because there many additional packages that are required to load Kivy.(At least they appear to be required) So I began working through them. I had to uninstall Cython because Kivy uses an earlier version than the one I installed. After a few minutes of navigating uninstall schemes, using `pip` turned out to be the really easy solution. But I ended up stuck without being able to install Kivy. [This](https://github.com/kivy/kivy/issues/3309) is the best resource I could find on my bug but I didn't understand how to implement the solution in xcode fully. Going to approach some Kivy user group soon.

Here's an idea I came across in the [PyGame install.txt](https://github.com/xamox/pygame/blob/master/install.txt):

>"most people prefer to leave the system Python alone, and use the python downloaded from python.org" 

I'm not on the side of "most people" in this case. I've installed all my packages into my native Python using the command line. I'm curious to learn how you install packages onto a downloaded version of Python.

Started writing out a timer app that measures a user's time until the 10,000 hour mastery level. Planning to put the finish product on Github in the next few days.
