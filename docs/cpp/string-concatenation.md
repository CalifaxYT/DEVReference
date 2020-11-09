---
layout: default
title: [STR] String Concatenation
parent: C++
nav_order: 5
---

# String Concatenation in C++

## A quick rundown of string concatenation in C++

Some languages allow to concatenate multiple in-lined strings when printing to the console in the following way:
```c#
Console.WriteLine("foo" + "bar" + "baz");
```

Some beginner C++ programmers might think that the same would be possible here, but at least in the current release of the language string concatenation **CAN NOT** be done with the sign "+" if both of the strings are in-lined. At least one of them should be an already defined variable:
```cpp
string bar = bar
cout << "foo" + bar << endl;
```

If concatenation of in-lined variables is needed it is done like so:
```cpp
cout << "foo" << "bar" < "baz" << endl;
```