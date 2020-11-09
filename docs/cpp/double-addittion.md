---
layout: default
title: [MATH] Adding numbers of type "double"
parent: C++
nav_order: 5
---

# Adding numbers of type "double"

## A quick reminder about adding "double"-type numbers

Some languages allow to add values of different types (eg. int + double) properly:
```c#
Console.WriteLine(77 + 3.14);
```

However, in C++ this would lead to an improper calculation. To combat this, all numbers should be of the same type:
```cpp
cout << (4.0 + 4.0) << endl;
```
