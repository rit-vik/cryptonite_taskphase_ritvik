# Intro to commands

1)Connected my LTS to hacker@pwncollege using command ssh -i key hacker@pwn.college
2)Used the command whoami to ensure it was connected
3)Then wrote the command 'hello' to find out the flag

```bash
  root@LAPTOP-MUVNNMSR:~# ssh -i key hacker@pwn.college
  Connected!
  hacker@hello~intro-to-commands:~$ whoami
  hacker
  hacker@hello~intro-to-commands:~$ hello
  Success! Here is your flag:
  pwn.college{M0YMQKycWlT7DsWRSmyYO2p7ySK.ddjNyUDL0czM2czW}
```

The resources used were
  1)Ubuntu 22.04.5 LTS
  2)pwn.college
  3)SSH Keys
