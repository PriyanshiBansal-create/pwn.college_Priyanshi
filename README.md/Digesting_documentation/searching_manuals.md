Challenge 4: Searching Manuals

What the challenge asks
Learn to search within manual pages to find specific information. The challenge explains that you can scroll with arrow keys, search with / (forward) or ? (backward), use n for next result and N for previous result. Need to find the option that gives the flag by reading the challenge man page.

My solve
Flag: pwn.college{IA_e-wkIwpYHB9Vvr99FtK7gY7h.QX1EDO0wCN5kjNzEzW}

Used search functionality in man page:

'''bash
hacker@man~searching-manuals:~$ man challenge
# Searched for "flag" using / inside the manual
hacker@man~searching-manuals:~$ /challenge/challenge --qh
Initializing...
Correct usage! Your flag: pwn.college{IA_e-wkIwpYHB9Vvr99FtK7gY7h.QX1EDO0wCN5kjNzEzW}
'''

What I learned
Can search inside manual pages using / followed by search term
Press n to go to next match, N for previous match

References
Did not use any external references for this challenge.
