Challenge 11: An Epic Filesystem Quest

What the challenge asks
A treasure hunt using cd, ls, and cat commands! Follow clues from file to file across the filesystem to find the final flag. Each clue gives location of next clue with special instructions.

My solve
Flag: pwn.college{Ysi3fCN5esAWaYvJ8Y_nT8AahRN.QX5IDO0wCN5kjNzEzW}


'''bash
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls -a
.           POINTER  challenge  flag  lib32   media  opt   run   sys  var
..          bin      dev        home  lib64   mnt    proc  sbin  tmp
.dockerenv  boot     etc        lib   libx32  nix    root  srv   usr
hacker@commands~an-epic-filesystem-quest:/$ cat POINTER
Lucky listing!
The next clue is in: /var/lib/emacsen-common

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/$ cd  /var/lib/emacsen-common
hacker@commands~an-epic-filesystem-quest:/var/lib/emacsen-common$ ls -a
.  ..  .INSIGHT  state
hacker@commands~an-epic-filesystem-quest:/var/lib/emacsen-common$ cat .INSIGHT
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/tools/arch/xtensa/include/uapi/asm
hacker@commands~an-epic-filesystem-quest:/var/lib/emacsen-common$ cd  /opt/linux/linux-5.4/tools/arch/xtensa/include/uapi/asm
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/tools/arch/xtensa/include/uapi/asm$ ls -a
.  ..  MESSAGE  mman.h
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/tools/arch/xtensa/include/uapi/asm$ cat MESSAGE
Tubular find!
The next clue is in: /usr/lib/debug/.build-id/e9

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/tools/arch/xtensa/include/uapi/asm$ ls  /usr/lib/debug/.build-id/e9 -a
.  ..  6ac5a313c00fdc37ac7b68121d4716efa9c209.debug  REVELATION-TRAPPED
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/tools/arch/xtensa/include/uapi/asm$ cat /usr/lib/debug/.build-id/e9/REVELATION-TRAPPED
Tubular find!
The next clue is in: /usr/local/lib/python3.8/dist-packages/networkx/algorithms/community/__pycache__

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/tools/arch/xtensa/include/uapi/asm$ cd  /usr/local/lib/python3.8/dist-packages/networkx/algorithms/community/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/networkx/algorithms/community/__pycache__$ ls -a
.                               kclique.cpython-38.pyc
..                              kernighan_lin.cpython-38.pyc
BLUEPRINT                       label_propagation.cpython-38.pyc
__init__.cpython-38.pyc         louvain.cpython-38.pyc
asyn_fluid.cpython-38.pyc       lukes.cpython-38.pyc
centrality.cpython-38.pyc       modularity_max.cpython-38.pyc
community_utils.cpython-38.pyc  quality.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/networkx/algorithms/community/__pycache__$ cat BLUEPRINT
Lucky listing!
The next clue is in: /usr/lib/debug/.build-id/31
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/networkx/algorithms/community/__pycache__$ cd /usr/lib/debug/.build-id/31
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/31$ ls -a
.
..
7a43bc138827d3f3c9abf8d9f29b7bfa8d9bcb.debug
DOSSIER
a57e90f254a40ff16b9aa0303e1557273b7df2.debug
ba4f94a99fb3d6698c7b40d4321e624fd5f000.debug
cc6a45fd0b5ab40c41775b0a4ce8d1ae150cfb.debug
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/31$ cat DOSSIER
Tubular find!
The next clue is in: /etc/apache2/sites-available
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/31$ cd /etc/apache2/sites-available
hacker@commands~an-epic-filesystem-quest:/etc/apache2/sites-available$ ls -a
.  ..  000-default.conf  README  default-ssl.conf
hacker@commands~an-epic-filesystem-quest:/etc/apache2/sites-available$ cat README
Yahaha, you found me!
The next clue is in: /opt/busybox/busybox-1.33.2/include/config/feature/nslookup/long

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/etc/apache2/sites-available$ cd /opt/busybox/busybox-1.33.2/include/config/feature/nslookup/long
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/nslookup/long$ ls -a
.  ..  .TIP  options.h
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/nslookup/long$ cat .TIP
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/drivers/clk/ingenic

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/nslookup/long$ ls /opt/linux/linux-5.4/drivers/clk/ingenic -a
.        .built-in.a.cmd  built-in.a  jz4725b-cgu.c  jz4780-cgu.c  tcu.c
..       Kconfig          cgu.c       jz4740-cgu.c   pm.c
.NUGGET  Makefile         cgu.h       jz4770-cgu.c   pm.h
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/nslookup/long$ cat /opt/linux/linux-5.4/drivers/clk/ingenic/.NUGGET
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{Ysi3fCN5esAWaYvJ8Y_nT8AahRN.QX5IDO0wCN5kjNzEzW}
'''


What I learned
Filesystem exploration using combination of cd, ls -a, and cat
Different types of clues: hidden files (need ls -a), trapped files (use absolute paths), delayed files (need cd first)
Real-world application of all commands learned so far

References
Did not use any external references for this challenge.
