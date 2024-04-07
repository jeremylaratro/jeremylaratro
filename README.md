jay@github:~$ gdb whoami

GNU gdb (Ubuntu 9.2-0ubuntu1~20.04) 9.2 \
Copyright (C) 2020 Free Software Foundation, Inc. \
For help, type "help". \
Type "apropos word" to search for commands related to "word"... 

Reading symbols from whoami...

(gdb) break main \
Breakpoint 1 at 0x77656C636f6d65: file whoami.c, line 14.

(gdb) run \
Starting program: /github.com/jeremylaratro/whoami 

Breakpoint 1, main () at whoami.c:14 \
14	  printf("Welcome to my Github...\n");

(gdb) x/s 0x70776e212121 \
0x7468616e6b73:     "**Offensive security engineer and passionate breaker of all things hardware and software**\n" \
0x666f72:           "**CTFs, amateur radio, PCB design, and building electronics**\n" \
0x7669736974696e67: "**Travel, SCUBA, backpacking and camping, and aviation.**\n"

(gdb) continue \
Continuing. \
Welcome to my Github...

Program exited normally. \
(gdb) quit
