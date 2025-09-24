Challenge 3: More Catting Practice

What the challenge asks
The flag is hidden in some random directory and I cannot use cd command. I must retrieve the flag using absolute path only. The system tells me where the flag is located.

My solve
Flag: pwn.college{kT3Wg-WZ63P5GKzJ8cMa2f8YMwX.QXwITO0wCN5kjNzEzW}

The system told me the flag is in /lib/ssl/misc/flag:
'''bash
hacker@commands~more-catting-practice:~$ cat /lib/ssl/misc/flag
pwn.college{kT3Wg-WZ63P5GKzJ8cMa2f8YMwX.QXwITO0wCN5kjNzEzW}
'''

What I learned
cd command restrictions can be bypassed using absolute paths
Files can be accessed from anywhere using their complete path


References
Did not use any external references for this challenge.
