Challenge 9: Home Sweet Home

What the challenge asks
This challenge teaches about home directory and the ~ shorthand. The ~ symbol represents my home directory /home/hacker. The /challenge/run program will write the flag to a file I specify, but with constraints:
1 Must be absolute path
2 Must be inside home directory
3 Must be 3 characters or less before expansion
I need to provide this path as an argument to /challenge/run.

My solve
flag:pwn.college{wuJwqMV4wjYkcNr_9oCZs-mOvg5.QXzMDO0wCN5kjNzEzW}
The trick is using ~ which is only 1 character but expands to /home/hacker. I can add a filename to make it ~/f:

'''bash
hacker@paths~home-sweet-home:~$ /challenge/run ~/f
Writing the file to /home/hacker/f!
... and reading it back to you:
pwn.college{wuJwqMV4wjYkcNr_9oCZs-mOvg5.QXzMDO0wCN5kjNzEzW}
'''

What I learned

1 ~ is shorthand for home directory /home/hacker
2 ~ expands to absolute path even though it's just 1 character
3 Can use ~/filename to create files in home directory

References
Did not use any external references for this challenge.
