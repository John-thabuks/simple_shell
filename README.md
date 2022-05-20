# README FILE FOR SIMPLE_SHELL PROJECT
## PID & PPID

#### 0. getppid

Write a program that prints the PID of the parent process. Run your program several times within the same shell. It should be the same. Does echo $$ print the same value? Why?

#### 1. /proc/sys/kernel/pid_max

Write a shell script that prints the maximum value a process ID can be.

#### 0. av

Write a program that prints all the arguments, without using ac.

#### 1. Read line

Write a program that prints "$ ", wait for the user to enter a command, prints it on the next line.

#### 2. command line to av

Write a function that splits a string and returns an array of each word of the string.

man strtok

advanced: Write the function without strtok

#### Exercise: fork + wait + execve

Write a program that executes the command ls -l /tmp in 5 different child processes. Each child should be created by the same process (the father). Wait for a child to exit before creating a new child.

#### Exercise: super simple shell

Using everything we saw, write a first version of a super simple shell that can run commands with their full path, without any argument.

#### Exercise: find a file in the PATH

Write a program that looks for files in the current PATH.

Usage: _which filename ...

#### 0. printenv with environ

Write a program that prints the environment using the global variable environ.

#### env vs environ

Write a program that prints the address of env (the third parameter of the main function) and environ (the global variable). Are they they same? Does this make sense?

#### getenv()

Write a function that gets an environment variable. (without using getenv)

Prototype: char *_getenv(const char *name);
man 3 getenv

#### PATH

Write a function that prints each directory contained in the the environment variable PATH, one directory per line.

#### PATH

Write a function that builds a linked list of the PATH directories.

#### setenv

Write a function that changes or adds an environment variable (without using setenv).

Prototype: int _setenv(const char *name, const char *value, int overwrite);
man 3 setenv

#### unsetenv

Write a function that deletes the variable name from the environment (without using unsetenv).

Prototype: int _unsetenv(const char *name);
man 3 unsetenv

#### 0.Betty would be proud
mandatory
Write a beautiful code that passes the Betty checks

#### Simple shell 0.1
mandatory
Write a UNIX command line interpreter.

Usage: simple_shell

#### 2. Simple shell 0.2
mandatory
Simple shell 0.1 +

Handle command lines with arguments

#### 3. Simple shell 0.3
mandatory
Simple shell 0.2 +

Handle the PATH
fork must not be called if the command doesn’t exist

#### 4. Simple shell 0.4
mandatory
Simple shell 0.3 +

Implement the exit built-in, that exits the shell
Usage: exit
You don’t have to handle any argument to the built-in exit

#### 5. Simple shell 1.0
mandatory
Simple shell 0.4 +

Implement the env built-in, that prints the current environment



