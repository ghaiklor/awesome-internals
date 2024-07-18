# awesome-internals

A curated list of awesome resources and learning materials in the field of X internals.
This list has a bias towards education.

- [Courses](#courses)
- [Hardware](#hardware)
- [Operating Systems](#operating-systems)
- [Parsers](#parsers)
- [Interpreters/Compilers](#interpreterscompilers)
- [Network](#network)
- [Databases](#databases)
- [Bundlers](#bundlers)
- [Package Managers](#package-managers)

## Courses

- [Compilers](https://www.edx.org/learn/computer-science/stanford-university-compilers) - Self-paced course from Stanford online on compilers.
- [From NAND to Tetris](https://www.nand2tetris.org) - The course contains all the project materials and software tools necessary for building a general-purpose computer system from the ground up. The materials are aimed at students, instructors, and self-learners. Everything is free and open-source, as long as you operate in a non-profit, educational setting.

## Hardware

- [Demystifying the Secure Enclave Processor, by Tarjei Mandt, Mathew Solnik, David Wang](http://mista.nu/research/sep-paper.pdf) - SEP is designed as a security circuit configured to perform secure services for the rest of the SOC, with no direct access from the main processor. The paper dives into its implementation and how it communicates with other components.

## Operating Systems

- [How debugger works, by Alexander Sandler](http://www.alexonlinux.com/how-debugger-works) - In this article, I’d like to tell you how real debugger works. What happens under the hood and why it happens. We’ll even write our own small debugger and see it in action.
- [How debuggers work, by Eli Bendersky](https://eli.thegreenplace.net/2011/01/23/how-debuggers-work-part-1/) - a series of articles on how debuggers work.
- [How OSX executes applications, by Mohit Muthanna Cheppudira](http://0xfe.blogspot.de/2006/03/how-os-x-executes-applications.html) - a deep intro into how OS X executes applications, Mach-O format, etc...
- [htop explained, by Pēteris Ņikiforovs](https://peteris.rocks/blog/htop) - explanation of everything you can see in htop/top on Linux.
- [Linux Inside, by 0xAX](https://0xax.gitbooks.io/linux-insides/) - book where author wants to share his modest knowledge about the insides of the linux kernel and help people who are interested in linux kernel insides, and other low-level subject matter.
- [Operating System Development Series](http://www.brokenthorn.com/Resources/OSDevIndex.html) - a series of posts on how to implement your own operating system from scratch.
- [Parsing Mach-O files, by Alex Denisov](https://lowlevelbits.org/parsing-mach-o-files/) - this article describes how to parse Mach-O file and explains its format.
- [The Adventures of OS: Making a RISC-V Operating System using Rust, by Stephen Marz](http://osblog.stephenmarz.com) - In this blog, we will write an operating system targeting the RISC-V architecture in Rust.
- [Writing a Minimal Mach-O Executable File, by Nicolas Seriot](http://seriot.ch/hello_macho.php) - a story about how author writes a minimal Mach-O executable file which fits into 164 bytes and prints Hello, World.
- [Writing a Simple Operating System, by Nick Blundell](http://www.cs.bham.ac.uk/%7Eexr/lectures/opsys/10_11/lectures/os-dev.pdf) - self-contained and coherent document, that will give you a hands-on experience of low-level programming, how operating systems are written, and the kind of problems they must solve.
- [Writing an OS in Rust, by Philipp Oppermann](https://os.phil-opp.com) - This blog series creates a small operating system in the Rust programming language. Each post is a small tutorial and includes all needed code, so you can follow along if you like.

## Parsers

- [Learning Parser Combinators With Rust, by Bodil Stokke](https://bodil.lol/parser-combinators/) - this article teaches the fundamentals of parser combinators to people who are already Rust programmers. It assumes no other knowledge, and will explain everything that isn't directly related to Rust, as well as a few of the more unexpected aspects of using Rust for this purpose. It will not teach you Rust if you don't already know it, and, if so, it probably also won't teach you parser combinators very well.

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
- [Compiler basics: lisp to assembly, by Phil Eaton](http://notes.eatonphil.com/compiler-basics-lisp-to-assembly.html) - in this post we'll write a simple compiler in Javascript (on Node) without any third-party libraries. Our goal is to take an input program like (+ 1 (+ 2 3)) and produce an output assembly program that does these operations to produce 6 as the exit code.
- [Efficient and General On-Stack Replacement for Aggressive Program Specialization, by Sunil Soman, Chandra Krintz](https://www.cs.ucsb.edu/%7Eckrintz/papers/osr.pdf) - in this paper, we present a novel, general-purpose OSR mechanism that is more amenable to optimization than prior approaches. In particular, we decouple the OSR implementation from the optimization process and update the program state information incrementally during optimization.
- [How JIT Compilers are Implemented and Fast: Pypy, LuaJIT, Graal and More, by Carol Chen](https://carolchen.me/blog/jits-impls/) - This post goes into details of 5+ JITs and various optimization strategies and discuss how they work with different JITs.
- [How to implement a programming language in JavaScript, by Mihai Bazon](http://lisperator.net/pltut) - this is a tutorial on how to implement a programming language. If you ever wrote an interpreter or a compiler, then there is probably nothing new for you here. But, if you're using regexps to “parse” anything that looks like a programming language, then please read at least the section on parsing. Let's write less buggy code!
- [Implementing a JIT Compiled Language with Haskell and LLVM, by Stephen Diehl](http://www.stephendiehl.com/llvm/) - welcome to the Haskell version of "Implementing a language with LLVM" tutorial. This tutorial runs through the implementation of a simple language, and the basics of how to build a compiler in Haskell, showing how fun and easy it can be.
- [Juozas Kaziukėnas - Building An Interpreter In RPython - PyCon 2016](https://www.youtube.com/watch?v=9tDpjzPLvNY) - a speech on how was built PHP interpreter with RPython.
- [Let's Build a Compiler, by Jack Crenshaw](https://compilers.iecc.com/crenshaw/) - this fifteen-part series, written from 1988 to 1995, is a non-technical introduction to compiler construction.
- [Let’s Build a Simple Interpreter, by Ruslan Spivak](https://ruslanspivak.com/lsbasi-part1/) - a series of articles about implementing Pascal interpreter in Python.
- [Optimizing Dynamically-Typed Object-Oriented Languages With Polymorphic Inline Caches, by Urs Hölzle, Craig Chambers, David Ungar](http://hoelzle.org/publications/ecoop91.pdf) - a paper about polymorphic inline caches which provide a new way to reduce the overhead of polymorphic message sends by extending inline caches to include more than one cached lookup result per call site.
- [Polymorphic Inline Caching on JavaScript for fun and profit, by Chris Leary](http://blog.cdleary.com/2010/09/picing-on-javascript-for-fun-and-profit) - what follows is a gentle-albeit-quirky introduction to what polymorphic inline caches (PICs) are and why they're useful to JavaScript Just-In-Time compilers like JaegerMonkey.
- [Project: A Programming Language, by Marijn Haverbeke](http://eloquentjavascript.net/12_language.html) - we will build a programming LISP-like language called Egg. It will be a tiny, simple language—but one that is powerful enough to express any computation you can think of. It will allow simple abstraction based on functions.
- [Speculation in JavaScriptCore, by Filip Pizlo](https://webkit.org/blog/10308/speculation-in-javascriptcore/) - this post is all about speculative compilation, or just speculation for short, in the context of the JavaScriptCore virtual machine.
- [Understanding Compiler Optimization - Chandler Carruth - Opening Keynote Meeting C++ 2015](https://www.youtube.com/watch?v=FnGCDLhaxKU) - talk from Chandler Carruth about compilers optimizations, implemented in LLVM.
- [V8: A tale of two compilers, by Andy Wingo](https://wingolog.org/archives/2011/07/05/v8-a-tale-of-two-compilers) - advanced intro into two compilers in V8: FullCodegen and Crankshaft.

## Network

- [A computer networking zine, by Julia Evans](https://jvns.ca/networking-zine.pdf) - zine about OSI layer with great examples and simplified for better understanding. What is going on under the hood, when you are requesting an image of cat, etc...
- [A container networking overview, by Julia Evans](https://jvns.ca/blog/2016/12/22/container-networking/) - there are a lot of different ways you can network containers together, and the documentation on the internet about how it works is often pretty bad. I got really confused about all of this, so I’m going to try to explain what it all is in laymen’s terms.
- [High Performance Browser Networking, by Ilya Grigorik](https://hpbn.co) - this book provides a hands-on overview of what every web developer needs to know about the various types of networks (WiFi, 3G/4G), transport protocols (UDP, TCP, and TLS), application protocols (HTTP/1.1, HTTP/2), and APIs available in the browser (XHR, WebSocket, WebRTC, and more) to deliver the best—fast, reliable, and resilient—user experience.
- [How can an Internet work and how does the Internet work, by Stanislav Shalunov](https://www.mccme.ru/computers/Shalunov-inet.pdf) - the purpose of this book is to give an understanding of how the Internet works. We won't discuss formats of packets and such exact technical details.
- [Monitoring and Tuning the Linux Networking Stack: Receiving Data, by packagecloud](https://blog.packagecloud.io/eng/2016/06/22/monitoring-tuning-linux-networking-stack-receiving-data) - this blog post explains how computers running the Linux kernel receive packets, as well as how to monitor and tune each component of the networking stack as packets flow from the network toward userland programs.

## Databases

- [How does a relational database work, by Christophe Kalenzaga](http://coding-geek.com/how-databases-work/) - a really deep explanation of how relational databases work.
- [Implementing Sorting in Database Systems, by Goetz Graefe](http://wwwlgis.informatik.uni-kl.de/archiv/wwwdvs.informatik.uni-kl.de/courses/DBSREAL/SS2005/Vorlesungsunterlagen/Implementing_Sorting.pdf) - it covers in-memory sorting, disk-based external sorting, and considerations that apply specifically to sorting in database systems.
- [Let's Build a Simple Database, by Connor Stack](https://cstack.github.io/db_tutorial/) - I’m building a clone of sqlite from scratch in C in order to understand, and I’m going to document my process as I go.

## Bundlers

- [How does Bundler work, anyway, by André Arko](https://andre.arko.net/2015/04/28/how-does-bundler-work-anyway/) - Blog post explaining how the Ruby package/dependency manager handles dependencies.
- [Let’s learn how module bundlers work and then write one ourselves, by Adam Kelly](https://www.freecodecamp.org/news/lets-learn-how-module-bundlers-work-and-then-write-one-ourselves-b2e3fe6c88ae/) - Brief tutorial explaining how module bundlers work in Javascript by building a toy bundler.
- [Un-bundling the JavaScript module bundler, by Luciano Mammino](https://www.youtube.com/watch?v=WGlT921ixx4) - This video explains how the module bundler Webpack works.
- [Understanding webpack from the inside out, by Sean Larkin & Tobias Koppers](https://www.youtube.com/watch?v=gEBUU6QfVzk) - Video explaining the internals of Webpack: entry point, output, loaders, building a dependency graph, and utilizing plugins.

## Package Managers

- [Let's Dev: A Package Manager, by Maël Nison](https://yarnpkg.com/blog/2017/07/11/lets-dev-a-package-manager/) - A tutorial explaining how package management works by building a toy package manager.
- [So you want to write a package manager, by Sam Boyer](https://medium.com/@sdboyer/so-you-want-to-write-a-package-manager-4ae9c17d9527) - A blog post explaining the core components of a package management system: project code, manifest file, lock file, and dependency code.
