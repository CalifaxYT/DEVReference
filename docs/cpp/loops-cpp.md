---
layout: default
title: LOOPS | While..do & more
parent: C++
nav_order: 5
---

# while..do & more in C++ (ak.a. repeatedly executable statements)

## The while loop
The ``while`` statement consists of condition and block of statements, called loop body. The loop
body is executed repeatedly, while the condition remains true. The ``while`` loop is a pre-test loop (the
condition is tested before each iteration).
```cpp
while (condition)
{
statement_1;
statement_2;
...
statement_n;
}
```

A real example would look like this:
```cpp
int i = 0;
double sum = 0, var = 0;
while (i < MAX)
{
cin >> var;
sum += var;
i++;
}
```


NOTE: Placing a semicolon after the ``while`` loop header will end the loop statement before its body. Nothing will modify the condition of the loop, and if the condition originally is true, the result will be an infinite loop.

## The do/while loop
``do loop`` works as ``while`` loop but the loop body is executed at least once. do loop is a post-test loop,
which means that the loop condition is after the body of the loop is executed.
```cpp
do
{
statement_1;
statement_2;
...
statement_n;
}while(condition);
```

A real example would look like this:
```cpp
char ch = 0;
do
{
cout << "Lower case letter: ";
cin >> ch;
}
while (ch < ’a’ || ch > ’z’);
```

NOTE: Placing a semicolon after the ``while`` loop header will end the loop statement before its body. Nothing will modify the condition of the loop, and if the condition originally is true, the result will be an infinite loop.

NOTE 2: The body of the do loop is executed at least once.

## The for loop
``for loop`` is used when the statements in the loop body are executed given number of times. Unlike
the while loop, for loop allows declaration of explicit counter. Although for loop can be written as
a while loop, it is considered more practical to use for when the number of iterations are known in
advance. The for loop is a pretest loop.
```cpp
for (init; condition; update)
{
statement_1;
statement_2;
...
statement_n;
}while(condition);
```

A real example would look like this:
```cpp
const int MAX = 10;
int sum = 0;
for (int i = 1; i <= MAX; i++)
{
sum += i;
}    
cout << sum << endl;

```