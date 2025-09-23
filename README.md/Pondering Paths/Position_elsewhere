Challenge 4: Position Elsewhere

What the challenge asks

Same concept as the previous challenge - I need to use cd to navigate to a specific directory before running /challenge/run. The program will tell me which directory I need to be in.

My solve
Flag: pwn.college{URG94sloXHhwruOlTLg2dAIQz7a.QX3QTN0wCN5kjNzEzW}
Following the same approach as before:

hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/doc/fontconfig directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /usr/share/doc/fontconfig
hacker@paths~position-elsewhere:/usr/share/doc/fontconfig$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{URG94sloXHhwruOlTLg2dAIQz7a.QX3QTN0wCN5kjNzEzW}

What I learned

Reinforced the concept of working directories. The pattern is consistent: run program then see error then cd to required directory then run again

References
Did not use any external references for this challenge.
