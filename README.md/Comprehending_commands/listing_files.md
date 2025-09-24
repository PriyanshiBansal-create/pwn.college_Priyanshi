Challenge 6: Listing Files

What the challenge asks
Learn ls command to list directory contents. The challenge renamed /challenge/run to some random name and I need to use ls to find the actual filename.

My solve
Flag: pwn.college{45gi0oVRsIWR8ov5cNkwfc8SzCE.QX4IDO0wCN5kjNzEzW}

First listed the directory contents, then ran the file:
'''bash
hacker@commands~listing-files:~$ ls /challenge
18295-renamed-run-669  DESCRIPTION.md
hacker@commands~listing-files:~$ /challenge/18295-renamed-run-669
Yahaha, you found me! Here is your flag:
pwn.college{45gi0oVRsIWR8ov5cNkwfc8SzCE.QX4IDO0wCN5kjNzEzW}
'''

What I learned
ls lists files and directories in specified path
If no path given, lists current directory contents

References
Did not use any external references for this challenge.
