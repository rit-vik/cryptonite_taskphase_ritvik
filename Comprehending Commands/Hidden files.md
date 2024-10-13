# Hidden files

1)Changed directory to '/'
2)Used 'ls -a' to retrieve hidden files
3)Used 'cat' to read the flag file

```bash
hacker@commands~hidden-files:/$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv            bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-19742119827958  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-19742119827958
pwn.college{AOTAWD4Jofyp3eqWkHKkmeXHaWK.dBTN4QDL0czM2czW}
```

The resources used were
1)Ubuntu 22.04.5 LTS
2)pwn.college
