# Ideas on how to get a quick overview of shell commands

**Problem:** While hacking into IoT devices via UART and getting a shell there are a ton of commands that I do not know.
The ones I dont know I search on the web or man page it. Searching for commands one at a time takes alot of time.
I want quick way to ls a dir and get a quick overview of each command to see if the command will be useful.

I would like to use a bash script to accomplish this.
I would like to be able to send the script a command or a list of commands and recieve the output.
I would like the script to also serve as a filter and follow the UNIX philosophy.

**Ideas** 
1. Run a ls and pipe the output to the script
2. Redirect a text file of commands to the script
3. Search a simple database of some sort. Txt file, arrays, dict, web API?

**Questions**
1. Can more than one screen be attached to a tty at the same time?
2. Can I capture the stdout of a tty and redirect to a script or file for parsing?
3. Can a bash script even accomplish this or do I need another tool?

    #IoT #shell #BASH #script
