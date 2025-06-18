### CPU

CPU usage under linux is a complicated thing. Most people want a simple % value, but they are not easi to come by.

We remember the command for a detailed cpu overview
`lscpu`{{exec}}

There was a line 'CPU(s)' which showed a number. We try to remember the number if it is larger than 1.

To take a closer look at the current CPU usage we can use
`top`{{exec}}

Press "q" to exit the top session.

There we can see the current usage in % for the different kind a linux systems differentiates in the CPU usage

```bash
Cpu(s):  0.8 us,  0.6 sy,  0.0 ni, 98.6 id,  0.0 wa,  0.0 hi,  0.0 si,  0.0 st

us => Time spent in user space (That is a process from any normal user on the machine)
sy => Time spent in kernel space (That are the linux kernels own calls)
ni => Time spent running niced user processes (User defined priority)
id => Time spent in idle operations
wa => Time spent on waiting on IO peripherals (eg. disk)
hi => Time spent handling hardware interrupt routines. (Whenever a peripheral unit want attention form the CPU, it literally pulls a line, to signal the CPU to service it)
si => Time spent handling software interrupt routines. (a piece of code, calls an interrupt routine...)
st => Time spent on involuntary waits by virtual cpu while hypervisor is servicing another processor (stolen from a virtual machine)
```

A fancier version of "top" can be
`htop`{{exec}}

"htop" is no standard tool in many linux Distribution, so you may of to install it yourself. More about that later.

"top" has many more useful information, take a look at it.
