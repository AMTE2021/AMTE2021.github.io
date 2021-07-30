---
layout: default
---

# Invited talk

## Speaker:

![Daisy Hollman](daisy.jpg)

Dr. Daisy S. Hollman, Google, USA

Dr. Daisy S. Hollman has been a member of the C++ standards committee since 2016, where she has made contributions to a wide range of library and language features, including proposals related to executors, atomics, generic programming, futures, and multidimensional arrays. Since receiving her Ph.D. in Quantum Chemistry in 2013, her research has focussed primarily on parallel and concurrent programming models, though a broader focus on general accessibility of complex abstractions has become her focus in more recent years. She currently works on C++ language and library design at Google, where she continues to focus on providing broad accessibility of programming models and abstractions, with a particularfocus on design for diversity and inclusivity.

 
**The Past, Present, and Future of Asynchrony in C++**

Over the past quarter century, C++ has emerged as the language of choice for performance-sensitive applications where large-scale software engineering challenges are present and zero-overhead abstraction is a requirement. As such, with the continued increase in hardware concurrency, the language standard and the accompanying standard library have evolved to remain at the forefront of parallel and concurrent programming model design.  From the introduction of standard threads, atomics, and eager futures in C++11 aimed at use cases with several cores, to the C++17 parallel algorithms and C++20 atomic references with fewer implicit constraints for use cases on hundreds to thousands of cores, to the emerging executor and Sender/Receiver models that can lazily describe intricately interdependent work spanning vast timescales and granularities, the demand for zero-overhead abstraction in C++ has led to an ever-widening—and often daunting—set of tools for solving difficult problems at scale.

In this talk, we'll discuss the evolution of past and present abstractions for parallelism and concurrency in standard C++, explore the reasons why the current state of affairs is unsustainable, and present several of the short-term and long-term directions for the future of asynchronous programming in standard C++. We will conclude with a particular focus on the challenges associated with (and upcoming solutions for) expressing asynchrony at interface boundaries in large-scale, multi-library software stacks that compose today's production-scale applications.


