---
title: Synchronous and Asynchronous Functions in JavaScript
tags: [Javascript]
style: fill
color: primary
description: Memory allocation, parsing, and execution of our code play a huge role whenever we are developing software regardless of the language used. But most developers...
---

## Introduction

Memory allocation, parsing, and execution of our code play a huge role whenever we are developing software regardless of the language used. But most developers tend to ignore these topics and they are not given much emphasis in our academic career and we also don’t need to know it when we are writing the code – so why not ignore it. But these topics are of much importance and every developer should take it seriously while working. Now talking specifically of JavaScript, we regularly hear buzz words like Call Stack, Web APIs, etc. They all work together to parse and execute the scripts that we write. On the basis of execution, these scripts are divided into two parts: Synchronous Functions and Asynchronous Functions. Let’s look deep into these functions, what they are and how are they handled.


## SYNCHRONOUS Functions

In most of the languages, program execution is fairly straightforward. Our program starts executing each line of code sequentially. Synchronous Functions are similar to this. Synchronous Functions starts with the execution from the top and finishes each line before moving to the next. The script is executed 
sequentially. \\

As many of us know, JavaScript is single threaded i.e. it cannot do multi-tasking or multi-threading. It uses a single stack named Call-Stack to keep track of our functions that has to be executed sequentially. So let’s take an example to understand this better. While executing a script, JS comes across a function named task(). It is pushed into the Call-Stack and until its execution, it remains there. After its execution is complete, it is pooped out of the Call-Stack. \\

That’s how Synchronous Functions work by only involving the Call-Stack. However, things get a little bit complex when we encounter an asynchronous task.


## ASYNCHRONOUS Functions

Let’s take the above example and say we have two lines of code. However, this time the first line is a time-consuming instruction. Therefore, unlike the Synchronous task, the first line will continue its execution in the background and the second line will start its execution. \\

We need this kind of functioning when the execution is slow. It would be time wasting to wait for the completion of the functions which usually takes long time to execute. Therefore, if we store these in Call-Stack as we did in case of Synchronous Functions, it would block Call-Stack, which would stop the execution of script further. We need something to rescue us from this problem. Asynchronous callbacks does the same and help us in execution of our script asynchronously.

