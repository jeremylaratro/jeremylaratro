jay@github:~$ gdb whoami

GNU gdb (Ubuntu 9.2-0ubuntu1~20.04) 9.2
Copyright (C) 2020 Free Software Foundation, Inc.
License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>
This is free software: you are free to change and redistribute it. There is NO WARRANTY, to the extent permitted by law.
Type "show copying" and "show warranty" for details.
This GDB was configured as "x86_64-linux-gnu".
Type "show configuration" for configuration details.
For bug reporting instructions, please see:
<http://www.gnu.org/software/gdb/bugs/>.
Find the GDB manual and other documentation resources online at:
    <http://www.gnu.org/software/gdb/documentation/>.

For help, type "help".
Type "apropos word" to search for commands related to "word"...

Reading symbols from whoami...

(gdb) break main
Breakpoint 1 at 0x114fd: file whoami.c, line 14.

(gdb) run
Starting program: /github.com/jeremylaratro/whoami 

Breakpoint 1, main () at whoami.c:14
14	  printf("Welcome to my Github...\n");

(gdb) x/s 0x400400
0x400400:       "penetration tester, security engineer, passionate breaker of all things technology - hardware and software\n"
0x4004a0:       "amateur radio enthusiast, hobbyist PCB designer, and gadget builder\n"
0x400540:       "scuba diver, soon to be private pilot, backpacker, and lover of all things travel\n"

(gdb) continue
Continuing.
Welcome to my Github...

Program exited normally.
(gdb) quit
