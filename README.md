Systemtap scripts
=================

page_faults_file.stp
--------------------

Print out pathes to mmap files, that cause major page faults.

Useful in cases when you're looking for files for warm up in a memory before start
(eg mongodb files, kioto cabinet, homebrew data base).

Using with custom command:
```
stap ./page_faults_file.stp -c 'firefox'
```
using with running app with PID:
```
stap ./page_faults_file.stp -x 2412
```
