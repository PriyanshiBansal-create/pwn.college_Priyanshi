Challenge 12: Making Directories

What the challenge asks
Learn the mkdir command to create directories. Need to create a /tmp/pwn directory and make a college file inside it. Then run /challenge/run to check the solution and get the flag.

My solve
Flag: pwn.college{kRoOLiDtxB32_PDTr2544Djh5yQ.QXxMDO0wCN5kjNzEzW}

Created directory and file step by step:

'''bash
hacker@commands~making-directories:~$ mkdir /tmp/pwn
hacker@commands~making-directories:~$ cd /tmp/pwn
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ /challenge/run
Success! Here is your flag:
pwn.college{kRoOLiDtxB32_PDTr2544Djh5yQ.QXxMDO0wCN5kjNzEzW}
'''

What I learned
mkdir command creates new directories
Can create directories using absolute paths
After creating directory, can navigate into it with cd


References
Did not use any external references for this challenge.
