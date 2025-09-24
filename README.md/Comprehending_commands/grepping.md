Challenge 4: Grepping for a Needle in a Haystack

What the challenge asks

Learn grep command to search for specific text in large files. The challenge has put 100,000 lines in /challenge/data.txt and I need to grep for the flag. Hint: flag starts with pwn.college.

My solve
Flag: pwn.college{cO2kKnUAWqIon1y_HpygHl_ud3N.QX3EDO0wCN5kjNzEzW}

Used grep to search for the flag pattern:

'''bash
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn.college /challenge/data.txt
pwn.college{cO2kKnUAWqIon1y_HpygHl_ud3N.QX3EDO0wCN5kjNzEzW}
'''

What I learned
grep searches for specific text patterns in files
Very useful for finding content in large files instead of reading everything
Syntax: grep SEARCH_STRING /path/to/file

References
Did not use any external references for this challenge.
