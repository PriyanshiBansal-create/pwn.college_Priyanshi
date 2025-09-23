Challenge 3: Command History

What the challenge asks
This challenge introduces the concept of command history - the shell saves a history of every command you invoke. You can scroll through saved commands using the up/down arrow keys.
The challenge states that it will inject the flag into your history, and you need to bring up a terminal, hit the up arrow, and grab the flag. This feature is useful for rerunning similar commands without typing everything from scratch.

My solve
Flag: pwn.college{ERggShtTejLsH4fVvTO_0sFgcpJ.0lNzEzNxwCN5kjNzEzW}

For this challenge, I understood that I needed to access the command history using the up arrow key. When I opened the terminal, instead of typing a command, I pressed the up arrow key to navigate through the command history.

hacker@dojo:~$ # Pressed up arrow key
hacker@dojo:~$ echo pwn.college{ERggShtTejLsH4fVvTO_0sFgcpJ.0lNzEzNxwCN5kjNzEzW}
pwn.college{ERggShtTejLsH4fVvTO_0sFgcpJ.0lNzEzNxwCN5kjNzEzW}

The flag was already pre-loaded in the command history, so when I pressed the up arrow, it appeared as a command that I could execute to display the flag.

What I learned
Through this challenge, I learned about command history functionality in Linux shells:
1.The shell automatically saves every command you execute in a history buffer
2.You can navigate through previous commands using the up and down arrow keys
3.This feature significantly improves productivity by allowing you to reuse or modify previous commands
This is especially useful when working with long or complex commands that you need to run multiple times with slight modifications

References
Did not use any references for this challenge.
