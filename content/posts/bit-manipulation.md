+++
author = "David Ulicny"
title = "Bit Manipulation"
date = "2022-03-23"
description = "Demonstrating bit manipulation"
tags = [
    "bit",
    "manipulation",
]
categories = [
    "bit manipulation",
]
+++

# Bit manipulation

## Bitwise logical operators

### Bitwise AND (&)
Compares every bit of two numbers and applies AND operation to each of them. 
For example 5 (101b) and 3 (011b) will give 1.

5 & 3 -> 1 

```
101
011
---
001
```

6 & 5 -> 4

```
110
101
---
100
```

### Bitwise OR (|)

Compares every bit of two numbers and applies OR operation to each of them.

5 | 3 -> 7

```
101
011
---
111
```

### Bitwise XOR (^)

Compares every bit of two numbers and applies XOR operation to each of them.

5 ^ 3 -> 6

```
101
011
---
110
```

### Bitwise complement (~)

Negates the number bit by bit.



### Shift operators

Shift left `<<` , shift right `>>` 

## Check n-th bit

## Set n-th bit

## Clear n-th bit

## Truth tables

Truth table

```
A B A&B A|B A^B
0 1  0   1   1
1 0  0   1   1
1 1  1   1   0
0 0  0   0   0
```