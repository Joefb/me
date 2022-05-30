# GMT Isosec Converter

### Problem
My zet directory is growing. The isosec names are starting to blur
together. I want a script that will convert the isosec names into a
readable format so I can quickly scan for certain days or times.
The script will convert the isosec to the default time zone of the
computer in a readable format.

I want the script to follow the UNIX philosophy so I can use it as a
filter as well.

### Ideas
I'm not sure how to approach this. One idea was to use the file creation
date to quickly get the day and time but that defeats the idea of using
the script as converter or filter.

Another idea is to spit up the file name using slices, storing each
slice into a single var with a format that the date command can use to
convert it to what ever the default timezone is of the computer.

Maybe theres some awesome way I dont know about! Hmmmm..

    #isosec #bash #scripting
