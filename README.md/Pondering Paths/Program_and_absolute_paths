Challenge 2: Program and Absolute Paths

What the challenge asks

This challenge is bit more complicated than the previous one. Instead of having the program directly in root directory like before, now the challenge program is inside a challenge directory. This challenge directory is located in the root /, so its path becomes /challenge.
The program I need to run is called run and it's sitting inside this /challenge directory. So the complete absolute path to reach this program is /challenge/run.
My task is simple - execute this run program using its full absolute path /challenge/run and get the flag!

My solve
Flag: pwn.college{g9jCr6-sePMEbDF7I4SSHrU5bJd.QX1QTN0wCN5kjNzEzW}
This challenge was building upon the previous one but with a slightly more complex path structure. Instead of just /pwn, now I had to navigate to /challenge/run.
I understood that the program run is located inside /challenge/ directory. The complete absolute path becomes /challenge/run. I directly executed this path from my home directory.

hacker@paths~program-and-absolute-paths:~$ /challenge/run
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{g9jCr6-sePMEbDF7I4SSHrU5bJd.QX1QTN0wCN5kjNzEzW}

What I learned
Nested Absolute Paths: Absolute paths can have multiple levels like /challenge/run. Each / separates directory levels, making it easy to understand the hierarchy.
Path Construction: To build absolute paths, I start from root /, then add each directory separated by /, and finally the program name. So / + challenge + / + run = /challenge/run.
Execution from Anywhere: The beauty of absolute paths is that I can execute any program from any location in the filesystem without changing directories first.

References
Did not use any external references for this challenge.
