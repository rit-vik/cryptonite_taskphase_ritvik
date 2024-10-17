# Linking Files

Hardlink is an alternate address that indexes the data.
Softlink contains the original file name, linux understands that this is a symbolic link and then access the file.
Both are same, just the mechanisms are different.
symlinks are created with ln command and -s as argument.

```bash
hacker@commands~linking-files:~$ rm ~/not-the-flag
hacker@commands~linking-files:~$ ln -sf /flag ~/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{4vYMGyyEl3usuM0q6NtC-xqo4X8.dlTM1UDL0czM2czW}
```

The resources used were
1)Ubuntu 22.04.5 LTS
2)pwn.college
