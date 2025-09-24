Challenge 5: Comparing Files

What the challenge asks
Learn diff command to compare files and find differences. Two files are given: one with 100 fake flags and another with 100 fake flags plus one real flag. I need to use diff to find what's different.

My solve
Flag: pwn.college{w2yM0kNs2lYjMjGic1lC_lWRDgN.01MwMDOxwCN5kjNzEzW}

Used diff to compare the two files:
'''bash
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
89a90
> pwn.college{w2yM0kNs2lYjMjGic1lC_lWRDgN.01MwMDOxwCN5kjNzEzW}
'''

What I learned
1 diff compares two files line by line
2 Shows exactly what's different between files
3 > symbol shows lines that exist in second file but not first


References
Did not use any external references for this challenge.
