---
title: Clean Code
layout: post
publishedOn: 04 October, 2014
---
I have to admit that the idea of **Clean Code** is really new to me, and all the code
smell signs that I never knew before! until I was exposed to Agile development framework - Scrum.
I was suggested to read a book called Clean Code after I attended the TDD workshop
from Odd-E. I really have to say that it changed my perspective about writing code!!!
and Martin Fowler once said that:

>Any fool can write code that machine can understand.
>Good programmers write code that humans can understand

Since then, I try pay more attention when I write code and here are a few things that
I have changed:

1. I won't write production code without having unit tests
2. I won't produce more duplicated code
3. I will leave the code base *better* than it was

So, does it really help me write a clean code? not totally, but it helps
me to care more about the code that I produce, at least it is better than it was!

### What is clean code?
The definition of clean code are different for different people but I think they
all agree that clean code is not *dirty code*. Em... you may ask what is
is dirty code then? Dirty code has one characteristic, it calls *code smell*. Like
many other dirty things, we try to avoid it, we don't want to get involve with it and
it applies to the code as well. So, my definition of clean code is a code base that
I am comfortable to work with, it's the code that is easy to change and maintain.
It just take only a few scroll to see how much the author care about the code.

### Why should I care about clean code?
Have you ever encounter a situation where you need to apply your changes and you have
Ctrl+C and Ctrl+V to all over the code base, scrolling through the few hundred lines of
a function trying to understand what it does, or don't know what function to use.
At least, those had happened to me once, and I have realised that those are the
sign of code smell!. Then, I try to reflect back to my code base, says, what if
there's no duplicated code, I would just have to change in only one place (sounds nice huh!)
I would say having a clean code base brings lots of benefits especially the code the
we are regularly maintaining.

### What are some signs of the code smells?
- *Duplication*, duplication is the root of all the evil! Most of the code smell are
related to the duplication. Duplication can come in many form, they could be something
that look similar but not the same. For example, two functions are doing the same thing,
but they just have different name and parameters. When I remove the duplication, It helps me to
discover other sign of code smell, and it was actually fun to remove those smell, and see
how code transforms to be cleaner.
- *Naming*, a good variable or function naming can help to understand the code without
getting to read the implementation. For example, if I have a function call **XX()**
can you tell by its name what it does? probably not and you need to find out where the function
declare and its implementation. But, if the function name **computeSquareOfX()**
it is pretty straightforward, isn't it?
- *Loooong Function*, it's sign showing that the function is trying to do too many things
and it's probably too complicated to making changes. We should try to keep the function
small, but how small is small enough? Well, according to what I read and my little experiences,
it tells me that any function more than 10-15 lines is considering long.
Again, that is what I feel right about it. You don't have to follow what I set here.

### How do I clean up code?
First, stop writing dirty code. Second, Refactoring. When you are refactoring the code,
it is like you are going into a war! you need a good armour to protect your
self from enemies (bugs) and you need a sword to help you to
eliminate those bugs. In other words, you need to have good unit tests wrapping around
the area you want to change before you do refactoring, and some good refacotring tools that help
you to do those job. For example in our case is NUnit, Resharper, Code Coverage tools
or Continuous Integration (CI) server

But, to have a good test in place, you need to refactoring you code first. Oh, wait
a minute, does it sound like the chicken and egg problem here? Probably not, there
are a few safe techniques that you can use to refactoring without having test first.
For examples, *lean in compiler*, *extract interface*, *scratch refactoring*,
*extract and override*, *renaming*, etc. These are just a few, and many useful that
are described in the book **Wokring Effectively With Legacy Code**
and it's available in our library!

### Where can I learn more?
Like other things, we learn best when we practise it and there are so many training and
tutorials online waiting for you tackle them. If you really can't find, just practise
with your code base. Just try to do and see you much you can change the code to
be cleaner. Reading books also help, it give you some techniques to deal with
certain problems, or showing you that there are other ways to look at the problems.

It is easy to write code, but writing a cleaner code is taking much more effort
to do and it's not just happen over night. It takes times to learn and experiment with.
Find your own motivation, I can you tell over and over about what is clean code,
but it probably get you to nowhere, if you just only read about it.
