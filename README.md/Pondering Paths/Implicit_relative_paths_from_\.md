Challenge 6: Implicit Relative Paths, From /

What the challenge asks

This challenge introduces relative paths - paths that don't start with /. Relative paths depend on your current working directory (cwd). For example, if I want to access /tmp/a/b/my_file:
From /: relative path is tmp/a/b/my_file
From /tmp: relative path is a/b/my_file
I need to run /challenge/run using a relative path while being in / directory. Hint: the relative path starts with c.

My solve
Flag: pwn.college{UW37mfWa6aMLRr7zyYeMh72Uv8c.QX5QTN0wCN5kjNzEzW}
Since /challenge/run is the absolute path and I need to be in /, the relative path from root would be challenge/run (removing the leading /).

''' bash
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{UW37mfWa6aMLRr7zyYeMh72Uv8c.QX5QTN0wCN5kjNzEzW}
'''

What I learned

1.Relative paths don't start with /
2.They depend on current working directory


References
Did not use any external references for this challenge.
