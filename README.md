jay@github:~$ gdb whoami

GNU gdb (Ubuntu 9.2-0ubuntu1~20.04) 9.2 \
Copyright (C) 2020 Free Software Foundation, Inc. \
For help, type "help". \
Type "apropos word" to search for commands related to "word"... 

Reading symbols from whoami...

(gdb) break main \
Breakpoint 1 at 0x114fd: file whoami.c, line 14.

(gdb) run \
Starting program: /github.com/jeremylaratro/whoami 

Breakpoint 1, main () at whoami.c:14 \
14	  printf("Welcome to my Github...\n");

(gdb) x/s 0x400400 \
0x400400:       "**penetration tester, security engineer, passionate breaker of all things technology - hardware and software**\n" \
0x4004a0:       "**amateur radio enthusiast, hobbyist PCB designer, and gadget builder**\n" \
0x400540:       "**scuba diver, soon to be private pilot, backpacker, and lover of all things travel**\n"

(gdb) continue \
Continuing. \
Welcome to my Github...

Program exited normally. \
(gdb) quit
