### Who am I

Sometimes on a linux server it is not only good to know the Server but also who is connecting to it. Some permission depend on the user executing a program. So everytime you are unsure who you are, you can ask the system

`whoami`

an it will print your username. "whoami" has no more other feature.

You can get the same information with

`id -un`{{exec}}

But "id" can give you many more information like

`id -a`{{exec}}

looks like this

```bash
uid=1002(sebastian) gid=1001(admin) groups=1001(admin)
```

There you can see your username, the internal userid (uid) of your user. And your primary group (gid) and name and any other group the user is a member of.

### is there someone else?

You can look at who is also loggend in on the server with

`who`{{exec}}

and also take a look at what they are doing with

`w`{{exec}}
