# 0x16.C Simple Shell
**Background Context**

- Writing a simple UNIX command interpreter.

## General Requirements

* Allowed editors:``` vi```, ```vim```, ```emacs```
* All your files will be compiled on```Ubuntu 20.04 LTS``` using ```gcc```, using the options ```-Wall -Werror -Wextra -pedantic -std=gnu89```
* All your files should end with a new line
* A ```README.md``` file, at the root of the folder of the project is mandatory
* Your code should use the Betty style. It will be checked using ```betty-style.pl``` and ```betty-doc.pl```
* Your shell should not have any memory leaks
* No more than ```5``` functions per file
* All your header files should be include guarded
* Use system calls only when you need to (why?)
***Usage***
#### In order to run this program,

``git clone https://github.com/Susiniosgit/simple_shell``

#### compile it with

``gcc 4.8.4 -Wall -Werror -Wextra -pedantic *.c -o hsh.``

### How to use it
#### In order to use this shell, in a terminal, first run the program:
``prompt$ ./hsh``
#### It wil then display a simple prompt and wait for commands.
``$``
**List of built-ins**
#### Currently the list of built-ins I wrote is:
- cd [directory]
#### Switch to the specified directory (path).
- env
#### Displays the environment variable
- exit [exitstatus]
#### Exit from the program with exitstatus value. 0 by default.
- getenv NAME
#### Return the value of the NAME variable if it is in the environment
- help [command]
#### Displays the syntax for the command, or all commands.
- history
#### Displays the last typed user.
- echo [$$] or [$?] or [$PATH] Return pid and exit statue and PATH.
**Command**
Basicly Every Program in $PATH It Support Single Word like ls

- It Handle Path ls /tmp
- it Handle Options Like ls -l
- it Handle All Three Togther Like ls -l /var
- it Handle Command Path Also Like /bin/ls And All The Option And Path Like /bin/ls -l /var
- it Handle Comments #
## Examples Command
**Example 1**
- Username@your-regular-prompt:~$ ./hsh
- $ pwd
/home/username/
- $ ^D
- Username@your-regular-prompt:~$
**Example 2**
- Username@your-regular-prompt:~$ ./hsh
- $ ls -l /tmp 
- -rw------- 1 username username    0 Dec  5 12:09 config-err-aAMZrR
- drwx------ 3 root   root   4096 Dec  5 12:09 systemd-private-062a0eca7f2a44349733e78cb4abdff4-colord.service-V7DUzr
- drwx------ 3 root   root   4096 Dec  5 12:09 systemd-private-062a0eca7f2a44349733e78cb4abdff4-rtkit-daemon.service-ANGvoV
- drwx------ 3 root   root   4096 Dec  5 12:07 systemd-private-062a0eca7f2a44349733e78cb4abdff4-systemd-timesyncd.service-CdXUtH
- -rw-rw-r-- 1 username username    0 Dec  5 12:09 unity_support_test.0
- $ ^D
``Username@your-regular-prompt:~$``
#### List of functions and system calls we could use
- access (man 2 access)
- chdir (man 2 chdir)
- close (man 2 close)
- closedir (man 3 closedir)
- execve (man 2 execve)
- exit (man 3 exit)
- fork (man 2 fork)
- free (man 3 free)
- fstat (man 2 fstat)
- getcwd (man 3 getcwd)
- getline (man 3 getline)
- kill (man 2 kill)
- lstat (man 2 lstat)
- malloc (man 3 malloc)
- open (man 2 open)
- opendir (man 3 opendir)
- perror (man 3 perror)
- read (man 2 read)
- readdir (man 3 readdir)
- signal (man 2 signal)
- stat (man 2 stat)
- strtok (man 3 strtok)
- wait (man 2 wait)
- waitpid (man 2 waitpid)
- wait3 (man 2 wait3)
- wait4 (man 2 wait4)
- write (man 2 write)
- _exit (man 2 _exit)

#### Custom Function (Recreation of Standard Function in C)

- strncpy
- _strlen
- _putchar
- _atoi
- _puts
- _strcmp
- _isalpha
- array_rev
- intlen
- _itoa
- _strcat
- _strcpy
- _strchr
- _strncmp
- _strdup
- _memcpy
- _calloc
- _realloc
- _getenv
- _getline
- _strtok

### For More Info About It Check The Man Page by
```Username@your-regular-prompt:~$ man ./man_1_simple_shell```

