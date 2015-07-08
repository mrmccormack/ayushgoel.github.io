---
tags: bash error
---

Handling strings in Bash
-

    if test ! -f $path
    
The above script would create bash warnings for you like

    test: too many arguments
    
The problem here is that the path contains spaces in it, and thus the test gets “more than one arguments”.

The solution for the above problem is a pretty simple one, wrap the path in inverted commas 😅.

    if test ! -f “$path”