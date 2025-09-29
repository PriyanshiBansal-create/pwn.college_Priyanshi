Challenge 5: Searching for Manuals
What the challenge asks
The manpage for the challenge is hidden with a random name. Need to search the man page database to find it. The hint says to read man man to learn how to search for manpages. Even though the manpage has a random name, still use /challenge/challenge to get the flag.

My solve
Flag: pwn.college{4yj8virC-lD3y2aSG8hzvN6-6o9.QX2EDO0wCN5kjNzEzW}
First read man page for man command, then searched for flag-related manpages:
'''bash
hacker@man~searching-for-manuals:~$ man man
# Learned about -k option to search man pages

hacker@man~searching-for-manuals:~$ man -k flag
# Got list of all manpages related to "flag"
# Found: yjvirlyahz (1)  - print the flag!

hacker@man~searching-for-manuals:~$ man yjvirlyahz
# Read the manual to find the secret option

hacker@man~searching-for-manuals:~$ /challenge/challenge --yjvirl 483
Correct usage! Your flag: pwn.college{4yj8virC-lD3y2aSG8hzvN6-6o9.QX2EDO0wCN5kjNzEzW}
'''

What I learned
man -k keyword searches the man page database for keyword
Useful when you don't know exact command name
Man pages have descriptions that can be searched
Even if manpage name is random, the actual command stays the same

References
Did not use any external references for this challenge.
