# Monty

# 0x19. C - Stacks, Queues - LIFO, FIFO

# Description

Monty 0.98 is a scripting language that is first compiled into Monty byte codes (Just like Python). It relies on a unique stack, with specific instructions to manipulate it. The goal of this project is to create an interpreter for Monty ByteCodes files.



# Monty byte code files

Files containing Monty byte codes usually have the .m extension. Most of the industry uses this standard but it is not required by the specification of the language. There is not more than one instruction per line. There can be any number of spaces before or after the opcode and its argument.

# Installation

clone the repository:

```
$ git clone https://github.com/utuedey/monty.git
$ cd monty

```
# Compilation

The code should be compiled this way

```
$ gcc -Wall -Werror -Wextra -pedantic -std=c89 *.c -o monty

```

# Usage

```
$ cat -e bytecodes/00.m
push 1$
push 2$
push 3$
pall$
$ ./monty bytecodes/00.m
3
2
1
```
## Table of Contents

File | Description
---- | -----------
[main.c](./main.c) | entry point of the program
[monty.h](./monty.h) | main header file
[lists.h](./lists.h) | header file for the lists functions
[fetch_func.c](./get_func.c) | function that picks the right function for the instruction
[funcs_handler1.c](./handler_funcs1.c) | handler functions for the instructions
[funcs_handler2.c](./handler_funcs2.c) | handler functions for the instructions
[funcs_handler3.c](./handler_funcs3.c) | handler functions for the instructions
[list_funcs1.c](./list_funcs1.c) | doubly linked list functions
[list_funcs2.c](./list_funcs2.c) | doubly linked list functions
[strtow.c](./strtow.c) | string tokenizing functions
[free.c](./free.c) | memory handling functions
[char.c](./char.c) | handler functions for ascii instructions
