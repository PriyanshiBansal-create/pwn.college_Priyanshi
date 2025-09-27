Challenge 2: Learning Complex Usage

What the challenge asks
Some commands take arguments that themselves need arguments. The documentation explains that /challenge/challenge has a --printfile argument that takes a file path as its own argument to print that file's contents.

My solve
Flag: pwn.college{oRzQMIxdK2gRA0U5W6VOlTEJQgj.QX1ITO0wCN5kjNzEzW}

First tried without the required argument, then provided the correct path:

'''bash
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile 
You must pass a file for --printfile to read!
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile /flag
Correct argument! Here is the /flag file:
pwn.college{oRzQMIxdK2gRA0U5W6VOlTEJQgj.QX1ITO0wCN5kjNzEzW}
'''

What I learned
Some arguments require their own arguments (nested arguments)
Error messages help understand what's missing
Complex commands can have multiple levels of parameters


References
Did not use any external references for this challenge.
