A curated list of awesome resources and learning materials in the field of X internals.
This list has a bias towards education.

## Contents

- [Interpreters/Compilers](#interpreterscompilers)
- [Databases](#databases)
- [Operating Systems](#operating-systems)
- [Network](#network)

## Interpreters/Compilers

- [A closer look at Crankshaft, V8's optimizing compiler, by Andy Wingo](https://wingolog.org/archives/2011/08/02/a-closer-look-at-crankshaft-v8s-optimizing-compiler) - continuing in my series of articles on V8, Google's JavaScript engine, in this article I'd like to take a closer look at V8's optimizing compiler, with a focus on the Hydrogen intermediate language.
- [A Simple Graph-Based Intermediate Representation, by Cliff Click, Michael Paleczny](http://www.oracle.com/technetwork/java/javase/tech/c2-ir95-150110.pdf) - a paper where they present a graph-based intermediate representation (IR) with simple semantics and a low-memory-cost C++ implementation.
- [A tour of V8: Crankshaft, the optimizing compiler, by Jay Conrod](http://jayconrod.com/posts/54/a-tour-of-v8-crankshaft-the-optimizing-compiler) - an intro into Crankshaft, optimizing compiler in V8, before Turbofan.
- [A tour of V8: Garbage Collection, by Jay Conrod](http://jayconrod.com/posts/55/a-tour-of-v8-garbage-collection) - an intro into garbage collection in V8.
- [Adventures in JIT compilation, by Eli Bendersky](https://eli.thegreenplace.net/2017/adventures-in-jit-compilation-part-1-an-interpreter/) - a series about JIT compilation with Brainfuck as an input language, implemented in C++.
- [An Introduction to Speculative Optimization in V8, by Benedikt Meurer](http://benediktmeurer.de/2017/12/13/an-introduction-to-speculative-optimization-in-v8/) - how TurboFan, V8’s optimizing compiler, works and how V8 turns your JavaScript into highly-optimized machine code.
- [Anders Hejlsberg on Modern Compiler Construction, by Anders Hejlsberg, Seth Juarez](https://channel9.msdn.com/Blogs/Seth-Juarez/Anders-Hejlsberg-on-Modern-Compiler-Construction) - in this video Anders a great foundation of compiler construction by describing the traditional methodologies that have been used in the last 30 or so years. He then uses that foundation to describe modern tooling needs and how compilers have adapted to meet increasing demands.
- [Beginner's Guide to Linkers, by David Drysdale](http://www.lurklurk.org/linkers/linkers.html) - this article is intended to help C & C++ programmers understand the essentials of what the linker does.
- [Build Your Own Lisp, by Daniel Holden](http://www.buildyourownlisp.com/contents) - a book about how to implement your own Lisp language with C compiler.
- [Combining Analyses, Combining Optimizations, by Cliff Click](https://www.researchgate.net/publication/2394127_Combining_Analyses_Combining_Optimizations) - this paper presents a framework for describing optimizations. It shows how to combine two such frameworks and how to reason about the properties of the resulting framework.
- [Efficient and General On-Stack Replacement for Aggressive Program Specialization, by Sunil Soman, Chandra Krintz](https://www.cs.ucsb.edu/%7Eckrintz/papers/osr.pdf) - in this paper, we present a novel, general-purpose OSR mechanism that is more amenable to optimiza- tion than prior approaches. In particular, we decou- ple the OSR implementation from the optimization pro- cess and update the program state information incre- mentally during optimization.
- [Implementing a JIT Compiled Language with Haskell and LLVM, by Stephen Diehl](http://www.stephendiehl.com/llvm/) - welcome to the Haskell version of "Implementing a language with LLVM" tutorial. This tutorial runs through the implementation of a simple language, and the basics of how to build a compiler in Haskell, showing how fun and easy it can be.
- [Juozas Kaziukėnas - Building An Interpreter In RPython - PyCon 2016](https://www.youtube.com/watch?v=9tDpjzPLvNY) - a speech on how was built PHP interpreter with RPython.
- [Let's Build a Compiler, by Jack Crenshaw](https://compilers.iecc.com/crenshaw/) - this fifteen-part series, written from 1988 to 1995, is a non-technical introduction to compiler construction.
- [Let’s Build a Simple Interpreter, by Ruslan Spivak](https://ruslanspivak.com/lsbasi-part1/) - a series of articles about implementing Pascal interpreter in Python.
- [Optimizing Dynamically-Typed Object-Oriented Languages With Polymorphic Inline Caches, by Urs Hölzle, Craig Chambers, David Ungar](http://hoelzle.org/publications/ecoop91.pdf) - a paper about polymorphic inlince caches which provide a new way to reduce the overhead of polymorphic message sends by extending inline caches to include more than one cached lookup result per call site.
- [Polymorphic Inline Caching on JavaScript for fun and profit, by Chris Leary](http://blog.cdleary.com/2010/09/picing-on-javascript-for-fun-and-profit) - what follows is a gentle-albeit-quirky introduction to what polymorphic inline caches (PICs) are and why they're useful to JavaScript Just-In-Time compilers like JaegerMonkey.
- [Project: A Programming Language, by Marijn Haverbeke](http://eloquentjavascript.net/12_language.html) - we will build a programming LISP-like language called Egg. It will be a tiny, simple language—but one that is powerful enough to express any computation you can think of. It will allow simple abstraction based on functions.
- [Understanding Compiler Optimization - Chandler Carruth - Opening Keynote Meeting C++ 2015](https://www.youtube.com/watch?v=FnGCDLhaxKU) - talk from Chandler Carruth about compilers optimizations, implemented in LLVM.
- [V8: A tale of two compilers, by Andy Wingo](https://wingolog.org/archives/2011/07/05/v8-a-tale-of-two-compilers) - advanced intro into two compilers in V8: FullCodegen and Crankshaft.

## Databases

- [How does a relational database work, by Christophe Kalenzaga](http://coding-geek.com/how-databases-work/) - a really deep explanation of how relational databases work.
- [Implementing Sorting in Database Systems, by Goetz Graefe](http://wwwlgis.informatik.uni-kl.de/archiv/wwwdvs.informatik.uni-kl.de/courses/DBSREAL/SS2005/Vorlesungsunterlagen/Implementing_Sorting.pdf) - it covers in-memory sorting, disk-based external sorting, and considerations that apply specifically to sorting in database systems.

## Operating Systems

- [Demystifying the Secure Enclave Processor, by Tarjei Mandt, Mathew Solnik, David Wang](http://mista.nu/research/sep-paper.pdf) - SEP is designed as a security circuit configured to perform secure services for the rest of the SOC, with no direct access from the main processor. The paper dives into its implementation and how it commnunicates with other components.
- [How OSX executes applications, by Mohit Muthanna Cheppudira](http://0xfe.blogspot.de/2006/03/how-os-x-executes-applications.html) - a deep intro into how OS X executes applications, Mach-O format, etc...
- [Linux Inside, by 0xAX](https://0xax.gitbooks.io/linux-insides/) - book where author wants to share his modest knowledge about the insides of the linux kernel and help people who are interested in linux kernel insides, and other low-level subject matter.
- [Operating System Development Series](http://www.brokenthorn.com/Resources/OSDevIndex.html) - a series of posts on how to implement your own operating system from scratch.
- [Parsing Mach-O files, by Alex Denisov](https://lowlevelbits.org/parsing-mach-o-files/) - this article describes how to parse Mach-O file and explains its format.
- [Writing a Minimal Mach-O Executable File, by Nicolas Seriot](http://seriot.ch/hello_macho.php) - a story about how author writes a minimal Mach-O executable file which fits into 164 bytes and prints Hello, World.
- [Writing a Simple Operating System, by Nick Blundell](http://www.cs.bham.ac.uk/%7Eexr/lectures/opsys/10_11/lectures/os-dev.pdf) - self-contained and coherent document, that will give you a hands-on experience of low-level programming, how operating systems are written, and the kind of problems they must solve.

## Network

- [A container networking overview, by Julia Evans](https://jvns.ca/blog/2016/12/22/container-networking/) - there are a lot of different ways you can network containers together, and the documentation on the internet about how it works is often pretty bad. I got really confused about all of this, so I’m going to try to explain what it all is in laymen’s terms.
- [High Performance Browser Networking, by Ilya Grigorik](https://hpbn.co) - this book provides a hands-on overview of what every web developer needs to know about the various types of networks (WiFi, 3G/4G), transport protocols (UDP, TCP, and TLS), application protocols (HTTP/1.1, HTTP/2), and APIs available in the browser (XHR, WebSocket, WebRTC, and more) to deliver the best—fast, reliable, and resilient—user experience.
