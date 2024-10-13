# Position elsewhere

1)Changed the directory to '/home' and executed the command '/challenge/run'
2)It provided the the directory as '/proc/67'
3)Changed the directory with 'cd /proc/67'
4) Executed '/challenge/run'


```bash
hacker@paths~position-elsewhere:~$ cd /home
hacker@paths~position-elsewhere:/home$ /challenge/run
Incorrect...
You are not currently in the /proc/67 directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:/home$ cd /proc/67
hacker@paths~position-elsewhere:/proc/67$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{sZ3U3P-kiT-i8YNJGS697xadorh.ddDN1QDL0czM2czW}
```

The resources used were
1)Ubuntu 22.04.5 LTS
2)pwn.college
