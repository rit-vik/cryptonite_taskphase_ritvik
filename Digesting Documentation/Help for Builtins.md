# Help for Builtins

Used help command with challenge as argument and found out the flag

```bash
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "U6V1pz4x".
hacker@man~help-for-builtins:~$ challenge --secret U6V1pz4x
Correct! Here is your flag!
pwn.college{U6V1pz4x_GSvrH7AI7bJvCFzEU0.dRTM5QDL0czM2czW}
```

The resources used were
1)Ubuntu 22.04.5 LTS
2)pwn.college
