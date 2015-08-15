---
layout: post
title: Dive Into My Underlinings
---

Here are my underlinings from [Dive Into Python](http://www.amazon.com/Dive-Into-Python-Mark-Pilgrim/dp/1590593561)...

* the built in `__name__` attribute is a special value, `__main__`
* `__class__` is a built-in attribute of every Python object, `__name__` is a built-in attribute of every Python class
* using the `locals()` and `globals()` functions, you can get value of arbitrary variables dynamically, while `locals() is read-only and `globals()` is not read-only.
* you can import modules within a function, which means that the imported module is only available within the function
* package = directory of modules, nested packages = subdirectories
* unicode is a system to represent characters from all the world's different languages
* the print function really calls `sys.stdout.write`
* when opening a file, if the file doesn't exist, it will be created. If the file does exist, it will be overwritten.
* `sys.argv[0]` is the name of the script 
* `os.path.dirname` takes a filename as a string and returns the directory path portion
* each test case must be able to work in isolation from any others, every test case is an island
* the code being tested is never "ahead" of the test cases
* Let it all go. Busywork code is not important.
