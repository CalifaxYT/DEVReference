---
layout: default
title: PRAG | Preprocessor ABS()
parent: C++
nav_order: 3
---

# Preprocessor ABS()

## A quick rundown of the ABS() preprocessor directive/pragma

While there is a way to get the so-called "absolute" value of a char/integer/double/float, not including the whole CMath library (and replacing it with a pragma) is sometimes the better choice - for example when there is **VERY** limited memory on the device or, when the program is relatively small. 

## Macro usage
```cpp
#define ABS (x) (x >= 0 ? x:-x)
```

NOTE: If using in-lined math, there needs to be a second pair of parentheses, for example:
```cpp
ABS((a - b))
```

Otherwise, it should be used in the following way:
```cpp
ABS(a)
```