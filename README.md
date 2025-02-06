# Simple Compiler using Flex & Bison

A basic compiler built using **Flex** (lexical analysis) and **Bison** (syntax analysis).

## Features
- Token recognition (keywords, operators, literals).
- Supports `if-else`, `for`, `switch-case`, and expressions.
- Built-in functions: `sin`, `cos`, `gcd`, `lcm`, `reverse`, `sort`, etc.
- Error handling for undeclared variables, redeclarations, division by zero.
- Preprocessor directive `@@include` for header inclusion.

## Build & Run
```sh
bison -d 1907094.y  
flex 1907094.l  
gcc lex.yy.c 1907094.tab.c -o compiler  
./compiler  
