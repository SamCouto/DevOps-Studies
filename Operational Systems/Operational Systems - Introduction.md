# Operational Systems - Introduction
## *Basic concepts on Operational Systems*
#### ***Notes by: Samuel Couto***
#### ***Reference Book: "Sistemas Operacionais: Conceitos e Mecanismos" - Carlos A. Maziero***
---

### Why does Operational Systems exists?

A computer is compound by the union of hardware and software, although it's really difficult for programs to manage the usage of the hardware, in a low level way, think about telling the motherboard every electricity pulse to find an specific value in the computer's RAM.

The operational systems were created to offer a software layer between the user's programs and the low level hardware requests.

So, the operational system (*OS*) works between hardware and software, abstracting the hardware complexity and making possible to programs to access the computer's hardware in a homogeneous and easy way.

Here's one graphical example of the communication between the *OS*, *Hardware* and *Software*.
![[OS_Interaction.png]]
Looking to this image will make us understand the OS as an management key point.

---

### ***Abstraction***

The abstraction is necessary in order to promote simple access to low level hardware interfaces, making the process of using the hardware easier to the programs *(like a step to step algorithm)*.

In fact, the abstraction objective it's to turn apps independent of the hardware, with this, both can be more autonomous, making the development of apps easier because the developer don't need to specify really low level requests to make the program works.

---

### ***Resource Management***

The OS will manage all the software's hardware requests and all the computer's hardware.
This management process aims to equalize the requests in order to avoid request collisions.

In this way, the OS will make a bridge between programs and the hardware fulfilling all the necessities (requests) presented by the programs, always managing the hardware consumption.

The resource management equalizes the hardware requests defining policies of hardware usage in order to resolve processing conflicts, sharing the processing throughout the CPU cores.

As an example of equalization, we have distribution of tasks for all the processor's cores.

- A lot of programs makes requests at the same time
- The OS will detect those requests
- Distribute those requests to different cores of the processor
- The processor processes those requests respecting the priorities defined by the user

![[Resource_Management.png]]

The same happens to the RAM that also needs to be distributed to the programs, preventing one program to interfere in other programs requests (processes).

This management will prevent a lot of processing overflows an memory overflows, avoiding that one process takeover the hole CPU.

> ***Printers (Print Jobs)***
> Printing processes needs to be resolved in a exclusive way - just one process per time.
> The OS creates a print job line in order to prevent mixing documents in the process of printing.

