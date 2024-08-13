# Operating Systems

The first computers of the 1940s were very primitive, operators entered programmes directly by flipping switches. Keypads with similar functionality existed on mainframes and minicomputers, right into the 1970s.&#x20;

As standardized computer hardware emerged in the 1950s, with each new generation of hardware, dedicated utilities were added to allow the hardware to be controlled by the software and applications. This is probably still the best definition of an Operating System (OS). These systems ran batch jobs, a range of tasks run one at a time in a single-tasking computer.&#x20;

The earliest record of an operating system I can find is an implementation by General Motors for an IBM 701 \[1].&#x20;

As computers became more powerful in the 1960s, operating systems were designed to allow multiple programmes to run at the same time, using time slices. As one programme became idle waiting for printing or disk access, another programme would use the CPU. Resources are shared and the algorithms for this sharing have been developing since. This was an era of time-sharing operating systems.&#x20;

One of the oldest technologies I have worked on was based on Multics, this introduced the concept of a process as an individual programme running in an operating system.  Process scheduling and management are still key topics in operating systems. At the time, Unix was a single process operating system.

One of the significant contributions of Multics was that it was the first operating system to be written in a high-level language, but it was eventually abandoned in favor of a multi-user version of Unix. When UNIX was being developed, the C programming language was specifically written to implement this operating system across hardware platforms. The original UNIX for the PDP11 was written c. 1973 in this way.&#x20;

All software which runs on a modern computer (including the operating system) is organized into processes, a process is an instance of an executing program. Each process appears to have its own memory space, CPU, etc. Each system appears as if it has multiple processes running concurrently, the CPU switches from process to process. However, there is a cost to this context switching.&#x20;

Threads are like lightweight processes. Many threads can run within the boundaries of a single process. Threads are the basic unit to which the operating system allocates processor time. A thread can execute any part of the process code, including parts currently being executed by another thread. Threads give the ability to have multiple things going on at the same time, without the performance cost of process switching.&#x20;

By the late 1970s, microcomputers were becoming available and some of them had floppy disks which required management. We began referring to the OS as a Disk Operating System (DOS). Early examples were CPM and MS-DOS.

\[1] Weizer, N., 1981. A history of operating systems
