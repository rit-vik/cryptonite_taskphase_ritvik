# Position thy self

1)Using the '~' command figured out the current directory
2)Changed the directory to home by using 'cd /home'
3)Executed the '/challenge/run' command

```bash
hacker@paths~position-thy-self:~$ ~
ssh-entrypoint: /home/hacker: Is a directory
hacker@paths~position-thy-self:~$ cd /home
hacker@paths~position-thy-self:/home$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{A9UVBwvsoi3QXKzYfIeVh1JjFKT.dZDN1QDL0czM2czW}
hacker@paths~position-thy-self:/home$
```

The resources used were
1)Ubuntu 22.04.5 LTS
2)pwn.college
3)SSH key
