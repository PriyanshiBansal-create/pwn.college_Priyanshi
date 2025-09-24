Challenge 1: Cat: Not the Pet, But the Command!

What the challenge asks
Learn about the cat command which is used to read files. The command can concatenate multiple files if given multiple arguments. The challenge will copy the flag to a flag file in my home directory, and I need to read it using cat.

My solve
Flag: pwn.college{QXQStdwCDwpH_ZHME0i1Y8SyOlT.QXxcTN0wCN5kjNzEzW}

I tried different ways to read the flag file and all worked:

'''bash
hacker@commands~cat-not-the-pet-but-the-command:~$ cat ./flag
pwn.college{QXQStdwCDwpH_ZHME0i1Y8SyOlT.QXxcTN0wCN5kjNzEzW}
hacker@commands~cat-not-the-pet-but-the-command:~$ cat /flag
pwn.college{QXQStdwCDwpH_ZHME0i1Y8SyOlT.QXxcTN0wCN5kjNzEzW}
hacker@commands~cat-not-the-pet-but-the-command:~$ cat ~/flag
pwn.college{QXQStdwCDwpH_ZHME0i1Y8SyOlT.QXxcTN0wCN5kjNzEzW}
'''

What I learned
1.cat command reads and displays file contents
2.Can use different path notations (relative, absolute, home shortcut)
3.cat can concatenate multiple files when given multiple arguments

References
Did not use any external references for this challenge.
