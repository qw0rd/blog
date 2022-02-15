---
title: "Hello World"
date: 2022-02-07T00:21:09+05:30
description: "Hello world of sorts"
draft: false
---

Thanks for checking out this blog. Here's an obligatory hello world program but in assembly :)

```asm
.intel_syntax noprefix

.section .text
.global main
main:
    lea rdi, msg
    mov rsi, 0
    mov rax, 0
    call printf
    ret

.section .data
    msg: .asciz "Hello, world!\n"

.att_syntax
```

And ofc, in C.
```c

#include <stdio.h>

int main()
{
    printf("Hello, world!\n");
}

```


