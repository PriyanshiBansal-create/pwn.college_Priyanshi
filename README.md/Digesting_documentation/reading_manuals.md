Challenge 3: Reading Manuals

What the challenge asks
Learn to use the man command to read manual pages for programs. Need to find a secret option for /challenge/challenge by reading its manual page that will print the flag.

My solve
Flag: pwn.college{missing-flag-from-incomplete-output}

Used man command to read the manual:

'''bash
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ /challenge/challenge --rnfnvk 091
'''

What I learned
man command displays manual pages for programs
Manual pages have standard sections: NAME, SYNOPSIS, DESCRIPTION, SEE ALSO
SYNOPSIS shows how to use the command with its arguments
Can navigate with arrow keys, PgUp/PgDn, and quit with 'q'
Manual pages are stored in /usr/share/man but accessed via man command
Need to use command names, not file paths with man

Key Manual Page Sections:

NAME: Command name and brief description
SYNOPSIS: Usage format showing optional [BRACKETS] and required arguments
DESCRIPTION: Detailed explanation of all options and behavior
SEE ALSO: Related commands and resources

References
Did not use any external references for this challenge.
