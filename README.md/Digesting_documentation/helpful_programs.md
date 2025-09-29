Challenge 6: Helpful Programs

What the challenge asks
Some programs don't have man pages but provide help through special arguments like --help, -h, or -?. Need to use --help to read the program's documentation.

My solve
Flag: pwn.college{MNKmEaFo3T7FVyvWdWcBiXsVZ6q.QX3IDO0wCN5kjNzEzW}
Used --help to understand options, then followed the instructions:
'''bash
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h]
                                            [--fortune]
                                            [-v]
                                            [-g GIVE_THE_FLAG]
                                            [-p]
optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag

hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 376

hacker@man~helpful-programs:~$ /challenge/challenge -g 376
Correct usage! Your flag: pwn.college{MNKmEaFo3T7FVyvWdWcBiXsVZ6q.QX3IDO0wCN5kjNzEzW}
'''

What I learned
--help option shows program usage information
Alternative to man pages for documentation
Help output shows all available options and their descriptions
Can chain commands - first get secret value, then use it

References
Did not use any external references for this challenge.
