Challenge 1: Intro to Commands
What the challenge asks
In this challenge, you will invoke your first command! When you type a command and hit enter, the command will be invoked. The challenge demonstrates this with the whoami command example:

hacker@dojo:~$ whoami
hacker
hacker@dojo:~$

The task is to invoke the hello command to get the flag. Keep in mind that commands in Linux are case sensitive: hello is different from HELLO.

My solve
Flag: pwn.college{8c5BRCriZij6TUQGVZPF3mo9M3X.QX3YjM1wCN5kjNzEzW}
For this challenge, I simply needed to execute the hello command as instructed. Since this was my first introduction to Linux commands, I understood that I needed to type the command exactly as specified and press Enter.

hacker@dojo:~$ hello
Success! Here is your flag:
pwn.college{8c5BRCriZij6TUQGVZPF3mo9M3X.QX3YjM1wCN5kjNzEzW}

The solution was straightforward - just typing hello and hitting Enter executed the command, which then displayed the success message and the flag.

What I learned
Through this challenge, I learned the fundamental concept of how Linux commands work:
1.Commands are executed by typing them in the terminal and pressing Enter
2.The shell processes the input and executes the corresponding program
3.Commands in Linux are case-sensitive, so exact spelling and capitalization matter
4.After a command completes, the shell returns to the prompt, ready for the next command

References
Did not use any references for this challenge.
