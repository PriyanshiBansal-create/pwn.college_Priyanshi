Challenge 8: Implicit Relative Paths

What the challenge asks
I need to run the program from inside /challenge directory, but there's a catch! Linux doesn't automatically look in current directory when I type just run. This is for safety - so I don't accidentally run programs with same names as system commands. I need to explicitly tell Linux to run the program from current directory using . notation.


My solve
Flag: pwn.college{Ug9Na-N3GLEgqOIiJWGzHMBNn9j.QXxUTN0wCN5kjNzEzW}

First I changed to /challenge directory, then used ./run to explicitly run the program from current directory:

'''bash
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{Ug9Na-N3GLEgqOIiJWGzHMBNn9j.QXxUTN0wCN5kjNzEzW}
'''

What I learned
1 Can't just type run even when inside /challenge directory
2 Must use ./run to tell Linux to look in current directory
3 This prevents accidentally running wrong programs with same names

References
Did not use any external references for this challenge.
