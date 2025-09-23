Challenge 5: Position Yet Elsewhere

What the challenge asks

Same concept as previous two challenges - find out which directory the program wants me to be in, navigate there, and run the program.

My solve
Flag: pwn.college{YYTQzKrvuyOHD5EdlzRsnnpd66u.QX4QTN0wCN5kjNzEzW}
Same workflow as previous challenges:

hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /etc directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /etc
hacker@paths~position-yet-elsewhere:/etc$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{YYTQzKrvuyOHD5EdlzRsnnpd66u.QX4QTN0wCN5kjNzEzW}

What I learned
Got comfortable with the cd command and directory navigation

References
Did not use any external references for this challenge.
