---
layout: default
title: [PRAG] Preprocessor CHAR_TO_INT()
parent: C++
nav_order: 4
---

# Preprocessor CHAR_TO_INT()

## A quick rundown of the CHAR_TO_INT() preprocessor directive/pragma

A char can be cast to an integer. This way its place in the ASCII table will be returned. While there might be some other ways to convert a **CHAR** to an **INTEGER** variable, the best (and probably the memory-lightest) way to do it is to use a simple and short preprocessor directive.

## Macro usage
```cpp
#define CHAR_TO_INT(char) ((int)char)
```

The macro is used in the following way:
```cpp
CHAR_TO_INT('a')
```

