# Reading manuals

Learnt about 'man' command which gives manual about a specific command

```bash
hacker@man~reading-manuals:~$ man challenge

CHALLENGE(1)                        Challenge Commands                        CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --odrhvk NUM
              print the flag if NUM is 454

AUTHOR
       Written by Zardus.
hacker@man~reading-manuals:~$ /challenge/challenge --odrhvk 454
Correct usage! Your flag: pwn.college{oGdrh4WRNMvYHkyPsneugT5IApY.dRTM4QDL0czM2czW}
```

The resources used were
1)Ubuntu 22.04.5 LTS
2)pwn.college
