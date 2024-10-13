# Position yet elsewhere

1)Changed the directory to '/home'
2)Executed '/challenge/run' and found out the the required directory
3)The reuired directory was '/usr/share/doc/fontconfig'
4)Executed '/challenge/run'


```bash
hacker@paths~position-yet-elsewhere:~$ cd /home
hacker@paths~position-yet-elsewhere:/home$ /challenge/run
Incorrect...
You are not currently in the /usr/share/doc/fontconfig directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:/home$ cd /usr/share/doc/fontconfig
hacker@paths~position-yet-elsewhere:/usr/share/doc/fontconfig$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{EqnKAR-SbDtwiCbuZhxBA8qZEt1.dhDN1QDL0czM2czW}
```

The resources used were
1)Ubuntu 22.04.5 LTS
2)pwn.college
