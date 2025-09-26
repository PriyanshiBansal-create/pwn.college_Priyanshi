Challenge 10: Hidden Files

What the challenge asks
Learn about hidden files that start with . and use ls -a to view them. Need to find a hidden flag file in root directory /.

My solve
Flag: pwn.college{EDx5e1hOEf6p2NBNZq5JXRAHvMH.QXwUDO0wCN5kjNzEzW}

First method (navigating to root first):

'''bash
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.                    bin        etc    lib64   nix   run   tmp
..                   boot       home   libx32  opt   sbin  usr
.dockerenv           challenge  lib    media   proc  srv   var
.flag-2263272102935  dev        lib32  mnt     root  sys
hacker@commands~hidden-files:/$ cat .flag-2263272102935
pwn.college{EDx5e1hOEf6p2NBNZq5JXRAHvMH.QXwUDO0wCN5kjNzEzW}
'''

Second method (using absolute paths):
'''bash
hacker@commands~hidden-files:~$ ls / -a
.                     bin        etc    lib64   nix   run   tmp
..                    boot       home   libx32  opt   sbin  usr
.dockerenv            challenge  lib    media   proc  srv   var
.flag-92412907814990  dev        lib32  mnt     root  sys
hacker@commands~hidden-files:~$ cat /.flag-92412907814990
pwn.college{EDx5e1hOEf6p2NBNZq5JXRAHvMH.QXwUDO0wCN5kjNzEzW}
'''

What I learned
Files starting with . are hidden by default
ls -a shows all files including hidden ones
Must use absolute path when reading hidden files from different directory

References
Did not use any external references for this challenge.
