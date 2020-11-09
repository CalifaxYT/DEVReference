---
layout: default
title: PRAG | MAX()
parent: C++
nav_order: 2
---

# Preprocessor MAX()

## A quick rundown of the MAX() preprocessor directive/pragma

While there is a way to get the so-called "bigger" value of a char/integer/double/float, not including the whole STD library (and replacing it with a pragma) is sometimes the better choice - for example when there is **VERY** limited memory on the device or, when the program is relatively small. 

## Macro usage
```cpp
#define MAX(x, y) (x > y ? x : y)
```