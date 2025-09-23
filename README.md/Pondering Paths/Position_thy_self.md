Challenge 3: Position Thy Self

What the challenge asks

This challenge introduces the cd (change directory) command for navigating the filesystem. The cd command changes your current working directory by taking a path as an argument. This affects where your shell is currently "hanging out" in the filesystem.
The challenge requires me to execute /challenge/run from a specific directory. The program will tell me which directory I need to be in, then I need to cd to that directory before running the program again.

My solve
Flag: pwn.college{Us2NlNhvxwqY43LTskpGa7eBNaP.QX2QTN0wCN5kjNzEzW}
First, I ran the program to see what directory it wants me to be in:

hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /proc/138/fd directory.
Please use the `cd` utility to change directory appropriately.

Then I changed to the required directory and ran the program again:

hacker@paths~position-thy-self:~$ cd /proc/138/fd
hacker@paths~position-thy-self:/proc/138/fd$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{Us2NlNhvxwqY43LTskpGa7eBNaP.QX2QTN0wCN5kjNzEzW}

What I learned

1.The cd command changes my current working directory
2.Programs can check which directory they're being run from
3.The shell prompt shows my current location (notice how it changed from ~ to /proc/138/fd )

References
Did not use any external references for this challenge.
