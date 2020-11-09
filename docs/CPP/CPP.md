---
layout: default
title: C++
nav_order: 2
has_children: true
permalink: docs/CPP
---

# [C++]
{: .no_toc }

{: .fs-6 .fw-300 }

# A Brief Description

## Preface

Computers are some of the most versatile tools that we have available. They are capable of performing stunning feats of computation, they allow information to be exchanged easily regardless of their physical location, they simplify many every-day tasks, and they allow us to automate many processes that would be tedious or boring to perform otherwise. However, computers are not "intelligent" as we are. They have to be told in no uncertain terms exactly what they're supposed to do, and their native languages are quite unlike anything we speak. Thus, there's a formidable language barrier between a person who wishes a computer to do something, and the computer that typically requires instructions in its native language, machine code, to do anything. So far, computers cannot figure out what they are supposed to do on their own, and thus they rely on **programs** which we create, which are sets of instructions that the computer can understand and follow.  

## An Overview of Programs and Programming Languages

In order to better communicate to our computers what exactly it is we want them to do, we've developed a wide range of **programming languages** to make the communication process easier.  

Depending on the type of project, there are many factors that have to be considered when choosing a language. Here is a list of some of the more noteworthy ones:  

*   <u>Compiled, interpreted, or JIT-compiled</u>  
    **Compiled languages** are translated to the target machine's native language by a program called a compiler. This can result in very fast code, especially if the compiler is effective at optimizing, however the resulting code may not port well across operating systems and the compilation process may take a while.  
    **Interpreted languages** are read by a program called an interpreter and are executed by that program. While they are as portable as their interpreter and have no long compile times, interpreted languages are usually _much_ slower than an equivalent compiled program.  
    Finally, **just-in-time compiled** (or JIT-compiled) languages are languages that are quickly compiled when programs written in them need to be run (usually with very little optimization), offering a balance between performance and portability.  

*   <u>High or Low Level</u> Level, in this case, refers to how much the nature of the language reflects the underlying system. In other words, a programming language's level refers to how similar the language is to a computer's native language. The higher the level, the _less_ similar it is.  
    A **low-level language** is generally quite similar to machine code, and thus is more suitable for programs like device drivers or very high performance programs that really need access to the hardware. Generally, the term is reserved for machine code itself and assembly languages, though many languages offer low-level elements. Since a low-level language is subject to all the nuances of the hardware it's accessing, however, a program written in a low-level language is generally difficult to port to other platforms. Low level languages are practically never interpreted, as this generally defeats the purpose.  
    A **high-level language** focuses more on concepts that are easy to understand by the human mind, such as objects or mathematical functions. A high-level language usually is easier to understand than a low-level language, and it usually takes less time to develop a program in a high-level language than it does in a low-level language. As a trade-off one generally needs to sacrifice some degree of control over what the resulting program actually does. It is not, however, impossible to mix high-level and low-level functionality in a language.  

*   <u>Type System</u>  
    A **type system** refers to the rules that the different types of variables of a language have to follow. Some languages (including most assembly languages) do not have types and thus this section does not apply to them. However, as most languages (including C++) have types, this information is important.  

    *   **Type Strength: Strong or Weak**  
        A strong typing system puts restrictions on how different types of variables can be converted to each other without any converting statements. An ideal strong typing system would forbid implicit "casts" to types that do not make any sense, such as an integer to a Fruit object. A weak typing system would try to find some way to make the cast work.  

    *   **Type Expression: Manifest or Inferred**  
        This deals with how the compiler/interpreter for a language infers the types of variables. Many languages require variables' types to be explicitly defined, and thus rely on manifest typing. Some however, will infer the type of the variable based on the contexts in which it is used, and thus use inferred typing.  

    *   **Type Checking: Static or Dynamic**  
        If a language is statically typed, then the compiler/interpreter does the type checking once before the program runs/is compiled. If the language is dynamically type checked, then the types are checked at run-time.  

    *   **Type Safety: Safe or Unsafe**  
        These refer to the degree to which a language will prohibit operations on typed variables that might lead to undefined behavior or errors. A safe language will do more to ensure that such operations or conversions do not occur, while an unsafe language will give more responsibility to the user in this regard.  

    These typing characteristics are not necessarily mutually exclusive, and some languages mix them.  

