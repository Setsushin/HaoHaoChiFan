+++
title = "Always Use Guard in Coding"
date = 2021-09-01T00:00:00+09:00
draft = false
tags = ["tech"]
catagories = ["tech"]
+++

You must ever been tormented by multiple nested _if-else_ statements, like following:  
```Python
if (case1):
    if (case2):
        if (case3):
            do_something()
```

Yes, it's very natural, but not good enough.
However, the fact is that even the author himself, he will forget all logics when he reviews after only a few days.  
So if you want to implement the above logic, it's recommended to use guard like this:  
```Python
if (not case1):
	break
if (not case2):
	break
if (not case3)
	break
do_something()
```
which makes the structure flatter and easier to understand.