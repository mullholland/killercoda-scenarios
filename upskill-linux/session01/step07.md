### Network

Network is another option you often have to take a look at.
To understand more of the network our server is using, we can use "ifconfig" to look at all the network interfaces we have

`ifconfig`{{exec}}

Tha show us all our network interfaces and some basic information like the IP adresse or how many packets there were incoming/outgoing.

Another tool for this could be

`netstat -i`{{exec}}

netstat or the newer 'socket statistics' can be used to show many interesting option about your server.

`ss -i`{{exec}}

most commonly used is to show all the ports your server if opening with

`ss -tulpen`{{exec}}

or

`netstat -tulpen`{{exec}}

that means

```bash
t => Display TCP sockets
u => Display UDP sockets
l => Display only listening sockets
p => Show process using socket
e => Show detailed socket information
n => Do not try to resolve service names. Show exact bandwidth values, instead of human-readable
```

They both have many other option. Take a look at them.

### Saturation

The next question often is, how much bandwidth is my server using.

For this you can use the tools

`ifstat`{{exec}}

you can end it with 'ctrl+c'

or

`iftop`{{exec}}

you can end it with 'q'
