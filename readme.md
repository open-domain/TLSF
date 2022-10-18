Source: http://www.gii.upv.es/tlsf/
 	
TLSF

This web site provides detailed information about the TLSF (Two-Level Segregate Fit) allocator. TLSF is a general purpose dynamic memory allocator specifically designed to meet real-time requirements:

    Bounded Response Time . The worst-case execution time (WCET) of memory allocation and deallocation has got to be known in advance and be independent of application data. TLSF has a constant cost O(1).
    Fast. Additionally to a bounded cost, the allocator has to be efficient and fast enough. TLSF executes a maximum of 168 processor instructions in a x86 architecture. Depending on the compiler version and optimisation flags, it can be slightly lower or higher.
    Efficient Memory Use . Traditionally, real-time systems run for long periods of time and some (embedded applications), have strong constraints of memory size. Fragmentation can have a significant impact on such systems. It can increase dramatically, and degrade the system performance. A way to measure this efficiency is the memory fragmentation incurred by the allocator. TLSF has been tested in hundreds of different loads (real-time tasks, general purpose applications, etc.) obtaining an average fragmentation lower than 15 %. The maximum fragmentation measured is lower than 25%. 

TLSF has been included in several Linux distributions and applications. Although TLSF works rather well in many scenarios, it stands out in applications with hard/soft real-time application which uses explicit memory allocation with high flexibility requirements due to a high variability of the data size or adaptability to new situations. Some examples are:

    RTOS dynamic memory management
    Multimedia applications
    Routers, Switches, ...
    3D reconstruction and rendering in video system applications
    Games
    .....

This work started thanks to an EU founded project called OCERA and has continued in FRESCOR

Keywords: Memory management, dynamic memory management, Real-Time dynamic allocators, embedded systems, real-time malloc and free.
