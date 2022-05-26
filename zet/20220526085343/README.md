# String Slicing in Bash

I just spent a bunch of time trying to figure out what the hell was
going on when trying to slice up a string in bash!

In other languages I have coded in you start at the string index where
you want to start the slice and end/include the index where you want to
stop.

Well bash is different unless Im missing something. You give it a
starting index and how many chars you want to include.

### Example
foo="Please slice me"</br>
echo "${foo:0:3}" -> "Ple"

At first glance I thought it was starting on index 0 and printing up to
but not including index 3 like Ive seen in a few other languages I have
messed with.

The 3 is not the dam index.... Ha!! O well. Lesson learned!

    #strings #bash #scripting
