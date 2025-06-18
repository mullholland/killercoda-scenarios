### RAM / Memory

Another question often ask is how much RAM is my system using.

`free -m`{{exec}}

```bash
          total   used   free   shared   buff/cache   available
  Mem:     1504    636     13        0          855         792
  Swap:    2047      6   2041
```

Often people are shocked to see, that linux took al their RAM and they are on the way to call support and order more RAM.
But Linux handles this a little bit different.
A nice compilation on what is heppening here is available at [Linux ate my ram](https://www.linuxatemyram.com/).

The short answer is

```bash
Like all modern operating systems, Linux is borrowing unused memory for disk caching. This makes it look like you are low on "free" memory, but you are not! Everything is fine!
```

a more detailed information can be get with
`vmstat`{{exec}}

This has many options, take a look at them i try a few.
