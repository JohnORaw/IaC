---
description: An example operating system
---

# Linux

Unix has been around since the early 1970s, its origins along with the C programming language has changed the course of computing and technology development. I am not going to rehash history in this paper, read some on-line descriptions of the origins of [UNIX](http://www.unix.org/what\_is\_unix/history\_timeline.html). UNIX was originally written in machine code but was rewritten in C for portability.&#x20;

The GNU project was developed due to the restrictive license practices that emerged with commercial UNIX. It is as much a philosophy and political movement as a software foundation. Read some on-line descriptions of the origins of [GNU](https://www.gnu.org/gnu/thegnuproject.en.html). Make sure you understand what Stallman means by “free” and what the GNU General Public License (GNU GPL) is.&#x20;

GNU created some great software and utilities which compiled on UNIX, but they lacked the core component of the operating system, the kernel. There were no real alternatives which were free in the sense of GNU.&#x20;

Andrew Tanenbaum is one of the stalwarts of operating systems teaching and education. His books remain required reading on most operating systems courses. I recommend that you lay hands on a copy of his textbook, Modern Operating Systems. This is currently at the fourth edition, but an earlier one should be fine. As a teaching tool, Tanenbaum developed Minix in the late 1980s and published the source code as an example of how a UNIX-like operating system could be built. In 1991 Linus Torvalds built and released a kernel developed on a Minix system and heavily influenced by it. This OS was released under the GNU GPL and Linux was born.&#x20;

Although you can assemble your own version of Linux from source, most of us use fixed assemblies of components where a team of people worked on the assembly and its maintenance. These are referred to as distributions or distros. There are hundreds of distributions out there, suitable for specific uses.&#x20;

In business, we see a commercial company (Red Hat) as one on the leading distributions. Red Hat Enterprise Linux (RHEL) has excellent support but is costly. Many other common distributions are downstream distributions of RHEL. The GNU GPL stipulates that derivative work can only be distributed under the same license terms. This means that a commercial company like Red Hat must make its source code freely available and anyone can copy and compile it. CentOS was a community-based project that used the RHEL source code but made the resulting OS freely available \[ ]. There are tensions here and it is not all as simple as I describe! We used CentOS and Fedora as preferred teaching distros for the RHEL family.&#x20;

OpenSUSE and SUSE Linux Enterprise Server are gaining market share and are a popular alternative to RHEL.&#x20;

In academia and many data centers, Debian and downstream derivatives are preferred. We use Ubuntu server and desktop versions as preferred teaching distros for the Debian family. Ubuntu have the concept of Long-Term Support releases or LTS. These releases have >=5 years’ support making them a favorite of system administrators (me!).

## The Kernel

The kernel of Linux is the hub of the operating system: it allocates time and memory to processes and handles files and communications in response to system calls. As an illustration of the way that the shell and the kernel work together, suppose a user types; rm myfile (which has the effect of removing the file myfile). The shell searches the file store for the file containing the program rm, and then requests the kernel, through system calls, to execute the program rm on myfile. When the process rm myfile has finished running, the shell then returns the LINUX prompt % to the user, indicating that it is waiting for further commands. Linux does not look for rm in every directory, it only checks certain directories specified by an environment variable, $PATH; more of that later.

## The Shell

The shell acts as an interface between the user and the kernel. When a user logs in, the login program checks the username and password, and then starts another program called the shell. The shell is a command line interpreter (CLI). It interprets the commands the user types in and arranges for them to be carried out. The commands are themselves programs: when they terminate, the shell gives the user another prompt.

## The Programs

There are internal commands which are part of the shell and there are separate programmes, external commands which are free standing binaries, independent of the shell. The original authors of UNIX took some simple philosophical approaches to commands and utilities. The notion was that each command should do only one thing and do it well. This seems to have been a visionary approach; many of us think that complexity is one of the reasons why modern software may be unreliable. Keeping the tools simple and dedicated removes this as a vector for error. Many of the utilities and programmes have been developed by the GNU Project and it is worthwhile doing some reading regarding this project and its licensing models. A user can customise his/her own shell, and users can use different shells on the same machine.
