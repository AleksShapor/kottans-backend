# GIT
As a person, who has never worked with a version control systems, I want to say that this is a powerful tool that allows you to manage the project completely and track all of its changes.
It is quite simple and flexible, I liked the fact that the training materials were made up for practice.  Thanks for the collection)
## Unix Shell
https://github.com/AleksShapor/kottans-backend/blob/master/1.png?raw=true
It was very difficult to give material about Linux, in fact, I think there is little practice on real tasks. And so it will be necessary to re-read a couple more times to fully understand how everything works
## Git Collaboration
https://github.com/AleksShapor/kottans-backend/blob/master/2.png?raw=true
It’s already like the sport of “repetition of mother teaching”
## Python Basics 1
https://www.hackerrank.com/aleksshapor?hr_r=1
## Memory Management
What's going to happen if program reaches maximum limit of stack ?
If the maximum stack size has been reached, we have a stack overflow and the program receives a Segmentation Fault.
What's going to happen if program requests a big (more then 128KB) memory allocation on heap ?
In Linux, if you request a large block of memory via malloc(), the C library will create such an anonymous mapping instead of using heap memory.
What's the difference between Text and Data memory segments ?
The string lives in the text segment, which is read-only and stores all of your code in addition to tidbits like string literals.
The data segment, on the other hand, holds the contents for static variables initialized in source code.
So, the difference between Text and Data memory segments is that the Text segments you can only read and in Data memory segments you can read and write for saving static variables.
```
00400000-004de000 r-xp 00000000 fd:00 50332975                           /usr/bin/bash
006dd000-006de000 r--p 000dd000 fd:00 50332975                           /usr/bin/bash
006de000-006e7000 rw-p 000de000 fd:00 50332975                           /usr/bin/bash
006e7000-006ed000 rw-p 00000000 00:00 0
01ddf000-01e21000 rw-p 00000000 00:00 0                                  [heap]
7f6d1f5ec000-7f6d1f5f8000 r-xp 00000000 fd:00 18295                      /usr/lib64/libnss_files-2.17.so
7f6d1f5f8000-7f6d1f7f7000 ---p 0000c000 fd:00 18295                      /usr/lib64/libnss_files-2.17.so
7f6d1f7f7000-7f6d1f7f8000 r--p 0000b000 fd:00 18295                      /usr/lib64/libnss_files-2.17.so
7f6d1f7f8000-7f6d1f7f9000 rw-p 0000c000 fd:00 18295                      /usr/lib64/libnss_files-2.17.so
7f6d1f7f9000-7f6d1f7ff000 rw-p 00000000 00:00 0
7f6d1f7ff000-7f6d25d29000 r--p 00000000 fd:00 50332970                   /usr/lib/locale/locale-archive
7f6d25d29000-7f6d25eec000 r-xp 00000000 fd:00 18277                      /usr/lib64/libc-2.17.so
7f6d25eec000-7f6d260ec000 ---p 001c3000 fd:00 18277                      /usr/lib64/libc-2.17.so
7f6d260ec000-7f6d260f0000 r--p 001c3000 fd:00 18277                      /usr/lib64/libc-2.17.so
7f6d260f0000-7f6d260f2000 rw-p 001c7000 fd:00 18277                      /usr/lib64/libc-2.17.so
7f6d260f2000-7f6d260f7000 rw-p 00000000 00:00 0
7f6d260f7000-7f6d260f9000 r-xp 00000000 fd:00 18283                      /usr/lib64/libdl-2.17.so
7f6d260f9000-7f6d262f9000 ---p 00002000 fd:00 18283                      /usr/lib64/libdl-2.17.so
7f6d262f9000-7f6d262fa000 r--p 00002000 fd:00 18283                      /usr/lib64/libdl-2.17.so
7f6d262fa000-7f6d262fb000 rw-p 00003000 fd:00 18283                      /usr/lib64/libdl-2.17.so
7f6d262fb000-7f6d26320000 r-xp 00000000 fd:00 18360                      /usr/lib64/libtinfo.so.5.9
7f6d26320000-7f6d26520000 ---p 00025000 fd:00 18360                      /usr/lib64/libtinfo.so.5.9
7f6d26520000-7f6d26524000 r--p 00025000 fd:00 18360                      /usr/lib64/libtinfo.so.5.9
7f6d26524000-7f6d26525000 rw-p 00029000 fd:00 18360                      /usr/lib64/libtinfo.so.5.9
7f6d26525000-7f6d26547000 r-xp 00000000 fd:00 18270                      /usr/lib64/ld-2.17.so
7f6d26736000-7f6d2673d000 r--s 00000000 fd:00 16815209                   /usr/lib64/gconv/gconv-modules.cache
7f6d2673d000-7f6d26740000 rw-p 00000000 00:00 0
7f6d26743000-7f6d26746000 rw-p 00000000 00:00 0
7f6d26746000-7f6d26747000 r--p 00021000 fd:00 18270                      /usr/lib64/ld-2.17.so
7f6d26747000-7f6d26748000 rw-p 00022000 fd:00 18270                      /usr/lib64/ld-2.17.so
7f6d26748000-7f6d26749000 rw-p 00000000 00:00 0
7ffe2e4ac000-7ffe2e4cd000 rw-p 00000000 00:00 0                          [stack]
7ffe2e50c000-7ffe2e50e000 r-xp 00000000 00:00 0                          [vdso]
ffffffffff600000-ffffffffff601000 r-xp 00000000 00:00 0                  [vsyscall]
```
Heap - 01ddf000-01e21000
Stack - 7ffe2e4ac000-7ffe2e4cd000
Memory Mapping Segment - 7f6d1f5ec000-7f6d1f5f8000

It was not easy, the most difficult thing for me was to get the output from the / proc command and put it on my repository, since it was impossible (CentOS) through a virtual machine, and I couldn’t connect to the server remotely because it itself was disconnected from the network. 
And about the materials, nothing is clear, but very interesting!
