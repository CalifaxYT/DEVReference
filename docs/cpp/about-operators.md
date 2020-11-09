---
layout: default
title: C++ Operators
nav_order: 4
has_children: true
permalink: docs/cpp
---

# C++ Operators

## An Overview of C++ Operators

C++ provides more than 35 operators, covering basic arithmetic, bit manipulation, indirection, comparisons, logical operations and others. Almost all operators can be overloaded for user-defined types, with a few notable exceptions such as member access (. and .*) as well as the conditional operator. The rich set of overloadable operators is central to making user-defined types in C++ seem like built-in types.

Overloadable operators are also an essential part of many advanced C++ programming techniques, such as smart pointers. Overloading an operator does not change the precedence of calculations involving the operator, nor does it change the number of operands that the operator uses (any operand may however be ignored by the operator, though it will be evaluated prior to execution). Overloaded double "&" and  double "|" operators lose their short-circuit evaluation property.