---
layout: page
title: PintOS
description: Implementing filesystems, user threads, and program invocation in a Linux-like x86 OS.
img: assets/img/projects/cs162bean.png
importance: 1
category: featured
---

*Project timeline: February 2023 to May 2023*

During my Spring 2023 semester at UC Berkeley, I took [CS 162: Operating Systems and Systems Programming](https://cs162.org/). We designed and implemented many interesting things -- a shell supporting program execution, path resolution, signal redirection, pipes, and more in C and an implementation of the coordinator of MapReduce in Rust were some stand-out examples. 

However, the main meat of the class came in developing out PintOS, an educational Linux-like x86 OS built in C. We started with an existing OS with some bare-bones bootstrap code. Throughout 3 projects and in a team of 4, we implemented major components of the OS, such as:
* Argument Passing
* Process Control Syscalls
* File Operation Syscalls
* Floating Point Unit Support
* Efficient (non-busy-waiting) system alarm clock
* Strict priority scheduling of threads
* Support for user threads (pthreads)
* Filesystem block cache in-memory
* A FFS-based filesystem (inode tree, etc)
* & Subdirectory support.

It was a great experience to work on a major piece of software with a team of 4. Working in an internship environment wasn't nearly as collaborative as working in this team; much of our code needed to fit into each other with very tight tolerances, and bugs could propagate throughout the codebase. This led me to really understanding how to manage pull requests -- in other classes, I could get away with just working on `main` the whole time. Furthermore the PintOS experience threw me deep into an existing system, packed with its own quirks, problems, and incredibly smart solutions. Learning all of the codebase to the level necessary to build out these features was an incredible experience, and has definitely impacted the speed at which I understand other large codebases.