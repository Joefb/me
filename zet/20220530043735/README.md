# Zettel Searching

**Problem**</br>
I need a way to quickly search my zettels for a keyword. I want to create
a script that will search the zettels, pull the title, and show the dir
and file its located in. This way I can easily link my zettels together
by doing a quick search.

**Ideas/Solutions**</br>
One idea is to use head and grep. Something like:</br>
`head -n 1 $(grep -rl "$1")` Ill hafta think about it.

Maybe I could add more functionality in the script. Im not not sure what.
I guess Ill add more as needed. For now I think the above script
would work for what I need.


    #zettel #bash
