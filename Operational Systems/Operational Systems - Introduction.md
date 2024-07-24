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

> ***Resource Management***
> The OS will manage all the software's hardware requests and all the computer's hardware.
> This management process aims to equalize the requests in order to avoid collisions.

In this way, the OS will make a bridge between programs and the hardware fulfilling all the necessities (requests) presented by the programs, always managing the hardware consumption.

The resource management, as said before, needs to equalize the hardware requests to avoid not only collisions, but overflows and denial of services (DoS) too.

> ***Abstraction***
> The abstraction is necessary in order to promote simple access to low level hardware interfaces, making the process of using the hardware in the correct way easier to the programs *(like a step to step algorithm)*.