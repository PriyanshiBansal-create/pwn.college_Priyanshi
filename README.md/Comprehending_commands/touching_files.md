Challenge 7: Touching Files

What the challenge asks
Learn touch command to create new empty files. I need to create two files /tmp/pwn and /tmp/college and then run /challenge/run to get the flag.

My solve
Flag: pwn.college{oAIMTR9LxSvPN6RWGEMD0NlWAA3.QXwMDO0wCN5kjNzEzW}

I tried three different methods and all worked:

Method 1: Using relative paths after cd
'''bash
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ touch pwn
hacker@commands~touching-files:/tmp$ touch college
hacker@commands~touching-files:/tmp$ /challenge/run
Success! Here is your flag:
pwn.college{oAIMTR9LxSvPN6RWGEMD0NlWAA3.QXwMDO0wCN5kjNzEzW}
'''

Method 2: Using absolute paths without cd
'''bash
hacker@commands~touching-files:~$ touch /tmp/pwn
hacker@commands~touching-files:~$ touch /tmp/college
hacker@commands~touching-files:~$ /challenge/run
Success! Here is your flag:
pwn.college{oAIMTR9LxSvPN6RWGEMD0NlWAA3.QXwMDO0wCN5kjNzEzW}
'''

Method 3: Mixed approach (cd first, then absolute paths)
'''bash
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ touch /tmp/pwn
hacker@commands~touching-files:/tmp$ touch /tmp/college
hacker@commands~touching-files:/tmp$ /challenge/run
Success! Here is your flag:
pwn.college{oAIMTR9LxSvPN6RWGEMD0NlWAA3.QXwMDO0wCN5kjNzEzW}
'''

What I learned
1 touch command creates new empty files
2 Multiple ways to achieve same result: Can use relative paths after navigating or absolute paths from anywhere
3 Flexibility: Even if I'm already in the target directory, I can still use absolute paths (Method 3)
4 Efficiency: Method 2 is most efficient as it doesn't require changing directories first

References
Did not use any external references for this challenge.
