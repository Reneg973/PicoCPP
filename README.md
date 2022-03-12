# PicoCPP
CPP for Pico based on Pico-SDK

## Introduction
Even if the embedded community often disencouraged me doing programming in C++, I always thought C++ may be the better design and also performance alternative to C. One of the biggest problems here is the answer to the question, how to design easy to use and hard to misuse, reusable but still efficient, and last but not least still performant C++ class.
Fortuitously I found Dan Saks' talks at CppCon16: https://youtu.be/D7Sd8A6_fYU and CppCon20: https://youtu.be/uwzuAGtAEFk, which encouraged me again to start a lightweight C++ wrapper around the pico-sdk.

Questions to make clear, what the goal of this repo should be:
1. *Why Pico-SDK?* Well, I like the RPi Pico and the SDK is often easy to use and to understand.
2. *Why C++?*
2.1 As Dan Saks already published in 2016, C++ already delivered the better performance.
2.2 I like the DRY principle, which can be achieved more easily in C++.
2.3 Especially with the new C++20 features like *constexpr*, program size may be reduced and performance may even get better.
...to be continued...

