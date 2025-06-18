### It looks interesting here?

Now that we know what kind of server we are visiting, lets take a look at the finer details.
There are many reason you connect to a server outside of a learning environment and often it is while something was unexpected.
So first we take a look at how long is this server running, maybe it rebooted recently?

`uptime`{{exec}}
or
`uptime -p`{{exec}}
or
`uptime -s`{{exec}}

Each of these commands shows us the same information, but presented a little bit different. Remember the one you like the most.

### Hardware

Linux hardware is a complex topic. But probably many time you are connected to a linux server it is a virtual machine, and hardware is much less important on those.

If you really want to know more 'low level stuff' about the server use these utilities:
Each of the has a '-h' switch to get more, or filtered information.

Try them out

#### Detailed information

`lshw`{{exec}}

#### Display information about the CPU architecture

`lscpu`{{exec}}

#### Block devices

`lsblk`{{exec}}

#### PCI devices

`lspci`{{exec}}

#### USB devices

`lsusb`{{exec}}