*   <u>Supported paradigms</u>  
    A programming paradigm is a methodology or way of programming that a programming language supports. Here is a summary of a few common paradigms:  

    *   **Declarative**  
        A declarative language will focus more on specifying what a language is supposed to accomplish rather than by what means it is supposed to accomplish it. Such a paradigm might be used to avoid undesired side-effects resulting from having to write one's own code.  

    *   **Functional**  
        Functional programming is a subset of declarative programming that tries to express problems in terms of mathematical equations and functions. It goes out of its way to avoid the concepts of states and mutable variables which are common in imperative languages.  

    *   **Generic**  
        Generic programming focuses on writing skeleton algorithms in terms of types that will be specified when the algorithm is actually used, thus allowing some leniency to programmers who wish to avoid strict strong typing rules. It can be a very powerful paradigm if well-implemented.  

    *   **Imperative**  
        Imperative languages allow programmers to give the computer ordered lists of instructions without necessarily having to explicitly state the task. It can be thought of being the opposite of declarative programming.  

    *   **Structured**  
        Structured programming languages aim to provide some form of noteworthy structure to a language, such as intuitive control over the order in which statements are executed (if X then do Y otherwise do Z, do X while Y is Z). Such languages generally deprecate "jumps", such as those provided by the goto statement in C and C++.  

    *   **Procedural**  
        Although it is sometimes used as a synonym for imperative programming, a procedural programming language can also refer to an imperative structured programming language which supports the concept of procedures and subroutines (also known as functions in C or C++).  

    *   **Object-Oriented**  
        Object-Oriented programming (sometimes abbreviated to OOP) is a subset of structured programming which expresses programs in the terms of "objects", which are meant to model objects in the real world. Such a paradigm allows code to be reused in remarkable ways and is meant to be easy to understand.  

*   <u>Standardization</u>  
    Does a language have a formal standard? This can be very important to ensure that programs written to work with one compiler/interpreter will work with another. Some languages are standardized by the American National Standards Institute (ANSI), some are standardized by the International Organization for Standardization (ISO), and some have an informal but de-facto standard not maintained by any standards organization.  

## The Features of C++ as a Language

Now that all the necessary theory has been covered, now it is possible to explain what C++ has to offer as a programming language. C++...  

*   <u>...is an open ISO-standardized language.</u>  
    For a time, C++ had no official standard and was maintained by a de-facto standard, however since 1998, C++ is standardized by a committee of the ISO. Their page may be accessed [here](http://www.open-std.org/jtc1/sc22/wg21/).  

*   <u>...is a compiled language.</u>  
    C++ compiles directly to a machine's native code, allowing it to be one of the fastest languages in the world, if optimized.  

*   <u>...is a strongly-typed unsafe language.</u>  
    C++ is a language that expects the programmer to know what he or she is doing, but allows for incredible amounts of control as a result.  

*   <u>...supports both manifest and inferred typing.</u>  
    As of the latest C++ standard, C++ supports both manifest and inferred typing, allowing flexibility and a means of avoiding verbosity where desired.  

*   <u>...supports both static and dynamic type checking.</u>  
    C++ allows type conversions to be checked either at compile-time or at run-time, again offering another degree of flexibility. Most C++ type checking is, however, static.  

*   <u>...offers many paradigm choices.</u>  
    C++ offers remarkable support for procedural, generic, and object-oriented programming paradigms, with many other paradigms being possible as well.  

*   <u>...is _portable._</u>  
    As one of the most frequently used languages in the world and as an open language, C++ has a wide range of [compilers](http://www2.research.att.com/~bs/compilers.html) that run on many different platforms that support it. Code that exclusively uses C++'s standard library will run on many platforms with few to no changes.  

*   <u>...is upwards compatible with C</u>  
    C++, being a language that directly builds off C, is compatible with almost all C code. C++ can use C libraries with few to no modifications of the libraries' code.  

*   <u>...has incredible library support.</u>  
    A search for "library" on the popular project-management website [SourceForge](http://www.sourceforge.net) will yield over 3000 results for C++ libraries. A link to the results of the search may be found [here](http://sourceforge.net/directory/language:C%2B%2B/?q=library).  
