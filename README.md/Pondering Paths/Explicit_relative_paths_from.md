Challenge 7: Explicit Relative Paths, From /

What the challenge asks
This time I need to use explicit relative paths with . notation. The . refers to the current directory, so challenge and ./challenge are the same thing. The challenge wants me to use . in my relative path instead of just typing the "naked" path.

My solve
Flag: pwn.college{AJufmEh1InqcaUVXLBdxYc1Tw5N.QXwUTN0wCN5kjNzEzW}
I need to be in root directory and use ./challenge/run instead of just challenge/run.

'''bash
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{AJufmEh1InqcaUVXLBdxYc1Tw5N.QXwUTN0wCN5kjNzEzW}
'''

What I learned
1 . means current directory
2 Both are same but using ./ makes it clear I'm starting from current directory

References
Did not use any external references for this challenge.
