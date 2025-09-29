Challenge 30: Help for Builtins

What the challenge asks
Some commands are shell builtins, not separate programs. They don't have man pages but can be looked up using the help builtin command. Need to use help challenge to find the secret value.

My solve
Flag: pwn.college{MtcuJJ86VVs8YNBG_Ac-ozlVfun.QX0ETO0wCN5kjNzEzW}

Used help command for builtin documentation:

'''bash
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!
    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct
    You must be sure to provide the right value to --secret. That value is "MtcuJJ86".

hacker@man~help-for-builtins:~$ challenge --secret MtcuJJ86
Correct! Here is your flag!
pwn.college{MtcuJJ86VVs8YNBG_Ac-ozlVfun.QX0ETO0wCN5kjNzEzW}
'''

What I learned
Builtins are commands handled by shell internally, not separate programs
Use help command to get documentation for builtins
help without arguments lists all available builtins
Builtins don't have man pages because they're part of shell itself
Examples include cd, help, and custom builtins like challenge

References
Did not use any external references for this challenge.
