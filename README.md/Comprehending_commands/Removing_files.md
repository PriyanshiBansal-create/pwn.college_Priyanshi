Challenge 8: Removing Files

What the challenge asks
Learn the rm command to delete files. The challenge creates a delete_me file in home directory and I need to delete it, then run /challenge/check to verify deletion and get the flag.

My solve
Flag: pwn.college{M-WI6tYDyF-vH_8ZQ_ZBQrQhu6z.QX2kDM1wCN5kjNzEzW}

Tried two methods and both worked:

'''bash
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{M-WI6tYDyF-vH_8ZQ_ZBQrQhu6z.QX2kDM1wCN5kjNzEzW}
'''

'''bash
hacker@commands~removing-files:~$ rm ~/delete_me
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{M-WI6tYDyF-vH_8ZQ_ZBQrQhu6z.QX2kDM1wCN5kjNzEzW}
'''

What I learned
rm command permanently deletes files
Can use relative path (delete_me) or absolute path (~/delete_me)
Both methods work when file is in current directory

References
Did not use any external references for this challenge.
