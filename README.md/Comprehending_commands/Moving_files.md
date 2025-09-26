Challenge 9: Moving Files

What the challenge asks
Learn the mv command to move files. Need to move the /flag file to /tmp/hack-the-planet location, then run /challenge/check to verify and get the flag.

My solve
Flag: pwn.college{ISytJ8GrOON5DlUapzHmu84X-IK.0VOxEzNxwCN5kjNzEzW}

Simple move operation:

'''bash
hacker@commands~moving-files:~$ mv /flag /tmp/hack-the-planet
Correct! Performing 'mv /flag /tmp/hack-the-planet'.
hacker@commands~moving-files:~$ /challenge/check
Congrats! You successfully moved the flag to /tmp/hack-the-planet! Here it is:
pwn.college{ISytJ8GrOON5DlUapzHmu84X-IK.0VOxEzNxwCN5kjNzEzW}
'''

What I learned
mv command moves
Syntax: mv source destination
File gets moved from original location to new location

References
Did not use any external references for this challenge.
