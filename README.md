# PicoCPP
CPP for Pico based on Pico-SDK

## Introduction
Even if the embedded community often disencouraged me doing programming in C++, I always thought C++ may be the better design and also performance alternative to C. One of the biggest problems here is the answer to the question, how to design easy to use and hard to misuse, reusable but still efficient, and last but not least still performant C++ class.
Fortuitously I found Dan Saks' talks at CppCon16: https://youtu.be/D7Sd8A6_fYU and CppCon20: https://youtu.be/uwzuAGtAEFk, which encouraged me again to start a lightweight C++ wrapper around the pico-sdk. Also very impressing the talk from Michael Caisse: https://youtu.be/LfRLQ7IChtg.

Questions to make clear, what the goal of this repo should be:
1. *Why Pico-SDK?*. 
    1.1  Well, I like the RPi Pico and the SDK is often easy to use and to understand.  
    1.2 Pico a very cheap dual core with higher clock than other M0+ concurrent chips.  
    1.2 Pico has nice addtional internals like the PIO and the interpolator.  
    1.3 Pico allows prototyping in Python.  
    1.4 easy and cheap debugging by using another Pico.  
    1.5 Pico has an acceptable amount of RAM.  
3. *Why C++?*. Whenever I propose to use C++ instead of C it feels like embedded developers want to throw shit on me with questions like "why(tf) do you ever want to do that? Unfortunately there is not one answer but a lot.  
    2.1 As Dan Saks already published in 2016, C++ already delivered the better performance.  
    2.2 I like the DRY principle, which can be achieved more easily in C++.  
    2.3 Especially with the new C++20 features like *constexpr*, program size may be reduced and performance may even get better.  
    2.4 C++ allows better and often more readable abstractions.  
    2.5 It is often possible to do C++ abstractions with zero overhead (will be eliminated during compilation)   
    2.6 better type safety reduces errors before debugging.  


...to be continued...

## Goals
- easy to use and hard to misuse
- easy to understand
- lightweight or zero-cost whenever possible

## Ideas
First implementing some communication classes with the outer world (GPIO, SPI, I2C, PWM...) to get the feeling how a HAL (hardware abstraction layer) should look like.
