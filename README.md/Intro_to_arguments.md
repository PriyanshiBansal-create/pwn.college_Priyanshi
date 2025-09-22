Challenge 2: Intro to Arguments

What the challenge asks
This challenge introduces the concept of command arguments - additional data passed to commands. When you type a line of text and hit Enter, the shell parses your input into a command and its arguments. The first word is the command, and subsequent words are arguments.
The challenge provides examples with the echo command:

hacker@dojo:~$ echo Hello
Hello
hacker@dojo:~$ echo Hello Hackers!
Hello Hackers!

The task is to run the hello command (NOT the echo command) with a single argument of hackers.

My solve
Flag: pwn.college{IQ6wyRJfjv_qMtgW-R_8nz90BVU.QX4YjM1wCN5kjNzEzW}

For this challenge, I needed to understand that command-line arguments are separated by spaces. The challenge specifically asked me to run the hello command with the argument hackers.

hacker@dojo:~$ hello hackers
Success! Here is your flag:
pwn.college{IQ6wyRJfjv_qMtgW-R_8nz90BVU.QX4YjM1wCN5kjNzEzW}

The key insight was understanding the syntax: command argument. So hello hackers means running the hello command with hackers as its single argument.

What I learned
Through this challenge, I learned about command arguments and how the shell parses input:
1.The shell splits command-line input into words separated by spaces
2.The first word is always the command name
3.All subsequent words are treated as arguments to that command

References
Did not use any references for this challenge.
