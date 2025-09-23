Challenge 1: The Root 

What the challenge asks
The filesystem starts at / which is called root directory. Under this root, there are many other directories, configuration files, programs, and most importantly flags! In this level, they have added a program directly in / called pwn that will give us the flag.
To complete this challenge, I need to invoke this program by providing its path on the command line. Since I have to give the exact path starting from /, the complete path would be /pwn. This type of path that starts with the root directory is called an "absolute path".
My task is simple - start the challenge, launch terminal, invoke the pwn program using its absolute path, and capture that flag!

My solve
Flag: pwn.college{AUXPNqmDw2lhq-_ITxiIxx4_uPr.QX4cTO0wCN5kjNzEzW}
Initially I was bit confused about where exactly this pwn program is located, but after reading the challenge description carefully, I understood that it's placed directly in the root directory /. So I need to use the absolute path /pwn to run it.
First I opened the terminal ,I was already in my home directory as shown by the prompt. Instead of navigating anywhere, I directly typed the absolute path of the program . Executed the command and boom! Got the flag

hacker@paths~the-root:~$ /pwn
BOOM!!!
Here is your flag:
pwn.college{AUXPNqmDw2lhq-_ITxiIxx4_uPr.QX4cTO0wCN5kjNzEzW}

What I learned
This challenge taught me several important concepts about Linux filesystem:
Filesystem Structure: The entire Linux filesystem is like a tree structure starting from root /. Everything - files, directories, programs - everything lives under this root directory.
Absolute vs Relative Paths: Absolute path starts with / and gives complete location from root (like /pwn)
                            Relative path starts from current directory (like ./file or just filename)
Program Execution: You can run any program by giving its full path, no matter where you currently are in the filesystem
Root Directory: The / is the topmost directory in Linux. It's like C: drive in Windows but much more organized.

References
Did not use any external references for this challenge, solved it by understanding the challenge description properly.
